---
title: Access המקומית משאבים ממכשיר מצורף AD תכלת הרקיע ב- Microsoft 365 Business
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
description: למד כיצד לקבל גישה למשאבים המקומית כמו יישומים שורה של העסק, שיתופי קבצים ומדפסות מתכלת הרקיע של Active Directory המצורפים להתקן Windows 10.
ms.openlocfilehash: fa3cf640e799feb81ff08c5b7b81d57f707e0152
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072029"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="68d27-103">Access המקומית משאבים ממכשיר מצורף AD תכלת הרקיע ב- Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="68d27-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="68d27-104">כל התקן Windows 10 הוא תכלת הרקיע Active Directory מצורף תהיה גישה לכל המשאבים מבוססות ענן כגון יישומי Office 365 שלך ואת להיות מוגן על-ידי Microsoft 365 עסקיים.</span><span class="sxs-lookup"><span data-stu-id="68d27-104">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="68d27-105">גם לאפשר גישה למשאבים המקומית כמו apps של קו עסקיים (LOB), שיתופי קבצים ומדפסות, עליך לסנכרן המקומית של Active Directory עם תכלת הרקיע Active Directory באמצעות [חיבור AD תכלת הרקיע](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="68d27-105">To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span></span> <span data-ttu-id="68d27-106">ראה [מבוא ניהול התקנים ב- Active Directory תכלת הרקיע](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) כדי ללמוד עוד.</span><span class="sxs-lookup"><span data-stu-id="68d27-106">See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) to learn more.</span></span> 
  
## <a name="run-azure-ad-connect"></a><span data-ttu-id="68d27-107">הפעל AD תכלת הרקיע ההתקשרות</span><span class="sxs-lookup"><span data-stu-id="68d27-107">Run Azure AD Connect</span></span>

<span data-ttu-id="68d27-108">השלם את השלבים הבאים כדי לאפשר להתקנים AD תכלת הרקיע מצורף של הארגון שלך לקבל גישה למשאבים המקומית.</span><span class="sxs-lookup"><span data-stu-id="68d27-108">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="68d27-109">כדי לסנכרן שלך משתמשים, קבוצות ואנשי קשר מ- Active Directory המקומי לתוך תכלת הרקיע Active Directory, הפעל את אשף סינכרון הספריה ולאחר התחבר AD תכלת הרקיע כפי שמתואר [להגדיר סינכרון ספריות עבור Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="68d27-109">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="68d27-110">לאחר סינכרון ספריות הושלמה, ודא ש-AD תכלת הרקיע מצורף הם התקני Windows 10 של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="68d27-110">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="68d27-111">שלב זה מבוצע בנפרד בכל התקן Windows 10.</span><span class="sxs-lookup"><span data-stu-id="68d27-111">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="68d27-112">לקבלת פרטים, ראה [הגדרת התקני Windows עבור משתמשים עסקיים 365 של Microsoft](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="68d27-112">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="68d27-113">לאחר ההתקנים 10 חלונות הם AD תכלת הרקיע המצורפים, כל משתמש עליך לאתחל מחדש התקנים והכניסה שלהם עם אישורי Microsoft 365 העסק שלהם.</span><span class="sxs-lookup"><span data-stu-id="68d27-113">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="68d27-114">כל ההתקנים כעת תהיה גישה למשאבים המקומית גם.</span><span class="sxs-lookup"><span data-stu-id="68d27-114">All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="68d27-115">ללא שלבים נוספים נדרשים כדי לקבל גישה מקומית משאבים עבור הפרסומת תכלת הרקיע לחבר התקנים.</span><span class="sxs-lookup"><span data-stu-id="68d27-115">No additional steps are required to get access to on-premise resources for Azure AD joined devices.</span></span> <span data-ttu-id="68d27-116">זהו פונקציונליות מובנית זמינה ב- Windows 10.</span><span class="sxs-lookup"><span data-stu-id="68d27-116">This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="68d27-117">אם הארגון שלך אינו מוכן לפריסה בתכלת הרקיע AD מצורף תצורת ההתקן המתואר לעיל, שקול להגדיר את [תצורת ההתקן Joined AD תכלת הרקיע היברידית](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="68d27-117">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="68d27-118">שיקולים בעת הצטרפות התקני Windows שלך כדי AD תכלת הרקיע</span><span class="sxs-lookup"><span data-stu-id="68d27-118">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="68d27-119">אם אתה AD תכלת הרקיע הצטרפות התקן Windows שהיתה בעבר לתחום או לקבוצת עבודה, עליך לקחת בחשבון את המגבלות הבאות:</span><span class="sxs-lookup"><span data-stu-id="68d27-119">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="68d27-120">כאשר התקן AD תכלת הרקיע מצטרף, הוא יוצר משתמש חדש ללא הפניה פרופיל קיים.</span><span class="sxs-lookup"><span data-stu-id="68d27-120">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="68d27-121">כדי לפתור בעיה זו, פרופילי צורך להעביר באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="68d27-121">To fix this, profiles need to be manually migrated.</span></span> <span data-ttu-id="68d27-122">פרופיל המשתמש מכיל מידע, כגון מועדפים קבצים מקומיים, הגדרות הדפדפן, הגדרות תפריט התחלה, וכו '. הגישה הטובה ביותר היא למצוא כלי צד שלישי כדי למפות הגדרות וקבצים קיימים לפרופיל החדש</span><span class="sxs-lookup"><span data-stu-id="68d27-122">A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>

- <span data-ttu-id="68d27-123">אם ההתקן משתמש אובייקטי מדיניות קבוצתית (GPO), אובייקטי Gpo מסוימים ייתכן שאין דומים [התצורה של ספק שירות](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) ב- Intune.</span><span class="sxs-lookup"><span data-stu-id="68d27-123">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="68d27-124">הפעל את [הכלי MMAT](https://www.microsoft.com/download/details.aspx?id=45520) כדי למצוא Csp דומים עבור אובייקטי Gpo קיים.</span><span class="sxs-lookup"><span data-stu-id="68d27-124">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="68d27-125">למשתמשים לא תהיה אפשרות לאמת ליישומים התלויים אימות של Active Directory.</span><span class="sxs-lookup"><span data-stu-id="68d27-125">Users will not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="68d27-126">כדי להתמודד עם זה להעריך באמצעות app מדור קודם ושקול עדכון ליישום העושה אימות מודרניים במידת האפשר.</span><span class="sxs-lookup"><span data-stu-id="68d27-126">To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>

- <span data-ttu-id="68d27-127">גילוי מדפסת הספריה הפעילה לא יפעלו.</span><span class="sxs-lookup"><span data-stu-id="68d27-127">Active Directory printer discovery will not work.</span></span> <span data-ttu-id="68d27-128">כדי לפתור בעיה זו, מספקים נתיבי הדפסה ישירה עבור כל המשתמשים או למנף [הדפסה ענן היברידי](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="68d27-128">To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
