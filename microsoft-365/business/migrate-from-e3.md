---
title: מעבר ל- Microsoft 365 Business מ- Office 365 E3
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
description: אם יש לך מנוי Office 365 E3 אך אין לך יותר מ- 300 עובדים, שקול לעבור Microsoft 365 Business Premium.
ms.openlocfilehash: c1b4da07b3bf28cce1a48424ab45cde6ea54d367
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/12/2021
ms.locfileid: "53394170"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="29aaa-103">מעבר מ- Office 365 E3 אל Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="29aaa-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span>

<span data-ttu-id="29aaa-104">Microsoft 365 Business Premium כולל את כל מה שאתה צריך עבור העסק הקטן שלך, המשלב את יישומי הפרודוקטיביות מבוססי הענן הטובים מסוגם עם ניהול מכשירים ואבטחה פשוטים.</span><span class="sxs-lookup"><span data-stu-id="29aaa-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="29aaa-105">אם יש לך כעת מנוי Office 365 E3, אך אין לך יותר מ- 300 עובדים, שקול לעבור ל- Microsoft 365 Business Premium לקבלת תכונות אבטחה נוספות.</span><span class="sxs-lookup"><span data-stu-id="29aaa-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="29aaa-106">העברה היא קלה: תחילה עליך להחליף רשיונות וכל הנתונים ומידע המשתמש שלך במנוי הנוכחי שלך נשמרים.</span><span class="sxs-lookup"><span data-stu-id="29aaa-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="29aaa-107">לאחר ההעברה, יהיה עליך להגדיר את התכונות שנוספו ב- Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="29aaa-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="29aaa-108">הבדלים בין Office 365 E3 לבין Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="29aaa-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="29aaa-109">טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium לבין Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="29aaa-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="29aaa-110">תכונה</span><span class="sxs-lookup"><span data-stu-id="29aaa-110">Feature</span></span>    | <span data-ttu-id="29aaa-111">תמיכה Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="29aaa-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="29aaa-112">תמיכה Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="29aaa-112">Support in Office 365 E3</span></span> |
|:-------|:-----|:-----|
| <span data-ttu-id="29aaa-113">**מקומי**</span><span class="sxs-lookup"><span data-stu-id="29aaa-113">**On-premises**</span></span>        | | |
| <span data-ttu-id="29aaa-114">Office<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="29aaa-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="29aaa-115">יישומי Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="29aaa-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="29aaa-116">יישומי Microsoft 365 עבור ארגונים</span><span class="sxs-lookup"><span data-stu-id="29aaa-116">Microsoft 365 Apps for enterprise</span></span> |
| <span data-ttu-id="29aaa-117">**יישומי פרודוקטיביות בענן**</span><span class="sxs-lookup"><span data-stu-id="29aaa-117">**Cloud productivity apps**</span></span>        | | |
| <span data-ttu-id="29aaa-118">Exchange Online ו- Outlook</span><span class="sxs-lookup"><span data-stu-id="29aaa-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="29aaa-119">מגבלת שטח אחסון של 50 GB לכל תיבת דואר אחסון בארכיון של Exchange Online</span><span class="sxs-lookup"><span data-stu-id="29aaa-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="29aaa-120">מגבלת שטח אחסון של 100 GB לכל תיבת דואר אחסון בארכיון של Exchange Online</span><span class="sxs-lookup"><span data-stu-id="29aaa-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> |
| <span data-ttu-id="29aaa-121">Teams</span><span class="sxs-lookup"><span data-stu-id="29aaa-121">Teams</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="29aaa-124">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="29aaa-124">OneDrive for Business</span></span>    | <span data-ttu-id="29aaa-125">מגבלת אחסון של 1 TB לכל משתמש</span><span class="sxs-lookup"><span data-stu-id="29aaa-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="29aaa-126">ללא הגבלה</span><span class="sxs-lookup"><span data-stu-id="29aaa-126">Unlimited</span></span> | 
| <span data-ttu-id="29aaa-127">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="29aaa-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="29aaa-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="29aaa-130">StaffHub</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) |
| <span data-ttu-id="29aaa-133">**הגנה מפני איומים**</span><span class="sxs-lookup"><span data-stu-id="29aaa-133">**Threat Protection**</span></span>        | | |
| <span data-ttu-id="29aaa-134">Defender for Office 365 תוכנית 1</span><span class="sxs-lookup"><span data-stu-id="29aaa-134">Defender for Office 365 Plan 1</span></span> | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="29aaa-136">לא כלול, אך ניתן להוסיף אותו</span><span class="sxs-lookup"><span data-stu-id="29aaa-136">Not included, but can be added on</span></span> |
| <span data-ttu-id="29aaa-137">**ניהול זהויות**</span><span class="sxs-lookup"><span data-stu-id="29aaa-137">**Identity management**</span></span>        | | |
| <span data-ttu-id="29aaa-138">איפוס סיסמה בשירות עצמי עבור חשבונות היברידיים של Azure Active Directory (Azure AD), אימות רב-גורמי של Azure AD (MFA), Access מותן, writeback באמצעות סיסמה עבור זהויות מקומיות</span><span class="sxs-lookup"><span data-stu-id="29aaa-138">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="29aaa-140">**ניהול מכשירים ואפליקציות**</span><span class="sxs-lookup"><span data-stu-id="29aaa-140">**Device and app management**</span></span>        | | |
| <span data-ttu-id="29aaa-141">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="29aaa-141">Microsoft Intune, Windows AutoPilot</span></span>|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="29aaa-143">הפעלת מחשב משותף</span><span class="sxs-lookup"><span data-stu-id="29aaa-143">Shared computer activation</span></span>|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="29aaa-146">שדרוג זכויות Windows 10 Pro מתוך Win 7/8.1 Pro רשיונות</span><span class="sxs-lookup"><span data-stu-id="29aaa-146">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    ||
| <span data-ttu-id="29aaa-148">**הגנה על מידע**</span><span class="sxs-lookup"><span data-stu-id="29aaa-148">**Information protection**</span></span>        | | |
|<span data-ttu-id="29aaa-149">Office 365 מניעת אובדן נתונים</span><span class="sxs-lookup"><span data-stu-id="29aaa-149">Office 365 Data Loss Prevention</span></span>|    ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)|![כלול ב- Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="29aaa-152">תוכנית הגנה מפני מידע של Azure 1, אכיפת BitLocker</span><span class="sxs-lookup"><span data-stu-id="29aaa-152">Azure Information Protection Plan 1, BitLocker enforcement</span></span>|![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="29aaa-154">Azure Information Protection Plan 1, תוויות רגישות</span><span class="sxs-lookup"><span data-stu-id="29aaa-154">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="29aaa-156">**לקוח Access רשיון (זכויות CAL)**</span><span class="sxs-lookup"><span data-stu-id="29aaa-156">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="29aaa-157">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="29aaa-157">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![כלול ב- Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="29aaa-159"><sup>1</sup> גירסת Microsoft 365 Business Premium של יישומי Office אינה כוללת הפעלת עוצמת קול באמצעות מדיניות קבוצתית, מדידת שימוש ביישומים, פקדים לעדכון, השוואה וחקירה של גיליון אלקטרוני או בינה עסקית.</span><span class="sxs-lookup"><span data-stu-id="29aaa-159"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="29aaa-160">העברה</span><span class="sxs-lookup"><span data-stu-id="29aaa-160">Migration</span></span>

<span data-ttu-id="29aaa-161">כדי להעביר את המנוי שלך, ראה [שינוי תוכניות באופן](../commerce/subscriptions/change-plans-manually.md) ידני לקבלת הוראות אם ברצונך להעביר רק כמה אנשים Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="29aaa-161">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="29aaa-162">באפשרותך גם לשדרג [את כולם באופן](../commerce/subscriptions/upgrade-to-different-plan.md)אוטומטי, או לעבוד עם שותף כדי להעביר את המנוי והרשיון שלך ל- E3 למנוי Microsoft 365 Business Premium שלך.</span><span class="sxs-lookup"><span data-stu-id="29aaa-162">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="29aaa-163">הסעיפים הבאים מתארים את השינויים שתצטרך לבצע, אם יש, ומה ניתן לעשות לאחר ההעברה.</span><span class="sxs-lookup"><span data-stu-id="29aaa-163">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="29aaa-164">Office 365 E3 תצורה ונתונים של מנוי</span><span class="sxs-lookup"><span data-stu-id="29aaa-164">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="29aaa-165">אין צורך לבצע שינויים כלשהם במנוי או בנתונים הנוכחיים שלך לפני המעבר, הכולל:</span><span class="sxs-lookup"><span data-stu-id="29aaa-165">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="29aaa-166">תצורת מנוי, כגון רשומות DNS ושמות תחומים.</span><span class="sxs-lookup"><span data-stu-id="29aaa-166">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="29aaa-167">חשבונות משתמשים וקבוצתיים והגדרות אימות, כגון אימות רב גורמי או פריטי מדיניות גישה מותנים.</span><span class="sxs-lookup"><span data-stu-id="29aaa-167">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="29aaa-168">תצורות שירות פרודוקטיביות והנתונים שלהן, כגון Teams, Exchange Online דואר, SharePoint Online, תיקיות OneDrive for Business ומחברות OneNote אחרות.</span><span class="sxs-lookup"><span data-stu-id="29aaa-168">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="29aaa-169">Office יתונו באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="29aaa-169">Office applications will scale automatically.</span></span> <span data-ttu-id="29aaa-170">Office 365 רישוי מודרני יבדוק את הקצאת הרשיונות של המשתמש כל 72 שעות ותמיר Office יישומים לגירסה התואמת למנוי המשתמש.</span><span class="sxs-lookup"><span data-stu-id="29aaa-170">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="29aaa-171">Windows 10</span><span class="sxs-lookup"><span data-stu-id="29aaa-171">Windows 10</span></span>

<span data-ttu-id="29aaa-172">אם Windows שלך עדיין לא נמצא בעדכון Windows Pro הבורא, שדרג אותם [לעדכון Windows Pro ליוצרים](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="29aaa-172">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="29aaa-173">הגדרת פריטי מדיניות להגנה על מכשירים וקבצים של משתמשים</span><span class="sxs-lookup"><span data-stu-id="29aaa-173">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="29aaa-174">אם תגדיר Office 365 והתקנים של MDM, מכשירים אלה יופיעו בדף **מכשירים** מרכז הניהול של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="29aaa-174">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="29aaa-175">כל פריטי המדיניות שתגדיר יופיעו ברשימת פריטי המדיניות הקלאסיים [בפורטל Intune](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span><span class="sxs-lookup"><span data-stu-id="29aaa-175">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="29aaa-176">לאחר הקצאת רשיונות ל- Microsoft 365 Business Premium, באפשרותך להתחיל להגן על המכשירים והקבצים של המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="29aaa-176">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="29aaa-177">אם שידרגת את כל האנשים בארגון שלך Microsoft 365 Business Premium, תראה את אשף ההגדרה בדף הבית, ופעל בהתאם להגדרה [Microsoft 365 Business Premium בשלבי](set-up.md) אשף ההגדרה כדי להגן על קבצים ומכשירים ניידים.</span><span class="sxs-lookup"><span data-stu-id="29aaa-177">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="29aaa-178">באפשרותך גם להשלים שלבים אלה בדף מכשירים:</span><span class="sxs-lookup"><span data-stu-id="29aaa-178">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="29aaa-179">במרכז הניהול, בסרגל הניווט הימני, עבור אל **מדיניות** \> **מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="29aaa-179">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>

2. <span data-ttu-id="29aaa-180">בדף מדיניות **מכשיר,** בחר **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="29aaa-180">On the **Device policies** page, choose **Add**.</span></span>

3. <span data-ttu-id="29aaa-181">בחלונית **הוספת** מדיניות, תן למדיניות שם ולאחר מכן בחר **סוג מדיניות** מהרשימה הנפתחת.</span><span class="sxs-lookup"><span data-stu-id="29aaa-181">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span>

     <span data-ttu-id="29aaa-182">באפשרותך להגדיר מדיניות יישומים להגנה על קבצים במכשירי Android ו- iPhone, וכן Windows 10, וכן להגדיר מדיניות תצורה של מכשיר עבור מכשירי Windows 10 חברה.</span><span class="sxs-lookup"><span data-stu-id="29aaa-182">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="29aaa-183">עיין בקישורים הבאים לקבלת פרטים:</span><span class="sxs-lookup"><span data-stu-id="29aaa-183">See the following links for details:</span></span>

  - [<span data-ttu-id="29aaa-184">קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS</span><span class="sxs-lookup"><span data-stu-id="29aaa-184">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)

  - [<span data-ttu-id="29aaa-185">קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10</span><span class="sxs-lookup"><span data-stu-id="29aaa-185">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)

  - [<span data-ttu-id="29aaa-186">הגדרת הגדרות הגנה על מכשיר עבור Windows 10 אישיים</span><span class="sxs-lookup"><span data-stu-id="29aaa-186">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="29aaa-187">לאחר הגדרת מדיניות, אתה והעובדים שלך יכולים להגדיר מכשירים:</span><span class="sxs-lookup"><span data-stu-id="29aaa-187">Once you set up policies, you and your employees can set up devices:</span></span>

  - <span data-ttu-id="29aaa-188">ראה [הגדרת Windows עבור משתמשים Microsoft 365 Business Premium לקבלת](set-up-windows-devices.md) שלבים עבור Windows אחרים.</span><span class="sxs-lookup"><span data-stu-id="29aaa-188">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 

  - <span data-ttu-id="29aaa-189">ראה [הגדרת מכשירים ניידים עבור Microsoft 365 Business Premium עבור](set-up-mobile-devices.md) שלבים עבור טלפונים ומכשירי iPhone של Android.</span><span class="sxs-lookup"><span data-stu-id="29aaa-189">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="29aaa-190">גודל תיבת דואר</span><span class="sxs-lookup"><span data-stu-id="29aaa-190">Mailbox Size</span></span>

<span data-ttu-id="29aaa-191">Microsoft 365 Business Premium יש מגבלת אחסון של 50 GB כאשר היא משתמשת Exchange Online תוכנית 1.</span><span class="sxs-lookup"><span data-stu-id="29aaa-191">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="29aaa-192">בעת המעבר ל- Microsoft 365 Business Premium, אם אחד מהמשתמשים שלך חורג מ- 50 GB של שטח אחסון בתיבות דואר, מומלץ להקצות למשתמש זה תוכנית Exchange Online תוכנית 2 ולהסיר את תוכנית Exchange Online 1, כי לא ניתן להקצות את שניהם.</span><span class="sxs-lookup"><span data-stu-id="29aaa-192">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>

### <a name="threat-protection"></a><span data-ttu-id="29aaa-193">הגנה מפני איומים</span><span class="sxs-lookup"><span data-stu-id="29aaa-193">Threat protection</span></span>

<span data-ttu-id="29aaa-194">לאחר המעבר ל- Microsoft 365 Business Premium, יש לך את Defender Office 365.</span><span class="sxs-lookup"><span data-stu-id="29aaa-194">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="29aaa-195">עיין [ב- Microsoft Defender לקבלת Office 365 לקבלת](../security/office-365-security/defender-for-office-365.md) מבט כולל.</span><span class="sxs-lookup"><span data-stu-id="29aaa-195">See [Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md) for an overview.</span></span> <span data-ttu-id="29aaa-196">כדי להגדיר, ראה [הגדרת כספת קישורים](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), הגדרת [כספת](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)קבצים מצורפים ו הגדרת מניעת דיוג [ב- Defender עבור Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span><span class="sxs-lookup"><span data-stu-id="29aaa-196">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="29aaa-197">תוויות רגישות</span><span class="sxs-lookup"><span data-stu-id="29aaa-197">Sensitivity labels</span></span>

<span data-ttu-id="29aaa-198">כדי להתחיל להשתמש בתוויות רגישות, ראה [מבט כולל על תוויות רגישות](../compliance/sensitivity-labels.md) [ויצירה וניהול של תוויות רגישות](../business-video/create-sensitivity-labels.md) וידאו.</span><span class="sxs-lookup"><span data-stu-id="29aaa-198">To start using sensitivity labels, see [Overview of sensitivity labels](../compliance/sensitivity-labels.md) and [create and manage sensitivity labels](../business-video/create-sensitivity-labels.md) video.</span></span>

## <a name="related-content"></a><span data-ttu-id="29aaa-199">תוכן קשור</span><span class="sxs-lookup"><span data-stu-id="29aaa-199">Related content</span></span>

<span data-ttu-id="29aaa-200">[שינוי תוכניות באופן ידני](../commerce/subscriptions/change-plans-manually.md) (מאמר)</span><span class="sxs-lookup"><span data-stu-id="29aaa-200">[Change plans manually](../commerce/subscriptions/change-plans-manually.md) (article)</span></span>\
<span data-ttu-id="29aaa-201">[שדרוג Windows למכשירי Windows 10 Pro](upgrade-to-windows-pro-creators-update.md) (וידאו)</span><span class="sxs-lookup"><span data-stu-id="29aaa-201">[Upgrade Windows devices to Windows 10 Pro](upgrade-to-windows-pro-creators-update.md) (video)</span></span>\
<span data-ttu-id="29aaa-202">[הגדרת הגדרות הגנה על יישומים עבור מכשירי Android או iOS](app-protection-settings-for-android-and-ios.md) (מאמר)</span><span class="sxs-lookup"><span data-stu-id="29aaa-202">[Set app protection settings for Android or iOS devices](app-protection-settings-for-android-and-ios.md) (article)</span></span>\
<span data-ttu-id="29aaa-203">[הגדרה או עריכה של הגדרות הגנת יישומים עבור Windows 10](protection-settings-for-windows-10-devices.md) (מאמר)</span><span class="sxs-lookup"><span data-stu-id="29aaa-203">[Set or edit application protection settings for Windows 10 devices](protection-settings-for-windows-10-devices.md) (article)</span></span>\
<span data-ttu-id="29aaa-204">[]</span><span class="sxs-lookup"><span data-stu-id="29aaa-204">[]</span></span>

