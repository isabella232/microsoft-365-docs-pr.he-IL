---
title: הפיכת מכשירי Windows 10 לתחום למנוהלים על-ידי Microsoft 365 לעסקים
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
description: למד כיצד לאפשר Microsoft 365 להגן על מכשירי Active-Directory Windows 10 מקומיים בכמה שלבים בלבד.
ms.openlocfilehash: ec80159bdceffd8a13d09a297a2acc1b78c9b1b3
ms.sourcegitcommit: 17f0aada83627d9defa0acf4db03a2d58e46842f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/24/2021
ms.locfileid: "52636085"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="b7e92-103">הפיכת מכשירי Windows 10 לתחום למנוהלים על-ידי Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="b7e92-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="b7e92-104">אם הארגון שלך משתמש ב- Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business Premium כדי להגן על מכשירי Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים הדורשים אימות מקומי.</span><span class="sxs-lookup"><span data-stu-id="b7e92-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="b7e92-105">כדי להגדיר הגנה זו, באפשרותך ליישם מכשירים **מצורפים היברידיים של Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="b7e92-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="b7e92-106">מכשירים אלה מצורפים הן ל- Active Directory המקומי ול- Azure Active Directory שלך.</span><span class="sxs-lookup"><span data-stu-id="b7e92-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

## <a name="watch-configure-hybrid-azure-active-directory-join"></a><span data-ttu-id="b7e92-107">צפה: קביעת תצורה של צירוף היברידי של Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="b7e92-107">Watch: Configure Hybrid Azure Active Directory join</span></span>

<span data-ttu-id="b7e92-108">סרטון וידאו זה מתאר את השלבים לאיך להגדיר זאת עבור התרחיש הנפוץ ביותר, המפורט גם בשלבים המפורטים.</span><span class="sxs-lookup"><span data-stu-id="b7e92-108">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="before-you-begin"></a><span data-ttu-id="b7e92-109">לפני שתתחיל</span><span class="sxs-lookup"><span data-stu-id="b7e92-109">Before you begin</span></span>

- <span data-ttu-id="b7e92-110">סינכרון משתמשים עם Azure AD עם Azure AD התחברות.</span><span class="sxs-lookup"><span data-stu-id="b7e92-110">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="b7e92-111">השלם את סינכרון התחברות Azure AD (OU).</span><span class="sxs-lookup"><span data-stu-id="b7e92-111">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="b7e92-112">ודא שלמשתמשי התחום שאתה מסנכרן יש רשיונות Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="b7e92-112">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="b7e92-113">ראה [סינכרון משתמשי תחום עם Microsoft](manage-domain-users.md) לקבלת השלבים.</span><span class="sxs-lookup"><span data-stu-id="b7e92-113">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="b7e92-114">1. אימות רשות MDM ב- Intune</span><span class="sxs-lookup"><span data-stu-id="b7e92-114">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="b7e92-115">עבור אל [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) ובדף Microsoft Intune, **בחר** הרשמה למכשירים ולאחר מכן,  בדף מבט כולל, ודא כי **רשות MDM** היא **Intune**.</span><span class="sxs-lookup"><span data-stu-id="b7e92-115">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="b7e92-116">אם **רשות MDM** היא **ללא**, לחץ על **רשות MDM** כדי להגדיר אותה ל- **Intune**.</span><span class="sxs-lookup"><span data-stu-id="b7e92-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="b7e92-117">אם **רשות MDM** **Microsoft Office 365,עבור** אל מכשירים הרשמה מכשירים והשתמש בתיבת הדו-שיח הוספת רשות MDM בצד ימין כדי להוסיף רשות  >   **Intune MDM** (תיבת הדו-שיח הוספת **רשות MDM** זמינה רק אם רשות **MDM** מוגדרת Microsoft Office 365). </span><span class="sxs-lookup"><span data-stu-id="b7e92-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="b7e92-118">2. ודא ש- Azure AD זמין להצטרפות למחשבים</span><span class="sxs-lookup"><span data-stu-id="b7e92-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="b7e92-119">עבור אל מרכז הניהול ב ובחר Azure Active Directory (בחר הצג הכל אם Azure Active Directory אינו <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> גלוי) **ברשימה מרכזי הניהול.** </span><span class="sxs-lookup"><span data-stu-id="b7e92-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="b7e92-120">במרכז הניהול **של Azure Active Directory**, עבור אל Azure Active **Directory** , בחר **מכשירים ולאחר** מכן בחר **הגדרות מכשיר**.</span><span class="sxs-lookup"><span data-stu-id="b7e92-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="b7e92-121">אימות **שמשתמשים עשויים להצטרף למכשירים ל- Azure AD** זמין</span><span class="sxs-lookup"><span data-stu-id="b7e92-121">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="b7e92-122">כדי להפוך את כל המשתמשים לזמינים, הגדר את **האפשרות הכל.**</span><span class="sxs-lookup"><span data-stu-id="b7e92-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="b7e92-123">כדי להפוך משתמשים ספציפיים לזמינים, הגדר **את האפשרות נבחר** כדי להפוך קבוצת משתמשים ספציפית לזמינה.</span><span class="sxs-lookup"><span data-stu-id="b7e92-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="b7e92-124">הוסף את משתמשי התחום הרצויים מסונכרנים ב- Azure AD [לקבוצת אבטחה](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="b7e92-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="b7e92-125">בחר **בחר קבוצות כדי** להפוך טווח משתמש MDM לזמין עבור קבוצת אבטחה זו.</span><span class="sxs-lookup"><span data-stu-id="b7e92-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="b7e92-126">3. ודא ש- Azure AD זמין עבור MDM</span><span class="sxs-lookup"><span data-stu-id="b7e92-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="b7e92-127">עבור אל מרכז הניהול ב ובחר באפשרות <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Endpoint Managemen** t (בחר **הצג** **הכל אם Endpoint Manager** אינו גלוי)</span><span class="sxs-lookup"><span data-stu-id="b7e92-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="b7e92-128">במרכז **הניהול Microsoft Endpoint Manager**, עבור אל **מכשירים**  >  **Windows**  >  **Windows הרשמה**  >  **אוטומטית**.</span><span class="sxs-lookup"><span data-stu-id="b7e92-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="b7e92-129">ודא שטווח המשתמש של MDM זמין.</span><span class="sxs-lookup"><span data-stu-id="b7e92-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="b7e92-130">כדי לרשום את כל המחשבים, **הגדר** הכל כדי לרשום באופן אוטומטי את כל מחשבי המשתמשים המצורפים ל- Azure AD ולמחשבים חדשים כאשר המשתמשים מוסיפים חשבון עבודה ל- Windows.</span><span class="sxs-lookup"><span data-stu-id="b7e92-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="b7e92-131">הגדר לחלק **כדי** לרשום את המחשבים של קבוצת משתמשים ספציפית.</span><span class="sxs-lookup"><span data-stu-id="b7e92-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="b7e92-132">הוסף את משתמשי התחום הרצויים מסונכרנים ב- Azure AD [לקבוצת אבטחה](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="b7e92-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="b7e92-133">בחר **בחר קבוצות כדי** להפוך טווח משתמש MDM לזמין עבור קבוצת אבטחה זו.</span><span class="sxs-lookup"><span data-stu-id="b7e92-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="b7e92-134">4. יצירת המשאבים הדרושים</span><span class="sxs-lookup"><span data-stu-id="b7e92-134">4. Create the required resources</span></span> 

<span data-ttu-id="b7e92-135">ביצוע המשימות הדרושות לקביעת התצורה של [צירוף Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) היברידי התפשט באמצעות השימוש [ב- cmdlet של Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) שנמצא במודול [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b7e92-135">Performing the required tasks to [configure hybrid Azure AD join](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="b7e92-136">כאשר אתה להפעיל cmdlet זה, הוא ייצור ויגדיר את נקודת החיבור הנדרשת של השירות ואת המדיניות הקבוצתית.</span><span class="sxs-lookup"><span data-stu-id="b7e92-136">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="b7e92-137">באפשרותך להתקין מודול זה על-ידי הפעלה של הפריטים הבאים ממופע של PowerShell:</span><span class="sxs-lookup"><span data-stu-id="b7e92-137">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="b7e92-138">מומלץ להתקין מודול זה בשרת Windows Azure AD התחברות.</span><span class="sxs-lookup"><span data-stu-id="b7e92-138">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="b7e92-139">כדי ליצור את נקודת החיבור הנדרשת של השירות ומדיניות קבוצתית, תוכל להפעיל את [cmdlet Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="b7e92-139">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="b7e92-140">תצטרך את אישורי Microsoft 365 Business Premium הכלליים שלך בעת ביצוע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="b7e92-140">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="b7e92-141">כאשר תהיה מוכן ליצור את המשאבים, להפעיל את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="b7e92-141">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="b7e92-142">הפקודה הראשונה תבסס חיבור עם הענן של Microsoft, וכאשר תתבקש, ציין את אישורי Microsoft 365 Business Premium הכלליים.</span><span class="sxs-lookup"><span data-stu-id="b7e92-142">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="b7e92-143">5. קישור המדיניות הקבוצתית</span><span class="sxs-lookup"><span data-stu-id="b7e92-143">5. Link the Group Policy</span></span>

1. <span data-ttu-id="b7e92-144">במסוף ניהול המדיניות הקבוצתית (GPMC), לחץ באמצעות לחצן העכבר הימני על המיקום שבו ברצונך לקשר את המדיניות ובחר קשר *GPO קיים...* בתפריט תלוי ההקשר.</span><span class="sxs-lookup"><span data-stu-id="b7e92-144">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="b7e92-145">בחר את המדיניות שנוצרה בשלב לעיל ולאחר מכן לחץ על **אישור.**</span><span class="sxs-lookup"><span data-stu-id="b7e92-145">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="b7e92-146">קבל את תבניות הניהול העדכניות ביותר</span><span class="sxs-lookup"><span data-stu-id="b7e92-146">Get the latest Administrative Templates</span></span>

<span data-ttu-id="b7e92-147">אם אינך רואה את המדיניות הפוך הרשמה **אוטומטית של MDM** לזמינה באמצעות אישורי Azure AD המוגדרים כברירת מחדל, ייתכן שהאפשרות היא ש- ADMX אינו מותקן עבור Windows 10, גירסה 1803 ואילך.</span><span class="sxs-lookup"><span data-stu-id="b7e92-147">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="b7e92-148">כדי לפתור את הבעיה, בצע את השלבים הבאים (הערה: MDM.admx העדכני ביותר תואם לאחור):</span><span class="sxs-lookup"><span data-stu-id="b7e92-148">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="b7e92-149">הורד: [תבניות מנהליות ( .admx) עבור עדכון Windows 10 אוקטובר 2020 (20H2)](https://www.microsoft.com/download/102157).</span><span class="sxs-lookup"><span data-stu-id="b7e92-149">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2.  <span data-ttu-id="b7e92-150">התקן את החבילה בבקר תחום.</span><span class="sxs-lookup"><span data-stu-id="b7e92-150">Install the package on a Domain Controller.</span></span>
3.  <span data-ttu-id="b7e92-151">נווט, בהתאם לגירסת תבניות הניהול לתיקיה: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 עדכון אוקטובר 2020 (20H2)**.</span><span class="sxs-lookup"><span data-stu-id="b7e92-151">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4.  <span data-ttu-id="b7e92-152">שנה את **שם התיקיה** הגדרות מדיניות בנתיב לעיל **למדיניותDefinitions**.</span><span class="sxs-lookup"><span data-stu-id="b7e92-152">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="b7e92-153">העתק את **התיקיה PolicyDefinitions** לשיתוף SYSVOL שלך, הממוקמת כברירת מחדל **ב- C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="b7e92-153">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="b7e92-154">אם בכוונתך להשתמש בחנות מדיניות מרכזית עבור התחום כולו, הוסף את התוכן של PolicyDefinitions שם.</span><span class="sxs-lookup"><span data-stu-id="b7e92-154">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="b7e92-155">במקרה שיש לך כמה בקרי תחום, המתן עד ש- SYSVOL ישכפל כדי שמדיניות תהיה זמינה.</span><span class="sxs-lookup"><span data-stu-id="b7e92-155">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="b7e92-156">הליך זה יעבוד גם עבור כל גירסה עתידית של תבניות הניהול.</span><span class="sxs-lookup"><span data-stu-id="b7e92-156">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="b7e92-157">בשלב זה, תוכל לראות את המדיניות הפוך הרשמה אוטומטית של MDM לזמינה באמצעות אישורי **Azure AD המוגדרים כברירת** מחדל.</span><span class="sxs-lookup"><span data-stu-id="b7e92-157">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

## <a name="related-content"></a><span data-ttu-id="b7e92-158">תוכן קשור</span><span class="sxs-lookup"><span data-stu-id="b7e92-158">Related content</span></span>

<span data-ttu-id="b7e92-159">[סינכרון משתמשי תחום Microsoft 365](manage-domain-users.md) (מאמר)</span><span class="sxs-lookup"><span data-stu-id="b7e92-159">[Synchronize domain users to Microsoft 365](manage-domain-users.md) (article)</span></span>\
<span data-ttu-id="b7e92-160">[יצירת קבוצה במרכז הניהול](../admin/create-groups/create-groups.md) (מאמר)</span><span class="sxs-lookup"><span data-stu-id="b7e92-160">[Create a group in the admin center](../admin/create-groups/create-groups.md) (article)</span></span>\
<span data-ttu-id="b7e92-161">[ערכת לימוד: קביעת תצורה של צירוף היברידי של Azure Active Directory עבור תחומים מנוהלים](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (מאמר)</span><span class="sxs-lookup"><span data-stu-id="b7e92-161">[Tutorial: Configure hybrid Azure Active Directory join for managed domains](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (article)</span></span>