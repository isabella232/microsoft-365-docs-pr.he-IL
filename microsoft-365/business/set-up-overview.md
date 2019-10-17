---
title: מבט כולל על הגדרת
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: מבט כולל על השלבים שנקבעו עבור Microsoft 365 Business.
ms.openlocfilehash: 50f172c235aa06aa78fec60fc119ac7f568df308
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575587"
---
# <a name="overview-of-setup"></a><span data-ttu-id="2b7ef-103">מבט כולל על הכיוונון</span><span class="sxs-lookup"><span data-stu-id="2b7ef-103">Overview of setup</span></span>

<span data-ttu-id="2b7ef-104">ניתן לבצע את רוב השלבים המפורטים באשף ההתקנה, אך גם האפשרויות האחרות מפורטות.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="2b7ef-105">שלב 1: הוספת התחום שלך והמשתמשים</span><span class="sxs-lookup"><span data-stu-id="2b7ef-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="2b7ef-106">**[הוסף את התחום שלך](set-up.md#add-your-domain-to-personalize-sign-in)** (אם רכשת את התחום שלך במהלך [ההרשמה](sign-up.md), שלב זה כבר נעשה.)</span><span class="sxs-lookup"><span data-stu-id="2b7ef-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="2b7ef-107">**הוסיף משתמשים**.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-107">**Add users**.</span></span> <span data-ttu-id="2b7ef-108">באפשרותך לעשות זאת בכל אחת משלוש הדרכים:</span><span class="sxs-lookup"><span data-stu-id="2b7ef-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="2b7ef-109">באשף [](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="2b7ef-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="2b7ef-110">השתמש בסינכרון ספריות כדי [להוסיף משתמשים על-ידי שימוש בתכלת AD להתקשרות](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) אם ברשותך ספריה פעילה מקומית.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="2b7ef-111">באפשרותך גם [להוסיף משתמשים בהמשך](add-users-m365b.md) מרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="2b7ef-112">שלב 2: הגדרת מדיניות אבטחה וקביעת תצורה של התקנים</span><span class="sxs-lookup"><span data-stu-id="2b7ef-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="2b7ef-113">השתמש [באשף ההתקנה](set-up.md#protect-data-and-devices) כדי לקבוע את תצורת מדיניות ההתקן והאבטחה.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-113">Use the [Setup wizard](set-up.md#protect-data-and-devices) to configure device and security policies.</span></span> 
  - <span data-ttu-id="2b7ef-114">באפשרותך גם להוסיף או לערוך אותם בהמשך [מרכז הניהול](view-policies-and-devices.md) [ובפורטל Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="2b7ef-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="2b7ef-115">בנוסף להגדרות האבטחה באשף ההתקנה, באפשרותך להגביר את האבטחה על-ידי הוספת ההגדרות הבאות:</span><span class="sxs-lookup"><span data-stu-id="2b7ef-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="2b7ef-116">**הגנה מפני תוכנות זדוניות דוא ל**</span><span class="sxs-lookup"><span data-stu-id="2b7ef-116">**Email malware protection**</span></span>
      - <span data-ttu-id="2b7ef-117">**קישורים מתקדמים להגנת האיומים (ATP)**</span><span class="sxs-lookup"><span data-stu-id="2b7ef-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="2b7ef-118">**מסמכים מצורפים בטוחים ב-ATP**</span><span class="sxs-lookup"><span data-stu-id="2b7ef-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="2b7ef-119">**ATP נגד דיוג**</span><span class="sxs-lookup"><span data-stu-id="2b7ef-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="2b7ef-120">**אחסון בארכיון של Exchange Online**</span><span class="sxs-lookup"><span data-stu-id="2b7ef-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="2b7ef-121">**מניעת אובדן נתונים (DLP)**</span><span class="sxs-lookup"><span data-stu-id="2b7ef-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="2b7ef-122">**תכלת הגנת מידע (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="2b7ef-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="2b7ef-123">כדי להתחיל לראות, [הגדר מדיניות אבטחה מתקדמת](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="2b7ef-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="2b7ef-124">ראה גם [top 10 דרכים לאבטח את Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) עבור מפת הדרכים של נוהלי האבטחה הטובה ביותר.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="2b7ef-125">שלב 3: הגדרת וניהול של התקני Windows 10</span><span class="sxs-lookup"><span data-stu-id="2b7ef-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="2b7ef-126">כאשר אתה מצטרף להתקן של Windows 10 לתכלת, המדיניות שהגדרת [בשלב 2](#step-2-set-up-security-policies-and-configure-devices) מוחלת עליו.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="2b7ef-127">Windows 10 Pro הוא [הכרחי מראש](pre-requisites-for-data-protection.md) עבור Microsoft 365 Business, אבל אם יש לך Windows 7 Pro, Windows 8 pro, או Windows 8.1 pro, המנוי שלך מזכה אותך [לשדרוג ל-Windows 10 pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="2b7ef-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="2b7ef-128">השתמש [באשף ההתקנה](set-up.md#protect-data-and-devices) כדי לקבוע את תצורת פריטי המדיניות עבור התקני Windows 10.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-128">Use the [Setup wizard](set-up.md#protect-data-and-devices) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="2b7ef-129">ס. ס 4: להתקין את Office 365 עסקים</span><span class="sxs-lookup"><span data-stu-id="2b7ef-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="2b7ef-130">באפשרותך להתקין את Office באופן אוטומטי בהתקני Windows באמצעות [אשף ההתקנה](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="2b7ef-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="2b7ef-131">התקן באופן אוטומטי את [Office](auto-install-or-uninstall-office.md) ממרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="2b7ef-132">אפשר למשתמשים [להתקין יישומי Office](https://docs.microsoft.com/office365/admin/setup/install-applications) עבור Windows והתקנים.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="2b7ef-133">מתקדם</span><span class="sxs-lookup"><span data-stu-id="2b7ef-133">Advanced</span></span>
- <span data-ttu-id="2b7ef-134">**השתמש בטייס אוטומטי כדי להגדיר התקנים חדשים**</span><span class="sxs-lookup"><span data-stu-id="2b7ef-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="2b7ef-135">באפשרותך להשתמש [בטייס אוטומטי של windows](add-autopilot-devices-and-profile.md) כדי לקבוע מראש את התצורה של התקנים **חדשים** של windows 10 עבור משתמש, אך ייתכן שיהיה קל יותר לקבל [שותף](https://www.microsoft.com/solution-providers/search) שיוכל לעשות זאת עבורך.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="2b7ef-136">באפשרותך גם לעבור ל- [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) ולבקש ממומחה טכנולוגיית ענן להגדיר התקנים חדשים שתרכוש עבורך.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="2b7ef-137">**גישה למשאבים מקומיים**</span><span class="sxs-lookup"><span data-stu-id="2b7ef-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="2b7ef-138">אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business כדי להגן על התקני Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים המחייבים אימות מקומי.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="2b7ef-139">בצע את השלבים [בהפעלת התקני Windows 10 המצורפים לתחום כדי שיוכלו להיות מנוהלים על-ידי Microsoft 365 Business](manage-windows-devices.md) כדי להגדיר זאת.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="2b7ef-140">זוהי השיטה המועדפת והתקנים במצב זה נקראים היברידית תכלת AD התקנים המצורפים.</span><span class="sxs-lookup"><span data-stu-id="2b7ef-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="2b7ef-141">אם לעסק שלך יש active Directory מקומי המכיל חלק מהמשאבים המקומיים (כגון שיתופי קבצים ומדפסות), באפשרותך להעניק להתקנים המצורפים למשאבים אלה גישה אל משאבים אלה על-ידי ביצוע השלבים כאן: [גישה למשאבים מקומיים מ המכשיר המצורף למודעה ב-Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="2b7ef-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  