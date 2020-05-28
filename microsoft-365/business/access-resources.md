---
title: גישה למשאבים מקומיים ממכשיר תכלת המצורף לאתר ב-Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: למד כיצד לקבל גישה למשאבים מקומיים כגון שורה של יישומים עסקיים, שיתופי קבצים ומדפסות מתוך מכשיר המצורף ל-Windows 10.
ms.openlocfilehash: da5fab99cf00a65986fb5e555cc19e432fe0fe8d
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44401113"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="598f9-103">גישה למשאבים מקומיים ממכשיר תכלת מחובר ב-Microsoft 365 עסקים פרימיום</span><span class="sxs-lookup"><span data-stu-id="598f9-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="598f9-104">לכל מכשיר של Windows 10 המצורף ל-"תכלת Active Directory" יש גישה לכל המשאבים המבוססים על ענן צמתים, כגון יישומי Microsoft 365, וניתן להגן עליהם על-ידי Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="598f9-104">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="598f9-105">כמו כן, באפשרותך לאפשר גישה למשאבים מקומיים כגון יישומים של שורה עסקית, שיתופי קבצים ומדפסות.</span><span class="sxs-lookup"><span data-stu-id="598f9-105">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="598f9-106">כדי לאפשר גישה, השתמש [בתכלת והתחבר](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) כדי לסנכרן את הספריה המקומית שלך באמצעות הספריה הפעילה.</span><span class="sxs-lookup"><span data-stu-id="598f9-106">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="598f9-107">לקבלת מידע נוסף, ראה [מבוא לניהול התקנים בתוך הספריה הפעילה](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="598f9-107">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="598f9-108">השלבים מסוכמים גם בסעיפים הבאים.</span><span class="sxs-lookup"><span data-stu-id="598f9-108">The steps are also summarized in the following sections.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="598f9-109">הליך זה ישים רק ל-OAuth ו-NTLM.</span><span class="sxs-lookup"><span data-stu-id="598f9-109">This procedure is only applicable to OAuth and NTLM.</span></span> <span data-ttu-id="598f9-110">אין תמיכה ב-Kerberos.</span><span class="sxs-lookup"><span data-stu-id="598f9-110">Kerberos is not supported.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="598f9-111">הפעל תכלת והתחבר</span><span class="sxs-lookup"><span data-stu-id="598f9-111">Run Azure AD Connect</span></span>

<span data-ttu-id="598f9-112">השלם את השלבים הבאים כדי לאפשר להתקנים המצורפים של הארגון לבצע גישה למשאבים מקומיים.</span><span class="sxs-lookup"><span data-stu-id="598f9-112">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="598f9-113">כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מתוך Active Directory המקומי לתוך מדריך כחול פעיל, הפעל את אשף סינכרון הספריות והשתמש בתכלת AD כמתואר [בהגדרת סינכרון ספריות עבור Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="598f9-113">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization).</span></span>
    
2. <span data-ttu-id="598f9-114">לאחר השלמת סינכרון הספריות, ודא שהתקני Windows 10 של הארגון שלך מצורפים לתכלת.</span><span class="sxs-lookup"><span data-stu-id="598f9-114">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="598f9-115">שלב זה נעשה בנפרד בכל התקן של Windows 10.</span><span class="sxs-lookup"><span data-stu-id="598f9-115">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="598f9-116">ראה [הגדרת התקני Windows עבור משתמשי Microsoft Business Premium 365](set-up-windows-devices.md) לקבלת פרטים.</span><span class="sxs-lookup"><span data-stu-id="598f9-116">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="598f9-117">לאחר התקני Windows 10 הם תכלת לספירה הצטרפו, כל משתמש חייב לאתחל את המכשירים שלהם ולהיכנס עם האישורים שלהם מיקרוסופט 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="598f9-117">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="598f9-118">לכל ההתקנים יש כעת גישה גם למשאבים מקומיים.</span><span class="sxs-lookup"><span data-stu-id="598f9-118">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="598f9-119">אין צורך בצעדים נוספים כדי לקבל גישה למשאבים מקומיים עבור התקנים המצורפים ל-תכלת AD.</span><span class="sxs-lookup"><span data-stu-id="598f9-119">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="598f9-120">פונקציונליות זו מוכללת ב-Windows 10.</span><span class="sxs-lookup"><span data-stu-id="598f9-120">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="598f9-121">אם יש לך תוכניות להתחבר למכשיר AADJ אחר מאשר שיטת סיסמה כמו PIN/Bio-מטרי באמצעות התחברות האישור WHFB ולאחר מכן לגשת למשאבים המקומי (מיקומים משותפים, מדפסות... וכו '), אנא עקוב אחרhttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="598f9-121">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="598f9-122">אם הארגון שלך אינו מוכן לפרוס בתצורת ההתקן המצורף של התכלת שתוארה לעיל, שקול להגדיר [תצורת התקן היברידית של התכלת ההיברידית](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="598f9-122">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="598f9-123">שיקולים כאשר אתה מצטרף להתקני Windows לתכלת</span><span class="sxs-lookup"><span data-stu-id="598f9-123">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="598f9-124">אם התקן Windows שאליו הצטרפת התכלת-לספירה הצטרף לתחום בעבר או בקבוצת עבודה, שקול את המגבלות הבאות:</span><span class="sxs-lookup"><span data-stu-id="598f9-124">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="598f9-125">כאשר התקן "תכלת לספירה" מצטרף, הוא יוצר משתמש חדש מבלי ליצור הפניה לפרופיל קיים.</span><span class="sxs-lookup"><span data-stu-id="598f9-125">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="598f9-126">יש להעביר באופן ידני פרופילים.</span><span class="sxs-lookup"><span data-stu-id="598f9-126">Profiles must be manually migrated.</span></span> <span data-ttu-id="598f9-127">פרופיל משתמש מכיל מידע כגון מועדפים, קבצים מקומיים, הגדרות דפדפן והגדרות תפריט התחלה.</span><span class="sxs-lookup"><span data-stu-id="598f9-127">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="598f9-128">הגישה הטובה ביותר היא למצוא כלי של ספק חיצוני כדי למפות קבצים והגדרות קיימים לפרופיל החדש.</span><span class="sxs-lookup"><span data-stu-id="598f9-128">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="598f9-129">אם ההתקן משתמש באובייקטי מדיניות קבוצתית (GPO), ייתכן שלאובייקטי Gpo מסוימים אין [ספק שירותי תצורה](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) דומה (CSP) ב-Intune.</span><span class="sxs-lookup"><span data-stu-id="598f9-129">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="598f9-130">הפעל את [הכלי Mmat](https://www.microsoft.com/download/details.aspx?id=45520) כדי לחפש מדיניות קבוצתית דומה עבור אובייקטי gpo קיימים.</span><span class="sxs-lookup"><span data-stu-id="598f9-130">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="598f9-131">משתמשים לא יוכלו לבצע אימות ליישומים התלויים באימות של Active Directory.</span><span class="sxs-lookup"><span data-stu-id="598f9-131">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="598f9-132">הערכת יישום מדור קודם ושקול לעדכן לאפליקציה המשתמשת ב-אימות מודרני, במידת האפשר.</span><span class="sxs-lookup"><span data-stu-id="598f9-132">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="598f9-133">גילוי מדפסות של active Directory לא יפעל.</span><span class="sxs-lookup"><span data-stu-id="598f9-133">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="598f9-134">באפשרותך לספק נתיבי מדפסת ישירים עבור כל המשתמשים או להשתמש [בהדפס ענן היברידי](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="598f9-134">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
