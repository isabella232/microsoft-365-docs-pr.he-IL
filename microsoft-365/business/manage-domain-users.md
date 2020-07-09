---
title: סנכרן משתמשי תחום ל-Microsoft 365
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
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
- MOE150
description: סנכרן משתמשים מבוקרים בתחום עם Microsoft 365 לעסקים.
ms.openlocfilehash: af9cb7c9b2b639edc2375679a73ab41c4cf6de71
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081847"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="0f1eb-103">סנכרן משתמשי תחום ל-Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0f1eb-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="0f1eb-104">1. היכונו לסנכרון ספריות</span><span class="sxs-lookup"><span data-stu-id="0f1eb-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="0f1eb-105">לפני שתסנכרן את המשתמשים והמחשבים שלך מקבוצת המחשבים המקומית של Active Directory, סקור את [ההכנה לסנכרון ספריות ל-Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="0f1eb-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="0f1eb-106">בפרט:</span><span class="sxs-lookup"><span data-stu-id="0f1eb-106">In particular:</span></span>

   - <span data-ttu-id="0f1eb-107">ודא שאין כפילויות בספריה שלך עבור התכונות הבאות: **דואר**, **כתובות Proxyaddresses שמות** **משתמשים**.</span><span class="sxs-lookup"><span data-stu-id="0f1eb-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="0f1eb-108">על ערכים אלה להיות ייחודיים ויש להסיר את כל הכפילויות.</span><span class="sxs-lookup"><span data-stu-id="0f1eb-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="0f1eb-109">מומלץ לקבוע את התצורה של התכונה **Userהפריפרישם** (UPN) עבור כל חשבון משתמש מקומי שיתאים לכתובת הדואר האלקטרוני הראשית המתאימה למשתמש Microsoft 365 המורשה.</span><span class="sxs-lookup"><span data-stu-id="0f1eb-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="0f1eb-110">לדוגמה: *mary.shelley@contoso.com* ולא *mary@contoso. מקומיים*</span><span class="sxs-lookup"><span data-stu-id="0f1eb-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="0f1eb-111">אם קבוצת המחשבים של Active Directory מסתיימת בסיומת שאינה ניתנת לניתוב כגון. *local* או *. lan*, במקום סיומת אינטרנט הניתנת לניתוב כגון *. com* או *. org*, התאם תחילה את סיומת ה-UPN של חשבונות המשתמשים המקומיים כמתואר [בהכנת תחום שאינו ניתן לניתוב עבור סינכרון ספריות](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="0f1eb-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="0f1eb-112">**הפעל IdFix** בשלב ארבע (4) להלן, גם יוודא שהמחשב המקומי שלך active Directory מוכן לסינכרון dir.</span><span class="sxs-lookup"><span data-stu-id="0f1eb-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for dir sync.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="0f1eb-113">2. התקנה והגדרה של התחברות תכלת</span><span class="sxs-lookup"><span data-stu-id="0f1eb-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="0f1eb-114">כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מ-Active Directory המקומי לתוך מדריך כחול פעיל, התקן את האפשרות התחבר לספריית המשימות הפעילה והגדר סינכרון ספריות.</span><span class="sxs-lookup"><span data-stu-id="0f1eb-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="0f1eb-115">במרכז הניהול של <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> בחירת **ההתקנה** בניווט השמאלי.</span><span class="sxs-lookup"><span data-stu-id="0f1eb-115">In the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="0f1eb-116">תחת **כניסה ואבטחה**, בחר באפשרות **תצוגה** תחת **משתמשי סינכרון מהספריה של הארגון**.</span><span class="sxs-lookup"><span data-stu-id="0f1eb-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="0f1eb-117">בתיקיה **משתמשי סינכרון מתוך הספריה של הארגון** , בחר באפשרות ' **התחל**'.</span><span class="sxs-lookup"><span data-stu-id="0f1eb-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="0f1eb-118">בשלב הראשון הכלי IdFix כדי להתכונן לסנכרון ספריות.</span><span class="sxs-lookup"><span data-stu-id="0f1eb-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="0f1eb-119">בצע את צעדי האשף כדי להוריד את החיבור התכלת ולהשתמש בו כדי לסנכרן את המשתמשים שבשליטת התחום שלך ל-Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0f1eb-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="0f1eb-120">ראה [הגדרת סינכרון ספריות עבור Microsoft 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) כדי ללמוד עוד.</span><span class="sxs-lookup"><span data-stu-id="0f1eb-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="0f1eb-121">כאשר אתה מגדיר את האפשרויות שלך עבור תכלת AD התחבר, אנו ממליצים לאפשר **סנכרון סיסמה**, **כניסה יחידה בודדת**, ואת **הסיסמה כתבה בחזרה** , אשר נתמך גם ב-Microsoft 365 לעסקים.</span><span class="sxs-lookup"><span data-stu-id="0f1eb-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="0f1eb-122">יש כמה שלבים נוספים עבור הסיסמה כתיבה מעבר לתיבת הסימון התחבר תכלת AD.</span><span class="sxs-lookup"><span data-stu-id="0f1eb-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="0f1eb-123">לקבלת מידע נוסף, ראה [כיצד-to: הגדרת התצורה של הסיסמה ככתוב](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="0f1eb-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="0f1eb-124">אם ברצונך לנהל גם התקנים המצורפים לתחום של Windows 10, ראה [הפעלת התקנים של windows 10 המצורפים לתחום כדי שתנוהל על-ידי Microsoft 365 Business Premium](manage-windows-devices.md) כדי להגדיר את הצירוף היברידי לתכלת.</span><span class="sxs-lookup"><span data-stu-id="0f1eb-124">If you want to manage domain-joined Windows 10 devices also, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 