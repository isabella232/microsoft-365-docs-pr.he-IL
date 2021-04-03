---
title: סינכרון משתמשי תחום עם Microsoft 365
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: סנכרן משתמשים הנשלטים על-ידי תחום עם Microsoft 365 לעסקים.
ms.openlocfilehash: b477b8a1f35a790d6c49937c973c141ad9f90ad4
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578406"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="b5b88-103">סינכרון משתמשי תחום עם Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b5b88-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="b5b88-104">1. התכונן לסינכרון מדריכי כתובות</span><span class="sxs-lookup"><span data-stu-id="b5b88-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="b5b88-105">לפני סינכרון המשתמשים והמחשבים שלך מתחום Active Directory המקומי, עיין בהכנה [לסינכרון מדריכי כתובות ל- Microsoft 365.](../enterprise/prepare-for-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="b5b88-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](../enterprise/prepare-for-directory-synchronization.md).</span></span> <span data-ttu-id="b5b88-106">בפרט:</span><span class="sxs-lookup"><span data-stu-id="b5b88-106">In particular:</span></span>

   - <span data-ttu-id="b5b88-107">ודא שלא קיימים כפילויות במדריך הכתובות שלך עבור התכונות הבאות: **דואר**, **proxyAddresses** **ו- userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="b5b88-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="b5b88-108">ערכים אלה חייבים להיות ייחודיים ויש להסיר את כל הכפילויות.</span><span class="sxs-lookup"><span data-stu-id="b5b88-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="b5b88-109">מומלץ להגדיר את התכונה **userPrincipalName** (UPN) עבור כל חשבון משתמש מקומי כך שתהתאים לכתובת הדואר האלקטרוני הראשית התואמת למשתמש בעל הרשיון של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b5b88-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="b5b88-110">לדוגמה: *mary.shelley@contoso.com* במקום *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="b5b88-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="b5b88-111">אם התחום של Active Directory מסתיים בסיומת לא ניתנת לניתוב, כגון *.local* או *.lan,* במקום סיומת הניתנת לניתוב באינטרנט, כגון *.com* או *.org,* התאם את סיומת UPN של חשבונות המשתמשים המקומיים תחילה כמתואר בנושא הכנת תחום שאינו ניתן לניתוב [עבור סינכרון מדריכי כתובות.](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="b5b88-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md).</span></span> 

<span data-ttu-id="b5b88-112">ה- **Run IdFix** בשלב ארבע (4) להלן, יוודא גם ש- Active Directory המקומי מוכן לסינכרון מדריכי כתובות.</span><span class="sxs-lookup"><span data-stu-id="b5b88-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for directory synchronization.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="b5b88-113">2. התקן וקבע את תצורת Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="b5b88-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="b5b88-114">כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מ- Active Directory המקומי לתוך Azure Active Directory, התקן את Azure Active Directory Connect והגדיר סינכרון מדריכי כתובות.</span><span class="sxs-lookup"><span data-stu-id="b5b88-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="b5b88-115">במרכז [](https://go.microsoft.com/fwlink/p/?linkid=2024339)הניהול, בחר **הגדרה** בסרגל הניווט הימני.</span><span class="sxs-lookup"><span data-stu-id="b5b88-115">In the [admin center](https://go.microsoft.com/fwlink/p/?linkid=2024339), select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="b5b88-116">תחת **כניסה ואבטחה, בחר** הצג תחת **סינכרון** **משתמשים מהמדריך הכתובות של האתרים שלך.**</span><span class="sxs-lookup"><span data-stu-id="b5b88-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="b5b88-117">בדף **סינכרון משתמשים ממדריך הכתובות של האתרים** שלך, בחר **תחילת העבודה**.</span><span class="sxs-lookup"><span data-stu-id="b5b88-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="b5b88-118">בשלב הראשון הפעל את הכלי IdFix כדי להתכונן לסינכרון מדריך כתובות.</span><span class="sxs-lookup"><span data-stu-id="b5b88-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="b5b88-119">בצע את שלבי האשף כדי להוריד את Azure AD Connect ולהשתמש בו כדי לסנכרן את המשתמשים הנשלטים על-ידי התחום שלך עם Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b5b88-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="b5b88-120">ראה [הגדרת סינכרון מדריכי כתובות עבור Microsoft 365](../enterprise/set-up-directory-synchronization.md) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="b5b88-120">See [Set up directory synchronization for Microsoft 365](../enterprise/set-up-directory-synchronization.md) to learn more.</span></span>

<span data-ttu-id="b5b88-121">בעת קביעת התצורה של האפשרויות עבור Azure AD Connect, מומלץ להפוך סינכרון סיסמאות **,** כניסה יחידה חלקה לזמינה ואת התכונה **writeback** של הסיסמה, הנתמכת גם היא ב- Microsoft 365 לעסקים. </span><span class="sxs-lookup"><span data-stu-id="b5b88-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="b5b88-122">ישנם כמה שלבים נוספים עבור writeback סיסמה מעבר לתיבת הסימון ב- Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b5b88-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="b5b88-123">לקבלת מידע נוסף, ראה [כיצד לעשות: קביעת תצורה של writeback של סיסמה](/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="b5b88-123">For more information, see [How-to: configure password writeback](/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="b5b88-124">אם ברצונך גם לנהל מכשירי Windows 10 המצורפים לתחום, ראה הפיכת מכשירי Windows 10 המצורפים לתחום לזמינים לניהול [על-ידי Microsoft 365 Business Premium](manage-windows-devices.md) כדי להגדיר צירוף Azure AD היברידי.</span><span class="sxs-lookup"><span data-stu-id="b5b88-124">If you also want to manage domain-joined Windows 10 devices, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span>