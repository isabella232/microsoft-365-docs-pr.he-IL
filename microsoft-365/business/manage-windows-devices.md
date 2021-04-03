---
title: אפשר ניהול של מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 לעסקים
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: למד כיצד לאפשר ל- Microsoft 365 להגן על מכשירי Windows 10 מקומיים המצורפים ל- Active-Directory בכמה שלבים בלבד.
ms.openlocfilehash: 8a45c6959bee368491c5c6424e3713300c443779
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580133"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="da82d-103">אפשר ניהול של מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="da82d-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="da82d-104">אם הארגון שלך משתמש ב- Windows Server Active Directory באופן מקומי, באפשרותך להגדיר את Microsoft 365 Business Premium כדי להגן על מכשירי Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים הדורשים אימות מקומי.</span><span class="sxs-lookup"><span data-stu-id="da82d-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="da82d-105">כדי להגדיר הגנה זו, באפשרותך ליישם מכשירים **מצורפים היברידיים של Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="da82d-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="da82d-106">מכשירים אלה מצורפים הן ל- Active Directory המקומי ול- Azure Active Directory שלך.</span><span class="sxs-lookup"><span data-stu-id="da82d-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="da82d-107">סרטון וידאו זה מתאר את השלבים לאיך להגדיר זאת עבור התרחיש הנפוץ ביותר, המפורט גם בשלבים המפורטים.</span><span class="sxs-lookup"><span data-stu-id="da82d-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="da82d-108">לפני תחילת העבודה, הקפד להשלים שלבים אלה:</span><span class="sxs-lookup"><span data-stu-id="da82d-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="da82d-109">סנכרן משתמשים עם Azure AD באמצעות Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="da82d-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="da82d-110">השלם את סינכרון היחידה הארגונית (OU) של Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="da82d-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="da82d-111">ודא שלמשתמשי התחום שאתה מסנכרן יש רשיונות ל- Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="da82d-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="da82d-112">ראה [סינכרון משתמשי תחום עם Microsoft](manage-domain-users.md) לקבלת השלבים.</span><span class="sxs-lookup"><span data-stu-id="da82d-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="da82d-113">1. אימות רשות MDM ב- Intune</span><span class="sxs-lookup"><span data-stu-id="da82d-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="da82d-114">עבור אל מנהל [נקודות הקצה](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) ובדף Microsoft Intune, בחר  הרשמה למכשירים ולאחר מכן, בדף מבט כולל, ודא כי **רשות MDM** היא **Intune**. </span><span class="sxs-lookup"><span data-stu-id="da82d-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="da82d-115">אם **רשות MDM** היא **ללא**, לחץ על **רשות MDM** כדי להגדיר אותה ל- **Intune**.</span><span class="sxs-lookup"><span data-stu-id="da82d-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="da82d-116">אם **רשות MDM** היא **Microsoft Office 365**,עבור אל מכשירים הרשמה מכשירים והשתמש בתיבת הדו-שיח הוספת רשות MDM בצד ימין כדי להוסיף רשות MDM של Intune (תיבת הדו-שיח הוספת רשות MDM זמינה רק אם רשות MDM מוגדרת ל- Microsoft Office  >   365).    </span><span class="sxs-lookup"><span data-stu-id="da82d-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="da82d-117">2. ודא ש- Azure AD זמין להצטרפות למחשבים</span><span class="sxs-lookup"><span data-stu-id="da82d-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="da82d-118">עבור אל מרכז הניהול ב ובחר Azure Active Directory (בחר הצג הכל אם Azure Active Directory אינו <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> גלוי) **ברשימה מרכזי הניהול.** </span><span class="sxs-lookup"><span data-stu-id="da82d-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="da82d-119">במרכז הניהול **של Azure Active Directory**, עבור אל Azure Active **Directory** , בחר **מכשירים ולאחר** מכן בחר **הגדרות מכשיר**.</span><span class="sxs-lookup"><span data-stu-id="da82d-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="da82d-120">אימות **שמשתמשים עשויים להצטרף למכשירים ל- Azure AD** זמין</span><span class="sxs-lookup"><span data-stu-id="da82d-120">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="da82d-121">כדי להפוך את כל המשתמשים לזמינים, הגדר את **האפשרות הכל.**</span><span class="sxs-lookup"><span data-stu-id="da82d-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="da82d-122">כדי להפוך משתמשים ספציפיים לזמינים, הגדר **את האפשרות נבחר** כדי להפוך קבוצת משתמשים ספציפית לזמינה.</span><span class="sxs-lookup"><span data-stu-id="da82d-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="da82d-123">הוסף את משתמשי התחום הרצויים מסונכרנים ב- Azure AD [לקבוצת אבטחה](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="da82d-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="da82d-124">בחר **בחר קבוצות כדי** להפוך טווח משתמש MDM לזמין עבור קבוצת אבטחה זו.</span><span class="sxs-lookup"><span data-stu-id="da82d-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="da82d-125">3. ודא ש- Azure AD זמין עבור MDM</span><span class="sxs-lookup"><span data-stu-id="da82d-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="da82d-126">עבור אל מרכז הניהול ב ובחר <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  באפשרות **Endpoint Managemen** t (בחר **הצג הכל אם** מנהל נקודות **הקצה** אינו גלוי)</span><span class="sxs-lookup"><span data-stu-id="da82d-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="da82d-127">במרכז הניהול **של Microsoft Endpoint Manager**, עבור אל 'הרשמה **אוטומטית'** של  >  **מכשירים** של Windows  >  **הרשמה** אוטומטית של Windows  >  .</span><span class="sxs-lookup"><span data-stu-id="da82d-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="da82d-128">ודא שטווח המשתמש של MDM זמין.</span><span class="sxs-lookup"><span data-stu-id="da82d-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="da82d-129">כדי לרשום את כל המחשבים, הגדר הכל **כדי** לרשום באופן אוטומטי את כל מחשבי המשתמשים המצורפים ל- Azure AD ולמחשבים חדשים כאשר המשתמשים מוסיפים חשבון עבודה ל- Windows.</span><span class="sxs-lookup"><span data-stu-id="da82d-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="da82d-130">הגדר לחלק **כדי** לרשום את המחשבים של קבוצת משתמשים ספציפית.</span><span class="sxs-lookup"><span data-stu-id="da82d-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="da82d-131">הוסף את משתמשי התחום הרצויים מסונכרנים ב- Azure AD [לקבוצת אבטחה](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="da82d-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="da82d-132">בחר **בחר קבוצות כדי** להפוך טווח משתמש MDM לזמין עבור קבוצת אבטחה זו.</span><span class="sxs-lookup"><span data-stu-id="da82d-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="da82d-133">4. יצירת המשאבים הדרושים</span><span class="sxs-lookup"><span data-stu-id="da82d-133">4. Create the required resources</span></span> 

<span data-ttu-id="da82d-134">ביצוע המשימות הדרושות לקביעת התצורה של [צירוף Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) היברידי התפשט באמצעות השימוש [ב- cmdlet של Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) שנמצא במודול [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="da82d-134">Performing the required tasks to [configure hybrid Azure AD join](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="da82d-135">כאשר אתה להפעיל cmdlet זה, הוא ייצור ויגדיר את נקודת החיבור הנדרשת של השירות ואת המדיניות הקבוצתית.</span><span class="sxs-lookup"><span data-stu-id="da82d-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="da82d-136">באפשרותך להתקין מודול זה על-ידי הפעלה של הפריטים הבאים ממופע של PowerShell:</span><span class="sxs-lookup"><span data-stu-id="da82d-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="da82d-137">מומלץ להתקין מודול זה בשרת Windows שבו פועל Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="da82d-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="da82d-138">כדי ליצור את נקודת החיבור הנדרשת של השירות ומדיניות קבוצתית, תוכל להפעיל את [cmdlet Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="da82d-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="da82d-139">תצטרך את אישורי מנהל המערכת הכלליים של Microsoft 365 Business Premium בעת ביצוע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="da82d-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="da82d-140">כאשר תהיה מוכן ליצור את המשאבים, להפעיל את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="da82d-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="da82d-141">הפקודה הראשונה תבסס חיבור לענן Microsoft, וכאשר תתבקש לעשות זאת, ציין את אישורי הניהול הכלליים של Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="da82d-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="da82d-142">5. קישור המדיניות הקבוצתית</span><span class="sxs-lookup"><span data-stu-id="da82d-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="da82d-143">במסוף ניהול המדיניות הקבוצתית (GPMC), לחץ באמצעות לחצן העכבר הימני על המיקום שבו ברצונך לקשר את המדיניות ובחר קשר *GPO קיים...* בתפריט תלוי ההקשר.</span><span class="sxs-lookup"><span data-stu-id="da82d-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="da82d-144">בחר את המדיניות שנוצרה בשלב לעיל ולאחר מכן לחץ על **אישור.**</span><span class="sxs-lookup"><span data-stu-id="da82d-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="da82d-145">קבל את תבניות הניהול העדכניות ביותר</span><span class="sxs-lookup"><span data-stu-id="da82d-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="da82d-146">אם אינך רואה את המדיניות הפוך הרשמה **אוטומטית של MDM** לזמינה באמצעות אישורי Azure AD המוגדרים כברירת מחדל, ייתכן שהאפשרות היא שה- ADMX אינו מותקן עבור Windows 10, גירסה 1803 ואילך.</span><span class="sxs-lookup"><span data-stu-id="da82d-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="da82d-147">כדי לפתור את הבעיה, בצע את השלבים הבאים (הערה: MDM.admx העדכני ביותר תואם לאחור):</span><span class="sxs-lookup"><span data-stu-id="da82d-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="da82d-148">הורד: [תבניות מנהליות (.admx) עבור Windows 10 אוקטובר 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span><span class="sxs-lookup"><span data-stu-id="da82d-148">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2.  <span data-ttu-id="da82d-149">התקן את החבילה בבקר תחום.</span><span class="sxs-lookup"><span data-stu-id="da82d-149">Install the package on a Domain Controller.</span></span>
3.  <span data-ttu-id="da82d-150">נווט, בהתאם לגירסת תבניות הניהול לתיקיה: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span><span class="sxs-lookup"><span data-stu-id="da82d-150">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4.  <span data-ttu-id="da82d-151">שנה את **שם התיקיה** הגדרות מדיניות בנתיב לעיל **למדיניותDefinitions**.</span><span class="sxs-lookup"><span data-stu-id="da82d-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="da82d-152">העתק את **התיקיה PolicyDefinitions** לשיתוף SYSVOL שלך, הממוקמת כברירת מחדל **ב- C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="da82d-152">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="da82d-153">אם בכוונתך להשתמש בחנות מדיניות מרכזית עבור התחום כולו, הוסף את התוכן של PolicyDefinitions שם.</span><span class="sxs-lookup"><span data-stu-id="da82d-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="da82d-154">במקרה שיש לך כמה בקרי תחום, המתן עד ש- SYSVOL ישכפל כדי שמדיניות תהיה זמינה.</span><span class="sxs-lookup"><span data-stu-id="da82d-154">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="da82d-155">הליך זה יעבוד גם עבור כל גירסה עתידית של תבניות הניהול.</span><span class="sxs-lookup"><span data-stu-id="da82d-155">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="da82d-156">בשלב זה, תוכל לראות את המדיניות הפוך הרשמה אוטומטית של MDM לזמינה באמצעות אישורי **Azure AD המוגדרים כברירת** מחדל.</span><span class="sxs-lookup"><span data-stu-id="da82d-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>