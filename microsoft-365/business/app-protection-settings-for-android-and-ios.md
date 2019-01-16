---
title: קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: למד כיצד ליצור, לערוך, או למחוק מדיניות ניהול app ולהגן על קבצי עבודה במכשירים Android או iOS.
ms.openlocfilehash: ed03227496120369b94bf2396974eebfd7798678
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983664"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="b8c51-103">קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS</span><span class="sxs-lookup"><span data-stu-id="b8c51-103">Set app protection settings for Android or iOS devices</span></span>

## <a name="create-an-app-management-policy"></a><span data-ttu-id="b8c51-104">יצירת מדיניות לניהול יישומים</span><span class="sxs-lookup"><span data-stu-id="b8c51-104">Create an app management policy</span></span>

1. <span data-ttu-id="b8c51-105">היכנס ל- [Microsoft 365 Business](https://portal.office.com) עם אישורים של מנהל מערכת כללי.</span><span class="sxs-lookup"><span data-stu-id="b8c51-105">Sign in to [Microsoft 365 Business](https://portal.office.com) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="b8c51-106">במרכז הניהול, בכרטיס **כללי מדיניות של מכשיר**, בחר **הוסף מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="b8c51-106">In the admin center, on the **Device policies** card, choose **Add policy**.</span></span>
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. <span data-ttu-id="b8c51-108">בחלונית **הוסף מדיניות**, הזן שם ייחודי עבור מדיניות זו.</span><span class="sxs-lookup"><span data-stu-id="b8c51-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="b8c51-109">תחת **סוג מדיניות**, בחר **ניהול אפליקציות עבור Android** או **ניהול אפליקציות עבור iOS** בהתאם לערכת כללי המדיניות שברצונך ליצור.</span><span class="sxs-lookup"><span data-stu-id="b8c51-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS** depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="b8c51-p101">הרחב את **הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים** ואת **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים** \> קבע את תצורת ההגדרות כפי שאתה רוצה. האפשרות **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים** **מבוטלת** כברירת מחדל, אך מומלץ להגדיר אותה למצב **מופעל** ולקבל את ערכי ברירת המחדל. ראה [הגדרות זמינות](app-protection-settings-for-android-and-ios.md#bkmk_availablesettings) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="b8c51-p101">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like. The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. See [Available settings](app-protection-settings-for-android-and-ios.md#bkmk_availablesettings) for more information.</span></span> 
    
    <span data-ttu-id="b8c51-113">ניתן להשתמש תמיד בקישור **איפוס הגדרות ברירת מחדל** כדי לחזור להגדרת ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="b8c51-113">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="b8c51-p102">לאחר מכן החלט **מי יקבל הגדרות אלה?** אם אינך מעוניין להשתמש בקבוצת האבטחה המוגדרת כברירת מחדל **כל המשתמשים**, בחר **שינוי**, בחר את קבוצות האבטחה שיקבלו הגדרות אלה \> **בחר**.</span><span class="sxs-lookup"><span data-stu-id="b8c51-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="b8c51-117">לבסוף, בחר **סיום** כדי לשמור את המדיניות והקצה אותה למכשירים.</span><span class="sxs-lookup"><span data-stu-id="b8c51-117">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="b8c51-118">עריכת מדיניות לניהול יישומים</span><span class="sxs-lookup"><span data-stu-id="b8c51-118">Edit an app management policy</span></span>

1. <span data-ttu-id="b8c51-119">בכרטיס **מדיניות** , בחרו ' **עריכת מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="b8c51-119">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="b8c51-120">בחלונית **ערוך מדיניות**, בחר את המדיניות שברצונך לשנות</span><span class="sxs-lookup"><span data-stu-id="b8c51-120">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="b8c51-p103">בחר **ערוך** לצד כל הגדרה כדי לשנות את הערכים במדיניות. בעת שינוי ערך, הוא נשמר באופן אוטומטי במדיניות</span><span class="sxs-lookup"><span data-stu-id="b8c51-p103">Choose **Edit** next to each setting to change the values in the policy. When you change a value, it is automatically saved into the policy</span></span> 
    
4. <span data-ttu-id="b8c51-123">לאחר שתסיים, סגור את החלונית **ערוך מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="b8c51-123">When you are finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="b8c51-124">מחיקת מדיניות לניהול יישומים</span><span class="sxs-lookup"><span data-stu-id="b8c51-124">Delete an app management policy</span></span>

1. <span data-ttu-id="b8c51-125">בכרטיס **פריטי מדיניות**, בחר **מחק מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="b8c51-125">On the **Policies** card, choose **Delete policy**.</span></span>
    
2. <span data-ttu-id="b8c51-126">בחלונית **מחק מדיניות**, בחר את פריטי המדיניות שברצונך למחוק \> **בחר**, לאחר מכן **אשר** כדי למחוק את המדיניות או פריטי המדיניות שבחרת.</span><span class="sxs-lookup"><span data-stu-id="b8c51-126">On the **Delete policy** pane, choose the policies you want to delete \> **Select**, then **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="b8c51-127">הגדרות זמינות</span><span class="sxs-lookup"><span data-stu-id="b8c51-127">Available settings</span></span>

<span data-ttu-id="b8c51-128">הטבלאות הבאות מספקות מידע מפורט אודות ההגדרות הזמינות כדי להגן על קבצי עבודה במכשירים וההגדרות הקובעות כיצד משתמשים ניגשים לקבצי Office מהמכשירים הניידים שלהם.</span><span class="sxs-lookup"><span data-stu-id="b8c51-128">The following tables give detailed information about the available settings to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="b8c51-129">ראה [כיצד תכונות ההגנה של Microsoft 365 Business ממפות להגדרות Intune](map-protection-features-to-intune-settings.md) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="b8c51-129">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="b8c51-130">הגדרות להגנה על קבצי עבודה</span><span class="sxs-lookup"><span data-stu-id="b8c51-130">Settings that protect work files</span></span>

<span data-ttu-id="b8c51-131">ההגדרות הבאות זמינות כדי להגן על קבצי עבודה במקרה אובדן או גניבה של מכשיר משתמש:</span><span class="sxs-lookup"><span data-stu-id="b8c51-131">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="b8c51-132">הגדרה</span><span class="sxs-lookup"><span data-stu-id="b8c51-132">Setting</span></span>  <br/> |<span data-ttu-id="b8c51-133">תיאור</span><span class="sxs-lookup"><span data-stu-id="b8c51-133">Description</span></span>  <br/> |
|<span data-ttu-id="b8c51-134">מחק קבצי עבודה ממכשיר לא פעיל לאחר</span><span class="sxs-lookup"><span data-stu-id="b8c51-134">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="b8c51-135">אם לא נעשה שימוש במכשיר במשך מספר הימים שאתה מציין כאן, כל קבצי העבודה המאוחסנים במכשיר יימחקו באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="b8c51-135">If a device is not used for the number of days that you specify here, any work files stored on the device will automatically be deleted.</span></span>  <br/> |
|<span data-ttu-id="b8c51-136">כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="b8c51-136">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="b8c51-137">אם הגדרה זו מוגדרת למצב **מופעל**, מיקום השמירה הזמין היחיד לקבצי העבודה יהיה OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="b8c51-137">If this setting is **On**, the only available save location for work files will be OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="b8c51-138">הצפן קבצי עבודה</span><span class="sxs-lookup"><span data-stu-id="b8c51-138">Encrypt work files</span></span>  <br/> |<span data-ttu-id="b8c51-p104">השאר הגדרה זו במצב **מופעל** כך שקבצי העבודה יהיו מוגנים על-ידי הצפנה. גם אם המכשיר אובד או נגנב, אף אחד לא יוכל לקרוא את נתוני החברה שלך.  </span><span class="sxs-lookup"><span data-stu-id="b8c51-p104">Keep this setting **On** so that work files are protected by encryption. Even if the device is lost or stolen, no one will be able to read your company data.  </span></span><br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="b8c51-141">הגדרות שקובעות כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים</span><span class="sxs-lookup"><span data-stu-id="b8c51-141">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="b8c51-142">ההגדרות הבאות זמינות לניהול אופן הגישה של משתמשים לקבצי עבודה של Office:</span><span class="sxs-lookup"><span data-stu-id="b8c51-142">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="b8c51-143">הגדרה</span><span class="sxs-lookup"><span data-stu-id="b8c51-143">Setting</span></span>  <br/> |<span data-ttu-id="b8c51-144">תיאור</span><span class="sxs-lookup"><span data-stu-id="b8c51-144">Description</span></span>  <br/> |
|<span data-ttu-id="b8c51-145">דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office</span><span class="sxs-lookup"><span data-stu-id="b8c51-145">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="b8c51-146">אם הגדרה זו נקבעה למצב **מופעל**, על המשתמשים לספק צורה אחרת של אימות, בנוסף לשם המשתמש והסיסמה שלהם, כדי שיוכלו להשתמש ביישומי Office במכשיר הנייד שלהם.</span><span class="sxs-lookup"><span data-stu-id="b8c51-146">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="b8c51-147">אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה</span><span class="sxs-lookup"><span data-stu-id="b8c51-147">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="b8c51-148">כדי למנוע ממשתמש לא מורשה לנחש באופן אקראי קוד PIN, הקוד יאופס לאחר מספר כניסות שגויות שאתה תציין.</span><span class="sxs-lookup"><span data-stu-id="b8c51-148">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="b8c51-149">דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך</span><span class="sxs-lookup"><span data-stu-id="b8c51-149">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="b8c51-150">הגדרה זו קובעת את משך הזמן שבו משתמש יכול להיות לא פעיל לפני שהוא מתבקש להיכנס שוב.</span><span class="sxs-lookup"><span data-stu-id="b8c51-150">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="b8c51-151">מנע גישה לקבצי עבודה במכשירים שנפרצו או שבוצעה בהם פעולת ROOT</span><span class="sxs-lookup"><span data-stu-id="b8c51-151">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="b8c51-p105">ייתכן מצב שבו משתמשים מתוחכמים יחזיקו במכשיר שנפרץ או שבוצעה בו פעולת ROOT. כלומר, המשתמש יכול לשנות את מערכת ההפעלה, עובדה שחושפת את המכשיר לתוכנות זדוניות. מכשירים אלה נחסמים כאשר ההגדרה מוגדרת למצב **פעיל**.  </span><span class="sxs-lookup"><span data-stu-id="b8c51-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="b8c51-155">אפשר למשתמשים להעתיק תוכן מאפליקציות Office לאפליקציות אישיות</span><span class="sxs-lookup"><span data-stu-id="b8c51-155">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="b8c51-p106">אנו מאפשרים זאת כברירת מחדל, אך אם **ההגדרה מופעלת,** המשתמש יוכל להעתיק מידע בקובץ העבודה לקובץ אישי. אם ההגדרה אינה **פעילה**, למשתמש לא תהיה אפשרות להעתיק מידע מחשבון עבודה לתוך app אישי או חשבון אישי.</span><span class="sxs-lookup"><span data-stu-id="b8c51-p106">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file. If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.  </span></span><br/> |
   

  

