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
ms.openlocfilehash: 857651081fb10856d28dd419333ebef655388407
ms.sourcegitcommit: e6e704cbd9a50fc7db1e6a0cf5d3f8c6cbb94363
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/04/2020
ms.locfileid: "44564944"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="29861-103">אפשר להפעיל התקנים של Windows 10 המצורפים לתחום כדי שינוהל על-ידי Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="29861-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="29861-104">אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business Premium כדי להגן על התקני Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים המחייבים אימות מקומי.</span><span class="sxs-lookup"><span data-stu-id="29861-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="29861-105">כדי להגדיר הגנה זו, באפשרותך ליישם **התקנים היברידית כחול לספירה המצורפים**.</span><span class="sxs-lookup"><span data-stu-id="29861-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="29861-106">התקנים אלה מצורפים הן ל-Active Directory המקומי והן לספריה הפעילה שלך.</span><span class="sxs-lookup"><span data-stu-id="29861-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="29861-107">סרטון וידאו זה מתאר את השלבים עבור אופן ההגדרה של התרחיש הנפוץ ביותר, המפורט גם בשלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="29861-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="29861-108">לפני שתתחיל, הקפד להשלים את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="29861-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="29861-109">סנכרן משתמשים לתכלת והתחבר כתכלת.</span><span class="sxs-lookup"><span data-stu-id="29861-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="29861-110">השלם תכלת AD חיבור יחידה ארגונית (OU) סינכרון.</span><span class="sxs-lookup"><span data-stu-id="29861-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="29861-111">ודא שכל משתמשי התחום שתסנכרן כוללים רשיונות ל-Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="29861-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="29861-112">ראה [סינכרון משתמשי קבוצת מחשבים ל-Microsoft](manage-domain-users.md) עבור השלבים.</span><span class="sxs-lookup"><span data-stu-id="29861-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="29861-113">1. ודא שרשות MDM בIntune</span><span class="sxs-lookup"><span data-stu-id="29861-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="29861-114">עבור אל portal.azure.com ובחלק העליון של חיפוש הדף עבור Intune.</span><span class="sxs-lookup"><span data-stu-id="29861-114">Go to portal.azure.com and on the top of the page search for Intune.</span></span>
<span data-ttu-id="29861-115">בדף Microsoft Intune, בחר **הרשמת התקן** ובעמוד **מבט כולל** ודא **שהסמכות של MDM** היא **Intune**.</span><span class="sxs-lookup"><span data-stu-id="29861-115">On the Microsoft Intune page, select **Device enrollment** and on the **Overview** page make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="29861-116">אם **רשות mdm** אינה **קיימת**, לחץ על **הרשות mdm** כדי להגדיר אותה ל- **Intune**.</span><span class="sxs-lookup"><span data-stu-id="29861-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="29861-117">אם **רשות mdm** היא **Microsoft Office 365**, עבור אל **התקנים**  >  **לרישום התקנים** והשתמש בתיבת הדו **הוספת הרשות של mdm** מימין כדי להוסיף את הרשות **Intune MDM** (תיבת הדו **הוספת הרשות של mdm** זמינה רק אם **הרשות MDM** מוגדרת ל-Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="29861-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="29861-118">2. ודא תכלת לספירה מופעל לצורך הצטרפות למחשבים</span><span class="sxs-lookup"><span data-stu-id="29861-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="29861-119">עבור אל מרכז הניהול ב- https://admin.microsoft.com ובחר באפשרות ' **active directory** ' (בחר הצג הכל אם הספריה הפעילה אינה גלויה) ברשימת **מרכזי הניהול** .</span><span class="sxs-lookup"><span data-stu-id="29861-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="29861-120">במרכז **הניהול של הספריה הפעילה**, עבור אל הכלי **הפעיל של active directory** , בחר באפשרות **התקנים** ולאחר מכן **הגדרות התקן**.</span><span class="sxs-lookup"><span data-stu-id="29861-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="29861-121">ודא**כי משתמשים יכולים לצרף התקנים ל-"תכלת לספירה** " מופעלת</span><span class="sxs-lookup"><span data-stu-id="29861-121">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="29861-122">כדי להפוך את כל המשתמשים **לזמינים**, הגדר לכל.</span><span class="sxs-lookup"><span data-stu-id="29861-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="29861-123">כדי להפוך משתמשים מסוימים לזמינים, הגדר **כנבחרת** כדי לאפשר קבוצה מסוימת של משתמשים.</span><span class="sxs-lookup"><span data-stu-id="29861-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="29861-124">הוסף את משתמשי התחום הרצויים המסונכרנת בתכלת לספירה [לקבוצת אבטחה](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="29861-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="29861-125">בחר **קבוצות בחירה** כדי להפוך את טווח המשתמשים של MDM לזמין עבור קבוצת אבטחה זו.</span><span class="sxs-lookup"><span data-stu-id="29861-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="29861-126">3. ודא תכלת לספירה מופעל עבור MDM</span><span class="sxs-lookup"><span data-stu-id="29861-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="29861-127">עבור אל מרכז הניהול https://admin.microsoft.com ובחר בחירת אנשי **מופע** של נקודות **הקצה**(בחר הצג הכל אם **מנהל נקודות הקצה** אינו גלוי)</span><span class="sxs-lookup"><span data-stu-id="29861-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="29861-128">במרכז **הניהול של מנהל נקודות הקצה של Microsoft**, עבור אל **Devices**  >  **Windows**  >  **Windows Enrollment**  >  **הרישום האוטומטי**של התקנים של windows windows הרשמה.</span><span class="sxs-lookup"><span data-stu-id="29861-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="29861-129">ודא שטווח המשתמש של MDM מופעל.</span><span class="sxs-lookup"><span data-stu-id="29861-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="29861-130">כדי לרשום את כל המחשבים, הגדר **כולם** כדי לרשום באופן אוטומטי את כל מחשבי המשתמש המצורפים לתכלת AD ולמחשבים חדשים כאשר המשתמשים מוסיפים חשבון עבודה ל-Windows.</span><span class="sxs-lookup"><span data-stu-id="29861-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="29861-131">מוגדר **כחלק** כדי לרשום את המחשבים של קבוצת משתמשים מסוימת.</span><span class="sxs-lookup"><span data-stu-id="29861-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="29861-132">הוסף את משתמשי התחום הרצויים המסונכרנת בתכלת לספירה [לקבוצת אבטחה](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="29861-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="29861-133">בחר **קבוצות בחירה** כדי להפוך את טווח המשתמשים של MDM לזמין עבור קבוצת אבטחה זו.</span><span class="sxs-lookup"><span data-stu-id="29861-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-set-up-service-connection-point-scp"></a><span data-ttu-id="29861-134">4. הגדרת נקודת חיבור של שירות (SCP)</span><span class="sxs-lookup"><span data-stu-id="29861-134">4. Set up Service connection point (SCP)</span></span>

<span data-ttu-id="29861-135">שלבים אלה הם פשוטים יותר מאשר [להגדיר היברידית תכלת להצטרף](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span><span class="sxs-lookup"><span data-stu-id="29861-135">These steps are simplified from [configure hybrid azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="29861-136">כדי להשלים את השלבים שאתה צריך להשתמש תכלת AD הקשר ואת מיקרוסופט 365 עסקים פרמיה הכללית ניהול וסיסמאות Active Directory מנהל.</span><span class="sxs-lookup"><span data-stu-id="29861-136">To complete the steps you need to use Azure AD Connect and your Microsoft 365 Business Premium global admin and Active Directory admin passwords.</span></span>

1.  <span data-ttu-id="29861-137">התחל להתחבר לתכלת ולאחר מכן בחר **בקביעת תצורה**.</span><span class="sxs-lookup"><span data-stu-id="29861-137">Start Azure AD Connect, and then select **Configure**.</span></span>
2.  <span data-ttu-id="29861-138">בדף **פעילויות נוספות** , בחר **באפשרות קביעת תצורה של אפשרויות התקן**ולאחר מכן בחר באפשרות **הבא**.</span><span class="sxs-lookup"><span data-stu-id="29861-138">On the **Additional tasks**  page, select **Configure device options**, and then select **Next**.</span></span>
3.  <span data-ttu-id="29861-139">בדף ' **מבט כולל** ', בחר באפשרות ' **הבא**'.</span><span class="sxs-lookup"><span data-stu-id="29861-139">On the **Overview** page, select **Next**.</span></span>
4.  <span data-ttu-id="29861-140">בדף ' **התחברות לתכלת** ', הזן את האישורים של מנהל כללי עבור Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="29861-140">On the **Connect to Azure AD** page, enter the credentials of a global administrator for Microsoft 365 Business Premium.</span></span>
5.  <span data-ttu-id="29861-141">בדף **אפשרויות התקן** , בחר באפשרות **הגדרת כחול היברידי כתכלת**ולאחר מכן בחר **בהבא**.</span><span class="sxs-lookup"><span data-stu-id="29861-141">On the **Device options** page, select **Configure Hybrid Azure AD join**, and then select **Next**.</span></span>
6.  <span data-ttu-id="29861-142">בדף **SCP** , עבור כל יער שבו ברצונך ש-"תכלת" תתחבר לקביעת התצורה של SCP, השלם את השלבים הבאים ולאחר מכן בחר **בהבא**:</span><span class="sxs-lookup"><span data-stu-id="29861-142">On the **SCP** page, for each forest where you want Azure AD Connect to configure the SCP, complete the following steps, and then select **Next**:</span></span>
    - <span data-ttu-id="29861-143">בדוק את התיבה שליד שם היער.</span><span class="sxs-lookup"><span data-stu-id="29861-143">Check the box beside the forest name.</span></span> <span data-ttu-id="29861-144">היער צריך להיות. שם הדומיין שלך</span><span class="sxs-lookup"><span data-stu-id="29861-144">The forest should be your AD domain name.</span></span>
    - <span data-ttu-id="29861-145">תחת עמודת **שירות האימות** , פתח את הרשימה הנפתחת ובחר את שם התחום התואם (קיימת רק אפשרות אחת בלבד).</span><span class="sxs-lookup"><span data-stu-id="29861-145">Under the **Authentication Service** column, open the dropdown and select matching domain name (there should only be one only option).</span></span>
    - <span data-ttu-id="29861-146">בחר **ב'הוספה** כדי להזין את האישורים של מנהל קבוצת המחשבים.</span><span class="sxs-lookup"><span data-stu-id="29861-146">Select **Add** to enter the domain administrator credentials.</span></span>  
7.  <span data-ttu-id="29861-147">בדף **מערכות ההפעלה של ההתקן** , בחר את Windows 10 או התקנים מאוחרים יותר המצורפים לתחום בלבד.</span><span class="sxs-lookup"><span data-stu-id="29861-147">On the **Device operating systems** page, select Windows 10 or later domain-joined devices only.</span></span>
8.  <span data-ttu-id="29861-148">בעמוד ' **מוכן לקביעת התצורה** ', בחר באפשרות ' **קביעת תצורה**'.</span><span class="sxs-lookup"><span data-stu-id="29861-148">On the **Ready to configure** page, select **Configure**.</span></span>
9.  <span data-ttu-id="29861-149">בעמוד **השלם של התצורה** , בחר באפשרות **יציאה**.</span><span class="sxs-lookup"><span data-stu-id="29861-149">On the **Configuration complete** page, select **Exit**.</span></span>


## <a name="5-create-a-gpo-for-intune-enrollment--admx-method"></a><span data-ttu-id="29861-150">5. יצירת GPO עבור Intune הרשמה – ADMX שיטה</span><span class="sxs-lookup"><span data-stu-id="29861-150">5. Create a GPO for Intune Enrollment – ADMX method</span></span>

<span data-ttu-id="29861-151">השתמש. קובץ תבנית ADMX.</span><span class="sxs-lookup"><span data-stu-id="29861-151">Use .ADMX template file.</span></span>

1.  <span data-ttu-id="29861-152">בצע כניסה לשרת AD, חפש ופתח את **Server Manager**  >  **Tools**  >  **ניהול המדיניות הקבוצתית**של כלי מנהל השרת.</span><span class="sxs-lookup"><span data-stu-id="29861-152">Log on to AD server, search and open **Server Manager** > **Tools** > **Group Policy Management**.</span></span>
2.  <span data-ttu-id="29861-153">בחר את שם התחום שלך תחת **קבוצות מחשבים** ולחץ לחיצה ימנית על **אובייקטי מדיניות קבוצתית** כדי לבחור **חדש**.</span><span class="sxs-lookup"><span data-stu-id="29861-153">Select your domain name under **Domains** and right-click **Group Policy Objects** to select **New**.</span></span>
3.  <span data-ttu-id="29861-154">תן לאובייקט הGPO החדש שם, לדוגמה "*Cloud_Enrollment*" ולאחר מכן בחר **באפשרות אישור**.</span><span class="sxs-lookup"><span data-stu-id="29861-154">Give the new GPO an name, for example “*Cloud_Enrollment*” and then select **OK**.</span></span>
4.  <span data-ttu-id="29861-155">לחץ לחיצה ימנית על אובייקט ה-GPO החדש תחת **אובייקטי מדיניות קבוצתית** ובחר בפקודה **עריכה**.</span><span class="sxs-lookup"><span data-stu-id="29861-155">Right-click the new GPO under **Group Policy Objects** and select **Edit**.</span></span>
5.  <span data-ttu-id="29861-156">בעורך **ניהול המדיניות הקבוצתית**, עבור אל פריטי מדיניות **תצורת המחשב**  >  **Policies**  >  **תבניות ניהול**  >  **של Windows רכיבי**  >  **MDM**.</span><span class="sxs-lookup"><span data-stu-id="29861-156">In the **Group Policy Management Editor**, go to **Computer Configuration** > **Policies** > **Administrative Templates** > **Windows Components** > **MDM**.</span></span>
6. <span data-ttu-id="29861-157">לחץ באמצעות לחצן העכבר הימני **הפעל הרשמה אוטומטית של MDM באמצעות אישורי התכלת לספירה** ולאחר מכן בחר **Enabled**  >  **באישור**זמין.</span><span class="sxs-lookup"><span data-stu-id="29861-157">Right-click **Enable automatic MDM enrollment using default Azure AD credentials** and then select **Enabled** > **OK**.</span></span> <span data-ttu-id="29861-158">סגור את חלון העורך.</span><span class="sxs-lookup"><span data-stu-id="29861-158">Close the editor window.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="29861-159">אם אינך רואה שהמדיניות **מאפשרת הרשמה אוטומטית של MDM המשתמשת באישורי תכלת לספירה**, ראה [קבלת תבניות הניהול העדכניות](#get-the-latest-administrative-templates)ביותר.</span><span class="sxs-lookup"><span data-stu-id="29861-159">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, see [Get the latest Administrative Templates](#get-the-latest-administrative-templates).</span></span>

## <a name="6-deploy-the-group-policy"></a><span data-ttu-id="29861-160">6. פריסת מדיניות קבוצתית</span><span class="sxs-lookup"><span data-stu-id="29861-160">6. Deploy the Group Policy</span></span>

1.  <span data-ttu-id="29861-161">במנהל השרת, תחת **קבוצות מחשבים** _ האובייקטים של מדיניות קבוצתית, בחר את ה-GPO משלב 3 לעיל, לדוגמה "Cloud_Enrollment".</span><span class="sxs-lookup"><span data-stu-id="29861-161">In the Server Manager, under **Domains** > Group Policy objects, select the GPO from Step 3 above, for example “Cloud_Enrollment”.</span></span>
2.  <span data-ttu-id="29861-162">בחר בכרטיסיה **טווח** עבור ה-GPO שלך.</span><span class="sxs-lookup"><span data-stu-id="29861-162">Select the **Scope** tab for your GPO.</span></span>
3.  <span data-ttu-id="29861-163">בכרטיסיה טווח של GPO, לחץ לחיצה ימנית על הקישור לתחום תחת **קישורים**.</span><span class="sxs-lookup"><span data-stu-id="29861-163">In the GPO’s Scope tab, right-click the link to the domain under **Links**.</span></span>
4.  <span data-ttu-id="29861-164">בחר באפשרות ' **נאכף** ' כדי לפרוס את ה-GPO ולאחר מכן **אישור** במסך האישור.</span><span class="sxs-lookup"><span data-stu-id="29861-164">Select **Enforced** to deploy the GPO and then **OK** in the confirmation screen.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="29861-165">קבל את התבניות המנהליות העדכניות ביותר</span><span class="sxs-lookup"><span data-stu-id="29861-165">Get the latest Administrative Templates</span></span>

<span data-ttu-id="29861-166">אם אינך רואה שהמדיניות **מאפשרת הרשמה אוטומטית של MDM המשתמשת באישורי תכלת לספירה**, ייתכן שהסיבה לכך היא שאין ברשותך את ה-admx המותקנת עבור Windows 10, גירסה 1803, גירסה 1809 או גירסה 1903.</span><span class="sxs-lookup"><span data-stu-id="29861-166">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="29861-167">כדי לפתור את הבעיה, בצע את הפעולות הבאות (הערה: MDM. admx האחרון תואם לאחור):</span><span class="sxs-lookup"><span data-stu-id="29861-167">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="29861-168">[להוריד: תבניות מנהליות (. admx) עבור Windows 10 מאי 2019 עדכון (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="29861-168">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="29861-169">התקן את החבילה בבקר התחום הראשי (PDC).</span><span class="sxs-lookup"><span data-stu-id="29861-169">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="29861-170">ניווט, בהתאם לגירסה לתיקיה: **C:\templletccome\n מיקרוסופט/Windows 10 May 2019 עדכון (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="29861-170">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="29861-171">שנה את שם התיקיה **הגדרות מדיניות** בנתיב שלעיל **להגדרות**המדיניות.</span><span class="sxs-lookup"><span data-stu-id="29861-171">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="29861-172">העתק את התיקיה ' **הגדרות** מדיניות ' ל- **C:\windows\so\t\uspe\n**.</span><span class="sxs-lookup"><span data-stu-id="29861-172">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="29861-173">אם בכוונתך להשתמש במאגר מדיניות מרכזי עבור כל התחום שלך, הוסף את תוכן המדיניות המבוטח.</span><span class="sxs-lookup"><span data-stu-id="29861-173">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="29861-174">הפעל מחדש את בקר קבוצת המחשבים הראשי כדי שהמדיניות תהיה זמינה.</span><span class="sxs-lookup"><span data-stu-id="29861-174">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="29861-175">הליך זה יפעל גם עבור כל גירסה עתידית.</span><span class="sxs-lookup"><span data-stu-id="29861-175">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="29861-176">בשלב זה אתה אמור להיות מסוגל לראות את המדיניות **לאפשר הרשמה אוטומטית MDM באמצעות ברירת המחדל של הודעות תכלת לספירה** זמין.</span><span class="sxs-lookup"><span data-stu-id="29861-176">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

