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
ms.openlocfilehash: fbd5c0710bffa92cfc17447094bb9b2683641d5f
ms.sourcegitcommit: c083602dda3cdcb5b58cb8aa070d77019075f765
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/22/2020
ms.locfileid: "48195518"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="5d3b9-103">העברה מ-Microsoft 365 Business Premium ל-Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="5d3b9-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="5d3b9-104">Microsoft 365 Business Premium כולל את כל מה שדרוש לך עבור העסק הקטן שלך, תוך שילוב יישומי הפרודוקטיביות המבוססים על ענן ברמה הטובה ביותר עם ניהול מכשירים ואבטחה פשוטים המאפשרים לעובדים לבצע את עבודתם הטובה ביותר.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="5d3b9-105">עם זאת, במקרים מסוימים, ייתכן שיהיה עליך להעביר את מנוי Microsoft 365 Business Premium שלך ל-Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span> 

<span data-ttu-id="5d3b9-106">לדוגמה, העסק שלך גדל וזקוק ליותר מ-300 רשיונות (מזל טוב, דרך אגב).</span><span class="sxs-lookup"><span data-stu-id="5d3b9-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="5d3b9-107">לחלופין, העסק שלך זקוק לתכונות ארגוניות, כגון יישומי Microsoft 365 עבור enterprise, Windows 10 Enterprise E3 או רשיונות של גישת לקוח ארגוניים (רשיונות גישת לקוח).</span><span class="sxs-lookup"><span data-stu-id="5d3b9-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="5d3b9-108">שדרוג קל: באפשרותך להפעיל את השדרוג [ממרכז הניהול](../commerce/subscriptions/upgrade-to-different-plan.md).</span><span class="sxs-lookup"><span data-stu-id="5d3b9-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="5d3b9-109">כל הנתונים והתצורה במנוי הנוכחי שלך נשמרים.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="5d3b9-110">אין לך מה לעשות כדי להתכונן להעברה ואין מה לעשות לאחר מכן, למעט לנצל את התכונות החדשות.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

>[!Note]
><span data-ttu-id="5d3b9-111">באפשרותך גם להשתמש במנוי של Microsoft 365 Business Premium עבור עד 300 מושבים ולקבל מנוי של Microsoft 365 E3 עבור יותר מ-300 מושבים.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="5d3b9-112">עם זאת, Office 365 ATP אינו כלול ב-Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-112">However, Office 365 ATP is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="5d3b9-113">לצורך הגנת האיום המתמשכת, עליך להוסיף רשיונות נוספים של Office 365 ATP כך שכל המשתמשים בטווח של משטרת ה-ATP של Office 365 שלך יהיו בעלי רשיון.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-113">For continued threat protection, you should add additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span>
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="5d3b9-114">הבדלים בין Microsoft 365 Business Premium ו-Microsoft 365 Enterprise</span><span class="sxs-lookup"><span data-stu-id="5d3b9-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="5d3b9-115">טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium ו-Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="5d3b9-116">תכונה</span><span class="sxs-lookup"><span data-stu-id="5d3b9-116">Feature</span></span>    | <span data-ttu-id="5d3b9-117">תמיכה ב-Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="5d3b9-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="5d3b9-118">תמיכה ב-Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="5d3b9-118">Support in Microsoft 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="5d3b9-119">**מקומי**</span><span class="sxs-lookup"><span data-stu-id="5d3b9-119">**On-premises**</span></span>        | | | 
| <span data-ttu-id="5d3b9-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="5d3b9-120">Windows 10</span></span>    | <span data-ttu-id="5d3b9-121">Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="5d3b9-121">Windows 10 Business</span></span>  |     <span data-ttu-id="5d3b9-122">Windows 10 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="5d3b9-122">Windows 10 Enterprise E3</span></span>| 
| <span data-ttu-id="5d3b9-123">יישומי Office \*</span><span class="sxs-lookup"><span data-stu-id="5d3b9-123">Office apps\*</span></span>    | [<span data-ttu-id="5d3b9-124">אפליקציות Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="5d3b9-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="5d3b9-125">Microsoft 365 Apps for enterprise</span><span class="sxs-lookup"><span data-stu-id="5d3b9-125">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="5d3b9-126">**אפליקציות לפרודוקטיביות בענן**</span><span class="sxs-lookup"><span data-stu-id="5d3b9-126">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="5d3b9-127">Exchange Online ו-Outlook</span><span class="sxs-lookup"><span data-stu-id="5d3b9-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="5d3b9-128">מגבלת אחסון של 50 GB לכל תיבת דואר ואחסון בארכיון באופן בלתי מוגבל של Exchange Online</span><span class="sxs-lookup"><span data-stu-id="5d3b9-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="5d3b9-129">מגבלת אחסון של 100 GB לכל תיבת דואר ואחסון בארכיון באופן בלתי מוגבל של Exchange Online</span><span class="sxs-lookup"><span data-stu-id="5d3b9-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> | 
| <span data-ttu-id="5d3b9-130">Teams</span><span class="sxs-lookup"><span data-stu-id="5d3b9-130">Teams</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-133">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="5d3b9-133">OneDrive for Business</span></span>    | <span data-ttu-id="5d3b9-134">מגבלת אחסון של 1 TB לכל משתמש</span><span class="sxs-lookup"><span data-stu-id="5d3b9-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="5d3b9-135">גבלה</span><span class="sxs-lookup"><span data-stu-id="5d3b9-135">Unlimited</span></span> | 
| <span data-ttu-id="5d3b9-136">קטרת, SharePoint Online, מתכנן תכנון, זרם</span><span class="sxs-lookup"><span data-stu-id="5d3b9-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-139">Outlook Customer Manager, MileIQ</span><span class="sxs-lookup"><span data-stu-id="5d3b9-139">Outlook Customer Manager, MileIQ</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="5d3b9-141">**הגנה מפני איום**</span><span class="sxs-lookup"><span data-stu-id="5d3b9-141">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="5d3b9-142">יכולות הפחתת משטח התקפה</span><span class="sxs-lookup"><span data-stu-id="5d3b9-142">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="5d3b9-143">הצגת רשימה זו</span><span class="sxs-lookup"><span data-stu-id="5d3b9-143">See this list</span></span>](#threat-protection) | <span data-ttu-id="5d3b9-144">ניהול ארגוני של בידוד מבוסס חומרה עבור Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="5d3b9-144">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> | 
| <span data-ttu-id="5d3b9-145">תוכנית מתקדמת של הגנה מפני איום של Office 365 (ATP) תוכנית 1</span><span class="sxs-lookup"><span data-stu-id="5d3b9-145">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="5d3b9-147">לא כלול, אך ניתן להוסיף אותו</span><span class="sxs-lookup"><span data-stu-id="5d3b9-147">Not included, but can be added on</span></span> | 
| <span data-ttu-id="5d3b9-148">**ניהול זהויות**</span><span class="sxs-lookup"><span data-stu-id="5d3b9-148">**Identity management**</span></span>        | | | 
| <span data-ttu-id="5d3b9-149">איפוס סיסמה בשירות עצמי עבור חשבונות היברידית תכלת Active Directory (תכלת לספירה), הודעות מרובות-גורמי אימות (מכשפות אחרות), גישה מותנית, סיסמה writeback עבור זהויות מקומיות</span><span class="sxs-lookup"><span data-stu-id="5d3b9-149">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-152">גילוי אפליקציית הענן, התחברות בריאות של תכלת</span><span class="sxs-lookup"><span data-stu-id="5d3b9-152">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-154">כניסה יחידה של הודעות מיידיות של Office 365 יישומי כניסה יחידה (SSO): 10 אפליקציות לכל משתמש (גלריה סאס apps כגון Salesforce) \*</span><span class="sxs-lookup"><span data-stu-id="5d3b9-154">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-157">התאמה אישית של תכלת לספירה 1-SSO: ללא מגבלה (יישומים מקומיים באמצעות האפליקציה ' הודעות מיידיות ' של יישומי Proxy ויישומים שאינם בגלריה באמצעות תבניות שילוב של יישומים בשירות עצמי</span><span class="sxs-lookup"><span data-stu-id="5d3b9-157">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-159">**ניהול מכשירים ויישומים**</span><span class="sxs-lookup"><span data-stu-id="5d3b9-159">**Device and app management**</span></span>        | | | 
| <span data-ttu-id="5d3b9-160">Microsoft intune, Windows טייס אוטומטי</span><span class="sxs-lookup"><span data-stu-id="5d3b9-160">Microsoft Intune, Windows Autopilot</span></span>|     ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="5d3b9-163">גישה לשולחן עבודה וירטואלי (VDA)</span><span class="sxs-lookup"><span data-stu-id="5d3b9-163">Virtual Desktop Access (VDA)</span></span>    |  |     ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="5d3b9-165">שולחן העבודה של Windows Virtual (WVD)</span><span class="sxs-lookup"><span data-stu-id="5d3b9-165">Windows Virtual Desktop (WVD)</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png) |     ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
|<span data-ttu-id="5d3b9-168">הפעלת מחשב משותף (SCA)</span><span class="sxs-lookup"><span data-stu-id="5d3b9-168">Shared Computer Activation (SCA)</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png) |     ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-171">חבילת אופטימיזציה לשולחן העבודה של Microsoft</span><span class="sxs-lookup"><span data-stu-id="5d3b9-171">Microsoft Desktop Optimization Package</span></span>    | |     ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-173">**הגנה על מידע**</span><span class="sxs-lookup"><span data-stu-id="5d3b9-173">**Information protection**</span></span>        | | | 
| <span data-ttu-id="5d3b9-174">מניעת אובדן נתונים של Office 365, מניעת הגנה על מידע תכלת 1</span><span class="sxs-lookup"><span data-stu-id="5d3b9-174">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-177">הגנה על מידע חלון עבור DLP של נקודת קצה</span><span class="sxs-lookup"><span data-stu-id="5d3b9-177">Window Information Protection for endpoint DLP</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-180">**רשיון גישת לקוח (זכויות CAL)**</span><span class="sxs-lookup"><span data-stu-id="5d3b9-180">**Client Access License (CAL rights)**</span></span>    | | |     
| <span data-ttu-id="5d3b9-181">חבילת CAL של Enterprise (Exchange, SharePoint, Skype, Windows, מנהל התצורה של נקודות קצה של Microsoft, ניהול זכויות של Windows)</span><span class="sxs-lookup"><span data-stu-id="5d3b9-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-183">**תאימות**</span><span class="sxs-lookup"><span data-stu-id="5d3b9-183">**Compliance**</span></span>        | | | 
| <span data-ttu-id="5d3b9-184">אחסון בארכיון של דואר אלקטרוני בלתי מוגבל</span><span class="sxs-lookup"><span data-stu-id="5d3b9-184">Unlimited email archiving</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-187">מנהל תאימות</span><span class="sxs-lookup"><span data-stu-id="5d3b9-187">Compliance Manager</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-190">גילוי אלקטרוני</span><span class="sxs-lookup"><span data-stu-id="5d3b9-190">eDiscovery</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-193">חסימה מקומית וחסימה לצורך תביעה משפטית</span><span class="sxs-lookup"><span data-stu-id="5d3b9-193">In-place hold and litigation hold</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="5d3b9-196">תגי שמירה של ניהול רשומות של העברת הודעות (MRM) ומדיניות שמירה</span><span class="sxs-lookup"><span data-stu-id="5d3b9-196">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
||||

<span data-ttu-id="5d3b9-199">\* משתמשים שהוקצו להם גישה לאפליקציות של SaaS יכולים לקבל גישה ל-SSO עד 10 אפליקציות.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-199">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="5d3b9-200">מנהלי מערכת יכולים לקבוע את התצורה של SSO ולשנות את גישת המשתמש ליישומים שונים של SaaS, אך גישת SSO מותרת רק עבור 10 אפליקציות לכל משתמש בכל פעם.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-200">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="5d3b9-201">כל יישומי Office 365 נספרים כאפליקציה אחת.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-201">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="5d3b9-202">העברה</span><span class="sxs-lookup"><span data-stu-id="5d3b9-202">Migration</span></span>

<span data-ttu-id="5d3b9-203">כדי להעביר, עבוד עם השותף שלך כדי להעביר את מנוי Microsoft 365 Business Premium ורשיונות למנוי מתאים של Microsoft 365 E3 עם הרשיונות שלו.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-203">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="5d3b9-204">הסעיפים הבאים מתארים אילו שינויים עליך לבצע, אם בכלל, ומה ניתן לעשות לאחר ההעברה.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-204">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="5d3b9-205">תצורת מנוי ונתונים של Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5d3b9-205">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="5d3b9-206">אין צורך לבצע שינויים במנוי או בנתונים הנוכחיים לפני ההעברה, הכוללת:</span><span class="sxs-lookup"><span data-stu-id="5d3b9-206">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="5d3b9-207">תצורת מנוי, כגון שמות תחומים של DNS.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-207">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="5d3b9-208">חשבונות משתמשים וקבוצות והגדרות אימות, כגון אימות רב-גורמי או מדיניות גישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-208">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="5d3b9-209">תצורות שירות פרודוקטיביות והנתונים שלהם, כגון Teams, תיבות דואר של Exchange Online, אתרי SharePoint Online, תיקיות OneDrive for Business ומחברות OneNote.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-209">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="5d3b9-210">כעת המשתמשים יכולים ליהנות משטח אחסון בלתי מוגבל בתיקיות ' תיבות דואר של Exchange Online ' OneDrive for Business '.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-210">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="5d3b9-211">באפשרותך להתחיל להשתמש בגילוי של אפליקציית הענן, לחבר את בריאות התכלת ולהשתמש ב-SSO עבור יותר מ-10 אפליקציות.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-211">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

>[!Note]
><span data-ttu-id="5d3b9-212">משתמשים שהועברו ל-Microsoft 365 E3 אינם יכולים עוד להשתמש ב-Outlook Customer Manager ו-MileIQ.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-212">Users migrated to Microsoft 365 E3 can no longer use Outlook Customer Manager and MileIQ.</span></span>
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="5d3b9-213">הגנה מפני איום</span><span class="sxs-lookup"><span data-stu-id="5d3b9-213">Threat protection</span></span>

<span data-ttu-id="5d3b9-214">Windows 10 Business כולל הגנות אלה:</span><span class="sxs-lookup"><span data-stu-id="5d3b9-214">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="5d3b9-215">אכיפת תקינות של תהליך אתחול מערכת ההפעלה</span><span class="sxs-lookup"><span data-stu-id="5d3b9-215">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="5d3b9-216">אכיפת תקינות של רכיבי הפעלה רגישים</span><span class="sxs-lookup"><span data-stu-id="5d3b9-216">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="5d3b9-217">פגיעות מתקדמת וגורמים מקלים לניצול של אפס ימים</span><span class="sxs-lookup"><span data-stu-id="5d3b9-217">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="5d3b9-218">הגנה על רשת מבוססת מוניטין עבור Microsoft Edge, Internet Explorer ו-Chrome</span><span class="sxs-lookup"><span data-stu-id="5d3b9-218">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="5d3b9-219">חומת אש מבוססת מארח</span><span class="sxs-lookup"><span data-stu-id="5d3b9-219">Host-based firewall</span></span>
- <span data-ttu-id="5d3b9-220">מזעור Ransomware</span><span class="sxs-lookup"><span data-stu-id="5d3b9-220">Ransomware mitigations</span></span>
- <span data-ttu-id="5d3b9-221">בידוד מבוסס חומרה עבור Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="5d3b9-221">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="5d3b9-222">בקרת יישומים מופעלת על-ידי גרף האבטחה החכם</span><span class="sxs-lookup"><span data-stu-id="5d3b9-222">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="5d3b9-223">פקד מכשיר (USB)</span><span class="sxs-lookup"><span data-stu-id="5d3b9-223">Device control (USB)</span></span>
- <span data-ttu-id="5d3b9-224">הגנה על הרשת עבור איומים מבוססי-אינטרנט</span><span class="sxs-lookup"><span data-stu-id="5d3b9-224">Network protection for web-based threats</span></span>
- <span data-ttu-id="5d3b9-225">כללי מניעת החדירה למארח</span><span class="sxs-lookup"><span data-stu-id="5d3b9-225">Host intrusion prevention rules</span></span>

<span data-ttu-id="5d3b9-226">Windows 10 Enterprise E3 כולל גם ניהול ארגוני של בידוד מבוסס חומרה עבור Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-226">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

>[!Note]
><span data-ttu-id="5d3b9-227">משתמשים שהועברו ל-Microsoft 365 E3 ידרשו לכל אחד מהם לדרוש רשיון של Office 365 ATP עבור הגנה מתמשכת על איום.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-227">Users migrated to Microsoft 365 E3 will each require an Office 365 ATP license for continued threat protection.</span></span> <span data-ttu-id="5d3b9-228">הקפד לרכוש רשיונות נוספים של Office 365 ATP כך שכל המשתמשים בטווח של משטרת ה-ATP של Office 365 שלך יהיו בעלי רשיון.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-228">Be sure to purchase additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span> 
>

### <a name="device-management-with-intune"></a><span data-ttu-id="5d3b9-229">ניהול מכשירים עם כוונון</span><span class="sxs-lookup"><span data-stu-id="5d3b9-229">Device management with Intune</span></span>

<span data-ttu-id="5d3b9-230">אין צורך לבצע שינויים בקביעת התצורה הנוכחית של ' שינוי כיוון ' לפני ההעברה, הכוללת התקנים רשומים והגדרות התקן ואפליקציה.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-230">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="5d3b9-231">Windows 10</span><span class="sxs-lookup"><span data-stu-id="5d3b9-231">Windows 10</span></span>

<span data-ttu-id="5d3b9-232">Microsoft 365 Business Premium כולל את Windows 10 Business, שניתן להתקין באמצעות Windows טייס אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-232">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="5d3b9-233">כאשר אתה מעביר ל-Microsoft 365 E3, כל רשיון משתמש כולל את Windows 10 Enterprise E3, שניתן גם להתקין באמצעות Windows טייס אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-233">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="5d3b9-234">אפליקציות Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="5d3b9-234">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="5d3b9-235">לקוח Microsoft 365 Apps לעסקים המותקן במכשירים שלך יתחיל להשתמש באופן אוטומטי בתכונות של יישומי Microsoft 365 עבור הארגון.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-235">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="5d3b9-236">לאחר ההעברה, כעת באפשרותך להשתמש ב:</span><span class="sxs-lookup"><span data-stu-id="5d3b9-236">After migration, you can now use:</span></span>

 - <span data-ttu-id="5d3b9-237">הפעלת עוצמת הקול במסגרת מדיניות קבוצתית</span><span class="sxs-lookup"><span data-stu-id="5d3b9-237">Volume activation through Group Policy</span></span>
 - <span data-ttu-id="5d3b9-238">טלמטריה באפליקציות</span><span class="sxs-lookup"><span data-stu-id="5d3b9-238">App telemetry</span></span>
 - <span data-ttu-id="5d3b9-239">פקדי עדכון</span><span class="sxs-lookup"><span data-stu-id="5d3b9-239">Update controls</span></span>
 - <span data-ttu-id="5d3b9-240">השוואה בין גליונות אלקטרוניים ובירורים</span><span class="sxs-lookup"><span data-stu-id="5d3b9-240">Spreadsheet compare and inquire</span></span>
 - <span data-ttu-id="5d3b9-241">בינה עסקית</span><span class="sxs-lookup"><span data-stu-id="5d3b9-241">Business intelligence</span></span>

