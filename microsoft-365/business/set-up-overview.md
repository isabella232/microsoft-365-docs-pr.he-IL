---
title: מבט כולל על הגדר
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: מבט כולל על הגדר השלבים עבור העסק 365 של Microsoft.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086326"
---
# <a name="overview-of-setup"></a><span data-ttu-id="1dacf-103">מבט כולל על כיוונון</span><span class="sxs-lookup"><span data-stu-id="1dacf-103">Overview of setup</span></span>

<span data-ttu-id="1dacf-104">ניתן לעשות זאת רוב להגדיר השלבים באשף ההתקנה, אך רשומים גם אפשרויות אחרות.</span><span class="sxs-lookup"><span data-stu-id="1dacf-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="1dacf-105">שלב 1: הוספת קבוצת המחשבים והמשתמשים שלך</span><span class="sxs-lookup"><span data-stu-id="1dacf-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="1dacf-106">**[הוסף קבוצת המחשבים שלך](set-up.md#add-your-domain-to-personalize-sign-in)** (אם רכשת את התחום שלך במהלך [להירשם](sign-up.md), שלב זה כבר בוצע.)</span><span class="sxs-lookup"><span data-stu-id="1dacf-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="1dacf-107">**הוסף משתמשים**.</span><span class="sxs-lookup"><span data-stu-id="1dacf-107">**Add users**.</span></span> <span data-ttu-id="1dacf-108">ניתן לעשות זאת באחת משלוש דרכים:</span><span class="sxs-lookup"><span data-stu-id="1dacf-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="1dacf-109">[אשף](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="1dacf-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="1dacf-110">השתמש סינכרון ספריות כדי [להוסיף משתמשים באמצעות חיבור AD תכלת הרקיע](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) אם ברשותך המקומית של Active directory.</span><span class="sxs-lookup"><span data-stu-id="1dacf-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="1dacf-111">באפשרותך גם [להוסיף משתמשים מאוחר יותר](add-users-m365b.md) במרכז admin.</span><span class="sxs-lookup"><span data-stu-id="1dacf-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="1dacf-112">שלב 2: הגדרת מדיניות אבטחה וקביעת תצורה של התקנים</span><span class="sxs-lookup"><span data-stu-id="1dacf-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="1dacf-113">השתמש [באשף ההתקנה](set-up.md#set-up-security-policies-and-device-configurations) כדי להגדיר פריטי מדיניות התקן ואבטחה.</span><span class="sxs-lookup"><span data-stu-id="1dacf-113">Use the [Setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure device and security policies.</span></span> 
  - <span data-ttu-id="1dacf-114">באפשרותך גם להוסיף יותר או לערוך אותם מאוחר יותר ב- [מרכז admin](view-policies-and-devices.md) [פורטל Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="1dacf-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="1dacf-115">בנוסף להגדרות אבטחה באשף ההתקנה, באפשרותך להגביר את האבטחה על-ידי הוספת את ההגדרות הבאות:</span><span class="sxs-lookup"><span data-stu-id="1dacf-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="1dacf-116">**הגנה מפני תוכנות זדוניות דוא**</span><span class="sxs-lookup"><span data-stu-id="1dacf-116">**Email malware protection**</span></span>
      - <span data-ttu-id="1dacf-117">**קישורים בטוח מתקדם של הגנה מפני איום (ATP)**</span><span class="sxs-lookup"><span data-stu-id="1dacf-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="1dacf-118">**קבצים מצורפים מתאימים ATP**</span><span class="sxs-lookup"><span data-stu-id="1dacf-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="1dacf-119">**ATP למניעת דיוג**</span><span class="sxs-lookup"><span data-stu-id="1dacf-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="1dacf-120">**אחסון בארכיון של Exchange Online**</span><span class="sxs-lookup"><span data-stu-id="1dacf-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="1dacf-121">**מניעת אובדן נתונים (DLP)**</span><span class="sxs-lookup"><span data-stu-id="1dacf-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="1dacf-122">**הגנה על מידע תכלת הרקיע (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="1dacf-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="1dacf-123">כדי לקבל מופעל, ראה [הגדרת מדיניות אבטחה מתקדמות](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="1dacf-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="1dacf-124">ראה גם [העליון 10 דרכים לאבטחת העסק 365 Microsoft](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) עבור מפת דרכים של שיטות עבודה מומלצות של אבטחה.</span><span class="sxs-lookup"><span data-stu-id="1dacf-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="1dacf-125">שלב 3: להגדיר ולנהל התקני Windows 10</span><span class="sxs-lookup"><span data-stu-id="1dacf-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="1dacf-126">בעת הצטרפות התקן Windows 10 כדי AD תכלת הרקיע, פריטי המדיניות שהגדרת [בשלב](#step-2-set-up-security-policies-and-configure-devices) 2 לקבל שהוחלה עליו.</span><span class="sxs-lookup"><span data-stu-id="1dacf-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="1dacf-127">Windows 10 Pro [קדם הדרושים](pre-requisites-for-data-protection.md) לעסקים 365 של Microsoft, אך אם יש לך Windows 7 Pro, Windows 8 Pro או Windows 8.1 Pro, המנוי שלך מקנה לך [שדרוג ל- Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="1dacf-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="1dacf-128">השתמש [באשף הגדרת](set-up.md#set-up-security-policies-and-device-configurations) כדי להגדיר פריטי מדיניות עבור התקני Windows 10.</span><span class="sxs-lookup"><span data-stu-id="1dacf-128">Use the [setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="1dacf-129">Stes 4: התקנת Office 365 עסקי</span><span class="sxs-lookup"><span data-stu-id="1dacf-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="1dacf-130">באפשרותך להתקין את Office באופן אוטומטי בהתקני Windows באמצעות [אשף ההתקנה](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="1dacf-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="1dacf-131">באופן אוטומטי [להתקין את Office](auto-install-or-uninstall-office.md) ממרכז admin.</span><span class="sxs-lookup"><span data-stu-id="1dacf-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="1dacf-132">לאפשר למשתמשים [להתקין את יישומי Office](https://docs.microsoft.com/office365/admin/setup/install-applications) עבור Windows והתקנים.</span><span class="sxs-lookup"><span data-stu-id="1dacf-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="1dacf-133">מתקדם</span><span class="sxs-lookup"><span data-stu-id="1dacf-133">Advanced</span></span>
- <span data-ttu-id="1dacf-134">**השתמש Autopilot כדי להגדיר התקנים חדשים**</span><span class="sxs-lookup"><span data-stu-id="1dacf-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="1dacf-135">באפשרותך להשתמש ב- [Windows Autopilot](add-autopilot-devices-and-profile.md) כדי לקבוע מראש של התקנים 10 חלונות **חדשים** עבור משתמש באופן אוטומטי, אך ייתכן שיהיה קל יותר לקבל [שותף](https://www.microsoft.com/solution-providers/search) מי יכול לבצע זאת עבורך.</span><span class="sxs-lookup"><span data-stu-id="1dacf-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="1dacf-136">באפשרותך גם לעבור לחנות [Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) ובקש טכנולוגיה ענן מומחה להגדיר התקנים חדשים שאתה רוכש עבורך.</span><span class="sxs-lookup"><span data-stu-id="1dacf-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="1dacf-137">**Access המקומית משאבים**</span><span class="sxs-lookup"><span data-stu-id="1dacf-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="1dacf-138">אם הארגון שלך משתמש Windows Server Active Directory המקומית, באפשרותך להגדיר עסקיים 365 של Microsoft להגנה על התקני Windows 10 שלך, תוך שמירה עדיין גישה למשאבים המקומית המחייבים אימות מקומי.</span><span class="sxs-lookup"><span data-stu-id="1dacf-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="1dacf-139">בצע את השלבים [אפשר לתחום התקני Windows 10 להיות מנוהל על-ידי Microsoft 365 עסקיים](manage-windows-devices.md) כדי להגדיר זאת.</span><span class="sxs-lookup"><span data-stu-id="1dacf-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="1dacf-140">זוהי השיטה המועדפת ואת התקנים במצב זה נקראות תכלת הרקיע היברידית AD לחבר התקנים.</span><span class="sxs-lookup"><span data-stu-id="1dacf-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="1dacf-141">אם בעסק שלך יש מקומי Active Directory המכילה כמה המקומית משאבים (כגון שיתופי קבצים ומדפסות), באפשרותך להעניק גישה ההתקנים המצורפים AD תכלת הרקיע שלך למשאבים אלה על-ידי ביצוע השלבים כאן: [Access המקומית משאבים מ תכלת הרקיע מצורף AD ההתקן ב- Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="1dacf-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  