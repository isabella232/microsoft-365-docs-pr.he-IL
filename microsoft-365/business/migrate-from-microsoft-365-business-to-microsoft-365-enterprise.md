---
title: מעבר מ- Microsoft 365 Business ל- Microsoft 365 E3
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
description: למד כיצד להעביר את העסק שלך Microsoft 365 Business Premium אל Microsoft 365 E3.
ms.openlocfilehash: 6502d79dbb283db37b00e4fccf89b15ab4291ce5
ms.sourcegitcommit: 48195345b21b409b175d68acdc25d9f2fc4fc5f1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/30/2021
ms.locfileid: "53227618"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="2818f-103">מעבר מ- Microsoft 365 Business Premium אל Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="2818f-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="2818f-104">Microsoft 365 Business Premium כולל את כל מה שאתה צריך עבור העסק הקטן שלך, המשלב את יישומי הפרודוקטיביות מבוססי הענן הטובים ביותר מסוגם עם ניהול מכשירים ואבטחה פשוטים המאפשרים לעובדים שלך לעשות את העבודה הטובה ביותר שלהם.</span><span class="sxs-lookup"><span data-stu-id="2818f-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="2818f-105">עם זאת, במקרים מסוימים, ייתכן שתצטרך להעביר את המנוי Microsoft 365 Business Premium שלך Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="2818f-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span>

<span data-ttu-id="2818f-106">לדוגמה, העסק שלך גדל וצרכים יותר מ- 300 רשיונות (מזל טוב, דרך אגב).</span><span class="sxs-lookup"><span data-stu-id="2818f-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="2818f-107">לחלופין, העסק שלך זקוק לתכונות ארגוניות, כגון יישומי Microsoft 365 לארגונים, Windows 10 Enterprise E3 או Enterprise Client Access (CALs).</span><span class="sxs-lookup"><span data-stu-id="2818f-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="2818f-108">השדרוג קל: באפשרותך להתחיל את השדרוג [ממרכז הניהול.](../commerce/subscriptions/upgrade-to-different-plan.md)</span><span class="sxs-lookup"><span data-stu-id="2818f-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="2818f-109">כל הנתונים והתצורה שלך במנוי הנוכחי שלך נשמרים.</span><span class="sxs-lookup"><span data-stu-id="2818f-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="2818f-110">אין לך מה לעשות כדי להתכונן להעברה ולא לעשות דבר לאחר מכן, למעט לנצל את התכונות החדשות.</span><span class="sxs-lookup"><span data-stu-id="2818f-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

> [!NOTE]
> <span data-ttu-id="2818f-111">באפשרותך גם להשתמש במנוי Microsoft 365 Business Premium עבור עד 300 מושבים, לקבל מנוי Microsoft 365 E3 עבור יותר מ- 300 מושבים.</span><span class="sxs-lookup"><span data-stu-id="2818f-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="2818f-112">עם זאת, Microsoft Defender עבור Office 365 אינו כלול ב- Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="2818f-112">However, Microsoft Defender for Office 365 is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="2818f-113">לקבלת הגנה ממשכת על איומים, עליך להוסיף את Defender Office 365 עבור רשיונות נוספים, כך שכל המשתמשים בטווח של Defender עבור Office 365 שלך מורשים.</span><span class="sxs-lookup"><span data-stu-id="2818f-113">For continued threat protection, you should add additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="2818f-114">הבדלים בין Microsoft 365 Business Premium לבין Microsoft 365 Enterprise</span><span class="sxs-lookup"><span data-stu-id="2818f-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="2818f-115">טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium לבין Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="2818f-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="2818f-116">תכונה</span><span class="sxs-lookup"><span data-stu-id="2818f-116">Feature</span></span>    | <span data-ttu-id="2818f-117">תמיכה Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="2818f-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="2818f-118">תמיכה Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="2818f-118">Support in Microsoft 365 E3</span></span> |
|:-------|:-----|:-----|
| <span data-ttu-id="2818f-119">**מקומי**</span><span class="sxs-lookup"><span data-stu-id="2818f-119">**On-premises**</span></span>        | | |
| <span data-ttu-id="2818f-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="2818f-120">Windows 10</span></span>    | <span data-ttu-id="2818f-121">Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="2818f-121">Windows 10 Business</span></span>  |     <span data-ttu-id="2818f-122">Windows 10 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="2818f-122">Windows 10 Enterprise E3</span></span>|
| <span data-ttu-id="2818f-123">Office אפליקציות\*</span><span class="sxs-lookup"><span data-stu-id="2818f-123">Office apps\*</span></span>    | [<span data-ttu-id="2818f-124">יישומי Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="2818f-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="2818f-125">יישומי Microsoft 365 עבור ארגונים</span><span class="sxs-lookup"><span data-stu-id="2818f-125">Microsoft 365 Apps for enterprise</span></span> |
| <span data-ttu-id="2818f-126">**יישומי פרודוקטיביות בענן**</span><span class="sxs-lookup"><span data-stu-id="2818f-126">**Cloud productivity apps**</span></span>        | | |
| <span data-ttu-id="2818f-127">Exchange Online ו- Outlook</span><span class="sxs-lookup"><span data-stu-id="2818f-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="2818f-128">מגבלת אחסון של 50 GB לכל תיבת דואר ואחסון Exchange Online בארכיון</span><span class="sxs-lookup"><span data-stu-id="2818f-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="2818f-129">מגבלת אחסון של 100 GB לכל תיבת דואר ואחסון Exchange Online בארכיון</span><span class="sxs-lookup"><span data-stu-id="2818f-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> |
| <span data-ttu-id="2818f-130">Teams</span><span class="sxs-lookup"><span data-stu-id="2818f-130">Teams</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-133">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="2818f-133">OneDrive for Business</span></span>    | <span data-ttu-id="2818f-134">מגבלת אחסון של 1 TB לכל משתמש</span><span class="sxs-lookup"><span data-stu-id="2818f-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="2818f-135">ללא הגבלה</span><span class="sxs-lookup"><span data-stu-id="2818f-135">Unlimited</span></span> |
| <span data-ttu-id="2818f-136">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="2818f-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-139">**הגנה מפני איומים**</span><span class="sxs-lookup"><span data-stu-id="2818f-139">**Threat Protection**</span></span>        | | |
| <span data-ttu-id="2818f-140">יכולות הפחתת פני השטח של תקיפה</span><span class="sxs-lookup"><span data-stu-id="2818f-140">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="2818f-141">ראה רשימה זו</span><span class="sxs-lookup"><span data-stu-id="2818f-141">See this list</span></span>](#threat-protection) | <span data-ttu-id="2818f-142">ניהול ארגוני של בידוד מבוסס-חומרה עבור Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2818f-142">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> |
| <span data-ttu-id="2818f-143">Defender for Office 365 תוכנית 1</span><span class="sxs-lookup"><span data-stu-id="2818f-143">Defender for Office 365 Plan 1</span></span> | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="2818f-145">לא כלול, אך ניתן להוסיף אותו</span><span class="sxs-lookup"><span data-stu-id="2818f-145">Not included, but can be added on</span></span> |
| <span data-ttu-id="2818f-146">**ניהול זהויות**</span><span class="sxs-lookup"><span data-stu-id="2818f-146">**Identity management**</span></span>        | | |
| <span data-ttu-id="2818f-147">איפוס סיסמה בשירות עצמי עבור חשבונות היברידיים של Azure Active Directory (Azure AD), אימות רב-גורמי של Azure AD (MFA), Access מותן, writeback באמצעות סיסמה עבור זהויות מקומיות</span><span class="sxs-lookup"><span data-stu-id="2818f-147">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-150">גילוי יישום ענן, Azure AD התחברות תקינות</span><span class="sxs-lookup"><span data-stu-id="2818f-150">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-152">Azure AD Office 365 יחיד Sign-On (SSO): 10 אפליקציות לכל משתמש (אפליקציות Gallery SaaS כגון Salesforce)\*</span><span class="sxs-lookup"><span data-stu-id="2818f-152">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-155">Azure AD Premium SSO 1: ללא הגבלה (יישומים מקומיים באמצעות Azure AD Application Proxy ואפליקציות שאינן גלריה באמצעות תבניות Self-Service שילוב יישומים)</span><span class="sxs-lookup"><span data-stu-id="2818f-155">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-157">**ניהול מכשירים ואפליקציות**</span><span class="sxs-lookup"><span data-stu-id="2818f-157">**Device and app management**</span></span>        | | |
| <span data-ttu-id="2818f-158">Microsoft Intune, Windows אוטומטי</span><span class="sxs-lookup"><span data-stu-id="2818f-158">Microsoft Intune, Windows Autopilot</span></span>|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
|<span data-ttu-id="2818f-161">Virtual Desktop Access (VDA)</span><span class="sxs-lookup"><span data-stu-id="2818f-161">Virtual Desktop Access (VDA)</span></span>    |  |     ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
|<span data-ttu-id="2818f-163">Windows Virtual Desktop (WVD)</span><span class="sxs-lookup"><span data-stu-id="2818f-163">Windows Virtual Desktop (WVD)</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png) |     ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
|<span data-ttu-id="2818f-166">הפעלת מחשב משותפת (SCA)</span><span class="sxs-lookup"><span data-stu-id="2818f-166">Shared Computer Activation (SCA)</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png) |     ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-169">חבילת מיטוב שולחן העבודה של Microsoft</span><span class="sxs-lookup"><span data-stu-id="2818f-169">Microsoft Desktop Optimization Package</span></span>    | |     ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-171">**הגנה על מידע**</span><span class="sxs-lookup"><span data-stu-id="2818f-171">**Information protection**</span></span>        | | |
| <span data-ttu-id="2818f-172">Office 365 מניעת אובדן נתונים, תוכנית Azure Information Protection 1</span><span class="sxs-lookup"><span data-stu-id="2818f-172">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-175">הגנה על פרטי חלון עבור DLP של נקודת קצה</span><span class="sxs-lookup"><span data-stu-id="2818f-175">Window Information Protection for endpoint DLP</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-178">**לקוח Access רשיון (זכויות CAL)**</span><span class="sxs-lookup"><span data-stu-id="2818f-178">**Client Access License (CAL rights)**</span></span>    | | |
| <span data-ttu-id="2818f-179">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows ניהול זכויות)</span><span class="sxs-lookup"><span data-stu-id="2818f-179">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-181">**תאימות**</span><span class="sxs-lookup"><span data-stu-id="2818f-181">**Compliance**</span></span>        | | |
| <span data-ttu-id="2818f-182">אחסון דואר אלקטרוני בארכיון ללא הגבלה</span><span class="sxs-lookup"><span data-stu-id="2818f-182">Unlimited email archiving</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-185">מנהל תאימות</span><span class="sxs-lookup"><span data-stu-id="2818f-185">Compliance Manager</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-188">גילוי אלקטרוני</span><span class="sxs-lookup"><span data-stu-id="2818f-188">eDiscovery</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-191">חסימה במקום והמתנה לתביעה משפטית</span><span class="sxs-lookup"><span data-stu-id="2818f-191">In-place hold and litigation hold</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="2818f-194">תגיות שמירה ומדיניות שמירה של ניהול רשומות העברת הודעות (MRM)</span><span class="sxs-lookup"><span data-stu-id="2818f-194">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
||||

<span data-ttu-id="2818f-197">\* משתמשים שהוקצו להם גישה לאפליקציות SaaS יכולים לקבל גישת SSO ל- 10 יישומים לכל אדם.</span><span class="sxs-lookup"><span data-stu-id="2818f-197">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="2818f-198">מנהלי מערכת יכולים לקבוע את התצורה של SSO ולשנות גישת משתמש לאפליקציות SaaS שונות, אך גישת SSO מותרת רק עבור 10 יישומים לכל משתמש בכל פעם.</span><span class="sxs-lookup"><span data-stu-id="2818f-198">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="2818f-199">כל Office 365 היישומים נספרים כיישום יחיד.</span><span class="sxs-lookup"><span data-stu-id="2818f-199">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="2818f-200">העברה</span><span class="sxs-lookup"><span data-stu-id="2818f-200">Migration</span></span>

<span data-ttu-id="2818f-201">כדי לעבור, עבוד עם השותף שלך כדי להעביר Microsoft 365 Business Premium המנוי והרשיון שלך למנוי מתאים Microsoft 365 E3 עם הרשיונות שלו.</span><span class="sxs-lookup"><span data-stu-id="2818f-201">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="2818f-202">הסעיפים הבאים מתארים אילו שינויים עליך לבצע, אם יש, ומה ניתן לבצע לאחר ההעברה.</span><span class="sxs-lookup"><span data-stu-id="2818f-202">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="2818f-203">Microsoft 365 ונתונים של מנוי</span><span class="sxs-lookup"><span data-stu-id="2818f-203">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="2818f-204">אין צורך לבצע שינויים כלשהם במנוי או בנתונים הנוכחיים שלך לפני ההעברה, הכוללים:</span><span class="sxs-lookup"><span data-stu-id="2818f-204">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="2818f-205">תצורת מנוי, כגון שמות תחומי DNS.</span><span class="sxs-lookup"><span data-stu-id="2818f-205">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="2818f-206">חשבונות משתמשים וקבוצתיים והגדרות אימות, כגון אימות רב גורמי או פריטי מדיניות גישה מותנים.</span><span class="sxs-lookup"><span data-stu-id="2818f-206">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="2818f-207">תצורות שירות פרודוקטיביות והנתונים שלהן, כגון Teams, Exchange Online דואר, SharePoint Online, תיקיות OneDrive for Business ומחברות OneNote אחרות.</span><span class="sxs-lookup"><span data-stu-id="2818f-207">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="2818f-208">כעת המשתמשים שלך יכולים ליהנות מאחסון בלתי מוגבל בתיבות הדואר Exchange Online ותיקיות OneDrive for Business שלך.</span><span class="sxs-lookup"><span data-stu-id="2818f-208">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="2818f-209">באפשרותך להתחיל להשתמש בגילוי יישומי ענן, ב- Azure AD התחברות תקינות וב- SSO עבור יותר מ- 10 יישומים.</span><span class="sxs-lookup"><span data-stu-id="2818f-209">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="2818f-210">הגנה מפני איומים</span><span class="sxs-lookup"><span data-stu-id="2818f-210">Threat protection</span></span>

<span data-ttu-id="2818f-211">Windows 10 Business כולל הגנות אלה:</span><span class="sxs-lookup"><span data-stu-id="2818f-211">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="2818f-212">אכיפת תקינות של תהליך אתחול מערכת ההפעלה</span><span class="sxs-lookup"><span data-stu-id="2818f-212">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="2818f-213">אכיפת תקינות של רכיבי הפעלה רגישים</span><span class="sxs-lookup"><span data-stu-id="2818f-213">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="2818f-214">פגיעות מתקדמת וניצול של אפס ימים</span><span class="sxs-lookup"><span data-stu-id="2818f-214">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="2818f-215">הגנת רשת מבוססת מוניטין עבור Microsoft Edge, Internet Explorer ו- Chrome</span><span class="sxs-lookup"><span data-stu-id="2818f-215">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="2818f-216">חומת אש מבוססת מארח</span><span class="sxs-lookup"><span data-stu-id="2818f-216">Host-based firewall</span></span>
- <span data-ttu-id="2818f-217">הפחתת הסיכון של תוכנות כופר</span><span class="sxs-lookup"><span data-stu-id="2818f-217">Ransomware mitigations</span></span>
- <span data-ttu-id="2818f-218">בידוד מבוסס חומרה עבור Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2818f-218">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="2818f-219">בקרת יישומים מופעלת על-ידי שרת האבטחה Graph</span><span class="sxs-lookup"><span data-stu-id="2818f-219">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="2818f-220">בקרת התקן (USB)</span><span class="sxs-lookup"><span data-stu-id="2818f-220">Device control (USB)</span></span>
- <span data-ttu-id="2818f-221">הגנת רשת עבור איומים מבוססי אינטרנט</span><span class="sxs-lookup"><span data-stu-id="2818f-221">Network protection for web-based threats</span></span>
- <span data-ttu-id="2818f-222">כללי מניעת חדירה מארחים</span><span class="sxs-lookup"><span data-stu-id="2818f-222">Host intrusion prevention rules</span></span>

<span data-ttu-id="2818f-223">Windows 10 Enterprise E3 כולל גם ניהול ארגוני של בידוד מבוסס חומרה עבור Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="2818f-223">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

> [!NOTE]
> <span data-ttu-id="2818f-224">משתמשים שהועברו ל- Microsoft 365 E3 יידרשו ל- Microsoft Defender עבור Office 365 עבור המשך הגנה מפני איומים.</span><span class="sxs-lookup"><span data-stu-id="2818f-224">Users migrated to Microsoft 365 E3 will each require a Microsoft Defender for Office 365 license for continued threat protection.</span></span> <span data-ttu-id="2818f-225">הקפד לרכוש Defender נוסף עבור Office 365 רישוי, כך שכל המשתמשים בטווח של Defender עבור Office 365 שלך מורשים.</span><span class="sxs-lookup"><span data-stu-id="2818f-225">Be sure to purchase additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span>

### <a name="device-management-with-intune"></a><span data-ttu-id="2818f-226">ניהול מכשירים עם Intune</span><span class="sxs-lookup"><span data-stu-id="2818f-226">Device management with Intune</span></span>

<span data-ttu-id="2818f-227">אין צורך לבצע שינויים בתצורת Intune הנוכחית לפני המעבר, הכוללת מכשירים והגדרות מכשירים ואפליקציות רשומים.</span><span class="sxs-lookup"><span data-stu-id="2818f-227">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="2818f-228">Windows 10</span><span class="sxs-lookup"><span data-stu-id="2818f-228">Windows 10</span></span>

<span data-ttu-id="2818f-229">Microsoft 365 Business Premium כולל Windows 10 Business, ש באפשרותך להתקין באמצעות Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="2818f-229">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="2818f-230">בעת העברה ל- Microsoft 365 E3, כל רשיון משתמש כולל Windows 10 Enterprise E3, שברצונך גם להתקין באמצעות Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2818f-230">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="2818f-231">יישומי Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="2818f-231">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="2818f-232">לקוח יישומי Microsoft 365 לעסקים שלך המותקן במכשירים שלך יתחיל להשתמש באופן אוטומטי בתכונות של יישומי Microsoft 365 לארגונים.</span><span class="sxs-lookup"><span data-stu-id="2818f-232">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="2818f-233">לאחר ההעברה, באפשרותך כעת להשתמש ב:</span><span class="sxs-lookup"><span data-stu-id="2818f-233">After migration, you can now use:</span></span>

- <span data-ttu-id="2818f-234">תמיכה במדיניות קבוצתית</span><span class="sxs-lookup"><span data-stu-id="2818f-234">Group Policy support</span></span>
- <span data-ttu-id="2818f-235">השוואה וחקירה של גיליון אלקטרוני</span><span class="sxs-lookup"><span data-stu-id="2818f-235">Spreadsheet compare and inquire</span></span>
- <span data-ttu-id="2818f-236">בינה עסקית</span><span class="sxs-lookup"><span data-stu-id="2818f-236">Business intelligence</span></span>
