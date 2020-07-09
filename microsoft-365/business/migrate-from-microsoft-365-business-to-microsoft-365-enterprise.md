---
title: העברה מ-Microsoft 365 Business ל-Microsoft 365 E3
f1.keywords:
- NOCSH
ms.author: josephd
author: JoeDavies-MSFT
manager: laurawi
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: למד כיצד להעביר את העסק שלך מ-Microsoft 365 Business Premium ל-Microsoft 365 E3.
ms.openlocfilehash: 6a795d96ccae7e054e7e52d4fd60a4e73b3c71dd
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/27/2020
ms.locfileid: "45081831"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="2088b-103">העברה מ-Microsoft 365 Business Premium ל-Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="2088b-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="2088b-104">Microsoft 365 Business Premium יש את כל מה שאתה צריך עבור העסק הקטן שלך, שילוב של יישומי הפרודוקטיביות המבוססת על ענן ברמה הטובה ביותר עם ניהול התקן פשוט ואבטחה המאפשרים לעובדים שלך לעשות את העבודה הטובה ביותר שלהם.</span><span class="sxs-lookup"><span data-stu-id="2088b-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="2088b-105">עם זאת, במקרים מסוימים, ייתכן שיהיה עליך להעביר את מנוי ה-365 Business Premium של Microsoft למיקרוסופט 365 E3.</span><span class="sxs-lookup"><span data-stu-id="2088b-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span> 

<span data-ttu-id="2088b-106">לדוגמה, העסק שלך גדל וזקוק ליותר מ 300 רשיונות (ברכות, דרך אגב).</span><span class="sxs-lookup"><span data-stu-id="2088b-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="2088b-107">לחלופין, העסק שלך זקוק לתכונות ארגוניות, כגון Microsoft 365 Apps עבור הארגון, Windows 10-E3 Enterprise, או רשיונות גישת לקוח ארגוניים (Cal).</span><span class="sxs-lookup"><span data-stu-id="2088b-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="2088b-108">השדרוג הוא קל: באפשרותך להפעיל את השדרוג [ממרכז הניהול](../commerce/subscriptions/upgrade-to-different-plan.md).</span><span class="sxs-lookup"><span data-stu-id="2088b-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="2088b-109">כל הנתונים והגדרות התצורה במנוי הנוכחי נשמרים.</span><span class="sxs-lookup"><span data-stu-id="2088b-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="2088b-110">אין לך מה לעשות כדי להתכונן להגירה ולא לעשות כלום לאחר מכן, מלבד לנצל את התכונות החדשות.</span><span class="sxs-lookup"><span data-stu-id="2088b-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

>[!Note]
><span data-ttu-id="2088b-111">באפשרותך גם להשתמש במנוי של Microsoft Business Premium 365 עבור עד 300 מושבים ולקבל מנוי של Microsoft 365 E3 עבור יותר מ-300 מושבים.</span><span class="sxs-lookup"><span data-stu-id="2088b-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="2088b-112">עם זאת, Office 365 ATP אינו כלול ב-Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="2088b-112">However, Office 365 ATP is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="2088b-113">לצורך הגנה על איום מתמשך, עליך להוסיף רשיונות Office 365 של ATP נוספים כך שכל המשתמשים בהיקף של מדיניות ה-ATP של Office 365 יהיו מורשים.</span><span class="sxs-lookup"><span data-stu-id="2088b-113">For continued threat protection, you should add additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span>
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="2088b-114">הבדלים בין מיקרוסופט 365 עסקים Premium ו-Microsoft 365 Enterprise</span><span class="sxs-lookup"><span data-stu-id="2088b-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="2088b-115">טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium ו-Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="2088b-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="2088b-116">תכונה</span><span class="sxs-lookup"><span data-stu-id="2088b-116">Feature</span></span>    | <span data-ttu-id="2088b-117">תמיכה ב-Microsoft 365 עסקים פרימיום</span><span class="sxs-lookup"><span data-stu-id="2088b-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="2088b-118">תמיכה ב-Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="2088b-118">Support in Microsoft 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="2088b-119">**מקומי**</span><span class="sxs-lookup"><span data-stu-id="2088b-119">**On-premises**</span></span>        | | | 
| <span data-ttu-id="2088b-120">ווינדוס 10</span><span class="sxs-lookup"><span data-stu-id="2088b-120">Windows 10</span></span>    | <span data-ttu-id="2088b-121">העסק של חלונות 10</span><span class="sxs-lookup"><span data-stu-id="2088b-121">Windows 10 Business</span></span>  |     <span data-ttu-id="2088b-122">Windows 10 E3 ארגון</span><span class="sxs-lookup"><span data-stu-id="2088b-122">Windows 10 Enterprise E3</span></span>| 
| <span data-ttu-id="2088b-123">יישומי Office \*</span><span class="sxs-lookup"><span data-stu-id="2088b-123">Office apps\*</span></span>    | [<span data-ttu-id="2088b-124">מיקרוסופט 365 אפליקציות לעסקים</span><span class="sxs-lookup"><span data-stu-id="2088b-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="2088b-125">מיקרוסופט 365 Apps עבור הארגון</span><span class="sxs-lookup"><span data-stu-id="2088b-125">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="2088b-126">**אפליקציות לפרודוקטיביות בענן**</span><span class="sxs-lookup"><span data-stu-id="2088b-126">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="2088b-127">Exchange Online ו-Outlook</span><span class="sxs-lookup"><span data-stu-id="2088b-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="2088b-128">50 ג'יגה-בתים של מגבלת אחסון לכל תיבת דואר וארכיון Exchange Online בלתי מוגבל</span><span class="sxs-lookup"><span data-stu-id="2088b-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="2088b-129">100 ג'יגה-בתים של מגבלת אחסון לכל תיבת דואר וארכיון Exchange Online בלתי מוגבל</span><span class="sxs-lookup"><span data-stu-id="2088b-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> | 
| <span data-ttu-id="2088b-130">צוותים</span><span class="sxs-lookup"><span data-stu-id="2088b-130">Teams</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-133">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="2088b-133">OneDrive for Business</span></span>    | <span data-ttu-id="2088b-134">1 TB מגבלת אחסון לכל משתמש</span><span class="sxs-lookup"><span data-stu-id="2088b-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="2088b-135">גבלה</span><span class="sxs-lookup"><span data-stu-id="2088b-135">Unlimited</span></span> | 
| <span data-ttu-id="2088b-136">Yammer, SharePoint מקוון, מתכנן, זרם</span><span class="sxs-lookup"><span data-stu-id="2088b-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-139">מנהל הלקוחות של Outlook, MileIQ</span><span class="sxs-lookup"><span data-stu-id="2088b-139">Outlook Customer Manager, MileIQ</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | | 
| <span data-ttu-id="2088b-141">**הגנה מפני איומים**</span><span class="sxs-lookup"><span data-stu-id="2088b-141">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="2088b-142">יכולות הפחתת משטח התקפה</span><span class="sxs-lookup"><span data-stu-id="2088b-142">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="2088b-143">ראה רשימה זו</span><span class="sxs-lookup"><span data-stu-id="2088b-143">See this list</span></span>](#threat-protection) | <span data-ttu-id="2088b-144">ניהול ארגוני של בידוד מבוסס חומרה עבור Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2088b-144">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> | 
| <span data-ttu-id="2088b-145">תוכנית הגנת האיומים המתקדמת של Office 365 (ATP) 1</span><span class="sxs-lookup"><span data-stu-id="2088b-145">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | <span data-ttu-id="2088b-147">לא כלול, אבל ניתן להוסיף על</span><span class="sxs-lookup"><span data-stu-id="2088b-147">Not included, but can be added on</span></span> | 
| <span data-ttu-id="2088b-148">**ניהול זהויות**</span><span class="sxs-lookup"><span data-stu-id="2088b-148">**Identity management**</span></span>        | | | 
| <span data-ttu-id="2088b-149">איפוס סיסמה של שירות עצמי עבור חשבונות היברידית של התכלת הפעילה (כחול לספירה), אימות מרובה-גורמים (משרד המידע), גישה מותנית, סיסמה שתכתוב עבור זהויות מקומיות</span><span class="sxs-lookup"><span data-stu-id="2088b-149">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-152">האפליקציה גילוי ענן, תכלת AD התחברות בריאות</span><span class="sxs-lookup"><span data-stu-id="2088b-152">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-154">תכלת המשרד 365 אפליקציות כניסה יחידה (SSO): 10 יישומים לכל משתמש (גלריית יישומים מסוג SaaS כגון מערכת המחיר) \*</span><span class="sxs-lookup"><span data-stu-id="2088b-154">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-157">תכלת AD פרימיום 1 SSO: אין מגבלה (יישומים מקומיים באמצעות התכלת AD היישום Proxy ויישומים שאינם הגלריה באמצעות שילוב עצמי יישום App תבניות)</span><span class="sxs-lookup"><span data-stu-id="2088b-157">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-159">**ניהול התקנים ואפליקציות**</span><span class="sxs-lookup"><span data-stu-id="2088b-159">**Device and app management**</span></span>        | | | 
| <span data-ttu-id="2088b-160">מיקרוסופט Intune, Windows טייס אוטומטי</span><span class="sxs-lookup"><span data-stu-id="2088b-160">Microsoft Intune, Windows Autopilot</span></span>|     ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="2088b-163">גישה לשולחן עבודה וירטואלי (VDA)</span><span class="sxs-lookup"><span data-stu-id="2088b-163">Virtual Desktop Access (VDA)</span></span>    |  |     ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="2088b-165">שולחן עבודה וירטואלי של Windows (WVD)</span><span class="sxs-lookup"><span data-stu-id="2088b-165">Windows Virtual Desktop (WVD)</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png) |     ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="2088b-168">הפעלה משותפת של מחשב (סקה)</span><span class="sxs-lookup"><span data-stu-id="2088b-168">Shared Computer Activation (SCA)</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png) |     ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-171">חבילת אופטימיזציה לשולחן העבודה של Microsoft</span><span class="sxs-lookup"><span data-stu-id="2088b-171">Microsoft Desktop Optimization Package</span></span>    | |     ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-173">**הגנה מפני מידע**</span><span class="sxs-lookup"><span data-stu-id="2088b-173">**Information protection**</span></span>        | | | 
| <span data-ttu-id="2088b-174">משרד 365 למניעת אובדן נתונים, תוכנית הגנת מידע תכלת 1</span><span class="sxs-lookup"><span data-stu-id="2088b-174">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-177">הגנה על מידע חלון עבור DLP של נקודת קצה</span><span class="sxs-lookup"><span data-stu-id="2088b-177">Window Information Protection for endpoint DLP</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-180">**רשיון גישת לקוח (זכויות CAL)**</span><span class="sxs-lookup"><span data-stu-id="2088b-180">**Client Access License (CAL rights)**</span></span>    | | |     
| <span data-ttu-id="2088b-181">סוויטת CAL של ארגון (Exchange, SharePoint, סקייפ, חלונות, מנהל תצורת נקודות קצה של מיקרוסופט, ניהול זכויות של Windows)</span><span class="sxs-lookup"><span data-stu-id="2088b-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-183">**תאימות**</span><span class="sxs-lookup"><span data-stu-id="2088b-183">**Compliance**</span></span>        | | | 
| <span data-ttu-id="2088b-184">בארכיון דוא ל ללא הגבלה</span><span class="sxs-lookup"><span data-stu-id="2088b-184">Unlimited email archiving</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-187">תוצאת תאימות/מנהל תאימות</span><span class="sxs-lookup"><span data-stu-id="2088b-187">Compliance Score/Compliance Manager</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-190">eDiscovery</span><span class="sxs-lookup"><span data-stu-id="2088b-190">eDiscovery</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-193">חסימה במקום והחזקת ליטיגציה</span><span class="sxs-lookup"><span data-stu-id="2088b-193">In-place hold and litigation hold</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="2088b-196">תגי שמירה של ניהול רשומות העברת הודעות (MRM) ומדיניות שמירה</span><span class="sxs-lookup"><span data-stu-id="2088b-196">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
||||

<span data-ttu-id="2088b-199">\*משתמשים שהוקצו להם גישה ליישומי SaaS יכולים לקבל גישה ל-SSO עד 10 אפליקציות.</span><span class="sxs-lookup"><span data-stu-id="2088b-199">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="2088b-200">מנהלים יכולים לקבוע את תצורת SSO ולשנות את גישת המשתמש ליישומי SaaS שונים, אך גישת SSO מותרת רק עבור 10 יישומים לכל משתמש בכל פעם.</span><span class="sxs-lookup"><span data-stu-id="2088b-200">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="2088b-201">כל יישומי Office 365 נספרים כיישום יחיד.</span><span class="sxs-lookup"><span data-stu-id="2088b-201">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="2088b-202">העברה</span><span class="sxs-lookup"><span data-stu-id="2088b-202">Migration</span></span>

<span data-ttu-id="2088b-203">כדי להעביר, עבוד עם השותף שלך כדי להעביר את Microsoft 365 Business Premium למנוי ורישיונות למנוי מתאים של Microsoft 365 E3 עם הרישיונות שלה.</span><span class="sxs-lookup"><span data-stu-id="2088b-203">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="2088b-204">הסעיפים הבאים מתארים את השינויים שעליך לבצע, אם בכלל, ומה באפשרותך לעשות לאחר ההעברה.</span><span class="sxs-lookup"><span data-stu-id="2088b-204">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="2088b-205">מיקרוסופט 365 תצורת מנויים ונתונים</span><span class="sxs-lookup"><span data-stu-id="2088b-205">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="2088b-206">אין צורך לבצע שינויים במנוי או בנתונים הנוכחיים לפני ההעברה, כולל:</span><span class="sxs-lookup"><span data-stu-id="2088b-206">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="2088b-207">תצורת מנוי, כגון שמות תחומים של DNS.</span><span class="sxs-lookup"><span data-stu-id="2088b-207">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="2088b-208">חשבונות משתמש וקבוצה והגדרות אימות, כגון אימות מרובה גורמים או מדיניות גישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="2088b-208">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="2088b-209">תצורות שירות של פרודוקטיביות והנתונים שלהם, כגון צוותים, תיבות דואר של Exchange Online, אתרים מקוונים של SharePoint, OneDrive עבור תיקיות עסקיות ומחברות של OneNote.</span><span class="sxs-lookup"><span data-stu-id="2088b-209">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="2088b-210">כעת, המשתמשים שלך יכולים ליהנות מאחסון בלתי מוגבל בתיבות הדואר של Exchange Online ובתיקיות עסקיות.</span><span class="sxs-lookup"><span data-stu-id="2088b-210">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="2088b-211">אתה יכול להתחיל להשתמש בגילוי קלאוד App, תכלת AD התחברות בריאות, ו-SSO עבור יותר מ 10 apps.</span><span class="sxs-lookup"><span data-stu-id="2088b-211">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

>[!Note]
><span data-ttu-id="2088b-212">משתמשים שהועברו ל-Microsoft 365 E3 לא יכולים עוד להשתמש במנהל הלקוחות של Outlook ו-MileIQ.</span><span class="sxs-lookup"><span data-stu-id="2088b-212">Users migrated to Microsoft 365 E3 can no longer use Outlook Customer Manager and MileIQ.</span></span>
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="2088b-213">הגנה מפני איומים</span><span class="sxs-lookup"><span data-stu-id="2088b-213">Threat protection</span></span>

<span data-ttu-id="2088b-214">Windows 10 Business כולל הגנות אלה:</span><span class="sxs-lookup"><span data-stu-id="2088b-214">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="2088b-215">אכיפת התקינות של תהליך האתחול של מערכת ההפעלה</span><span class="sxs-lookup"><span data-stu-id="2088b-215">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="2088b-216">אכיפת שלמות של רכיבי הפעלה רגישים</span><span class="sxs-lookup"><span data-stu-id="2088b-216">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="2088b-217">פגיעות מתקדמת והגורמים המקלים על ניצול של אפס ימים</span><span class="sxs-lookup"><span data-stu-id="2088b-217">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="2088b-218">הגנת רשת מבוססת מוניטין עבור Microsoft Edge, Internet Explorer וכרום</span><span class="sxs-lookup"><span data-stu-id="2088b-218">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="2088b-219">חומת אש מבוססת-מארח</span><span class="sxs-lookup"><span data-stu-id="2088b-219">Host-based firewall</span></span>
- <span data-ttu-id="2088b-220">הגורמים המקלים Ransomware</span><span class="sxs-lookup"><span data-stu-id="2088b-220">Ransomware mitigations</span></span>
- <span data-ttu-id="2088b-221">בידוד מבוסס חומרה עבור Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2088b-221">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="2088b-222">בקרת יישומים המונעת על-ידי גרף האבטחה החכם</span><span class="sxs-lookup"><span data-stu-id="2088b-222">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="2088b-223">בקרת התקן (USB)</span><span class="sxs-lookup"><span data-stu-id="2088b-223">Device control (USB)</span></span>
- <span data-ttu-id="2088b-224">הגנת רשת עבור איומים מבוססי אינטרנט</span><span class="sxs-lookup"><span data-stu-id="2088b-224">Network protection for web-based threats</span></span>
- <span data-ttu-id="2088b-225">כללי מניעת חדירה למחשב</span><span class="sxs-lookup"><span data-stu-id="2088b-225">Host intrusion prevention rules</span></span>

<span data-ttu-id="2088b-226">Windows 10 מארגון E3 כולל גם ניהול ארגוני של בידוד מבוסס חומרה עבור Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="2088b-226">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

>[!Note]
><span data-ttu-id="2088b-227">משתמשים שהועברו ל-Microsoft 365 E3 ידרשו רישיון של Office 365 ATP לצורך הגנה על האיום המתמשך.</span><span class="sxs-lookup"><span data-stu-id="2088b-227">Users migrated to Microsoft 365 E3 will each require an Office 365 ATP license for continued threat protection.</span></span> <span data-ttu-id="2088b-228">הקפד לרכוש רשיונות נוספים של Office 365 ATP כך שכל המשתמשים בטווח של מדיניות ה-ATP של Office 365 יהיו מורשים.</span><span class="sxs-lookup"><span data-stu-id="2088b-228">Be sure to purchase additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span> 
>

### <a name="device-management-with-intune"></a><span data-ttu-id="2088b-229">ניהול התקנים באמצעות Intune</span><span class="sxs-lookup"><span data-stu-id="2088b-229">Device management with Intune</span></span>

<span data-ttu-id="2088b-230">אין צורך לבצע שינויים כלשהם בתצורת Intune הנוכחית לפני ההעברה, הכוללת התקנים רשומים והגדרות התקן ויישום.</span><span class="sxs-lookup"><span data-stu-id="2088b-230">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="2088b-231">ווינדוס 10</span><span class="sxs-lookup"><span data-stu-id="2088b-231">Windows 10</span></span>

<span data-ttu-id="2088b-232">מיקרוסופט 365 עסקים Premium כולל Windows 10 עסקים, אשר ניתן להתקין עם Windows טייס אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="2088b-232">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="2088b-233">כאשר אתה מעביר ל-Microsoft 365 E3, כל רשיון משתמש כולל Windows 10 Enterprise E3, אשר ניתן גם להתקין עם Windows טייס אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="2088b-233">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="2088b-234">מיקרוסופט 365 אפליקציות לעסקים</span><span class="sxs-lookup"><span data-stu-id="2088b-234">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="2088b-235">היישומים שלך ב-Microsoft 365 ללקוח עסקי המותקנים במכשירים שלך יתחילו באופן אוטומטי להשתמש בתכונות של Microsoft 365 Apps עבור הארגון.</span><span class="sxs-lookup"><span data-stu-id="2088b-235">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="2088b-236">לאחר ההעברה, באפשרותך להשתמש כעת:</span><span class="sxs-lookup"><span data-stu-id="2088b-236">After migration, you can now use:</span></span>

 - <span data-ttu-id="2088b-237">הפעלת אמצעי אחסון באמצעות מדיניות קבוצתית</span><span class="sxs-lookup"><span data-stu-id="2088b-237">Volume activation through Group Policy</span></span>
 - <span data-ttu-id="2088b-238">טלמטריה אפליקציות</span><span class="sxs-lookup"><span data-stu-id="2088b-238">App telemetry</span></span>
 - <span data-ttu-id="2088b-239">עדכן פקדים</span><span class="sxs-lookup"><span data-stu-id="2088b-239">Update controls</span></span>
 - <span data-ttu-id="2088b-240">גיליון אלקטרוני להשוות ולברר</span><span class="sxs-lookup"><span data-stu-id="2088b-240">Spreadsheet compare and inquire</span></span>
 - <span data-ttu-id="2088b-241">בינה עסקית</span><span class="sxs-lookup"><span data-stu-id="2088b-241">Business intelligence</span></span>

