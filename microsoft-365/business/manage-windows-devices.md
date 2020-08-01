---
title: הפעל התקנים של Windows 10 המצורפים לתחום לניהול באמצעות Microsoft 365 עבור עסקים
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
description: למד כיצד לאפשר ל-Microsoft 365 להגן על התקנים מקומיים המצורפים ל-Windows 10 באמצעות ספריות בתוך מספר צעדים בלבד.
ms.openlocfilehash: 2eaf5aa76cae1680b93af008af615ae872e4fb20
ms.sourcegitcommit: fab425ea4580d1924fb421e6db233d135f5b7d19
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/31/2020
ms.locfileid: "46533784"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="27b70-103">אפשר להפעיל התקנים של Windows 10 המצורפים לתחום כדי שינוהל על-ידי Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="27b70-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="27b70-104">אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business Premium כדי להגן על התקני Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים המחייבים אימות מקומי.</span><span class="sxs-lookup"><span data-stu-id="27b70-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="27b70-105">כדי להגדיר הגנה זו, באפשרותך ליישם **התקנים היברידית כחול לספירה המצורפים**.</span><span class="sxs-lookup"><span data-stu-id="27b70-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="27b70-106">התקנים אלה מצורפים הן ל-Active Directory המקומי והן לספריה הפעילה שלך.</span><span class="sxs-lookup"><span data-stu-id="27b70-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="27b70-107">סרטון וידאו זה מתאר את השלבים עבור אופן ההגדרה של התרחיש הנפוץ ביותר, המפורט גם בשלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="27b70-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="27b70-108">לפני שתתחיל, הקפד להשלים את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="27b70-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="27b70-109">סנכרן משתמשים לתכלת והתחבר כתכלת.</span><span class="sxs-lookup"><span data-stu-id="27b70-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="27b70-110">השלם תכלת AD חיבור יחידה ארגונית (OU) סינכרון.</span><span class="sxs-lookup"><span data-stu-id="27b70-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="27b70-111">ודא שכל משתמשי התחום שתסנכרן כוללים רשיונות ל-Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="27b70-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="27b70-112">ראה [סינכרון משתמשי קבוצת מחשבים ל-Microsoft](manage-domain-users.md) עבור השלבים.</span><span class="sxs-lookup"><span data-stu-id="27b70-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="27b70-113">1. ודא שרשות MDM בIntune</span><span class="sxs-lookup"><span data-stu-id="27b70-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="27b70-114">עבור אל portal.azure.com ובחלק העליון של חיפוש הדף עבור Intune.</span><span class="sxs-lookup"><span data-stu-id="27b70-114">Go to portal.azure.com and on the top of the page search for Intune.</span></span>
<span data-ttu-id="27b70-115">בדף Microsoft Intune, בחר **הרשמת התקן** ובעמוד **מבט כולל** ודא **שהסמכות של MDM** היא **Intune**.</span><span class="sxs-lookup"><span data-stu-id="27b70-115">On the Microsoft Intune page, select **Device enrollment** and on the **Overview** page make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="27b70-116">אם **רשות mdm** אינה **קיימת**, לחץ על **הרשות mdm** כדי להגדיר אותה ל- **Intune**.</span><span class="sxs-lookup"><span data-stu-id="27b70-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="27b70-117">אם **רשות mdm** היא **Microsoft Office 365**, עבור אל **התקנים**  >  **לרישום התקנים** והשתמש בתיבת הדו **הוספת הרשות של mdm** מימין כדי להוסיף את הרשות **Intune MDM** (תיבת הדו **הוספת הרשות של mdm** זמינה רק אם **הרשות MDM** מוגדרת ל-Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="27b70-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="27b70-118">2. ודא תכלת לספירה מופעל לצורך הצטרפות למחשבים</span><span class="sxs-lookup"><span data-stu-id="27b70-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="27b70-119">עבור אל מרכז הניהול ב- <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ובחר באפשרות ' **active directory** ' (בחר הצג הכל אם הספריה הפעילה אינה גלויה) ברשימת **מרכזי הניהול** .</span><span class="sxs-lookup"><span data-stu-id="27b70-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="27b70-120">במרכז **הניהול של הספריה הפעילה**, עבור אל הכלי **הפעיל של active directory** , בחר באפשרות **התקנים** ולאחר מכן **הגדרות התקן**.</span><span class="sxs-lookup"><span data-stu-id="27b70-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="27b70-121">ודא**כי משתמשים יכולים לצרף התקנים ל-"תכלת לספירה** " מופעלת</span><span class="sxs-lookup"><span data-stu-id="27b70-121">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="27b70-122">כדי להפוך את כל המשתמשים **לזמינים**, הגדר לכל.</span><span class="sxs-lookup"><span data-stu-id="27b70-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="27b70-123">כדי להפוך משתמשים מסוימים לזמינים, הגדר **כנבחרת** כדי לאפשר קבוצה מסוימת של משתמשים.</span><span class="sxs-lookup"><span data-stu-id="27b70-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="27b70-124">הוסף את משתמשי התחום הרצויים המסונכרנת בתכלת לספירה [לקבוצת אבטחה](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="27b70-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="27b70-125">בחר **קבוצות בחירה** כדי להפוך את טווח המשתמשים של MDM לזמין עבור קבוצת אבטחה זו.</span><span class="sxs-lookup"><span data-stu-id="27b70-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="27b70-126">3. ודא תכלת לספירה מופעל עבור MDM</span><span class="sxs-lookup"><span data-stu-id="27b70-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="27b70-127">עבור אל מרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ובחר בחירת אנשי **מופע** של נקודות **הקצה**(בחר הצג הכל אם **מנהל נקודות הקצה** אינו גלוי)</span><span class="sxs-lookup"><span data-stu-id="27b70-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="27b70-128">במרכז **הניהול של מנהל נקודות הקצה של Microsoft**, עבור אל **Devices**  >  **Windows**  >  **Windows Enrollment**  >  **הרישום האוטומטי**של התקנים של windows windows הרשמה.</span><span class="sxs-lookup"><span data-stu-id="27b70-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="27b70-129">ודא שטווח המשתמש של MDM מופעל.</span><span class="sxs-lookup"><span data-stu-id="27b70-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="27b70-130">כדי לרשום את כל המחשבים, הגדר **כולם** כדי לרשום באופן אוטומטי את כל מחשבי המשתמש המצורפים לתכלת AD ולמחשבים חדשים כאשר המשתמשים מוסיפים חשבון עבודה ל-Windows.</span><span class="sxs-lookup"><span data-stu-id="27b70-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="27b70-131">מוגדר **כחלק** כדי לרשום את המחשבים של קבוצת משתמשים מסוימת.</span><span class="sxs-lookup"><span data-stu-id="27b70-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="27b70-132">הוסף את משתמשי התחום הרצויים המסונכרנת בתכלת לספירה [לקבוצת אבטחה](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="27b70-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="27b70-133">בחר **קבוצות בחירה** כדי להפוך את טווח המשתמשים של MDM לזמין עבור קבוצת אבטחה זו.</span><span class="sxs-lookup"><span data-stu-id="27b70-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="27b70-134">4. צור את המשאבים הדרושים</span><span class="sxs-lookup"><span data-stu-id="27b70-134">4. Create the required resources</span></span> 

<span data-ttu-id="27b70-135">ביצוע המשימות הנדרשות כדי [לקבוע את התצורה של היברידית התכלת להצטרף](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) היתה פשוטה באמצעות שימוש של [ההרשמה לאתחל-Secmgmthyהרשמה](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Cmdlet נמצא במודול [secmgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="27b70-135">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="27b70-136">בעת הפעלת יישומון cmdlet זה, הוא ייצור ויקבע את התצורה של נקודת חיבור השירות הנדרשת והמדיניות הקבוצתית.</span><span class="sxs-lookup"><span data-stu-id="27b70-136">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="27b70-137">באפשרותך להתקין מודול זה על-ידי הפעלת הפעולה הבאה ממופע של PowerShell:</span><span class="sxs-lookup"><span data-stu-id="27b70-137">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="27b70-138">מומלץ להתקין מודול זה ב-Windows Server שבו פועל התקשרות תכלת AD.</span><span class="sxs-lookup"><span data-stu-id="27b70-138">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="27b70-139">כדי ליצור את נקודת החיבור הדרושה של השירות והמדיניות הקבוצתית, עליך להפעיל את ה-cmdlet של [הרשמת ההתקן של התקנת האבטחה](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) .</span><span class="sxs-lookup"><span data-stu-id="27b70-139">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="27b70-140">תזדקק לאישורי המנהל הגלובלי של Microsoft Business Premium 365 במהלך ביצוע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="27b70-140">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="27b70-141">כאשר תהיה מוכן ליצור את המשאבים, הפעל את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="27b70-141">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="27b70-142">הפקודה הראשונה תיצור חיבור עם ענן של Microsoft, וכאשר תתבקש, ציין את אישורי המנהל הכללי של מנהל העסקים של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="27b70-142">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="27b70-143">5. קשר את המדיניות הקבוצתית</span><span class="sxs-lookup"><span data-stu-id="27b70-143">5. Link the Group Policy</span></span>

1. <span data-ttu-id="27b70-144">במסוף ניהול המדיניות הקבוצתית (GPMC), לחץ באמצעות לחצן העכבר הימני על המיקום שבו ברצונך לקשר את המדיניות ובחר *קישור של GPO קיים.* ...</span><span class="sxs-lookup"><span data-stu-id="27b70-144">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="27b70-145">בחר את המדיניות שנוצרה בשלב הנ ל ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="27b70-145">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="27b70-146">קבל את התבניות המנהליות העדכניות ביותר</span><span class="sxs-lookup"><span data-stu-id="27b70-146">Get the latest Administrative Templates</span></span>

<span data-ttu-id="27b70-147">אם אינך רואה שהמדיניות **מאפשרת הרשמה אוטומטית של MDM המשתמשת באישורי תכלת לספירה**, ייתכן שהסיבה לכך היא שאין ברשותך את ה-admx המותקנת עבור Windows 10, גירסה 1803, גירסה 1809 או גירסה 1903.</span><span class="sxs-lookup"><span data-stu-id="27b70-147">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="27b70-148">כדי לפתור את הבעיה, בצע את הפעולות הבאות (הערה: MDM. admx האחרון תואם לאחור):</span><span class="sxs-lookup"><span data-stu-id="27b70-148">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="27b70-149">[להוריד: תבניות מנהליות (. admx) עבור Windows 10 מאי 2019 עדכון (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="27b70-149">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="27b70-150">התקן את החבילה בבקר התחום הראשי (PDC).</span><span class="sxs-lookup"><span data-stu-id="27b70-150">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="27b70-151">ניווט, בהתאם לגירסה לתיקיה: **C:\templletccome\n מיקרוסופט/Windows 10 May 2019 עדכון (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="27b70-151">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="27b70-152">שנה את שם התיקיה **הגדרות מדיניות** בנתיב שלעיל **להגדרות**המדיניות.</span><span class="sxs-lookup"><span data-stu-id="27b70-152">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="27b70-153">העתק את התיקיה ' **הגדרות** מדיניות ' ל- **C:\windows\so\t\uspe\n**.</span><span class="sxs-lookup"><span data-stu-id="27b70-153">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="27b70-154">אם בכוונתך להשתמש במאגר מדיניות מרכזי עבור כל התחום שלך, הוסף את תוכן המדיניות המבוטח.</span><span class="sxs-lookup"><span data-stu-id="27b70-154">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="27b70-155">הפעל מחדש את בקר קבוצת המחשבים הראשי כדי שהמדיניות תהיה זמינה.</span><span class="sxs-lookup"><span data-stu-id="27b70-155">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="27b70-156">הליך זה יפעל גם עבור כל גירסה עתידית.</span><span class="sxs-lookup"><span data-stu-id="27b70-156">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="27b70-157">בשלב זה אתה אמור להיות מסוגל לראות את המדיניות **לאפשר הרשמה אוטומטית MDM באמצעות ברירת המחדל של הודעות תכלת לספירה** זמין.</span><span class="sxs-lookup"><span data-stu-id="27b70-157">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>
