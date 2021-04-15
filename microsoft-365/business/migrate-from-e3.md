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
search.appverid:
- BCS160
- MET150
description: למד כיצד להעביר את העסק שלך ל- Microsoft 365 Business Premium מ- Office 365 E3.
ms.openlocfilehash: f2b7962918186f4a1063c5a66596135c2972ec71
ms.sourcegitcommit: 07dea2aa98daf0c4086f8590375167830027c802
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/13/2021
ms.locfileid: "51749999"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="be95b-103">העברה מ- Office 365 E3 ל- Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="be95b-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span>

<span data-ttu-id="be95b-104">Microsoft 365 Business Premium כולל את כל מה שאתה צריך עבור העסק הקטן שלך, המשלב את יישומי הפרודוקטיביות מבוססי הענן הטובים ביותר מסוגם עם ניהול ואבטחה פשוטים של מכשירים.</span><span class="sxs-lookup"><span data-stu-id="be95b-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="be95b-105">אם יש לך כעת מנוי Office 365 E3, אך אין לך יותר מ- 300 עובדים, שקול לעבור ל- Microsoft 365 Business Premium לקבלת תכונות אבטחה נוספות.</span><span class="sxs-lookup"><span data-stu-id="be95b-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="be95b-106">העברה היא קלה: תחילה עליך להחליף רשיונות וכל הנתונים ומידע המשתמש שלך במנוי הנוכחי שלך נשמרים.</span><span class="sxs-lookup"><span data-stu-id="be95b-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="be95b-107">לאחר ההעברה, יהיה עליך להגדיר את התכונות שנוספו ב- Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="be95b-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="be95b-108">הבדלים בין Office 365 E3 לבין Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="be95b-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="be95b-109">טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium לבין Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="be95b-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="be95b-110">תכונה</span><span class="sxs-lookup"><span data-stu-id="be95b-110">Feature</span></span>    | <span data-ttu-id="be95b-111">תמיכה ב- Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="be95b-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="be95b-112">תמיכה ב- Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="be95b-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="be95b-113">**מקומי**</span><span class="sxs-lookup"><span data-stu-id="be95b-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="be95b-114">יישומי Office<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="be95b-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="be95b-115">יישומי Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="be95b-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="be95b-116">יישומי Microsoft 365 עבור ארגונים</span><span class="sxs-lookup"><span data-stu-id="be95b-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="be95b-117">**יישומי פרודוקטיביות בענן**</span><span class="sxs-lookup"><span data-stu-id="be95b-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="be95b-118">Exchange Online ו- Outlook</span><span class="sxs-lookup"><span data-stu-id="be95b-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="be95b-119">מגבלת אחסון של 50 GB לכל תיבת דואר ואחסון בארכיון בלתי מוגבל של Exchange Online</span><span class="sxs-lookup"><span data-stu-id="be95b-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="be95b-120">מגבלת אחסון של 100 GB לכל תיבת דואר ואחסון בארכיון בלתי מוגבל של Exchange Online</span><span class="sxs-lookup"><span data-stu-id="be95b-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="be95b-121">Teams</span><span class="sxs-lookup"><span data-stu-id="be95b-121">Teams</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="be95b-124">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="be95b-124">OneDrive for Business</span></span>    | <span data-ttu-id="be95b-125">מגבלת אחסון של 1 TB לכל משתמש</span><span class="sxs-lookup"><span data-stu-id="be95b-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="be95b-126">ללא הגבלה</span><span class="sxs-lookup"><span data-stu-id="be95b-126">Unlimited</span></span> | 
| <span data-ttu-id="be95b-127">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="be95b-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="be95b-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="be95b-130">StaffHub</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="be95b-133">MileIQ</span><span class="sxs-lookup"><span data-stu-id="be95b-133">MileIQ</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="be95b-135">**הגנה מפני איומים**</span><span class="sxs-lookup"><span data-stu-id="be95b-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="be95b-136">Defender for Office 365 Plan 1</span><span class="sxs-lookup"><span data-stu-id="be95b-136">Defender for Office 365 Plan 1</span></span> | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="be95b-138">לא כלול, אך ניתן להוסיף אותו</span><span class="sxs-lookup"><span data-stu-id="be95b-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="be95b-139">**ניהול זהויות**</span><span class="sxs-lookup"><span data-stu-id="be95b-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="be95b-140">איפוס סיסמה בשירות עצמי עבור חשבונות היברידיים של Azure Active Directory (Azure AD), אימות רב-גורמי של Azure AD (MFA), Access מותן, writeback באמצעות סיסמה עבור זהויות מקומיות</span><span class="sxs-lookup"><span data-stu-id="be95b-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| <span data-ttu-id="be95b-142">**ניהול מכשירים ואפליקציות**</span><span class="sxs-lookup"><span data-stu-id="be95b-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="be95b-143">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="be95b-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="be95b-145">הפעלת מחשב משותף</span><span class="sxs-lookup"><span data-stu-id="be95b-145">Shared computer activation</span></span>|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="be95b-148">זכויות שדרוג ל- Windows 10 Pro מ- Win 7/8.1 Pro</span><span class="sxs-lookup"><span data-stu-id="be95b-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    || 
| <span data-ttu-id="be95b-150">**הגנה על מידע**</span><span class="sxs-lookup"><span data-stu-id="be95b-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="be95b-151">מניעת אובדן נתונים של Office 365</span><span class="sxs-lookup"><span data-stu-id="be95b-151">Office 365 Data Loss Prevention</span></span>|    ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)|![כלול ב- Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="be95b-154">תוכנית הגנה מפני מידע של Azure 1, אכיפת BitLocker</span><span class="sxs-lookup"><span data-stu-id="be95b-154">Azure Information Protection Plan 1, BitLocker enforcement</span></span>|![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="be95b-156">Azure Information Protection Plan 1, תוויות רגישות</span><span class="sxs-lookup"><span data-stu-id="be95b-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="be95b-158">**לקוח Access רשיון (זכויות CAL)**</span><span class="sxs-lookup"><span data-stu-id="be95b-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="be95b-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="be95b-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![כלול ב- Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="be95b-161"><sup>1</sup> גירסת Microsoft 365 Business Premium של יישומי Office אינה כוללת הפעלת עוצמת קול באמצעות מדיניות קבוצתית, מדידת שימוש ביישומים, פקדים לעדכון, השוואה וחקירה של גיליון אלקטרוני או בינה עסקית.</span><span class="sxs-lookup"><span data-stu-id="be95b-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="be95b-162">העברה</span><span class="sxs-lookup"><span data-stu-id="be95b-162">Migration</span></span>

<span data-ttu-id="be95b-163">כדי להעביר את המנוי שלך, ראה [שינוי תוכניות](../commerce/subscriptions/change-plans-manually.md) באופן ידני לקבלת הוראות אם ברצונך להעביר רק כמה אנשים ל- Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="be95b-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="be95b-164">באפשרותך גם לשדרג [את כולם באופן אוטומטי,](../commerce/subscriptions/upgrade-to-different-plan.md)או לעבוד עם שותף כדי להעביר את המנוי והרשיון שלך ל- Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="be95b-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="be95b-165">הסעיפים הבאים מתארים את השינויים שתצטרך לבצע, אם יש, ומה ניתן לעשות לאחר ההעברה.</span><span class="sxs-lookup"><span data-stu-id="be95b-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="be95b-166">קביעת תצורה ונתונים של מנוי Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="be95b-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="be95b-167">אין צורך לבצע שינויים כלשהם במנוי או בנתונים הנוכחיים שלך לפני המעבר, הכולל:</span><span class="sxs-lookup"><span data-stu-id="be95b-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="be95b-168">תצורת מנוי, כגון רשומות DNS ושמות תחומים.</span><span class="sxs-lookup"><span data-stu-id="be95b-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="be95b-169">חשבונות משתמשים וקבוצתיים והגדרות אימות, כגון אימות רב גורמי או פריטי מדיניות גישה מותנים.</span><span class="sxs-lookup"><span data-stu-id="be95b-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="be95b-170">תצורות שירות פרודוקטיביות והנתונים שלהם, כגון Teams, תיבות דואר של Exchange Online, אתרי SharePoint Online, תיקיות OneDrive for Business ומחברות OneNote.</span><span class="sxs-lookup"><span data-stu-id="be95b-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="be95b-171">יישומי Office יתווו את קנה המידה באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="be95b-171">Office applications will scale automatically.</span></span> <span data-ttu-id="be95b-172">רישוי מודרני של Office 365 יבדוק את הקצאת הרשיונות של המשתמש כל 72 שעות ותמיר יישומי Office לגירסה התואמת למנוי המשתמש.</span><span class="sxs-lookup"><span data-stu-id="be95b-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="be95b-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="be95b-173">Windows 10</span></span>

<span data-ttu-id="be95b-174">אם Windows שלך עדיין לא נמצא בעדכון Windows Pro Creator, [שדרג אותם לעדכון יוצרי Windows Pro](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="be95b-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="be95b-175">הגדרת פריטי מדיניות להגנה על מכשירים וקבצים של משתמשים</span><span class="sxs-lookup"><span data-stu-id="be95b-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="be95b-176">אם תגדיר פריטי מדיניות ומכשירי MDM של Office 365,  מכשירים אלה יופיעו בדף מכשירים במרכז הניהול של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="be95b-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="be95b-177">כל פריטי המדיניות שתגדיר יופיעו ברשימת פריטי המדיניות הקלאסיים [בפורטל Intune](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span><span class="sxs-lookup"><span data-stu-id="be95b-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="be95b-178">לאחר הקצאת רשיונות ל- Microsoft 365 Business Premium, באפשרותך להתחיל להגן על המכשירים והקבצים של המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="be95b-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="be95b-179">אם שידרגת את כל האנשים בארגון שלך ל- Microsoft 365 Business Premium, תראה את אשף ההגדרה בדף הבית, ופעל בהתאם להגדרה [של Microsoft 365 Business Premium](set-up.md) בשלבי אשף ההגדרה כדי להגן על קבצים ומכשירים ניידים.</span><span class="sxs-lookup"><span data-stu-id="be95b-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="be95b-180">באפשרותך גם להשלים שלבים אלה בדף מכשירים:</span><span class="sxs-lookup"><span data-stu-id="be95b-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="be95b-181">במרכז הניהול, בסרגל הניווט הימני, עבור אל **מדיניות** \> **מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="be95b-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="be95b-182">בדף מדיניות **מכשיר,** בחר **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="be95b-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="be95b-183">בחלונית **הוספת** מדיניות, תן למדיניות שם ולאחר מכן בחר **סוג מדיניות** מהרשימה הנפתחת.</span><span class="sxs-lookup"><span data-stu-id="be95b-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="be95b-184">באפשרותך להגדיר מדיניות יישומים להגנה על קבצים במכשירי Android ו- iPhone, וכן Windows 10, וכן להגדיר מדיניות תצורה של מכשיר עבור מכשירי Windows 10 בבעלות החברה.</span><span class="sxs-lookup"><span data-stu-id="be95b-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="be95b-185">עיין בקישורים הבאים לקבלת פרטים:</span><span class="sxs-lookup"><span data-stu-id="be95b-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="be95b-186">קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS</span><span class="sxs-lookup"><span data-stu-id="be95b-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="be95b-187">קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10</span><span class="sxs-lookup"><span data-stu-id="be95b-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="be95b-188">הגדרת הגדרות הגנה על מכשיר עבור מחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="be95b-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="be95b-189">לאחר הגדרת מדיניות, אתה והעובדים שלך יכולים להגדיר מכשירים:</span><span class="sxs-lookup"><span data-stu-id="be95b-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="be95b-190">ראה [הגדרת מכשירי Windows עבור משתמשי Microsoft 365 Business Premium לקבלת שלבים](set-up-windows-devices.md) עבור מכשירי Windows.</span><span class="sxs-lookup"><span data-stu-id="be95b-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="be95b-191">ראה [הגדרת מכשירים ניידים עבור משתמשי Microsoft 365 Business Premium](set-up-mobile-devices.md) לקבלת שלבים עבור טלפונים ומכשירי iPhone של Android.</span><span class="sxs-lookup"><span data-stu-id="be95b-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="be95b-192">גודל תיבת דואר</span><span class="sxs-lookup"><span data-stu-id="be95b-192">Mailbox Size</span></span>

<span data-ttu-id="be95b-193">Microsoft 365 Business Premium כולל מגבלת אחסון של 50 GB, כאשר היא משתמשת בתוכנית Exchange Online 1.</span><span class="sxs-lookup"><span data-stu-id="be95b-193">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="be95b-194">בעת המעבר ל- Microsoft 365 Business Premium, אם אחד מהמשתמשים שלך חורג מאחסון תיבת דואר בנפח 50 GB, מומלץ להקצות למשתמש זה תוכנית Exchange Online 2 ולהסיר את תוכנית Exchange Online 1, כפי שלא ניתן להקצות את שניהם.</span><span class="sxs-lookup"><span data-stu-id="be95b-194">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>


### <a name="threat-protection"></a><span data-ttu-id="be95b-195">הגנה מפני איומים</span><span class="sxs-lookup"><span data-stu-id="be95b-195">Threat protection</span></span>

<span data-ttu-id="be95b-196">לאחר המעבר ל- Microsoft 365 Business Premium, יש לך את Defender for Office 365.</span><span class="sxs-lookup"><span data-stu-id="be95b-196">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="be95b-197">עיין [ב- Microsoft Defender עבור Office 365](../security/office-365-security/defender-for-office-365.md) לקבלת מבט כולל.</span><span class="sxs-lookup"><span data-stu-id="be95b-197">See [Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md) for an overview.</span></span> <span data-ttu-id="be95b-198">כדי להגדיר, ראה [הגדרת קישורים בטוחים](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [הגדרת](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)קבצים מצורפים בטוחים והגדרת מניעת [דיוג ב- Defender עבור Office 365.](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)</span><span class="sxs-lookup"><span data-stu-id="be95b-198">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="be95b-199">תוויות רגישות</span><span class="sxs-lookup"><span data-stu-id="be95b-199">Sensitivity labels</span></span>

<span data-ttu-id="be95b-200">כדי להתחיל להשתמש בתוויות רגישות, ראה [מבט כולל על תוויות רגישות](../compliance/sensitivity-labels.md) [ויצירה וניהול של תוויות רגישות](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) וידאו.</span><span class="sxs-lookup"><span data-stu-id="be95b-200">To start using sensitivity labels, see [Overview of sensitivity labels](../compliance/sensitivity-labels.md) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
