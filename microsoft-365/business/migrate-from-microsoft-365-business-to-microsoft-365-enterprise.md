---
title: העברה מ-Microsoft 365 Business אל Microsoft 365 E3
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
ms.openlocfilehash: 10630671f3deb7eff0ad0f601d301b90743ee35f
ms.sourcegitcommit: 2a708650b7e30a53d10a2fe3164c6ed5ea37d868
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2021
ms.locfileid: "51164512"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="540be-103">העברה מ-Microsoft 365 Business Premium ל-Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="540be-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="540be-104">Microsoft 365 Business Premium כולל את כל מה שדרוש לך עבור העסק הקטן שלך, תוך שילוב יישומי הפרודוקטיביות המבוססים על ענן ברמה הטובה ביותר עם ניהול מכשירים ואבטחה פשוטים המאפשרים לעובדים לבצע את עבודתם הטובה ביותר.</span><span class="sxs-lookup"><span data-stu-id="540be-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="540be-105">עם זאת, במקרים מסוימים, ייתכן שיהיה עליך להעביר את מנוי Microsoft 365 Business Premium שלך ל-Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="540be-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span> 

<span data-ttu-id="540be-106">לדוגמה, העסק שלך גדל וזקוק ליותר מ-300 רשיונות (מזל טוב, דרך אגב).</span><span class="sxs-lookup"><span data-stu-id="540be-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="540be-107">לחלופין, העסק שלך זקוק לתכונות ארגוניות, כגון יישומי Microsoft 365 עבור enterprise, Windows 10 Enterprise E3 או רשיונות של גישת לקוח ארגוניים (רשיונות גישת לקוח).</span><span class="sxs-lookup"><span data-stu-id="540be-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="540be-108">שדרוג קל: באפשרותך להפעיל את השדרוג [ממרכז הניהול](../commerce/subscriptions/upgrade-to-different-plan.md).</span><span class="sxs-lookup"><span data-stu-id="540be-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="540be-109">כל הנתונים והתצורה במנוי הנוכחי שלך נשמרים.</span><span class="sxs-lookup"><span data-stu-id="540be-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="540be-110">אין לך מה לעשות כדי להתכונן להעברה ואין מה לעשות לאחר מכן, למעט לנצל את התכונות החדשות.</span><span class="sxs-lookup"><span data-stu-id="540be-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

>[!Note]
><span data-ttu-id="540be-111">באפשרותך גם להשתמש במנוי של Microsoft 365 Business Premium עבור עד 300 מושבים ולקבל מנוי של Microsoft 365 E3 עבור יותר מ-300 מושבים.</span><span class="sxs-lookup"><span data-stu-id="540be-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="540be-112">עם זאת, Microsoft Defender עבור Office 365 אינו כלול ב-Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="540be-112">However, Microsoft Defender for Office 365 is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="540be-113">לצורך הגנת האיום המתמשכת, עליך להוסיף רשיונות נוספים של Defender עבור Office 365 כך שכל המשתמשים בטווח של המגן שלך עבור משטרת Office 365 יהיו בעלי רשיון.</span><span class="sxs-lookup"><span data-stu-id="540be-113">For continued threat protection, you should add additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span>
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="540be-114">הבדלים בין Microsoft 365 Business Premium ו-Microsoft 365 Enterprise</span><span class="sxs-lookup"><span data-stu-id="540be-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="540be-115">טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium ו-Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="540be-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="540be-116">תכונה</span><span class="sxs-lookup"><span data-stu-id="540be-116">Feature</span></span>    | <span data-ttu-id="540be-117">תמיכה ב-Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="540be-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="540be-118">תמיכה ב-Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="540be-118">Support in Microsoft 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="540be-119">**מקומי**</span><span class="sxs-lookup"><span data-stu-id="540be-119">**On-premises**</span></span>        | | | 
| <span data-ttu-id="540be-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="540be-120">Windows 10</span></span>    | <span data-ttu-id="540be-121">Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="540be-121">Windows 10 Business</span></span>  |     <span data-ttu-id="540be-122">Windows 10 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="540be-122">Windows 10 Enterprise E3</span></span>| 
| <span data-ttu-id="540be-123">יישומי Office \*</span><span class="sxs-lookup"><span data-stu-id="540be-123">Office apps\*</span></span>    | [<span data-ttu-id="540be-124">אפליקציות Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="540be-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="540be-125">יישומי Microsoft 365 עבור ארגונים</span><span class="sxs-lookup"><span data-stu-id="540be-125">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="540be-126">**אפליקציות לפרודוקטיביות בענן**</span><span class="sxs-lookup"><span data-stu-id="540be-126">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="540be-127">Exchange Online ו-Outlook</span><span class="sxs-lookup"><span data-stu-id="540be-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="540be-128">מגבלת אחסון של 50 GB לכל תיבת דואר ואחסון בארכיון באופן בלתי מוגבל של Exchange Online</span><span class="sxs-lookup"><span data-stu-id="540be-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="540be-129">מגבלת אחסון של 100 GB לכל תיבת דואר ואחסון בארכיון באופן בלתי מוגבל של Exchange Online</span><span class="sxs-lookup"><span data-stu-id="540be-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> | 
| <span data-ttu-id="540be-130">Teams</span><span class="sxs-lookup"><span data-stu-id="540be-130">Teams</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-133">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="540be-133">OneDrive for Business</span></span>    | <span data-ttu-id="540be-134">מגבלת אחסון של 1 TB לכל משתמש</span><span class="sxs-lookup"><span data-stu-id="540be-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="540be-135">גבלה</span><span class="sxs-lookup"><span data-stu-id="540be-135">Unlimited</span></span> | 
| <span data-ttu-id="540be-136">קטרת, SharePoint Online, מתכנן תכנון, זרם</span><span class="sxs-lookup"><span data-stu-id="540be-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-139">**הגנה מפני איום**</span><span class="sxs-lookup"><span data-stu-id="540be-139">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="540be-140">יכולות הפחתת משטח התקפה</span><span class="sxs-lookup"><span data-stu-id="540be-140">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="540be-141">הצגת רשימה זו</span><span class="sxs-lookup"><span data-stu-id="540be-141">See this list</span></span>](#threat-protection) | <span data-ttu-id="540be-142">ניהול ארגוני של בידוד מבוסס חומרה עבור Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="540be-142">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> | 
| <span data-ttu-id="540be-143">Defender עבור Office 365 תוכנית 1</span><span class="sxs-lookup"><span data-stu-id="540be-143">Defender for Office 365 Plan 1</span></span> | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="540be-145">לא כלול, אך ניתן להוסיף אותו</span><span class="sxs-lookup"><span data-stu-id="540be-145">Not included, but can be added on</span></span> | 
| <span data-ttu-id="540be-146">**ניהול זהויות**</span><span class="sxs-lookup"><span data-stu-id="540be-146">**Identity management**</span></span>        | | | 
| <span data-ttu-id="540be-147">איפוס סיסמה בשירות עצמי עבור חשבונות היברידית תכלת Active Directory (תכלת לספירה), באמצעות מספר מרבי של אימות רב-גורמי (מפעל מרכזי), גישה מותנית, סיסמה writeback עבור זהויות מקומיות</span><span class="sxs-lookup"><span data-stu-id="540be-147">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-150">גילוי אפליקציית הענן, התחברות בריאות של תכלת</span><span class="sxs-lookup"><span data-stu-id="540be-150">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-152">אפליקציות של הודעות מיידיות של Office 365 בודדות Sign-On (SSO): 10 אפליקציות לכל משתמש (גלריה סאס apps כגון Salesforce) \*</span><span class="sxs-lookup"><span data-stu-id="540be-152">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-155">Self-Service שילוב מוגבל של הודעות מיידיות באפליקציות מקומיות באמצעות מכ</span><span class="sxs-lookup"><span data-stu-id="540be-155">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-157">**ניהול מכשירים ויישומים**</span><span class="sxs-lookup"><span data-stu-id="540be-157">**Device and app management**</span></span>        | | | 
| <span data-ttu-id="540be-158">Microsoft intune, Windows טייס אוטומטי</span><span class="sxs-lookup"><span data-stu-id="540be-158">Microsoft Intune, Windows Autopilot</span></span>|     ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="540be-161">גישה לשולחן עבודה וירטואלי (VDA)</span><span class="sxs-lookup"><span data-stu-id="540be-161">Virtual Desktop Access (VDA)</span></span>    |  |     ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="540be-163">שולחן העבודה של Windows Virtual (WVD)</span><span class="sxs-lookup"><span data-stu-id="540be-163">Windows Virtual Desktop (WVD)</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png) |     ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="540be-166">הפעלת מחשב משותף (SCA)</span><span class="sxs-lookup"><span data-stu-id="540be-166">Shared Computer Activation (SCA)</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png) |     ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-169">חבילת אופטימיזציה לשולחן העבודה של Microsoft</span><span class="sxs-lookup"><span data-stu-id="540be-169">Microsoft Desktop Optimization Package</span></span>    | |     ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-171">**הגנה על מידע**</span><span class="sxs-lookup"><span data-stu-id="540be-171">**Information protection**</span></span>        | | | 
| <span data-ttu-id="540be-172">מניעת אובדן נתונים של Office 365, מניעת הגנה על מידע תכלת 1</span><span class="sxs-lookup"><span data-stu-id="540be-172">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-175">הגנה על מידע חלון עבור DLP של נקודת קצה</span><span class="sxs-lookup"><span data-stu-id="540be-175">Window Information Protection for endpoint DLP</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-178">**רשיון גישת לקוח (זכויות CAL)**</span><span class="sxs-lookup"><span data-stu-id="540be-178">**Client Access License (CAL rights)**</span></span>    | | |     
| <span data-ttu-id="540be-179">חבילת CAL של Enterprise (Exchange, SharePoint, Skype, Windows, מנהל התצורה של נקודות קצה של Microsoft, ניהול זכויות של Windows)</span><span class="sxs-lookup"><span data-stu-id="540be-179">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-181">**תאימות**</span><span class="sxs-lookup"><span data-stu-id="540be-181">**Compliance**</span></span>        | | | 
| <span data-ttu-id="540be-182">אחסון בארכיון של דואר אלקטרוני בלתי מוגבל</span><span class="sxs-lookup"><span data-stu-id="540be-182">Unlimited email archiving</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-185">מנהל תאימות</span><span class="sxs-lookup"><span data-stu-id="540be-185">Compliance Manager</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-188">גילוי אלקטרוני</span><span class="sxs-lookup"><span data-stu-id="540be-188">eDiscovery</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-191">חסימה מקומית וחסימה לצורך תביעה משפטית</span><span class="sxs-lookup"><span data-stu-id="540be-191">In-place hold and litigation hold</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="540be-194">תגי שמירה של ניהול רשומות של העברת הודעות (MRM) ומדיניות שמירה</span><span class="sxs-lookup"><span data-stu-id="540be-194">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
||||

<span data-ttu-id="540be-197">\* משתמשים שהוקצו להם גישה לאפליקציות של SaaS יכולים לקבל גישה ל-SSO עד 10 אפליקציות.</span><span class="sxs-lookup"><span data-stu-id="540be-197">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="540be-198">מנהלי מערכת יכולים לקבוע את התצורה של SSO ולשנות את גישת המשתמש ליישומים שונים של SaaS, אך גישת SSO מותרת רק עבור 10 אפליקציות לכל משתמש בכל פעם.</span><span class="sxs-lookup"><span data-stu-id="540be-198">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="540be-199">כל יישומי Office 365 נספרים כאפליקציה אחת.</span><span class="sxs-lookup"><span data-stu-id="540be-199">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="540be-200">העברה</span><span class="sxs-lookup"><span data-stu-id="540be-200">Migration</span></span>

<span data-ttu-id="540be-201">כדי להעביר, עבוד עם השותף שלך כדי להעביר את מנוי Microsoft 365 Business Premium ורשיונות למנוי מתאים של Microsoft 365 E3 עם הרשיונות שלו.</span><span class="sxs-lookup"><span data-stu-id="540be-201">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="540be-202">הסעיפים הבאים מתארים אילו שינויים עליך לבצע, אם בכלל, ומה ניתן לעשות לאחר ההעברה.</span><span class="sxs-lookup"><span data-stu-id="540be-202">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="540be-203">תצורת מנוי ונתונים של Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="540be-203">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="540be-204">אין צורך לבצע שינויים במנוי או בנתונים הנוכחיים לפני ההעברה, הכוללת:</span><span class="sxs-lookup"><span data-stu-id="540be-204">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="540be-205">תצורת מנוי, כגון שמות תחומים של DNS.</span><span class="sxs-lookup"><span data-stu-id="540be-205">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="540be-206">חשבונות משתמשים וקבוצות והגדרות אימות, כגון אימות רב-גורמי או מדיניות גישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="540be-206">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="540be-207">תצורות שירות פרודוקטיביות והנתונים שלהם, כגון Teams, תיבות דואר של Exchange Online, אתרי SharePoint Online, תיקיות OneDrive for Business ומחברות OneNote.</span><span class="sxs-lookup"><span data-stu-id="540be-207">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="540be-208">כעת המשתמשים יכולים ליהנות משטח אחסון בלתי מוגבל בתיקיות ' תיבות דואר של Exchange Online ' OneDrive for Business '.</span><span class="sxs-lookup"><span data-stu-id="540be-208">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="540be-209">באפשרותך להתחיל להשתמש בגילוי של אפליקציית הענן, לחבר את בריאות התכלת ולהשתמש ב-SSO עבור יותר מ-10 אפליקציות.</span><span class="sxs-lookup"><span data-stu-id="540be-209">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="540be-210">הגנה מפני איום</span><span class="sxs-lookup"><span data-stu-id="540be-210">Threat protection</span></span>

<span data-ttu-id="540be-211">Windows 10 Business כולל הגנות אלה:</span><span class="sxs-lookup"><span data-stu-id="540be-211">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="540be-212">אכיפת תקינות של תהליך אתחול מערכת ההפעלה</span><span class="sxs-lookup"><span data-stu-id="540be-212">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="540be-213">אכיפת תקינות של רכיבי הפעלה רגישים</span><span class="sxs-lookup"><span data-stu-id="540be-213">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="540be-214">פגיעות מתקדמת וגורמים מקלים לניצול של אפס ימים</span><span class="sxs-lookup"><span data-stu-id="540be-214">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="540be-215">הגנה על רשת מבוססת מוניטין עבור Microsoft Edge, Internet Explorer ו-Chrome</span><span class="sxs-lookup"><span data-stu-id="540be-215">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="540be-216">חומת אש מבוססת מארח</span><span class="sxs-lookup"><span data-stu-id="540be-216">Host-based firewall</span></span>
- <span data-ttu-id="540be-217">מזעור Ransomware</span><span class="sxs-lookup"><span data-stu-id="540be-217">Ransomware mitigations</span></span>
- <span data-ttu-id="540be-218">בידוד מבוסס חומרה עבור Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="540be-218">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="540be-219">בקרת יישומים מופעלת על-ידי גרף האבטחה החכם</span><span class="sxs-lookup"><span data-stu-id="540be-219">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="540be-220">פקד מכשיר (USB)</span><span class="sxs-lookup"><span data-stu-id="540be-220">Device control (USB)</span></span>
- <span data-ttu-id="540be-221">הגנה על הרשת עבור איומים מבוססי-אינטרנט</span><span class="sxs-lookup"><span data-stu-id="540be-221">Network protection for web-based threats</span></span>
- <span data-ttu-id="540be-222">כללי מניעת החדירה למארח</span><span class="sxs-lookup"><span data-stu-id="540be-222">Host intrusion prevention rules</span></span>

<span data-ttu-id="540be-223">Windows 10 Enterprise E3 כולל גם ניהול ארגוני של בידוד מבוסס חומרה עבור Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="540be-223">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

>[!Note]
><span data-ttu-id="540be-224">משתמשים שהועברו ל-Microsoft 365 E3 ידרשו מכל אחד מהם לדרוש רשיון של Microsoft Defender עבור Office 365 לצורך הגנה על האיום המתמשך.</span><span class="sxs-lookup"><span data-stu-id="540be-224">Users migrated to Microsoft 365 E3 will each require a Microsoft Defender for Office 365 license for continued threat protection.</span></span> <span data-ttu-id="540be-225">הקפד לרכוש רשיונות נוספים של Defender עבור Office 365 כך שכל המשתמשים בטווח של המגן שלך עבור משטרת Office 365 יהיו בעלי רשיון.</span><span class="sxs-lookup"><span data-stu-id="540be-225">Be sure to purchase additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span> 
>

### <a name="device-management-with-intune"></a><span data-ttu-id="540be-226">ניהול מכשירים עם כוונון</span><span class="sxs-lookup"><span data-stu-id="540be-226">Device management with Intune</span></span>

<span data-ttu-id="540be-227">אין צורך לבצע שינויים בקביעת התצורה הנוכחית של ' שינוי כיוון ' לפני ההעברה, הכוללת התקנים רשומים והגדרות התקן ואפליקציה.</span><span class="sxs-lookup"><span data-stu-id="540be-227">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="540be-228">Windows 10</span><span class="sxs-lookup"><span data-stu-id="540be-228">Windows 10</span></span>

<span data-ttu-id="540be-229">Microsoft 365 Business Premium כולל את Windows 10 Business, שניתן להתקין באמצעות Windows טייס אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="540be-229">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="540be-230">כאשר אתה מעביר ל-Microsoft 365 E3, כל רשיון משתמש כולל את Windows 10 Enterprise E3, שניתן גם להתקין באמצעות Windows טייס אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="540be-230">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="540be-231">אפליקציות Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="540be-231">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="540be-232">לקוח Microsoft 365 Apps לעסקים המותקן במכשירים שלך יתחיל להשתמש באופן אוטומטי בתכונות של יישומי Microsoft 365 עבור הארגון.</span><span class="sxs-lookup"><span data-stu-id="540be-232">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="540be-233">לאחר ההעברה, כעת באפשרותך להשתמש ב:</span><span class="sxs-lookup"><span data-stu-id="540be-233">After migration, you can now use:</span></span>

 - <span data-ttu-id="540be-234">תמיכה במדיניות קבוצתית</span><span class="sxs-lookup"><span data-stu-id="540be-234">Group Policy support</span></span>
 - <span data-ttu-id="540be-235">השוואה בין גליונות אלקטרוניים ובירורים</span><span class="sxs-lookup"><span data-stu-id="540be-235">Spreadsheet compare and inquire</span></span>
 - <span data-ttu-id="540be-236">בינה עסקית</span><span class="sxs-lookup"><span data-stu-id="540be-236">Business intelligence</span></span>

