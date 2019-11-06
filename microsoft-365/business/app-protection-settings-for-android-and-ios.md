---
title: קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: למד כיצד ליצור, לערוך או למחוק מדיניות ניהול יישומים ולהגן על קבצי עבודה בהתקני Android או iOS.
ms.openlocfilehash: 914e6848ac46eb334516aadff2827da2b83a38c4
ms.sourcegitcommit: 0fa897d06b664c0ed005817752da1426d4ee17cb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/06/2019
ms.locfileid: "38002084"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="33dd7-103">קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS</span><span class="sxs-lookup"><span data-stu-id="33dd7-103">Set app protection settings for Android or iOS devices</span></span>

![. באנר שיצביע על https://aka.ms/aboutM365previewכך](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a><span data-ttu-id="33dd7-105">יצירת מדיניות לניהול יישומים</span><span class="sxs-lookup"><span data-stu-id="33dd7-105">Create an app management policy</span></span>

1. <span data-ttu-id="33dd7-106"><a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. לך למרכז המנהלה</span><span class="sxs-lookup"><span data-stu-id="33dd7-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="33dd7-107">בניווט השמאלי, בחר באפשרות **מדיניות** \> \*\*\*\* **התקנים** \> .</span><span class="sxs-lookup"><span data-stu-id="33dd7-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="33dd7-108">בחלונית **הוסף מדיניות**, הזן שם ייחודי עבור מדיניות זו.</span><span class="sxs-lookup"><span data-stu-id="33dd7-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="33dd7-109">תחת **סוג מדיניות**, בחר **ניהול אפליקציות עבור Android** או **ניהול אפליקציות עבור iOS** בהתאם לערכת כללי המדיניות שברצונך ליצור.</span><span class="sxs-lookup"><span data-stu-id="33dd7-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS** depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="33dd7-110">הרחב את **הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים** ואת **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים** \> קבע את תצורת ההגדרות כפי שאתה רוצה.</span><span class="sxs-lookup"><span data-stu-id="33dd7-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span></span> <span data-ttu-id="33dd7-111">האפשרות **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים** **מבוטלת** כברירת מחדל, אך מומלץ להגדיר אותה למצב **מופעל** ולקבל את ערכי ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="33dd7-111">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="33dd7-112">לקבלת מידע נוסף, ראה [הגדרות זמינות](#available-settings) .</span><span class="sxs-lookup"><span data-stu-id="33dd7-112">See [Available settings](#available-settings)  for more information.</span></span> 
    
    <span data-ttu-id="33dd7-113">ניתן להשתמש תמיד בקישור **איפוס הגדרות ברירת מחדל** כדי לחזור להגדרת ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="33dd7-113">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="33dd7-p102">לאחר מכן החלט **מי יקבל הגדרות אלה?** אם אינך מעוניין להשתמש בקבוצת האבטחה המוגדרת כברירת מחדל **כל המשתמשים**, בחר **שינוי**, בחר את קבוצות האבטחה שיקבלו הגדרות אלה \> **בחר**.</span><span class="sxs-lookup"><span data-stu-id="33dd7-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="33dd7-117">לבסוף, בחר **סיום** כדי לשמור את המדיניות והקצה אותה למכשירים.</span><span class="sxs-lookup"><span data-stu-id="33dd7-117">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="33dd7-118">עריכת מדיניות לניהול יישומים</span><span class="sxs-lookup"><span data-stu-id="33dd7-118">Edit an app management policy</span></span>

1. <span data-ttu-id="33dd7-119">בכרטיס **המדיניות** , בחר **מדיניות עריכה**.</span><span class="sxs-lookup"><span data-stu-id="33dd7-119">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="33dd7-120">בחלונית **ערוך מדיניות**, בחר את המדיניות שברצונך לשנות</span><span class="sxs-lookup"><span data-stu-id="33dd7-120">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="33dd7-p103">בחר **ערוך** לצד כל הגדרה כדי לשנות את הערכים במדיניות. בעת שינוי ערך, הוא נשמר באופן אוטומטי במדיניות</span><span class="sxs-lookup"><span data-stu-id="33dd7-p103">Choose **Edit** next to each setting to change the values in the policy. When you change a value, it is automatically saved into the policy</span></span> 
    
4. <span data-ttu-id="33dd7-123">לאחר שתסיים, סגור את החלונית **ערוך מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="33dd7-123">When you are finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="33dd7-124">מחיקת מדיניות לניהול יישומים</span><span class="sxs-lookup"><span data-stu-id="33dd7-124">Delete an app management policy</span></span>

1. <span data-ttu-id="33dd7-125">בדף ' **פריטי מדיניות** ', בחר מדיניות ולאחר מכן **מחק**.</span><span class="sxs-lookup"><span data-stu-id="33dd7-125">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="33dd7-126">בחלונית **המדיניות מחק** בחר **באישור** כדי למחוק את המדיניות או את פריטי המדיניות שבחרת.</span><span class="sxs-lookup"><span data-stu-id="33dd7-126">On the **Delete policy** pane choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="33dd7-127">הגדרות זמינות</span><span class="sxs-lookup"><span data-stu-id="33dd7-127">Available settings</span></span>

<span data-ttu-id="33dd7-128">הטבלאות הבאות מאפשרות מידע מפורט אודות הגדרות הזמינות להגנה על קבצי עבודה בהתקנים ועל ההגדרות השולטות באופן שבו משתמשים ניגשים לקבצי Office מההתקנים הניידים שלהם.</span><span class="sxs-lookup"><span data-stu-id="33dd7-128">The following tables give detailed information about settings available to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="33dd7-129">ראה [כיצד תכונות ההגנה של Microsoft 365 Business ממפות להגדרות Intune](map-protection-features-to-intune-settings.md) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="33dd7-129">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="33dd7-130">הגדרות להגנה על קבצי עבודה</span><span class="sxs-lookup"><span data-stu-id="33dd7-130">Settings that protect work files</span></span>

<span data-ttu-id="33dd7-131">ההגדרות הבאות זמינות כדי להגן על קבצי עבודה במקרה אובדן או גניבה של מכשיר משתמש:</span><span class="sxs-lookup"><span data-stu-id="33dd7-131">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="33dd7-132">הגדרה</span><span class="sxs-lookup"><span data-stu-id="33dd7-132">Setting</span></span>  <br/> |<span data-ttu-id="33dd7-133">תיאור</span><span class="sxs-lookup"><span data-stu-id="33dd7-133">Description</span></span>  <br/> |
|<span data-ttu-id="33dd7-134">מחק קבצי עבודה ממכשיר לא פעיל לאחר מספר הימים הבא</span><span class="sxs-lookup"><span data-stu-id="33dd7-134">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="33dd7-135">אם לא נעשה שימוש במכשיר במשך מספר הימים שאתה מציין כאן, כל קבצי העבודה המאוחסנים במכשיר יימחקו באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="33dd7-135">If a device is not used for the number of days that you specify here, any work files stored on the device will automatically be deleted.</span></span>  <br/> |
|<span data-ttu-id="33dd7-136">אלץ משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="33dd7-136">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="33dd7-137">אם הגדרה זו מוגדרת למצב **פעיל**, מיקום השמירה הזמין היחיד לקבצי העבודה יהיה OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="33dd7-137">If this setting is **On**, the only available save location for work files will be OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="33dd7-138">הצפן קבצי עבודה</span><span class="sxs-lookup"><span data-stu-id="33dd7-138">Encrypt work files</span></span>  <br/> |<span data-ttu-id="33dd7-p104">השאר הגדרה זו במצב **פעיל** כך שקבצי העבודה יהיו מוגנים על-ידי הצפנה. גם אם המכשיר אובד או נגנב, אף אחד לא יוכל לקרוא את נתוני החברה שלך.  </span><span class="sxs-lookup"><span data-stu-id="33dd7-p104">Keep this setting **On** so that work files are protected by encryption. Even if the device is lost or stolen, no one will be able to read your company data.  </span></span><br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="33dd7-141">הגדרות שקובעות כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים</span><span class="sxs-lookup"><span data-stu-id="33dd7-141">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="33dd7-142">ההגדרות הבאות זמינות לניהול אופן הגישה של משתמשים לקבצי עבודה של Office:</span><span class="sxs-lookup"><span data-stu-id="33dd7-142">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="33dd7-143">הגדרה</span><span class="sxs-lookup"><span data-stu-id="33dd7-143">Setting</span></span>  <br/> |<span data-ttu-id="33dd7-144">תיאור</span><span class="sxs-lookup"><span data-stu-id="33dd7-144">Description</span></span>  <br/> |
|<span data-ttu-id="33dd7-145">דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office</span><span class="sxs-lookup"><span data-stu-id="33dd7-145">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="33dd7-146">אם הגדרה זו נקבעה למצב **מופעל**, על המשתמשים לספק צורה אחרת של אימות, בנוסף לשם המשתמש והסיסמה שלהם, כדי שיוכלו להשתמש ביישומי Office במכשיר הנייד שלהם.</span><span class="sxs-lookup"><span data-stu-id="33dd7-146">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="33dd7-147">אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה</span><span class="sxs-lookup"><span data-stu-id="33dd7-147">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="33dd7-148">כדי למנוע ממשתמש לא מורשה לנחש באופן אקראי קוד PIN, הקוד יאופס לאחר מספר כניסות שגויות שאתה תציין.</span><span class="sxs-lookup"><span data-stu-id="33dd7-148">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="33dd7-149">דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך</span><span class="sxs-lookup"><span data-stu-id="33dd7-149">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="33dd7-150">הגדרה זו קובעת את משך הזמן שבו משתמש יכול להיות לא פעיל לפני שהוא מתבקש להיכנס שוב.</span><span class="sxs-lookup"><span data-stu-id="33dd7-150">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="33dd7-151">מנע גישה לקבצי עבודה במכשירים שנפרצו או שבוצעה בהם פעולת ROOT</span><span class="sxs-lookup"><span data-stu-id="33dd7-151">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="33dd7-p105">ייתכן מצב שבו משתמשים מתוחכמים יחזיקו במכשיר שנפרץ או שבוצעה בו פעולת ROOT. כלומר, המשתמש יכול לשנות את מערכת ההפעלה, עובדה שחושפת את המכשיר לתוכנות זדוניות. מכשירים אלה נחסמים כאשר ההגדרה מוגדרת למצב **פעיל**.  </span><span class="sxs-lookup"><span data-stu-id="33dd7-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="33dd7-155">אפשר למשתמשים להעתיק תוכן מאפליקציות Office לאפליקציות אישיות</span><span class="sxs-lookup"><span data-stu-id="33dd7-155">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="33dd7-156">אנחנו מאפשרים זאת כברירת מחדל, אך אם ההגדרה **מופעלת**, המשתמש יכול להעתיק מידע בקובץ עבודה לקובץ אישי.</span><span class="sxs-lookup"><span data-stu-id="33dd7-156">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="33dd7-157">אם ההגדרה **מבוטלת**, למשתמש אין אפשרות להעתיק מידע מקובץ עבודה לאפליקציה אישית או לחשבון אישי.</span><span class="sxs-lookup"><span data-stu-id="33dd7-157">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
   

  

