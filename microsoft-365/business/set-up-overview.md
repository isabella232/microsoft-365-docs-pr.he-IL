---
title: מבט כולל על הכיוונון
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
description: מבט כולל על שלבי ההתקנה של Microsoft 365 Business.
ms.openlocfilehash: 4aca617015cceb85ca35c8d8ada7b83d1416d959
ms.sourcegitcommit: 178ecb21cacdeaf440f3df2fe6e539e9127fcf15
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/23/2019
ms.locfileid: "40850803"
---
# <a name="overview-of-setup"></a><span data-ttu-id="d634a-103">מבט כולל על הכיוונון</span><span class="sxs-lookup"><span data-stu-id="d634a-103">Overview of setup</span></span>

<span data-ttu-id="d634a-104">צפה בסרטון וידאו קצר אודות ההתקנה העסקית של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d634a-104">Watch a short video about Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="d634a-105">אם מצאת את הסרטון הזה מועיל, בדוק את [סידרת ההדרכה המלאה לעסקים קטנים ולאלה החדשים ל-Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="d634a-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="d634a-106">ניתן לבצע את רוב שלבי ההתקנה באשף ההתקנה, אך גם האפשרויות האחרות מפורטות.</span><span class="sxs-lookup"><span data-stu-id="d634a-106">Most of the setup steps can be done in the setup wizard, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="d634a-107">שלב 1: הוספת התחום שלך והמשתמשים</span><span class="sxs-lookup"><span data-stu-id="d634a-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="d634a-108">**[הוסף את התחום שלך](set-up.md#add-your-domain-to-personalize-sign-in)** (אם רכשת את התחום שלך במהלך [ההרשמה](sign-up.md), שלב זה כבר נעשה.)</span><span class="sxs-lookup"><span data-stu-id="d634a-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="d634a-109">**הוסיף משתמשים**.</span><span class="sxs-lookup"><span data-stu-id="d634a-109">**Add users**.</span></span> <span data-ttu-id="d634a-110">באפשרותך להוסיף משתמשים בכל אחת משלוש הדרכים:</span><span class="sxs-lookup"><span data-stu-id="d634a-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="d634a-111">באשף [](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="d634a-111">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="d634a-112">השתמש בסינכרון ספריות כדי [להוסיף משתמשים על-ידי שימוש בתכלת AD להתקשרות](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) אם ברשותך ספריה פעילה מקומית.</span><span class="sxs-lookup"><span data-stu-id="d634a-112">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="d634a-113">באפשרותך גם [להוסיף משתמשים בהמשך](add-users-m365b.md) מרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="d634a-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="d634a-114">שלב 2: הגדרת מדיניות אבטחה וקביעת תצורה של התקנים</span><span class="sxs-lookup"><span data-stu-id="d634a-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="d634a-115">השתמש [באשף ההתקנה](set-up.md#protect-your-organization) כדי לקבוע את התצורה של מדיניות התקנים.</span><span class="sxs-lookup"><span data-stu-id="d634a-115">Use the [Setup wizard](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="d634a-116">באפשרותך גם להוסיף או לערוך אותם בהמשך [מרכז הניהול](view-policies-and-devices.md) [ובפורטל Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="d634a-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="d634a-117">אשף ההתקנה גם תגדיר הגנה בסיסית על איומים והגדרות מניעת אובדן נתונים.</span><span class="sxs-lookup"><span data-stu-id="d634a-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="d634a-118">בנוסף להגדרות האבטחה באשף ההתקנה, באפשרותך להגביר את האבטחה על-ידי הוספת ההגדרות הבאות:</span><span class="sxs-lookup"><span data-stu-id="d634a-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="d634a-119">**הגנה מפני תוכנות זדוניות דוא ל**</span><span class="sxs-lookup"><span data-stu-id="d634a-119">**Email malware protection**</span></span>
- <span data-ttu-id="d634a-120">**ATP נגד דיוג**</span><span class="sxs-lookup"><span data-stu-id="d634a-120">**ATP anti-phishing**</span></span>
- <span data-ttu-id="d634a-121">**אחסון בארכיון של Exchange Online**</span><span class="sxs-lookup"><span data-stu-id="d634a-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="d634a-122">**תכלת הגנת מידע (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="d634a-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="d634a-123">כדי להתחיל, ראה [הגדרת מדיניות אבטחה מתקדמת](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="d634a-123">To get started, see [set up advanced security policies](set-up-advanced-security.md).</span></span>

<span data-ttu-id="d634a-124">ראה גם [top 10 דרכים לאבטח את Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) עבור מפת הדרכים של נוהלי האבטחה הטובה ביותר.</span><span class="sxs-lookup"><span data-stu-id="d634a-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="d634a-125">שלב 3: הגדרת וניהול של התקני Windows 10</span><span class="sxs-lookup"><span data-stu-id="d634a-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="d634a-126">לאחר שתפעיל את אשף ההגדרה, תרצה להתקין את כל מחשבי Windwos 10 בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="d634a-126">After you run the set up wizard, you will want to proctect all the Windwos 10 computers in your organization.</span></span>
  
- <span data-ttu-id="d634a-127">Windows 10 Pro הוא [תנאי מוקדם](pre-requisites-for-data-protection.md) עבור Microsoft 365 Business, אבל אם יש לך Windows 7 Pro, Windows 8 pro, או Windows 8.1 pro, המנוי שלך מזכה אותך [לשדרוג ל-Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="d634a-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="d634a-128">בצע את השלבים [במחשבים מאובטחים של windows 10](secure-win-10-pcs.md) כדי להגדיר מדיניות עבור התקני windows 10.</span><span class="sxs-lookup"><span data-stu-id="d634a-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="d634a-129">כאשר אתה מצטרף להתקן של Windows 10 לתכלת, מדיניות המדיניות שקבעת עבור מחשבי Windows 10 מוחלת עליו.</span><span class="sxs-lookup"><span data-stu-id="d634a-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="d634a-130">לקבלת מידע נוסף, ראה [הגדרת התקני Windows עבור משתמשים עסקיים של Microsoft 365](set-up-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="d634a-130">For more information, see [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-office-365-business"></a><span data-ttu-id="d634a-131">שלב 4: התקנת Office 365 עסקים</span><span class="sxs-lookup"><span data-stu-id="d634a-131">Step 4: Install Office 365 Business</span></span>
- <span data-ttu-id="d634a-132">באפשרותך להתקין את Office באופן אוטומטי בהתקני Windows באמצעות [אשף ההתקנה](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="d634a-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="d634a-133">אפשר למשתמשים [להתקין יישומי Office](https://docs.microsoft.com/office365/admin/setup/install-applications) עבור Windows והתקנים.</span><span class="sxs-lookup"><span data-stu-id="d634a-133">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="d634a-134">מתקדם</span><span class="sxs-lookup"><span data-stu-id="d634a-134">Advanced</span></span>
- <span data-ttu-id="d634a-135">**השתמש בטייס אוטומטי כדי להגדיר התקנים חדשים**</span><span class="sxs-lookup"><span data-stu-id="d634a-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="d634a-136">באפשרותך להשתמש [בטייס אוטומטי של windows](add-autopilot-devices-and-profile.md) כדי לקבוע מראש את התצורה של התקנים **חדשים** של windows 10 עבור משתמש, אך ייתכן שיהיה קל יותר לקבל [שותף](https://www.microsoft.com/solution-providers/search) שיוכל לעשות זאת עבורך.</span><span class="sxs-lookup"><span data-stu-id="d634a-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="d634a-137">באפשרותך גם לעבור אל [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)ולבקש ממומחה טכנולוגיית ענן להגדיר התקנים חדשים שתרכוש.</span><span class="sxs-lookup"><span data-stu-id="d634a-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="d634a-138">**גישה למשאבים מקומיים**</span><span class="sxs-lookup"><span data-stu-id="d634a-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="d634a-139">אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business כדי להגן על התקני Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים המחייבים אימות מקומי.</span><span class="sxs-lookup"><span data-stu-id="d634a-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="d634a-140">בצע את השלבים [בהפעלת התקני Windows 10 המצורפים לתחום כדי שיוכלו להיות מנוהלים על-ידי Microsoft 365 Business](manage-windows-devices.md) כדי להגדיר זאת.</span><span class="sxs-lookup"><span data-stu-id="d634a-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="d634a-141">זוהי השיטה המועדפת, והתקנים במצב זה נקראים "היברידית תכלת" התקנים המצורפים.</span><span class="sxs-lookup"><span data-stu-id="d634a-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="d634a-142">אם לעסק שלך יש Active Directory מקומי המכיל משאבים מסוימים מקומיים (כגון שיתופי קבצים ומדפסות), באפשרותך להעניק להתקנים המצורפים למשאבים אלה גישה אל משאבים אלה על-ידי ביצוע השלבים כאן: [גישה למשאבים מקומיים מהתקן תכלת-הצטרף ב-Microsoft 365 business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="d634a-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="d634a-143">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="d634a-143">See also</span></span>

[<span data-ttu-id="d634a-144">סרטוני הדרכה עסקיים של Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d634a-144">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
