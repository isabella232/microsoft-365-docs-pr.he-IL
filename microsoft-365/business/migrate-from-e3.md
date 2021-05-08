---
title: מעבר אל Microsoft 365 Business מ- Office 365 E3
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
search.appverid:
- BCS160
- MET150
description: למד כיצד להעביר את העסק שלך Microsoft 365 Business Premium מ- Office 365 E3.
ms.openlocfilehash: f08b054473fdd63ec2372e81c776a1b64f89fe9d
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/06/2021
ms.locfileid: "52244835"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="69265-103">מעבר מ- Office 365 E3 Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="69265-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span>

<span data-ttu-id="69265-104">Microsoft 365 Business Premium כולל את כל מה שאתה צריך עבור העסק הקטן שלך, המשלב את יישומי הפרודוקטיביות מבוססי הענן הטובים מסוגם עם ניהול מכשירים ואבטחה פשוטים.</span><span class="sxs-lookup"><span data-stu-id="69265-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="69265-105">אם יש לך כעת Office 365 E3, אך אין לך יותר מ- 300 עובדים, שקול לעבור ל- Microsoft 365 Business Premium לקבלת תכונות אבטחה נוספות.</span><span class="sxs-lookup"><span data-stu-id="69265-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="69265-106">העברה היא קלה: תחילה עליך להחליף רשיונות וכל הנתונים ומידע המשתמש שלך במנוי הנוכחי שלך נשמרים.</span><span class="sxs-lookup"><span data-stu-id="69265-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="69265-107">לאחר ההעברה, יהיה עליך להגדיר את התכונות שנוספו ב- Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="69265-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="69265-108">הבדלים בין Office 365 E3 לבין Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="69265-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="69265-109">טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium לבין Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="69265-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="69265-110">תכונה</span><span class="sxs-lookup"><span data-stu-id="69265-110">Feature</span></span>    | <span data-ttu-id="69265-111">תמיכה Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="69265-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="69265-112">תמיכה ב- Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="69265-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="69265-113">**מקומי**</span><span class="sxs-lookup"><span data-stu-id="69265-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="69265-114">Office<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="69265-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="69265-115">יישומי Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="69265-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="69265-116">יישומי Microsoft 365 עבור ארגונים</span><span class="sxs-lookup"><span data-stu-id="69265-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="69265-117">**יישומי פרודוקטיביות בענן**</span><span class="sxs-lookup"><span data-stu-id="69265-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="69265-118">Exchange Online ו- Outlook</span><span class="sxs-lookup"><span data-stu-id="69265-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="69265-119">מגבלת שטח אחסון של 50 GB לכל תיבת דואר אחסון בארכיון של Exchange Online</span><span class="sxs-lookup"><span data-stu-id="69265-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="69265-120">מגבלת שטח אחסון של 100 GB לכל תיבת דואר אחסון בארכיון של Exchange Online</span><span class="sxs-lookup"><span data-stu-id="69265-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="69265-121">Teams</span><span class="sxs-lookup"><span data-stu-id="69265-121">Teams</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="69265-124">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="69265-124">OneDrive for Business</span></span>    | <span data-ttu-id="69265-125">מגבלת אחסון של 1 TB לכל משתמש</span><span class="sxs-lookup"><span data-stu-id="69265-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="69265-126">ללא הגבלה</span><span class="sxs-lookup"><span data-stu-id="69265-126">Unlimited</span></span> | 
| <span data-ttu-id="69265-127">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="69265-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="69265-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="69265-130">StaffHub</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="69265-133">MileIQ</span><span class="sxs-lookup"><span data-stu-id="69265-133">MileIQ</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="69265-135">**הגנה מפני איומים**</span><span class="sxs-lookup"><span data-stu-id="69265-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="69265-136">Defender for Office 365 תוכנית 1</span><span class="sxs-lookup"><span data-stu-id="69265-136">Defender for Office 365 Plan 1</span></span> | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="69265-138">לא כלול, אך ניתן להוסיף אותו</span><span class="sxs-lookup"><span data-stu-id="69265-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="69265-139">**ניהול זהויות**</span><span class="sxs-lookup"><span data-stu-id="69265-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="69265-140">איפוס סיסמה בשירות עצמי עבור חשבונות היברידיים של Azure Active Directory (Azure AD), אימות רב-גורמי של Azure AD (MFA), Access מותן, writeback באמצעות סיסמה עבור זהויות מקומיות</span><span class="sxs-lookup"><span data-stu-id="69265-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| <span data-ttu-id="69265-142">**ניהול מכשירים ואפליקציות**</span><span class="sxs-lookup"><span data-stu-id="69265-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="69265-143">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="69265-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="69265-145">הפעלת מחשב משותף</span><span class="sxs-lookup"><span data-stu-id="69265-145">Shared computer activation</span></span>|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="69265-148">שדרוג זכויות Windows 10 Pro מתוך Win 7/8.1 Pro רשיונות</span><span class="sxs-lookup"><span data-stu-id="69265-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    || 
| <span data-ttu-id="69265-150">**הגנה על מידע**</span><span class="sxs-lookup"><span data-stu-id="69265-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="69265-151">Office 365 מניעת אובדן נתונים</span><span class="sxs-lookup"><span data-stu-id="69265-151">Office 365 Data Loss Prevention</span></span>|    ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)|![כלול ב- Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="69265-154">Azure Information Protection Plan 1, BitLocker אכיפה</span><span class="sxs-lookup"><span data-stu-id="69265-154">Azure Information Protection Plan 1, BitLocker enforcement</span></span>|![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="69265-156">Azure Information Protection Plan 1, תוויות רגישות</span><span class="sxs-lookup"><span data-stu-id="69265-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="69265-158">**לקוח Access רשיון (זכויות CAL)**</span><span class="sxs-lookup"><span data-stu-id="69265-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="69265-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="69265-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![כלול ב- Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="69265-161"><sup>1</sup> גירסת Microsoft 365 Business Premium של יישומי Office אינה כוללת הפעלת עוצמת קול באמצעות מדיניות קבוצתית, מדידת שימוש ביישומים, פקדים לעדכון, השוואה וחקירה של גיליון אלקטרוני או בינה עסקית.</span><span class="sxs-lookup"><span data-stu-id="69265-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="69265-162">העברה</span><span class="sxs-lookup"><span data-stu-id="69265-162">Migration</span></span>

<span data-ttu-id="69265-163">כדי להעביר את המנוי שלך, ראה [שינוי תוכניות באופן](../commerce/subscriptions/change-plans-manually.md) ידני לקבלת הוראות אם ברצונך להעביר רק כמה אנשים Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="69265-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="69265-164">באפשרותך גם לשדרג [את כולם באופן](../commerce/subscriptions/upgrade-to-different-plan.md)אוטומטי, או לעבוד עם שותף כדי להעביר את המנוי והרשיון שלך ל- E3 למנוי Microsoft 365 Business Premium שלך.</span><span class="sxs-lookup"><span data-stu-id="69265-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="69265-165">הסעיפים הבאים מתארים את השינויים שתצטרך לבצע, אם יש, ומה ניתן לעשות לאחר ההעברה.</span><span class="sxs-lookup"><span data-stu-id="69265-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="69265-166">Office 365 תצורה ונתונים של מנוי E3</span><span class="sxs-lookup"><span data-stu-id="69265-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="69265-167">אין צורך לבצע שינויים כלשהם במנוי או בנתונים הנוכחיים שלך לפני המעבר, הכולל:</span><span class="sxs-lookup"><span data-stu-id="69265-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="69265-168">תצורת מנוי, כגון רשומות DNS ושמות תחומים.</span><span class="sxs-lookup"><span data-stu-id="69265-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="69265-169">חשבונות משתמשים וקבוצתיים והגדרות אימות, כגון אימות רב גורמי או פריטי מדיניות גישה מותנים.</span><span class="sxs-lookup"><span data-stu-id="69265-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="69265-170">תצורות שירות פרודוקטיביות והנתונים שלהן, כגון Teams, Exchange Online דואר, SharePoint Online, תיקיות OneDrive for Business ומחברות OneNote אחרות.</span><span class="sxs-lookup"><span data-stu-id="69265-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="69265-171">Office יתונו באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="69265-171">Office applications will scale automatically.</span></span> <span data-ttu-id="69265-172">Office 365 רישוי מודרני יבדוק את הקצאת הרשיונות של המשתמש כל 72 שעות ותמיר Office יישומים לגירסה התואמת למנוי המשתמש.</span><span class="sxs-lookup"><span data-stu-id="69265-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="69265-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="69265-173">Windows 10</span></span>

<span data-ttu-id="69265-174">אם Windows שלך עדיין לא נמצא בעדכון Windows Pro הבורא, שדרג אותם [לעדכון Windows Pro ליוצרים](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="69265-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="69265-175">הגדרת פריטי מדיניות להגנה על מכשירים וקבצים של משתמשים</span><span class="sxs-lookup"><span data-stu-id="69265-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="69265-176">אם תגדיר Office 365 והתקנים של MDM, מכשירים אלה יופיעו בדף **מכשירים** במרכז Microsoft 365 הניהול.</span><span class="sxs-lookup"><span data-stu-id="69265-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="69265-177">כל פריטי המדיניות שתגדיר יופיעו ברשימת פריטי המדיניות הקלאסיים [בפורטל Intune](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span><span class="sxs-lookup"><span data-stu-id="69265-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="69265-178">לאחר הקצאת רשיונות ל- Microsoft 365 Business Premium, באפשרותך להתחיל להגן על המכשירים והקבצים של המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="69265-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="69265-179">אם שידרגת את כל האנשים בארגון שלך Microsoft 365 Business Premium, תראה את אשף ההגדרה בדף הבית, ופעל בהתאם להגדרה [Microsoft 365 Business Premium בשלבי](set-up.md) אשף ההגדרה כדי להגן על קבצים ומכשירים ניידים.</span><span class="sxs-lookup"><span data-stu-id="69265-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="69265-180">באפשרותך גם להשלים שלבים אלה בדף מכשירים:</span><span class="sxs-lookup"><span data-stu-id="69265-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="69265-181">במרכז הניהול, בסרגל הניווט הימני, עבור אל **מדיניות** \> **מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="69265-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="69265-182">בדף מדיניות **מכשיר,** בחר **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="69265-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="69265-183">בחלונית **הוספת** מדיניות, תן למדיניות שם ולאחר מכן בחר **סוג מדיניות** מהרשימה הנפתחת.</span><span class="sxs-lookup"><span data-stu-id="69265-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="69265-184">באפשרותך להגדיר מדיניות יישומים להגנה על קבצים במכשירי Android ו- iPhone, וכן Windows 10, וכן להגדיר מדיניות תצורה של מכשיר עבור מכשירי Windows 10 חברה.</span><span class="sxs-lookup"><span data-stu-id="69265-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="69265-185">עיין בקישורים הבאים לקבלת פרטים:</span><span class="sxs-lookup"><span data-stu-id="69265-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="69265-186">קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS</span><span class="sxs-lookup"><span data-stu-id="69265-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="69265-187">קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10</span><span class="sxs-lookup"><span data-stu-id="69265-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="69265-188">הגדרת הגדרות הגנה על מכשיר עבור Windows 10 אישיים</span><span class="sxs-lookup"><span data-stu-id="69265-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="69265-189">לאחר הגדרת מדיניות, אתה והעובדים שלך יכולים להגדיר מכשירים:</span><span class="sxs-lookup"><span data-stu-id="69265-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="69265-190">ראה [הגדרת Windows עבור משתמשים Microsoft 365 Business Premium לקבלת](set-up-windows-devices.md) שלבים עבור Windows אחרים.</span><span class="sxs-lookup"><span data-stu-id="69265-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="69265-191">ראה [הגדרת מכשירים ניידים עבור Microsoft 365 Business Premium עבור](set-up-mobile-devices.md) שלבים עבור טלפונים ומכשירי iPhone של Android.</span><span class="sxs-lookup"><span data-stu-id="69265-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="69265-192">גודל תיבת דואר</span><span class="sxs-lookup"><span data-stu-id="69265-192">Mailbox Size</span></span>

<span data-ttu-id="69265-193">Microsoft 365 Business Premium יש מגבלת אחסון של 50 GB כאשר היא משתמשת Exchange Online תוכנית 1.</span><span class="sxs-lookup"><span data-stu-id="69265-193">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="69265-194">בעת המעבר ל- Microsoft 365 Business Premium, אם אחד מהמשתמשים שלך חורג מ- 50 GB של שטח אחסון בתיבות דואר, מומלץ להקצות למשתמש זה תוכנית Exchange Online תוכנית 2 ולהסיר את תוכנית Exchange Online 1, כי לא ניתן להקצות את שניהם.</span><span class="sxs-lookup"><span data-stu-id="69265-194">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>


### <a name="threat-protection"></a><span data-ttu-id="69265-195">הגנה מפני איומים</span><span class="sxs-lookup"><span data-stu-id="69265-195">Threat protection</span></span>

<span data-ttu-id="69265-196">לאחר המעבר ל- Microsoft 365 Business Premium, יש לך את Defender Office 365.</span><span class="sxs-lookup"><span data-stu-id="69265-196">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="69265-197">עיין [ב- Microsoft Defender לקבלת Office 365 לקבלת](../security/office-365-security/defender-for-office-365.md) מבט כולל.</span><span class="sxs-lookup"><span data-stu-id="69265-197">See [Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md) for an overview.</span></span> <span data-ttu-id="69265-198">כדי להגדיר, ראה [הגדרת קישורים בטוחים](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [הגדרת](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)קבצים מצורפים בטוחים והגדרת מניעת דיוג [ב- Defender עבור Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span><span class="sxs-lookup"><span data-stu-id="69265-198">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="69265-199">תוויות רגישות</span><span class="sxs-lookup"><span data-stu-id="69265-199">Sensitivity labels</span></span>

<span data-ttu-id="69265-200">כדי להתחיל להשתמש בתוויות רגישות, ראה [מבט כולל על תוויות רגישות](../compliance/sensitivity-labels.md) [ויצירה וניהול של תוויות רגישות](../business-video/create-sensitivity-labels.md) וידאו.</span><span class="sxs-lookup"><span data-stu-id="69265-200">To start using sensitivity labels, see [Overview of sensitivity labels](../compliance/sensitivity-labels.md) and [create and manage sensitivity labels](../business-video/create-sensitivity-labels.md) video.</span></span>
