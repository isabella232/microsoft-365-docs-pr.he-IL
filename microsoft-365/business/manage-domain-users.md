---
title: סינכרון משתמשי תחום ל-Microsoft 365
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
description: סנכרן משתמשים שנשלטים על-ידי תחום באמצעות Microsoft 365 for business.
ms.openlocfilehash: 9495d893eb6870ef7c417a78f921296bfc0e6705
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306448"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="a53e4-103">סינכרון משתמשי תחום ל-Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a53e4-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="a53e4-104">1. הכנה לסינכרון מדריכי כתובות</span><span class="sxs-lookup"><span data-stu-id="a53e4-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="a53e4-105">לפני שתסנכרן את המשתמשים והמחשבים שלך מהתחום המקומי של Active Directory, סקור את האפשרות [התכונן לסינכרון מדריכי כתובות ב-Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="a53e4-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="a53e4-106">בפרט:</span><span class="sxs-lookup"><span data-stu-id="a53e4-106">In particular:</span></span>

   - <span data-ttu-id="a53e4-107">ודא שהאפשרות ללא כפילויות קיימת במדריך הכתובות של התכונות הבאות: **mail**, **ProxyAddresses**ו- **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="a53e4-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="a53e4-108">ערכים אלה חייבים להיות ייחודיים ולהסיר כל כפילויות.</span><span class="sxs-lookup"><span data-stu-id="a53e4-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="a53e4-109">מומלץ לקבוע את תצורת התכונה **userPrincipalName** (UPN) עבור כל חשבון משתמש מקומי כדי להתאים לכתובת הדואר האלקטרוני הראשית התואמת למשתמש Microsoft 365 המורשה.</span><span class="sxs-lookup"><span data-stu-id="a53e4-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="a53e4-110">לדוגמה: *mary.shelley@contoso.com* ולא *mary@contoso. local*</span><span class="sxs-lookup"><span data-stu-id="a53e4-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="a53e4-111">אם התחום של Active Directory מסתיים בסיומת שאינה ניתנת לניתוב *, כגון.* lan או. lan, במקום סיומת לאינטרנט הניתנת לניתוב כגון *. com* או *.* *lan*, התאם את סיומת ה-UPN של חשבונות המשתמשים המקומיים תחילה כמתואר [בהכנת תחום שאינו ניתן לניתוב עבור סינכרון מדריכי כתובות](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="a53e4-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="a53e4-112">הפעל את **IdFix** בשלב 4 (4) להלן, ודא גם שמדריך Active Directory המקומי שלך מוכן לסינכרון של dir.</span><span class="sxs-lookup"><span data-stu-id="a53e4-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for dir sync.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="a53e4-113">2. התקנה וקביעת תצורה של התחברות למודעת תכלת</span><span class="sxs-lookup"><span data-stu-id="a53e4-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="a53e4-114">כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מ-Active Directory המקומי לתכלת Active Directory, התקן את תכלת Active Directory התחבר והגדר סינכרון מדריכי כתובות.</span><span class="sxs-lookup"><span data-stu-id="a53e4-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="a53e4-115">במרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> , בחר **הגדרה** בניווט הימני.</span><span class="sxs-lookup"><span data-stu-id="a53e4-115">In the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="a53e4-116">תחת **כניסה ואבטחה**, בחר **הצג**  תחת **סנכרן משתמשים ממדריך הארגון שלך**.</span><span class="sxs-lookup"><span data-stu-id="a53e4-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="a53e4-117">בדף **סינכרון משתמשים מתוך מדריך הכתובות של הארגון שלך** , בחר **תחילת**העבודה.</span><span class="sxs-lookup"><span data-stu-id="a53e4-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="a53e4-118">בכלי השלב הראשון של ההפעלה IdFix כדי להתכונן לסינכרון מדריכי כתובות.</span><span class="sxs-lookup"><span data-stu-id="a53e4-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="a53e4-119">בצע את שלבי האשף כדי להוריד את תכלת AD Connect והשתמש בו כדי לסנכרן את המשתמשים שנשלטים על-ידי התחום שלך ב-Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a53e4-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="a53e4-120">ראה [הגדרת סינכרון מדריכי כתובות עבור Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="a53e4-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="a53e4-121">בעת קביעת התצורה של האפשרויות עבור התחברות של תכלת לספירה, אנו ממליצים להפוך **סינכרון סיסמה**לזמין, **כניסה יחידה חלקה**והתכונה **Password writeback** , הנתמכת גם ב-Microsoft 365 for business.</span><span class="sxs-lookup"><span data-stu-id="a53e4-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="a53e4-122">קיימים כמה שלבים נוספים עבור סיסמה writeback מעבר לתיבת הסימון בקישור תכלת AD.</span><span class="sxs-lookup"><span data-stu-id="a53e4-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="a53e4-123">לקבלת מידע נוסף, ראה [כיצד לעשות זאת: קביעת תצורה של writeback password](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="a53e4-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="a53e4-124">אם ברצונך לנהל מכשירים המצורפים לתחום של Windows 10 בנוסף, ראה [הפיכת מכשירי windows 10 המצורפים לתחום למנוהל על-ידי Microsoft 365 Business Premium](manage-windows-devices.md) כדי להגדיר הצטרפות משולבת של תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="a53e4-124">If you want to manage domain-joined Windows 10 devices also, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 