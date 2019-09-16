---
title: מתן אפשרות לניהול מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: למד כיצד לאפשר ל-Microsoft 365 להגן על התקנים המקומיים המצורפים ל-Windows 10.
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992228"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="1622a-103">מתן אפשרות לניהול מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="1622a-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="1622a-104">אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business כדי להגן על התקני Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים המחייבים אימות מקומי.</span><span class="sxs-lookup"><span data-stu-id="1622a-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="1622a-105">אתה יכול להגדיר את זה על ידי הראשון סינכרון הספרייה הפעילה שלך עם כחול Active Directory, ואחריו רישום התקנים של Windows 10 עם תכלת AD ולרשום אותם לניהול המכשיר הנייד על ידי Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="1622a-105">You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
<span data-ttu-id="1622a-106">הסרטון הבא מפרט את השלבים עבור אופן ההגדרה של התרחיש השכיח ביותר.</span><span class="sxs-lookup"><span data-stu-id="1622a-106">The following video details the steps for how to set this up for the most common scenario.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="1622a-107">הגדרת התקנים המצורפים לתחום לניהול על-ידי Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="1622a-107">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="1622a-108">כדי להגדיר את ההתקנים המצורפים לתחום של הארגון שלך כדי להפיק תועלת מהיכולות שסופקו על-ידי התכונה ' פעיל בספריה ' בנוסף ל-Active Directory המקומי, באפשרותך ליישם **התקנים מצורפים של ' תכלת היברידית**'.</span><span class="sxs-lookup"><span data-stu-id="1622a-108">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="1622a-109">אלה הם התקנים המצורפים הן ל-Active Directory המקומי ולספריה הפעילה שלך.</span><span class="sxs-lookup"><span data-stu-id="1622a-109">These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory.</span></span> <span data-ttu-id="1622a-110">היברידית תכלת AD התקנים המצורפים יכול להיות מוגן ומנוהל על ידי מיקרוסופט 365 עסקים.</span><span class="sxs-lookup"><span data-stu-id="1622a-110">Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business.</span></span> 
  
<span data-ttu-id="1622a-111">להשלים את השלבים הבאים כדי להפוך את Windows 10 התקנים היברידית תכלת AD הצטרף והמנוהל על ידי Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="1622a-111">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="1622a-112">כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מתוך Active Directory המקומי לתוך מדריך כחול פעיל, הפעל את אשף סינכרון הספריות והתחבר באמצעות התיקיה ' פעיל בספריה ' כמתואר [בהגדרת סינכרון ספריות עבור Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="1622a-112">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="1622a-113">השלבים זהים בדיוק עבור Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="1622a-113">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="1622a-114">לפני שתשלים את שלב 3 כדי לאפשר להתקני Windows 10 להיות מצורפים להתקן התכלת ההיברידית, עליך לוודא שאתה עומד בדרישות המוקדמות הבאות:</span><span class="sxs-lookup"><span data-stu-id="1622a-114">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="1622a-115">אתה מפעיל את הגירסה העדכנית ביותר של התחברות התכלת AD.</span><span class="sxs-lookup"><span data-stu-id="1622a-115">You are running the latest version of Azure AD connect.</span></span>

   - <span data-ttu-id="1622a-116">החיבור התכלת לספירה מסנכרן את כל אובייקטי המחשב של המכשירים שברצונך להיות היברידית תכלת לספירה הצטרפו.</span><span class="sxs-lookup"><span data-stu-id="1622a-116">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="1622a-117">אם אובייקטי המחשב שייכים ליחידות ארגוניות מסוימות (OU), ודא שאלה אלה מוגדרות לסנכרון בתכלת הספירה גם כן.</span><span class="sxs-lookup"><span data-stu-id="1622a-117">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="1622a-118">רישום התקנים קיימים המצורפים ל-Windows 10 להיות היברידית תכלת AD הצטרפו ולרשום אותם לניהול המכשיר הנייד על ידי Intune (Microsoft 365 Business):</span><span class="sxs-lookup"><span data-stu-id="1622a-118">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="1622a-119">בצע את ההוראות צעד אחר צעד [כיצד להגדיר היברידי היברידית התקנים של התכלת המצורפים למכשירים](https://go.microsoft.com/fwlink/p/?linkid=872870).</span><span class="sxs-lookup"><span data-stu-id="1622a-119">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870).</span></span> <span data-ttu-id="1622a-120">פעולה זו תאפשר את הסינכרון של מחשבי Active Directory המקומיים המצורפים ל-Windows 10 ויגרום להם להיות מוכנים לעננים.</span><span class="sxs-lookup"><span data-stu-id="1622a-120">This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="1622a-121">כדי לרשום מכשיר Windows 10 עבור ניהול התקנים ניידים, ראה [רישום התקן של windows 10 באמצעות Intune באמצעות מדיניות קבוצתית](https://go.microsoft.com/fwlink/p/?linkid=872871) לקבלת הוראות.</span><span class="sxs-lookup"><span data-stu-id="1622a-121">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions.</span></span> <span data-ttu-id="1622a-122">באפשרותך להגדיר את המדיניות הקבוצתית ברמת מחשב מקומית או עבור פעולות בצובר, באפשרותך ליצור הגדרת מדיניות קבוצתית זו בשרת בקר התחום שלך.</span><span class="sxs-lookup"><span data-stu-id="1622a-122">You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span>