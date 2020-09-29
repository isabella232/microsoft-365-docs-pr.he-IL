---
title: גישה למשאבים מקומיים באמצעות מכשיר מצורף לכיוון תכלת ב-Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: למד כיצד לקבל גישה למשאבים מקומיים כגון שורה של אפליקציות עסקיות, מניות קבצים ומדפסות ממכשיר של תכלת Active Directory המצורף ל-Windows 10.
ms.openlocfilehash: 2144268f5cbab67c39d5902622c61c0c35e6481c
ms.sourcegitcommit: 15be7822220041c25fc52565f1c64d252e442d89
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/28/2020
ms.locfileid: "48295309"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="60b59-103">גישה למשאבים מקומיים באמצעות מכשיר תכלת מצורף ב-Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="60b59-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="60b59-104">מאמר זה חל על Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="60b59-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="60b59-105">כל מכשיר Windows 10 שהוא תכלת Active Directory הצטרף אליו כולל גישה לכל המשאבים המבוססים על ענן, כגון יישומי Microsoft 365, וניתן להתגונן על-ידי Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="60b59-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="60b59-106">באפשרותך גם לאפשר גישה למשאבים מקומיים כגון יישומי line-business (LOB), מניות קבצים ומדפסות.</span><span class="sxs-lookup"><span data-stu-id="60b59-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="60b59-107">כדי לאפשר גישה, השתמש ב- [תכלת AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) כדי לסנכרן את active directory המקומי עם תכלת active directory.</span><span class="sxs-lookup"><span data-stu-id="60b59-107">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="60b59-108">לקבלת מידע נוסף, ראה [מבוא לניהול מכשירים ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="60b59-108">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="60b59-109">השלבים מסוכמים גם בסעיפים הבאים.</span><span class="sxs-lookup"><span data-stu-id="60b59-109">The steps are also summarized in the following sections.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="60b59-110">הרצת התחברות של תכלת לספירה</span><span class="sxs-lookup"><span data-stu-id="60b59-110">Run Azure AD Connect</span></span>

<span data-ttu-id="60b59-111">בצע את השלבים הבאים כדי להפוך את המכשירים המצורפים של הארגון שלך ל-תכלת לזמינים כדי לגשת למשאבים מקומיים.</span><span class="sxs-lookup"><span data-stu-id="60b59-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="60b59-112">כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מ-Active Directory המקומי ל-תכלת Active Directory, הפעל את אשף סינכרון מדריכי הכתובות והקישור תכלת AD כמתואר [בהגדרת סינכרון מדריכי כתובות עבור Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="60b59-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization).</span></span>
    
2. <span data-ttu-id="60b59-113">לאחר השלמת סינכרון מדריכי הכתובות, ודא שמכשירי Windows 10 של הארגון שלך מצורפים ל-תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="60b59-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="60b59-114">שלב זה מתבצע בנפרד בכל מכשיר Windows 10.</span><span class="sxs-lookup"><span data-stu-id="60b59-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="60b59-115">ראה [הגדרת מכשירי Windows עבור משתמשי Microsoft 365 Business Premium](set-up-windows-devices.md) לקבלת פרטים.</span><span class="sxs-lookup"><span data-stu-id="60b59-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="60b59-116">לאחר הצטרפות המכשירים של Windows 10, כל משתמש צריך להפעיל מחדש את המכשירים ולהיכנס באמצעות האישורים שלהם ב-Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="60b59-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="60b59-117">לכל המכשירים יש כעת גישה גם למשאבים מקומיים.</span><span class="sxs-lookup"><span data-stu-id="60b59-117">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="60b59-118">אין צורך לבצע שלבים נוספים כדי לקבל גישה למשאבים מקומיים עבור מכשירים המצורפים של תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="60b59-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="60b59-119">פונקציונליות זו מוכללת ב-Windows 10.</span><span class="sxs-lookup"><span data-stu-id="60b59-119">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="60b59-120">אם יש לך תוכניות להיכנס למכשיר AADJ מלבד שיטת סיסמה כגון PIN/Bio-מדד באמצעות כניסת האישורים של WHFB ולאחר מכן גישה למשאבים מקומיים (מיקומים משותפים, מדפסות. וכדומה), פעל בהתאם https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="60b59-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="60b59-121">אם הארגון שלך אינו מוכן לפריסה בתצורת ההתקן של תכלת לספירה שתוארה לעיל, שקול להגדיר את הגדרת [התצורה ההיברידית של תכלת לספירה הצטרפת למכשיר](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="60b59-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="60b59-122">שיקולים בעת הצטרפות למכשירי Windows לתכלת לספירה</span><span class="sxs-lookup"><span data-stu-id="60b59-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="60b59-123">אם התקן Windows שאתה מחובר אליו באמצעות הודעות מיידיות, הצטרף בעבר לתחום או לקבוצת עבודה, שקול את המגבלות הבאות:</span><span class="sxs-lookup"><span data-stu-id="60b59-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="60b59-124">כאשר התקן תכלת מצטרף להודעה, הוא יוצר משתמש חדש ללא הפניה לפרופיל קיים.</span><span class="sxs-lookup"><span data-stu-id="60b59-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="60b59-125">יש להעביר את הפרופילים באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="60b59-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="60b59-126">פרופיל משתמש מכיל מידע כגון מועדפים, קבצים מקומיים, הגדרות דפדפן והגדרות תפריט התחלה.</span><span class="sxs-lookup"><span data-stu-id="60b59-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="60b59-127">הגישה הטובה ביותר היא למצוא כלי של ספק חיצוני כדי למפות קבצים והגדרות קיימים לפרופיל החדש.</span><span class="sxs-lookup"><span data-stu-id="60b59-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="60b59-128">אם ההתקן משתמש באובייקטי מדיניות קבוצתית (GPO), ייתכן שאובייקטי Gpo מסוימים לא יהיו בעלי [ספק שירותי תצורה](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) מקביל (CSP) בתוך המנגינה.</span><span class="sxs-lookup"><span data-stu-id="60b59-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="60b59-129">הפעילו את [הכלי MMAT](https://www.microsoft.com/download/details.aspx?id=45520) כדי למצוא את מחשב ה-csp הדומה לאובייקטי gpo קיימים.</span><span class="sxs-lookup"><span data-stu-id="60b59-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="60b59-130">משתמשים לא יוכלו לבצע אימות ליישומים התלויים באימות של Active Directory.</span><span class="sxs-lookup"><span data-stu-id="60b59-130">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="60b59-131">הערך את האפליקציה legacy ושקול לעדכן את היישום המשתמש באימות מודרני, אם ניתן.</span><span class="sxs-lookup"><span data-stu-id="60b59-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="60b59-132">גילוי מדפסת של Active Directory לא יפעל.</span><span class="sxs-lookup"><span data-stu-id="60b59-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="60b59-133">באפשרותך לספק נתיבי מדפסת ישירים עבור כל המשתמשים או להשתמש [בהדפסת ענן היברידית](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="60b59-133">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
