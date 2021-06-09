---
title: Access משאבים מקומיים ממכשיר מצורף ל- Azure AD ב- Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: למד כיצד לקבל גישה למשאבים מקומיים, כמו שורה של אפליקציות עסקיות, שיתופי קבצים ומדפסות ממכשיר Azure Active Directory המצורף Windows 10 שלך.
ms.openlocfilehash: 72b3c5ae538cad24fc12e25717dedccb2fdc9017
ms.sourcegitcommit: 4fb1226d5875bf5b9b29252596855a6562cea9ae
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/08/2021
ms.locfileid: "52843321"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="b8875-103">Access משאבים מקומיים ממכשיר מצורף ל- Azure AD ב- Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="b8875-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="b8875-104">מאמר זה חל על Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="b8875-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="b8875-105">לכל Windows 10 המצורף ל- Azure Active Directory יש גישה לכל המשאבים המבוססים על ענן, כגון יישומי Microsoft 365 שלך, ומוגנות על-ידי Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="b8875-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="b8875-106">באפשרותך גם לאפשר גישה למשאבים מקומיים, כמו יישומי קו עסקים (LOB), שיתופי קבצים ומדפסות.</span><span class="sxs-lookup"><span data-stu-id="b8875-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="b8875-107">כדי לאפשר גישה, השתמש [ב- Azure AD התחברות כדי](/azure/active-directory/connect/active-directory-aadconnect) לסנכרן את Active Directory המקומי שלך עם Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8875-107">To allow access, use [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span>

<span data-ttu-id="b8875-108">כדי ללמוד עוד, ראה [מבוא לניהול מכשירים ב- Azure Active Directory](/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="b8875-108">To learn more, see [Introduction to device management in Azure Active Directory](/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="b8875-109">השלבים מסוכמים גם בסעיפים הבאים.</span><span class="sxs-lookup"><span data-stu-id="b8875-109">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="b8875-110">הפעל את Azure AD התחברות</span><span class="sxs-lookup"><span data-stu-id="b8875-110">Run Azure AD Connect</span></span>

<span data-ttu-id="b8875-111">בצע את השלבים הבאים כדי לאפשר למכשירים המצורפים ל- Azure AD של הארגון שלך לגשת למשאבים מקומיים.</span><span class="sxs-lookup"><span data-stu-id="b8875-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>

1. <span data-ttu-id="b8875-112">כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מ- Active Directory המקומי לתוך Azure Active Directory, הפעל את אשף סינכרון מדריכי הכתובות ואת Azure AD התחברות כמתואר במאמר הגדרת [סינכרון מדריכי כתובות עבור Office 365.](../enterprise/set-up-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="b8875-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](../enterprise/set-up-directory-synchronization.md).</span></span>

2. <span data-ttu-id="b8875-113">לאחר השלמת סינכרון מדריכי הכתובות, ודא שהמכשירים Windows 10 של Azure AD מצורפים.</span><span class="sxs-lookup"><span data-stu-id="b8875-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="b8875-114">שלב זה נעשה בנפרד בכל Windows 10 שלך.</span><span class="sxs-lookup"><span data-stu-id="b8875-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="b8875-115">ראה [הגדרת Windows עבור משתמשים Microsoft 365 Business Premium לקבלת](set-up-windows-devices.md) פרטים.</span><span class="sxs-lookup"><span data-stu-id="b8875-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span>

3. <span data-ttu-id="b8875-116">לאחר שהמכשירים Windows 10 Azure AD מצורפים, כל משתמש חייב לאתחל את המכשירים שלו ולהירשם באמצעות אישורי Microsoft 365 Business Premium שלהם.</span><span class="sxs-lookup"><span data-stu-id="b8875-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="b8875-117">לכל המכשירים יש כעת גישה למשאבים מקומיים גם כן.</span><span class="sxs-lookup"><span data-stu-id="b8875-117">All devices now have access to on-premises resources as well.</span></span>

<span data-ttu-id="b8875-118">אין צורך בשלבים נוספים כדי לקבל גישה למשאבים מקומיים עבור מכשירים מצורפים של Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b8875-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="b8875-119">פונקציונליות זו מוכללת Windows 10.</span><span class="sxs-lookup"><span data-stu-id="b8875-119">This functionality is built into Windows 10.</span></span>

<span data-ttu-id="b8875-120">אם יש לך תוכניות להתחבר למכשיר AADJ, מלבד שיטת הסיסמה כמו PIN/Bio-metric באמצעות כניסת אישור WHFB ולאחר מכן לגשת למשאבים מקומיים (שיתופים, מדפסות וכדומה), בצע [מאמר זה.](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)</span><span class="sxs-lookup"><span data-stu-id="b8875-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares, printers, etc.), please follow [this article](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="b8875-121">אם הארגון שלך אינו מוכן לפרוס בתצורת המכשיר המצורף של Azure AD המתוארת לעיל, שקול להגדיר תצורת [התקן היברידי של Azure AD Joined](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="b8875-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>

### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="b8875-122">שיקולים בעת הצטרפות Windows ל- Azure AD</span><span class="sxs-lookup"><span data-stu-id="b8875-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="b8875-123">אם המכשיר Windows שמצורף ל- Azure-AD היה בעבר לתחום או בקבוצת עבודה, שקול את המגבלות הבאות:</span><span class="sxs-lookup"><span data-stu-id="b8875-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>

- <span data-ttu-id="b8875-124">כאשר התקן Azure AD מצטרף, הוא יוצר משתמש חדש מבלי להפנות לפרופיל קיים.</span><span class="sxs-lookup"><span data-stu-id="b8875-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="b8875-125">יש להעביר פרופילים באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="b8875-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="b8875-126">פרופיל משתמש מכיל מידע כמו מועדפים, קבצים מקומיים, הגדרות דפדפן והגדרות תפריט התחלה.</span><span class="sxs-lookup"><span data-stu-id="b8875-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="b8875-127">הגישה הטובה ביותר היא למצוא כלי של ספקים אחרים כדי למפות קבצים והגדרות קיימים לפרופיל החדש.</span><span class="sxs-lookup"><span data-stu-id="b8875-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="b8875-128">אם המכשיר משתמש באובייקטי מדיניות קבוצתית (GPO), ייתכן של- [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) GPO מסוימים אין ספק שירותי תצורה (CSP) דומה ב- Intune.</span><span class="sxs-lookup"><span data-stu-id="b8875-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="b8875-129">הפעל את [הכלי MMAT כדי](https://www.microsoft.com/download/details.aspx?id=45520) למצוא CSPs ניתנים להשוואה עבור אובייקטי GPO קיימים.</span><span class="sxs-lookup"><span data-stu-id="b8875-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="b8875-130">ייתכן שמשתמשים לא יוכלו לבצע אימות עבור יישומים התלויים באימות של Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8875-130">Users might not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="b8875-131">הערכת היישום מדור קודם ושקול לעדכן ליישום המשתמש באות מודרנית, אם הדבר אפשרי.</span><span class="sxs-lookup"><span data-stu-id="b8875-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="b8875-132">גילוי מדפסת של Active Directory לא יתפקד.</span><span class="sxs-lookup"><span data-stu-id="b8875-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="b8875-133">באפשרותך לספק נתיבי מדפסת ישירים עבור כל המשתמשים או להשתמש [בהדפסה אוניברסלית.](/universal-print/)</span><span class="sxs-lookup"><span data-stu-id="b8875-133">You can provide direct printer paths for all users or use [Universal Print](/universal-print/).</span></span>

### <a name="related-articles"></a><span data-ttu-id="b8875-134">מאמרים קשורים</span><span class="sxs-lookup"><span data-stu-id="b8875-134">Related Articles</span></span>

[<span data-ttu-id="b8875-135">דרישות מוקדמות עבור Azure AD התחברות</span><span class="sxs-lookup"><span data-stu-id="b8875-135">Prerequisites for Azure AD Connect</span></span>](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
