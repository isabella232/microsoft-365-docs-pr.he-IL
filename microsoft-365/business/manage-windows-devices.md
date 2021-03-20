---
title: הפיכת מכשירי Windows 10 המצורפים לתחום למנוהל על-ידי Microsoft 365 for business
f1.keywords:
- CSH
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: למד כיצד להפוך את Microsoft 365 לזמין כדי להגן על מכשירים מקומיים של Active Directory המצורפים ל-Windows 10 בשלבים ספורים בלבד.
ms.openlocfilehash: 82d4ac3f1d6aba9489f9ea153de3a3d2083b47ec
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913193"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="d9b5f-103">הפיכת מכשירי Windows 10 המצורפים לתחום למנוהל על-ידי Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="d9b5f-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="d9b5f-104">אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business Premium כדי להגן על מכשירי Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים הדורשים אימות מקומי.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="d9b5f-105">כדי להגדיר הגנה זו, באפשרותך ליישם **מכשירים המצורפים להודעה משולבת של תכלת**.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="d9b5f-106">מכשירים אלה מצורפים הן ל-Active Directory המקומי והן ל-תכלת Active Directory שלך.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="d9b5f-107">סרטון וידאו זה מתאר את השלבים להגדרת פעולה זו עבור התרחיש הנפוץ ביותר, המפורט גם בשלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="d9b5f-108">לפני שתתחיל, הקפד להשלים שלבים אלה:</span><span class="sxs-lookup"><span data-stu-id="d9b5f-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="d9b5f-109">סנכרן משתמשים לתכלת לספירה באמצעות התחברות של תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="d9b5f-110">השלם את הסינכרון של היחידה הארגונית של "תכלת" (OU).</span><span class="sxs-lookup"><span data-stu-id="d9b5f-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="d9b5f-111">ודא שכל משתמשי התחום שאתה מסנכרן הם בעלי רשיונות ל-Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="d9b5f-112">ראה [סינכרון משתמשי תחום ל-Microsoft](manage-domain-users.md) לקבלת השלבים.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="d9b5f-113">1. אימות הרשות של MDM בתוך המנגינה</span><span class="sxs-lookup"><span data-stu-id="d9b5f-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="d9b5f-114">עבור אל [מנהל נקודות הקצה](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) ולאחר מכן, בעמוד ההתאמה של Microsoft, בחר באפשרות **הרשמת מכשיר** ולאחר מכן, בדף **מבט כולל** , ודא **שסמכות MDM** מתכוונת **.**</span><span class="sxs-lookup"><span data-stu-id="d9b5f-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="d9b5f-115">אם **הרשות של mdm** היא **None**, לחץ על **הרשות mdm** כדי **להגדיר** אותה כתכונה.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="d9b5f-116">אם **הרשות של MDM** היא **microsoft office 365**, **עבור אל** מכשירי רישום של מכשירים  >   והשתמש בתיבת הדו **הוספת רשות mdm** בצד שמאל כדי להוסיף **כוונון רשות mdm** (תיבת הדו **הוספת רשות mdm** זמינה רק אם **הרשות mdm** מוגדרת ל-Microsoft office 365).</span><span class="sxs-lookup"><span data-stu-id="d9b5f-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="d9b5f-117">2. ודא שתכלת לספירה מופעל לצורך הצטרפות למחשבים</span><span class="sxs-lookup"><span data-stu-id="d9b5f-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="d9b5f-118">עבור אל מרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  ובחר **תכלת active directory** (בחר הצג הכל אם תכלת active directory אינו גלוי) ברשימת **מרכזי הניהול** .</span><span class="sxs-lookup"><span data-stu-id="d9b5f-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="d9b5f-119">במרכז **הניהול של תכלת Active directory**, עבור **אל תכלת active directory** , בחר **התקנים** ולאחר מכן **הגדרות התקן**.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="d9b5f-120">אימות **משתמשים עשויים לצרף מכשירים לתכלת AD** מופעל</span><span class="sxs-lookup"><span data-stu-id="d9b5f-120">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="d9b5f-121">כדי להפוך את כל המשתמשים לזמינים, הגדר **הכל**.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="d9b5f-122">כדי להפוך משתמשים ספציפיים לזמינים, הגדר לאפשרות **נבחרה** כדי להפוך קבוצת משתמשים ספציפית לזמינה.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="d9b5f-123">הוסף את משתמשי התחום הרצויים מסונכרנים בתכלת לספירה [לקבוצת אבטחה](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="d9b5f-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="d9b5f-124">בחר **באפשרות בחר קבוצות** כדי להפוך את טווח המשתמש של MDM לזמין עבור קבוצת אבטחה זו.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="d9b5f-125">3. אימות תכלת לספירה מופעל עבור MDM</span><span class="sxs-lookup"><span data-stu-id="d9b5f-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="d9b5f-126">עבור אל מרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  ובחר באפשרות בחר **נקודת קצה Managemen** t (בחר **הצג הכל** אם **מנהל נקודות הקצה** אינו גלוי)</span><span class="sxs-lookup"><span data-stu-id="d9b5f-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="d9b5f-127">במרכז **הניהול של מנהל נקודות הקצה של Microsoft**, עבור אל מכשירים   >    >    >  **ההרשמה האוטומטית** של windows windows הרשמה.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="d9b5f-128">אימות טווח המשתמשים של MDM זמין.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="d9b5f-129">כדי לרשום את כל המחשבים, הגדר **הכל** כדי לרשום באופן אוטומטי את כל מחשבי המשתמש המצורפים לתכלת לספירה ולמחשבים חדשים כאשר המשתמשים מוסיפים חשבון עבודה ל-Windows.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="d9b5f-130">הגדר **כמה** כדי לרשום את המחשבים של קבוצת משתמשים ספציפית.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="d9b5f-131">הוסף את משתמשי התחום הרצויים מסונכרנים בתכלת לספירה [לקבוצת אבטחה](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="d9b5f-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="d9b5f-132">בחר **באפשרות בחר קבוצות** כדי להפוך את טווח המשתמש של MDM לזמין עבור קבוצת אבטחה זו.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="d9b5f-133">4. יצירת המשאבים הדרושים</span><span class="sxs-lookup"><span data-stu-id="d9b5f-133">4. Create the required resources</span></span> 

<span data-ttu-id="d9b5f-134">ביצוע המשימות הנדרשות כדי [לקבוע את התצורה של הצטרפות היברידית של ' תכלת לספירה](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) ' היה פשוט יותר באמצעות ה-Cmdlet ' [אתחול-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) ' שנמצא במודול [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-134">Performing the required tasks to [configure hybrid Azure AD join](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="d9b5f-135">כאשר אתה מפעיל את ה-cmdlet הזה, הוא ייצור ויקבע את התצורה של נקודת חיבור השירות הנדרשת והמדיניות הקבוצתית.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="d9b5f-136">באפשרותך להתקין מודול זה על-ידי הפעלת הפרטים הבאים מתוך מופע של PowerShell:</span><span class="sxs-lookup"><span data-stu-id="d9b5f-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="d9b5f-137">מומלץ להתקין מודול זה בשרת Windows שבו פועל הקישור תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="d9b5f-138">כדי ליצור את נקודת חיבור השירות הדרושה ומדיניות קבוצתית, עליך להפעיל את ה  [-Cmdlet אתחול-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) .</span><span class="sxs-lookup"><span data-stu-id="d9b5f-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="d9b5f-139">תזדקק לאישורי מנהל מערכת כללי של Microsoft 365 Business Premium בעת ביצוע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="d9b5f-140">כאשר תהיה מוכן ליצור את המשאבים, הפעל את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="d9b5f-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="d9b5f-141">הפקודה הראשונה תיצור חיבור עם הענן של Microsoft, וכאשר תתבקש, ציין את אישורי מנהל המערכת הכלליים של Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="d9b5f-142">5. קישור מדיניות קבוצתית</span><span class="sxs-lookup"><span data-stu-id="d9b5f-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="d9b5f-143">במסוף ניהול מדיניות קבוצתית (GPMC), לחץ באמצעות לחצן העכבר הימני על המיקום שבו ברצונך לקשר את המדיניות ובחר קשר אובייקט מדיניות *קיים.* ... מהתפריט תלוי ההקשר.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="d9b5f-144">בחר את המדיניות שנוצרה בשלב שלעיל ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="d9b5f-145">קבל את תבניות הניהול האחרונות</span><span class="sxs-lookup"><span data-stu-id="d9b5f-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="d9b5f-146">אם אינך רואה את המדיניות **הפיכת הרשמה אוטומטית של MDM לזמינה באמצעות כברירת מחדל של הודעות מיידיות**, ייתכן שהסיבה לכך היא ש-ADMX אינו מותקן עבור Windows 10, גירסה 1803 ואילך.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="d9b5f-147">כדי לפתור את הבעיה, בצע שלבים אלה (הערה: הגירסה העדכנית ביותר של MDM. admx היא תואמת לאחור):</span><span class="sxs-lookup"><span data-stu-id="d9b5f-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="d9b5f-148">[הורד: תבניות ניהול (. admx) עבור Windows 10 באוקטובר 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span><span class="sxs-lookup"><span data-stu-id="d9b5f-148">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2.  <span data-ttu-id="d9b5f-149">התקן את החבילה בבקר תחום.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-149">Install the package on a Domain Controller.</span></span>
3.  <span data-ttu-id="d9b5f-150">נווט, בהתאם לגירסת תבניות הניהול לתיקיה: **C:\Program Files (x86) \Microsoft Group Policy\Windows 10 באוקטובר 2020 Update (20H2)**.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-150">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4.  <span data-ttu-id="d9b5f-151">שנה את שם התיקיה ' **הגדרות מדיניות** ' בנתיב שלעיל אל **PolicyDefinitions**.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="d9b5f-152">העתק את התיקיה **PolicyDefinitions** למיקום המשותף של SYSVOL, כברירת מחדל, הממוקמת ב- **C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-152">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="d9b5f-153">אם בכוונתך להשתמש בחנות מדיניות מרכזית עבור התחום כולו, הוסף את התוכן של PolicyDefinitions שם.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="d9b5f-154">למקרה שיהיו לך כמה בקרי תחומים, המתן עד ש-SYSVOL ישכפל כדי שהמדיניות תהיה זמינה.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-154">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="d9b5f-155">הליך זה יפעל גם עבור כל גירסה עתידית של תבניות ניהול.</span><span class="sxs-lookup"><span data-stu-id="d9b5f-155">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="d9b5f-156">בשלב זה, תוכל לראות את המדיניות **הפיכת הרשמה אוטומטית של MDM לזמינה באמצעות כברירת מחדל של הודעות מיידיות** .</span><span class="sxs-lookup"><span data-stu-id="d9b5f-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>