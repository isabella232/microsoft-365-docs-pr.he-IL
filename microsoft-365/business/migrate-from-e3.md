---
title: העברה ל-Microsoft 365 Business מ-Office 365 E3
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
description: למד כיצד להעביר את העסק שלך ל-Microsoft 365 Business Premium מ-Office 365 E3.
ms.openlocfilehash: eebf78c24ed4bfd1a4fc2d843f37aebbe3d35e31
ms.sourcegitcommit: c1dd5be42fe0c5dcc7c05817c941edd9076febf8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/02/2020
ms.locfileid: "49558257"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="cf17e-103">העברה מ-Office 365 E3 ל-Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="cf17e-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span> 

<span data-ttu-id="cf17e-104">Microsoft 365 Business Premium כולל את כל מה שדרוש לך עבור העסק הקטן שלך, תוך שילוב אפליקציות הפרודוקטיביות המבוססות על ענן ברמה הטובה ביותר עם ניהול מכשירים ואבטחה פשוטים.</span><span class="sxs-lookup"><span data-stu-id="cf17e-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="cf17e-105">אם יש לך כעת מנוי של Office 365 E3, אך אין לך יותר מ-300 עובדים, שקול לעבור ל-Microsoft 365 Business Premium לקבלת תכונות אבטחה נוספות.</span><span class="sxs-lookup"><span data-stu-id="cf17e-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="cf17e-106">העברה קלה: תחילה עליך להחליף רשיונות וכל הנתונים ופרטי המשתמש שלך במנוי הנוכחי יישמרו.</span><span class="sxs-lookup"><span data-stu-id="cf17e-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="cf17e-107">לאחר ההעברה, יהיה עליך להגדיר את התכונות שנוספו ב-Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="cf17e-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="cf17e-108">הבדלים בין Office 365 E3 ו-Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="cf17e-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="cf17e-109">טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium ו-Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="cf17e-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="cf17e-110">תכונה</span><span class="sxs-lookup"><span data-stu-id="cf17e-110">Feature</span></span>    | <span data-ttu-id="cf17e-111">תמיכה ב-Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="cf17e-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="cf17e-112">תמיכה ב-Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="cf17e-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="cf17e-113">**מקומי**</span><span class="sxs-lookup"><span data-stu-id="cf17e-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="cf17e-114">יישומי Office<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="cf17e-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="cf17e-115">אפליקציות Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="cf17e-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="cf17e-116">Microsoft 365 Apps for enterprise</span><span class="sxs-lookup"><span data-stu-id="cf17e-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="cf17e-117">**אפליקציות לפרודוקטיביות בענן**</span><span class="sxs-lookup"><span data-stu-id="cf17e-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="cf17e-118">Exchange Online ו-Outlook</span><span class="sxs-lookup"><span data-stu-id="cf17e-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="cf17e-119">מגבלת אחסון של 50 GB לכל תיבת דואר ואחסון בארכיון באופן בלתי מוגבל של Exchange Online</span><span class="sxs-lookup"><span data-stu-id="cf17e-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="cf17e-120">מגבלת אחסון של 100 GB לכל תיבת דואר ואחסון בארכיון באופן בלתי מוגבל של Exchange Online</span><span class="sxs-lookup"><span data-stu-id="cf17e-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="cf17e-121">Teams</span><span class="sxs-lookup"><span data-stu-id="cf17e-121">Teams</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cf17e-124">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="cf17e-124">OneDrive for Business</span></span>    | <span data-ttu-id="cf17e-125">מגבלת אחסון של 1 TB לכל משתמש</span><span class="sxs-lookup"><span data-stu-id="cf17e-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="cf17e-126">גבלה</span><span class="sxs-lookup"><span data-stu-id="cf17e-126">Unlimited</span></span> | 
| <span data-ttu-id="cf17e-127">קטרת, SharePoint Online, מתכנן תכנון, זרם</span><span class="sxs-lookup"><span data-stu-id="cf17e-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cf17e-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="cf17e-130">StaffHub</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="cf17e-133">Outlook Customer Manager, MileIQ</span><span class="sxs-lookup"><span data-stu-id="cf17e-133">Outlook Customer Manager, MileIQ</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="cf17e-135">**הגנה מפני איום**</span><span class="sxs-lookup"><span data-stu-id="cf17e-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="cf17e-136">Defender עבור Office 365 תוכנית 1</span><span class="sxs-lookup"><span data-stu-id="cf17e-136">Defender for Office 365 Plan 1</span></span> | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="cf17e-138">לא כלול, אך ניתן להוסיף אותו</span><span class="sxs-lookup"><span data-stu-id="cf17e-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="cf17e-139">**ניהול זהויות**</span><span class="sxs-lookup"><span data-stu-id="cf17e-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="cf17e-140">איפוס סיסמה בשירות עצמי עבור חשבונות היברידית תכלת Active Directory (תכלת לספירה), באמצעות מספר מרבי של אימות רב-גורמי (מפעל מרכזי), גישה מותנית, סיסמה writeback עבור זהויות מקומיות</span><span class="sxs-lookup"><span data-stu-id="cf17e-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| <span data-ttu-id="cf17e-142">**ניהול מכשירים ויישומים**</span><span class="sxs-lookup"><span data-stu-id="cf17e-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="cf17e-143">Microsoft intune, Windows טייס אוטומטי</span><span class="sxs-lookup"><span data-stu-id="cf17e-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="cf17e-145">הפעלת מחשב משותף</span><span class="sxs-lookup"><span data-stu-id="cf17e-145">Shared computer activation</span></span>|     ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="cf17e-148">הרשאות שדרוג ל-Windows 10 Pro מ-Win 7/8.1 Pro רשיונות</span><span class="sxs-lookup"><span data-stu-id="cf17e-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    || 
| <span data-ttu-id="cf17e-150">**הגנה על מידע**</span><span class="sxs-lookup"><span data-stu-id="cf17e-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="cf17e-151">מניעת אובדן נתונים של Office 365</span><span class="sxs-lookup"><span data-stu-id="cf17e-151">Office 365 Data Loss Prevention</span></span>|    ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)|![כלול ב-Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="cf17e-154">הגנה על מידע של תכלת בתוכנית 1, אכיפה של Bitlocker</span><span class="sxs-lookup"><span data-stu-id="cf17e-154">Azure Information Protection Plan 1, Bitlocker enforcement</span></span>|![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="cf17e-156">הגנה על מידע ב-תכלת-תוכנית 1, תוויות רגישות</span><span class="sxs-lookup"><span data-stu-id="cf17e-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="cf17e-158">**רשיון גישת לקוח (זכויות CAL)**</span><span class="sxs-lookup"><span data-stu-id="cf17e-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="cf17e-159">חבילת CAL של Enterprise (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="cf17e-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![כלול ב-Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="cf17e-161"><sup>1</sup> גירסת Microsoft 365 Business Premium של יישומי Office אינה כוללת הפעלת עוצמת הקול באמצעות מדיניות קבוצתית, טלמטריה ביישומים, פקדי עדכון, השוואה בין גליונות אלקטרוניים ובירורים או בינה עסקית.</span><span class="sxs-lookup"><span data-stu-id="cf17e-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="cf17e-162">העברה</span><span class="sxs-lookup"><span data-stu-id="cf17e-162">Migration</span></span>

<span data-ttu-id="cf17e-163">כדי להעביר את המנוי שלך, ראה [שינוי התוכניות באופן ידני](../commerce/subscriptions/change-plans-manually.md) לקבלת הוראות אם ברצונך להעביר רק כמה אנשים ל-Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="cf17e-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="cf17e-164">באפשרותך גם [לשדרג את כולם באופן אוטומטי](../commerce/subscriptions/upgrade-to-different-plan.md), או לעבוד עם שותף כדי להעביר את מנוי E3 ואת הרשיונות למנוי של Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="cf17e-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="cf17e-165">הסעיפים הבאים מתארים את השינויים שעליך לבצע, אם בכלל, ומה ניתן לעשות לאחר ההעברה.</span><span class="sxs-lookup"><span data-stu-id="cf17e-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="cf17e-166">תצורת המנוי והנתונים של Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="cf17e-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="cf17e-167">אין צורך לבצע שינויים במנוי או בנתונים הנוכחיים לפני ההעברה, הכוללת:</span><span class="sxs-lookup"><span data-stu-id="cf17e-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="cf17e-168">תצורת מנוי, כגון רשומות DNS ושמות תחומים.</span><span class="sxs-lookup"><span data-stu-id="cf17e-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="cf17e-169">חשבונות משתמשים וקבוצות והגדרות אימות, כגון אימות רב-גורמי או מדיניות גישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="cf17e-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="cf17e-170">תצורות שירות פרודוקטיביות והנתונים שלהם, כגון Teams, תיבות דואר של Exchange Online, אתרי SharePoint Online, תיקיות OneDrive for Business ומחברות OneNote.</span><span class="sxs-lookup"><span data-stu-id="cf17e-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="cf17e-171">יישומי Office יתבצעו בקנה מידה באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="cf17e-171">Office applications will scale automatically.</span></span> <span data-ttu-id="cf17e-172">הרישוי המודרני של Office 365 יבדוק את משימת הרשיון של המשתמש כל 72 שעות וימיר את יישומי Office לגירסה התואמת למנוי המשתמש.</span><span class="sxs-lookup"><span data-stu-id="cf17e-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="cf17e-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="cf17e-173">Windows 10</span></span>

<span data-ttu-id="cf17e-174">אם החלונות שלך אינם נמצאים כבר בעדכון Windows Pro Creator, [שדרג אותם לעדכון Windows Pro creators](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="cf17e-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="cf17e-175">הגדרת מדיניות להגנה על התקני משתמשים וקבצים</span><span class="sxs-lookup"><span data-stu-id="cf17e-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="cf17e-176">אם תגדיר את מדיניות ומכשירים של Office 365 MDM, מכשירים אלה יופיעו בדף **מכשירים** במרכז הניהול של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cf17e-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="cf17e-177">כל פריטי המדיניות שתגדיר יופיעו ברשימה של פריטי המדיניות הקלאסיים [בפורטל ' כוונון](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)'.</span><span class="sxs-lookup"><span data-stu-id="cf17e-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="cf17e-178">לאחר שהקצית רשיונות ל-Microsoft 365 Business Premium, באפשרותך להתחיל להגן על המכשירים והקבצים של המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="cf17e-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="cf17e-179">אם שדרגת את כל המשתמשים בארגון שלך ל-Microsoft 365 Business Premium, תוכל לראות את אשף ההגדרה בדף הבית ולעקוב אחר [ההגדרה של Microsoft 365 Business Premium בשלבי אשף ההגדרה](set-up.md) כדי להגן על קבצים ומכשירים ניידים.</span><span class="sxs-lookup"><span data-stu-id="cf17e-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="cf17e-180">באפשרותך גם להשלים שלבים אלה בדף ' מכשירים ':</span><span class="sxs-lookup"><span data-stu-id="cf17e-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="cf17e-181">במרכז הניהול, בסרגל הניווט הימני, **Devices** עבור אל \> **פריטי מדיניות** של מכשירים.</span><span class="sxs-lookup"><span data-stu-id="cf17e-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="cf17e-182">בדף ' **פריטי מדיניות מכשיר** ', בחר **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="cf17e-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="cf17e-183">בחלונית **הוספת מדיניות** , הענק שם למדיניות ולאחר מכן בחר **סוג מדיניות** מהרשימה הנפתחת.</span><span class="sxs-lookup"><span data-stu-id="cf17e-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="cf17e-184">באפשרותך להגדיר פריטי מדיניות של יישומים להגנה על קבצים במכשירי Android ו-iPhone, וכן Windows 10, ובאפשרותך להגדיר מדיניות תצורת מכשיר עבור מכשירי Windows 10 בבעלות החברה.</span><span class="sxs-lookup"><span data-stu-id="cf17e-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="cf17e-185">עיין בקישורים הבאים לקבלת פרטים:</span><span class="sxs-lookup"><span data-stu-id="cf17e-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="cf17e-186">קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS</span><span class="sxs-lookup"><span data-stu-id="cf17e-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="cf17e-187">קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10</span><span class="sxs-lookup"><span data-stu-id="cf17e-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="cf17e-188">קביעת הגדרות הגנה על מכשירים עבור מחשבי Pc של Windows 10</span><span class="sxs-lookup"><span data-stu-id="cf17e-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="cf17e-189">לאחר הגדרת מדיניות, אתה והעובדים שלך יכולים להגדיר מכשירים:</span><span class="sxs-lookup"><span data-stu-id="cf17e-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="cf17e-190">ראה [הגדרת מכשירי windows עבור משתמשי Microsoft 365 Business Premium](set-up-windows-devices.md) לקבלת שלבים עבור מכשירי Windows.</span><span class="sxs-lookup"><span data-stu-id="cf17e-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="cf17e-191">ראה [הגדרת מכשירים ניידים עבור משתמשי Microsoft 365 Business Premium](set-up-mobile-devices.md) לקבלת שלבים עבור טלפונים ומכשירי Iphone של Android.</span><span class="sxs-lookup"><span data-stu-id="cf17e-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="cf17e-192">גודל תיבת הדואר</span><span class="sxs-lookup"><span data-stu-id="cf17e-192">Mailbox Size</span></span>

<span data-ttu-id="cf17e-193">Microsoft 365 Business Premium כולל מגבלת אחסון של 50 GB כאשר הוא משתמש ב-Exchange Online תוכנית 1.</span><span class="sxs-lookup"><span data-stu-id="cf17e-193">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="cf17e-194">בעת המעבר ל-Microsoft 365 Business Premium, אם אחד מהמשתמשים שלך חורג מ-50 ג'יגה-בתים של אחסון תיבת הדואר, מומלץ להקצות למשתמש זה תוכנית Exchange Online 2 ולהסיר את Exchange Online Plan 1 מכיוון שלא ניתן להקצות את שניהם.</span><span class="sxs-lookup"><span data-stu-id="cf17e-194">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>


### <a name="threat-protection"></a><span data-ttu-id="cf17e-195">הגנה מפני איום</span><span class="sxs-lookup"><span data-stu-id="cf17e-195">Threat protection</span></span>

<span data-ttu-id="cf17e-196">לאחר המעבר ל-Microsoft 365 Business Premium, יש לך Defender עבור Office 365.</span><span class="sxs-lookup"><span data-stu-id="cf17e-196">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="cf17e-197">ראה [Microsoft Defender עבור Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) לקבלת מבט כולל.</span><span class="sxs-lookup"><span data-stu-id="cf17e-197">See [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for an overview.</span></span> <span data-ttu-id="cf17e-198">כדי להגדיר, ראה [הגדרת קישורים בטוחים](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [הגדרת קבצים מצורפים בטוחים](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5) [והגדרת אנטי-דיוג ב-Defender עבור Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span><span class="sxs-lookup"><span data-stu-id="cf17e-198">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="cf17e-199">תוויות רגישות</span><span class="sxs-lookup"><span data-stu-id="cf17e-199">Sensitivity labels</span></span>

<span data-ttu-id="cf17e-200">כדי להתחיל להשתמש בתוויות רגישות, ראה [מבט כולל על תוויות רגישות](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) ולאחר מכן [יצירה וניהול של וידאו וניהול של תוויות רגישות](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) .</span><span class="sxs-lookup"><span data-stu-id="cf17e-200">To start using sensitivity labels, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
