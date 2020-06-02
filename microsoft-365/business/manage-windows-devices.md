---
title: הפעל התקנים של Windows 10 המצורפים לתחום לניהול באמצעות Microsoft 365 עבור עסקים
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: למד כיצד לאפשר ל-Microsoft 365 להגן על התקנים מקומיים המצורפים ל-Windows 10 באמצעות ספריות בתוך מספר צעדים בלבד.
ms.openlocfilehash: 7bfe5da8701a17712fa249eac99a22b8d5a1b2d1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471046"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="94cc4-103">אפשר להפעיל התקנים של Windows 10 המצורפים לתחום כדי שינוהל על-ידי Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="94cc4-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="94cc4-104">אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business Premium כדי להגן על התקני Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים המחייבים אימות מקומי.</span><span class="sxs-lookup"><span data-stu-id="94cc4-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="94cc4-105">כדי להגדיר הגנה זו, באפשרותך ליישם **התקנים היברידית כחול לספירה המצורפים**.</span><span class="sxs-lookup"><span data-stu-id="94cc4-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="94cc4-106">התקנים אלה מצורפים הן ל-Active Directory המקומי והן לספריה הפעילה שלך.</span><span class="sxs-lookup"><span data-stu-id="94cc4-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="94cc4-107">סרטון וידאו זה מתאר את השלבים עבור אופן ההגדרה של התרחיש הנפוץ ביותר, המפורט גם בשלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="94cc4-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="94cc4-108">1. היכונו לסנכרון ספריות</span><span class="sxs-lookup"><span data-stu-id="94cc4-108">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="94cc4-109">לפני שתסנכרן את המשתמשים והמחשבים שלך מקבוצת המחשבים המקומית של Active Directory, סקור את [ההכנה לסנכרון ספריות ל-Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="94cc4-109">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="94cc4-110">בפרט:</span><span class="sxs-lookup"><span data-stu-id="94cc4-110">In particular:</span></span>

   - <span data-ttu-id="94cc4-111">ודא שאין כפילויות בספריה שלך עבור התכונות הבאות: **דואר**, **כתובות Proxyaddresses שמות** **משתמשים**.</span><span class="sxs-lookup"><span data-stu-id="94cc4-111">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="94cc4-112">על ערכים אלה להיות ייחודיים ויש להסיר את כל הכפילויות.</span><span class="sxs-lookup"><span data-stu-id="94cc4-112">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="94cc4-113">מומלץ לקבוע את התצורה של התכונה **Userהפריפרישם** (UPN) עבור כל חשבון משתמש מקומי שיתאים לכתובת הדואר האלקטרוני הראשית המתאימה למשתמש Microsoft 365 המורשה.</span><span class="sxs-lookup"><span data-stu-id="94cc4-113">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="94cc4-114">לדוגמה: *mary.shelley@contoso.com* ולא *mary@contoso. מקומיים*</span><span class="sxs-lookup"><span data-stu-id="94cc4-114">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="94cc4-115">אם קבוצת המחשבים של Active Directory מסתיימת בסיומת שאינה ניתנת לניתוב כגון. *local* או *. lan*, במקום סיומת אינטרנט הניתנת לניתוב כגון *. com* או *. org*, התאם תחילה את סיומת ה-UPN של חשבונות המשתמשים המקומיים כמתואר [בהכנת תחום שאינו ניתן לניתוב עבור סינכרון ספריות](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="94cc4-115">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="94cc4-116">2. התקנה והגדרה של התחברות תכלת</span><span class="sxs-lookup"><span data-stu-id="94cc4-116">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="94cc4-117">כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מ-Active Directory המקומי לתוך מדריך כחול פעיל, התקן את האפשרות התחבר לספריית המשימות הפעילה והגדר סינכרון ספריות.</span><span class="sxs-lookup"><span data-stu-id="94cc4-117">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> <span data-ttu-id="94cc4-118">ראה [הגדרת סינכרון ספריות עבור Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) כדי ללמוד עוד.</span><span class="sxs-lookup"><span data-stu-id="94cc4-118">See [Set up directory synchronization for Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

> [!NOTE]
> <span data-ttu-id="94cc4-119">השלבים זהים בדיוק עבור Microsoft 365 עבור עסקים.</span><span class="sxs-lookup"><span data-stu-id="94cc4-119">The steps are exactly the same for Microsoft 365 for business.</span></span> 

<span data-ttu-id="94cc4-120">כאשר אתה מגדיר את האפשרויות שלך עבור תכלת AD התחבר, אנו ממליצים לאפשר **סנכרון סיסמה**, **כניסה יחידה בודדת**, ואת **הסיסמה כתבה בחזרה** , אשר נתמך גם ב-Microsoft 365 לעסקים.</span><span class="sxs-lookup"><span data-stu-id="94cc4-120">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="94cc4-121">יש כמה שלבים נוספים עבור הסיסמה כתיבה מעבר לתיבת הסימון התחבר תכלת AD.</span><span class="sxs-lookup"><span data-stu-id="94cc4-121">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="94cc4-122">לקבלת מידע נוסף, ראה [כיצד-to: הגדרת התצורה של הסיסמה ככתוב](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="94cc4-122">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

## <a name="3-configure-hybrid-azure-ad-join"></a><span data-ttu-id="94cc4-123">3. להגדיר היברידית תכלת הצטרפות</span><span class="sxs-lookup"><span data-stu-id="94cc4-123">3. Configure Hybrid Azure AD Join</span></span>

<span data-ttu-id="94cc4-124">לפני שתאפשר ל-Windows 10 להיות מצורף להתקן התכלת ההיברידית לספירה, ודא שאתה עומד בדרישות המוקדמות הבאות:</span><span class="sxs-lookup"><span data-stu-id="94cc4-124">Before you enable Windows 10 devices to be Hybrid Azure AD joined, make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="94cc4-125">אתה מריץ את הגרסה העדכנית ביותר של התחברות לספירה.</span><span class="sxs-lookup"><span data-stu-id="94cc4-125">You're running the latest version of Azure AD Connect.</span></span>

   - <span data-ttu-id="94cc4-126">החיבור התכלת לספירה מסנכרן את כל אובייקטי המחשב של המכשירים שברצונך להיות היברידית תכלת לספירה הצטרפו.</span><span class="sxs-lookup"><span data-stu-id="94cc4-126">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="94cc4-127">אם אובייקטי המחשב שייכים ליחידות ארגוניות מסוימות (OU), ודא שאלה אלה מוגדרות לסנכרון בתכלת הספירה גם כן.</span><span class="sxs-lookup"><span data-stu-id="94cc4-127">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>

<span data-ttu-id="94cc4-128">כדי לרשום התקן קיים המצורפים ל-Windows 10 התקנים כמו תכלת היברידית לספירה הצטרף, בצע את השלבים [במדריך: קביעת תצורה של היברידית תכלת היברידי להצטרף לתחומים מנוהלים](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span><span class="sxs-lookup"><span data-stu-id="94cc4-128">To register existing domain-joined Windows 10 devices as Hybrid Azure AD joined, follow the steps in the [Tutorial: Configure hybrid Azure Active Directory join for managed domains](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="94cc4-129">היברידית זו מאפשרת ל-Active Directory המקומי הקיים שלך להצטרף למחשבי Windows 10 ולגרום להם להיות מוכנים לעננים.</span><span class="sxs-lookup"><span data-stu-id="94cc4-129">This hybrid-enables your existing on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a><span data-ttu-id="94cc4-130">4. אפשר הרשמה אוטומטית ל-Windows 10</span><span class="sxs-lookup"><span data-stu-id="94cc4-130">4. Enable automatic enrollment for Windows 10</span></span>

 <span data-ttu-id="94cc4-131">כדי לרשום באופן אוטומטי התקני Windows 10 עבור ניהול התקנים ניידים ב-Intune, ראה [רישום התקן windows 10 באופן אוטומטי באמצעות מדיניות קבוצתית](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span><span class="sxs-lookup"><span data-stu-id="94cc4-131">To automatically enroll Windows 10 devices for mobile device management in Intune, see [Enroll a Windows 10 device automatically using Group Policy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span></span> <span data-ttu-id="94cc4-132">באפשרותך להגדיר את המדיניות הקבוצתית ברמת מחשב מקומית, או עבור פעולות בצובר, באפשרותך להשתמש ב-מסוף ניהול המדיניות הקבוצתית ובתבניות ADMX כדי ליצור הגדרת מדיניות קבוצתית זו בבקר התחום שלך.</span><span class="sxs-lookup"><span data-stu-id="94cc4-132">You can set the Group Policy at a local computer level, or for bulk operations, you can use the Group Policy Management Console and ADMX templates to create this Group Policy setting on your Domain Controller.</span></span>

## <a name="5-configure-seamless-single-sign-on"></a><span data-ttu-id="94cc4-133">5. קביעת תצורה של כניסה יחידה חלקה</span><span class="sxs-lookup"><span data-stu-id="94cc4-133">5. Configure Seamless Single Sign-On</span></span>

  <span data-ttu-id="94cc4-134">מערכת SSO חלקה מאותלת משתמשים באופן אוטומטי למשאבי הענן של Microsoft 365 כשהם משתמשים במחשבים ארגוניים.</span><span class="sxs-lookup"><span data-stu-id="94cc4-134">Seamless SSO automatically signs users into their Microsoft 365 cloud resources when they use corporate computers.</span></span> <span data-ttu-id="94cc4-135">פשוט לפרוס אחת משתי אפשרויות המדיניות הקבוצתית המתוארות [כניסה יחידה של Active Directory בודדת: התחלה מהירה](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span><span class="sxs-lookup"><span data-stu-id="94cc4-135">Simply deploy one of the two Group Policy options described in [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span></span> <span data-ttu-id="94cc4-136">האפשרות **מדיניות קבוצתית** אינה מאפשרת למשתמשים לשנות את הגדרותיו, בעוד שהאפשרות **העדפת מדיניות קבוצתית** מגדירה את הערכים, אך גם משאירה אותם להגדרה של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="94cc4-136">The **Group Policy** option doesn't allow users to change their settings, while the **Group Policy Preference** option sets the values but also leaves them user-configurable.</span></span>

## <a name="6-set-up-windows-hello-for-business"></a><span data-ttu-id="94cc4-137">6. הגדרת Windows שלום עבור עסקים</span><span class="sxs-lookup"><span data-stu-id="94cc4-137">6. Set up Windows Hello for Business</span></span>

 <span data-ttu-id="94cc4-138">Windows שלום לעסק מחליף סיסמאות עם אימות שני גורמים חזק (2FA) לצורך כניסה למחשב מקומי.</span><span class="sxs-lookup"><span data-stu-id="94cc4-138">Windows Hello for Business replaces passwords with strong two-factor authentication (2FA) for signing into a local computer.</span></span> <span data-ttu-id="94cc4-139">גורם אחד הוא זוג מפתחות אסימטרי, והשני הוא PIN או מחווה מקומית אחרת, כגון טביעת אצבע או זיהוי פנים אם המכשיר תומך בו.</span><span class="sxs-lookup"><span data-stu-id="94cc4-139">One factor is an asymmetric key pair, and the other is a PIN or other local gesture such as fingerprint or facial recognition if your device supports it.</span></span> <span data-ttu-id="94cc4-140">מומלץ להחליף סיסמאות באמצעות 2FA ו-Windows שלום לעסקים במידת האפשר.</span><span class="sxs-lookup"><span data-stu-id="94cc4-140">We recommend that you replace passwords with 2FA and Windows Hello for Business where possible.</span></span>

<span data-ttu-id="94cc4-141">כדי להגדיר היברידית Windows שלום עבור עסקים, לסקור את [מפתח היברידית אמון Windows שלום עבור דרישות מוקדמות בעסקים](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span><span class="sxs-lookup"><span data-stu-id="94cc4-141">To configure Hybrid Windows Hello for Business, review the [Hybrid Key trust Windows Hello for Business Prerequisites](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span></span> <span data-ttu-id="94cc4-142">לאחר מכן בצע את ההוראות ב- [קביעת תצורה של Windows Hybrid שלום עבור הגדרות אמון מפתח עסקי](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span><span class="sxs-lookup"><span data-stu-id="94cc4-142">Then follow the instructions in [Configure Hybrid Windows Hello for Business key trust settings](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span></span> 
