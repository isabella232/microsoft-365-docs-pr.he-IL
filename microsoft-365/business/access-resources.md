---
title: גישה למשאבים מקומיים ממכשיר תכלת המצורף לאתר ב-Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: למד כיצד לקבל גישה למשאבים מקומיים כגון יישומים עסקיים, שיתופי קבצים ומדפסות מתוך מכשיר המצורף ל-Windows 10.
ms.openlocfilehash: ab9049e78617372463b8446dc8f8bc0089d8c117
ms.sourcegitcommit: 91ff1d4339f0f043c2b43997d87d84677c79e279
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2019
ms.locfileid: "36981660"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="e4b8f-103">גישה למשאבים מקומיים ממכשיר תכלת המצורף לאתר ב-Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="e4b8f-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="e4b8f-104">כל מכשיר של Windows 10 שהוא הצטרף למשרד התכלת הפעילה יקבל גישה לכל המשאבים המבוססים על ענן צמתים כגון יישומי Office 365 וניתן להגן עליהם על-ידי Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-104">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="e4b8f-105">כדי לאפשר גם גישה למשאבים מקומיים כגון יישומים של שורה של עסקים (בלוב), מיקומים משותפים של קבצים ומדפסות, עליך לסנכרן את ה-Active Directory המקומי שלך עם מדריך הפעלה תכלת באמצעות [התחברות לספירה](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="e4b8f-105">To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span></span> <span data-ttu-id="e4b8f-106">הסרטון הבא מפרט את השלבים עבור אופן ההגדרה של התרחיש השכיח ביותר.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-106">The following video details the steps for how to set this up for the most common scenario.</span></span>
 
> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]

<span data-ttu-id="e4b8f-107">ראה [מבוא לניהול התקנים ב-תכלת Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) כדי ללמוד עוד.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-107">See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) to learn more.</span></span>
<span data-ttu-id="e4b8f-108">השלבים מסוכמים גם בסעיפים הבאים.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-108">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="e4b8f-109">הפעל תכלת והתחבר</span><span class="sxs-lookup"><span data-stu-id="e4b8f-109">Run Azure AD Connect</span></span>

<span data-ttu-id="e4b8f-110">השלם את השלבים הבאים כדי לאפשר להתקנים המצורפים של הארגון לבצע גישה למשאבים מקומיים.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-110">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="e4b8f-111">כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מתוך Active Directory המקומי לתוך הספריה הפעילה של המשרד, הפעל את אשף סינכרון הספריות ואת ' כחול לספירה ' כמתואר [בהגדרת סינכרון ספריות עבור Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="e4b8f-111">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="e4b8f-112">לאחר השלמת סינכרון הספריות, ודא שהתקני Windows 10 של הארגון שלך הם המצורפים לתכלת.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-112">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="e4b8f-113">שלב זה נעשה בנפרד בכל התקן של Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-113">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="e4b8f-114">ראה [הגדרת התקני Windows עבור משתמשים עסקיים של Microsoft 365](set-up-windows-devices.md) לפרטים.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-114">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="e4b8f-115">לאחר התקני Windows 10 הם תכלת לספירה הצטרפו, כל משתמש צריך לאתחל את המכשירים שלהם להתחבר עם האישורים העסקיים שלהם Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-115">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="e4b8f-116">לכל ההתקנים תהיה כעת גישה גם למשאבים מקומיים.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-116">All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="e4b8f-117">אין צורך בצעדים נוספים כדי לקבל גישה למשאבים מקומיים עבור התקנים המצורפים ל-תכלת AD.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-117">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="e4b8f-118">זוהי פונקציונליות מוכללת הזמינה ב-Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-118">This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="e4b8f-119">אם הארגון שלך אינו מוכן לפרוס בתצורת ההתקן המצורף למטה לספירה המתוארת לעיל, שקול להגדיר את [תצורת ההתקן היברידית של התכלת ההיברידית](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="e4b8f-119">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="e4b8f-120">שיקולים בעת הצטרפות להתקני Windows לתכלת</span><span class="sxs-lookup"><span data-stu-id="e4b8f-120">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="e4b8f-121">אם אתה מצטרף להתקן של מערכת Windows שכבר הצטרף לתחום או בקבוצת עבודה, עליך לשקול את המגבלות הבאות:</span><span class="sxs-lookup"><span data-stu-id="e4b8f-121">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="e4b8f-122">כאשר התקן "תכלת לספירה" מצטרף, הוא יוצר משתמש חדש מבלי ליצור הפניה לפרופיל קיים.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-122">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="e4b8f-123">כדי לתקן זאת, יש להעביר את הפרופילים באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-123">To fix this, profiles need to be manually migrated.</span></span> <span data-ttu-id="e4b8f-124">פרופיל משתמש מכיל מידע כגון מועדפים, קבצים מקומיים, הגדרות דפדפן, הגדרות תפריט התחלה וכו '. הגישה הטובה ביותר היא למצוא כלי של ספק חיצוני כדי למפות קבצים והגדרות קיימים לפרופיל החדש</span><span class="sxs-lookup"><span data-stu-id="e4b8f-124">A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>

- <span data-ttu-id="e4b8f-125">אם ההתקן משתמש באובייקטי מדיניות קבוצתית (GPO), ייתכן שלאובייקטי Gpo מסוימים אין [ספק שירותי תצורה](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) דומה (CSP) ב-Intune.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-125">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="e4b8f-126">הפעל את [הכלי Mmat](https://www.microsoft.com/download/details.aspx?id=45520) כדי לחפש מדיניות קבוצתית דומה עבור אובייקטי gpo קיימים.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-126">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="e4b8f-127">למשתמשים לא תהיה אפשרות לבצע אימות ליישומים התלויים באימות של Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-127">Users will not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="e4b8f-128">כדי להתמודד עם זה להעריך באמצעות יישום מדור קודם ולשקול עדכון לאפליקציה המשתמשת באימות מודרני אם אפשרי.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-128">To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>

- <span data-ttu-id="e4b8f-129">גילוי מדפסות של active Directory לא יפעל.</span><span class="sxs-lookup"><span data-stu-id="e4b8f-129">Active Directory printer discovery will not work.</span></span> <span data-ttu-id="e4b8f-130">כדי לתקן זאת, ספק נתיבי מדפסת ישירים עבור כל המשתמשים או לחץ על [הדפסת ענן היברידית](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="e4b8f-130">To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
