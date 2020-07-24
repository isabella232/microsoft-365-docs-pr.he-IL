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
ms.openlocfilehash: d72f0c52a745ff973868b6fdaa95efa1a37a3dbd
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/18/2020
ms.locfileid: "45081836"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="1ea9e-103">הגירה מ-Office 365 E3 ל-Microsoft 365 עסקים פרימיום</span><span class="sxs-lookup"><span data-stu-id="1ea9e-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span> 

<span data-ttu-id="1ea9e-104">Microsoft 365 Business Premium יש את כל מה שאתה צריך עבור העסק הקטן שלך, שילוב של יישומי הפרודוקטיביות המבוססת על ענן ברמה הטובה ביותר עם ניהול התקנים פשוטים ואבטחה.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="1ea9e-105">אם יש לך כרגע מנוי של Office 365 E3, אך אין ברשותך יותר מ-300 עובדים, שקול לעבור ל-Microsoft 365 Business Premium לקבלת תכונות אבטחה נוספות.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="1ea9e-106">ההעברה קלה: תחילה אתה מחליף רישיונות וכל הנתונים ופרטי המשתמש שלך במנוי הנוכחי שלך נשמרים.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="1ea9e-107">לאחר ההעברה, יהיה עליך להגדיר את התכונות הנוספות ב-Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="1ea9e-108">הבדלים בין Office 365 E3 ו-Microsoft 365 עסקים Premium</span><span class="sxs-lookup"><span data-stu-id="1ea9e-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="1ea9e-109">טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium ו-Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="1ea9e-110">תכונה</span><span class="sxs-lookup"><span data-stu-id="1ea9e-110">Feature</span></span>    | <span data-ttu-id="1ea9e-111">תמיכה ב-Microsoft 365 עסקים פרימיום</span><span class="sxs-lookup"><span data-stu-id="1ea9e-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="1ea9e-112">תמיכה ב-Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="1ea9e-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="1ea9e-113">**מקומי**</span><span class="sxs-lookup"><span data-stu-id="1ea9e-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="1ea9e-114">יישומים משרדיים<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="1ea9e-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="1ea9e-115">מיקרוסופט 365 אפליקציות לעסקים</span><span class="sxs-lookup"><span data-stu-id="1ea9e-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="1ea9e-116">מיקרוסופט 365 Apps עבור הארגון</span><span class="sxs-lookup"><span data-stu-id="1ea9e-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="1ea9e-117">**אפליקציות לפרודוקטיביות בענן**</span><span class="sxs-lookup"><span data-stu-id="1ea9e-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="1ea9e-118">Exchange Online ו-Outlook</span><span class="sxs-lookup"><span data-stu-id="1ea9e-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="1ea9e-119">50 ג'יגה-בתים של מגבלת אחסון עבור תיבת דואר ובלתי מוגבל לארכיון Exchange Online</span><span class="sxs-lookup"><span data-stu-id="1ea9e-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="1ea9e-120">100 ג'יגה-בתים של מגבלת אחסון עבור תיבת דואר ובלתי מוגבל לארכיון Exchange Online</span><span class="sxs-lookup"><span data-stu-id="1ea9e-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="1ea9e-121">צוותים</span><span class="sxs-lookup"><span data-stu-id="1ea9e-121">Teams</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="1ea9e-124">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="1ea9e-124">OneDrive for Business</span></span>    | <span data-ttu-id="1ea9e-125">1 TB מגבלת אחסון לכל משתמש</span><span class="sxs-lookup"><span data-stu-id="1ea9e-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="1ea9e-126">גבלה</span><span class="sxs-lookup"><span data-stu-id="1ea9e-126">Unlimited</span></span> | 
| <span data-ttu-id="1ea9e-127">Yammer, SharePoint מקוון, מתכנן, זרם</span><span class="sxs-lookup"><span data-stu-id="1ea9e-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="1ea9e-130">מרכז הצוות</span><span class="sxs-lookup"><span data-stu-id="1ea9e-130">StaffHub</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="1ea9e-133">מנהל הלקוחות של Outlook, MileIQ</span><span class="sxs-lookup"><span data-stu-id="1ea9e-133">Outlook Customer Manager, MileIQ</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | | 
| <span data-ttu-id="1ea9e-135">**הגנה מפני איומים**</span><span class="sxs-lookup"><span data-stu-id="1ea9e-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="1ea9e-136">תוכנית הגנת האיומים המתקדמת של Office 365 (ATP) 1</span><span class="sxs-lookup"><span data-stu-id="1ea9e-136">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | <span data-ttu-id="1ea9e-138">לא כלול, אבל ניתן להוסיף על</span><span class="sxs-lookup"><span data-stu-id="1ea9e-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="1ea9e-139">**ניהול זהויות**</span><span class="sxs-lookup"><span data-stu-id="1ea9e-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="1ea9e-140">איפוס סיסמה של שירות עצמי עבור חשבונות היברידית של התכלת הפעילה (כחול לספירה), אימות מרובה-גורמים (משרד המידע), גישה מותנית, סיסמה שתכתוב עבור זהויות מקומיות</span><span class="sxs-lookup"><span data-stu-id="1ea9e-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    |  | 
| <span data-ttu-id="1ea9e-142">**ניהול התקנים ואפליקציות**</span><span class="sxs-lookup"><span data-stu-id="1ea9e-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="1ea9e-143">מיקרוסופט Intune, Windows טייס אוטומטי</span><span class="sxs-lookup"><span data-stu-id="1ea9e-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    |  |
| <span data-ttu-id="1ea9e-145">הפעלת מחשב משותף</span><span class="sxs-lookup"><span data-stu-id="1ea9e-145">Shared computer activation</span></span>|     ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="1ea9e-148">זכויות שדרוג ל-Windows 10 Pro מ-Win 7/8.1 Pro רשיונות</span><span class="sxs-lookup"><span data-stu-id="1ea9e-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    || 
| <span data-ttu-id="1ea9e-150">**הגנה מפני מידע**</span><span class="sxs-lookup"><span data-stu-id="1ea9e-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="1ea9e-151">מניעת אובדן נתונים של Office 365</span><span class="sxs-lookup"><span data-stu-id="1ea9e-151">Office 365 Data Loss Prevention</span></span>|    ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)|![כלול ב-Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="1ea9e-154">התוכנית להגנה מפני מידע תכלת 1, אכיפה של Bitlocker</span><span class="sxs-lookup"><span data-stu-id="1ea9e-154">Azure Information Protection Plan 1, Bitlocker enforcement</span></span>|![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)||
|<span data-ttu-id="1ea9e-156">שיטת הגנת מידע תכלת, תוויות רגישות</span><span class="sxs-lookup"><span data-stu-id="1ea9e-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)||
|<span data-ttu-id="1ea9e-158">**רשיון גישת לקוח (זכויות CAL)**</span><span class="sxs-lookup"><span data-stu-id="1ea9e-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="1ea9e-159">סוויטת CAL ארגונית (Exchange, SharePoint, סקייפ)</span><span class="sxs-lookup"><span data-stu-id="1ea9e-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![כלול ב-Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="1ea9e-161"><sup>1</sup> מיקרוסופט 365 עסקים Premium גירסה של יישומי המשרד אינו כולל הפעלת אמצעי אחסון באמצעות מדיניות קבוצתית, apps טלמטריה, עדכון פקדים, גיליון אלקטרוני להשוות ולברר, או בינה עסקית.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="1ea9e-162">העברה</span><span class="sxs-lookup"><span data-stu-id="1ea9e-162">Migration</span></span>

<span data-ttu-id="1ea9e-163">כדי להעביר את המנוי שלך, ראה [שינוי תוכניות באופן ידני](../commerce/subscriptions/change-plans-manually.md) לקבלת הוראות אם ברצונך להעביר רק כמה אנשים ל-Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="1ea9e-164">באפשרותך גם [לשדרג את כולם באופן אוטומטי](../commerce/subscriptions/upgrade-to-different-plan.md), או לעבוד עם שותף כדי להעביר את מנוי ה-E3 והרשיונות שלך למנוי של Microsoft Business Premium של מיקרוסופט 365.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="1ea9e-165">הסעיפים הבאים מתארים את השינויים שעליך לבצע, אם בכלל, ומה באפשרותך לעשות לאחר ההעברה.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="1ea9e-166">תצורה ונתונים של מנויים ב-Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="1ea9e-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="1ea9e-167">אין צורך לבצע שינויים כלשהם במנוי או בנתונים הנוכחיים לפני ההעברה, הכוללת:</span><span class="sxs-lookup"><span data-stu-id="1ea9e-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="1ea9e-168">תצורת מנוי, כגון רשומות DNS ושמות תחומים.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="1ea9e-169">חשבונות משתמש וקבוצה והגדרות אימות, כגון אימות מרובה גורמים או מדיניות גישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="1ea9e-170">תצורות שירות של פרודוקטיביות והנתונים שלהם, כגון צוותים, תיבות דואר של Exchange Online, אתרים מקוונים של SharePoint, OneDrive עבור תיקיות עסקיות ומחברות של OneNote.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="1ea9e-171">יישומי Office יגודלם באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-171">Office applications will scale automatically.</span></span> <span data-ttu-id="1ea9e-172">הרישוי המודרני של Office 365 יבדוק את הקצאת הרשיון של המשתמש כל 72 שעות וימיר יישומי Office לגירסה התואמת למנוי המשתמש.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="1ea9e-173">ווינדוס 10</span><span class="sxs-lookup"><span data-stu-id="1ea9e-173">Windows 10</span></span>

<span data-ttu-id="1ea9e-174">אם Windows שברשותך אינו נמצא כבר בעדכון Windows Pro Creator, [שדרג אותם לעדכון יוצרי Windows pro](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="1ea9e-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="1ea9e-175">כוונן פריטי מדיניות כדי להגן על התקני משתמש וקבצים</span><span class="sxs-lookup"><span data-stu-id="1ea9e-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="1ea9e-176">אם תגדיר מדיניות והתקנים של Office 365 MDM, התקנים אלה יפורטו בדף **ההתקנים** במרכז הניהול של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="1ea9e-177">כל פריטי המדיניות שתגדיר יופיעו ברשימת המדיניות הקלאסית [בפורטל Intune](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span><span class="sxs-lookup"><span data-stu-id="1ea9e-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="1ea9e-178">לאחר שהקצית רשיונות ל-Microsoft 365 Business Premium, באפשרותך להתחיל להגן על ההתקנים והקבצים של המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="1ea9e-179">אם שדרגת את כל האנשים בארגון שלך ל-Microsoft 365 Business Premium, תראה את אשף ההגדרה בדף הבית, ותוכל לעקוב אחר [הגדרת Microsoft 365 Business Premium בשלבי אשף ההתקנה](set-up.md) כדי להגן על קבצים ומכשירים ניידים.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="1ea9e-180">באפשרותך גם להשלים שלבים אלה בדף ' התקנים ':</span><span class="sxs-lookup"><span data-stu-id="1ea9e-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="1ea9e-181">במרכז הניהול, בניווט השמאלי, עבור אל **Devices** \> **מדיניות**התקנים.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="1ea9e-182">בדף ' **מדיניות התקן** ', בחר באפשרות ' **הוסף**'.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="1ea9e-183">בחלונית **המדיניות הוסף** את שם המדיניות ולאחר מכן בחר **סוג מדיניות** מהרשימה הנפתחת.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="1ea9e-184">באפשרותך להגדיר מדיניות יישומים להגנה על קבצים בהתקני Android ו-iPhone, כמו גם ב-Windows 10, ובאפשרותך להגדיר מדיניות תצורת התקנים עבור התקנים של Windows 10 השייכים לחברה.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="1ea9e-185">לפרטים, עיין בקישורים הבאים:</span><span class="sxs-lookup"><span data-stu-id="1ea9e-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="1ea9e-186">קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS</span><span class="sxs-lookup"><span data-stu-id="1ea9e-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="1ea9e-187">קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10</span><span class="sxs-lookup"><span data-stu-id="1ea9e-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="1ea9e-188">הגדרת הגדרות הגנת התקן עבור מחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="1ea9e-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="1ea9e-189">לאחר הגדרת פריטי מדיניות, אתה ועובדיך יכולים להגדיר התקנים:</span><span class="sxs-lookup"><span data-stu-id="1ea9e-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="1ea9e-190">ראה [הגדרת התקני windows עבור משתמשי Microsoft Business Premium 365](set-up-windows-devices.md) עבור שלבים עבור התקני windows.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="1ea9e-191">ראה [הגדרת התקנים ניידים עבור Microsoft 365 Business Premium משתמשים](set-up-mobile-devices.md) עבור שלבים עבור טלפונים אנדרואיד ו-iphone.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 

### <a name="threat-protection"></a><span data-ttu-id="1ea9e-192">הגנה מפני איומים</span><span class="sxs-lookup"><span data-stu-id="1ea9e-192">Threat protection</span></span>

<span data-ttu-id="1ea9e-193">לאחר הגירה ל-Microsoft 365 Business Premium, יש לך Office 365 ATP.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-193">After migrating to Microsoft 365 Business Premium, you have Office 365 ATP.</span></span> <span data-ttu-id="1ea9e-194">לקבלת סקירה, ראה [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) .</span><span class="sxs-lookup"><span data-stu-id="1ea9e-194">See [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for an overview.</span></span> <span data-ttu-id="1ea9e-195">כדי להגדיר, ראה [הגדרת קישורים בטוחים של atp](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [הגדר קבצים מצורפים של atp בטוחים](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5) [והגדר את האנטי-דיוג של atp](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span><span class="sxs-lookup"><span data-stu-id="1ea9e-195">To set up, see [set up ATP safe links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up ATP safe attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up ATP anti-phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="1ea9e-196">תוויות רגישות</span><span class="sxs-lookup"><span data-stu-id="1ea9e-196">Sensitivity labels</span></span>

<span data-ttu-id="1ea9e-197">כדי להתחיל להשתמש בתוויות רגישות, ראה [מבט כולל על תוויות רגישות](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) [ויצירה וניהול של תוויות רגישות](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) וידאו.</span><span class="sxs-lookup"><span data-stu-id="1ea9e-197">To start using sensitivity labels, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>