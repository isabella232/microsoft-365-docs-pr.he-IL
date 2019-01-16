---
title: אמת את הגדרות ההגנה app במכשירים Android או iOS
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: 'Learn how to validate the Microsoft 365 Business app protection settings in your Android or iOS devices.  '
ms.openlocfilehash: 300f59e81a93cc3dfc03fd1d98891be1ac4f7795
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983674"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="c4363-103">אמת את הגדרות ההגנה app במכשירים Android או iOS</span><span class="sxs-lookup"><span data-stu-id="c4363-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="c4363-104">בצע את ההוראות המופיעות בכרטיסיות כדי לאמת הגדרות הגנה app במכשירים Android או iOS.</span><span class="sxs-lookup"><span data-stu-id="c4363-104">Follow the instructions in the tabs to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="androidtab"></a>[<span data-ttu-id="c4363-105">Android</span><span class="sxs-lookup"><span data-stu-id="c4363-105">Android</span></span>](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="c4363-106">בדיקה שהגדרות הגנה על יישומים פועלות במכשירי המשתמשים</span><span class="sxs-lookup"><span data-stu-id="c4363-106">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="c4363-107">לאחר [קביעת תצורות של יישומים עבור מכשירי Android](app-protection-settings-for-android-and-ios.md) כדי להגן על יישומים, ניתן לבצע את השלבים הבאים כדי לאמת שההגדרות שבחרת פועלות.</span><span class="sxs-lookup"><span data-stu-id="c4363-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="c4363-108">תחילה, ודא שהמדיניות חלה על היישום שבו אתה עומד לאמת אותה.</span><span class="sxs-lookup"><span data-stu-id="c4363-108">First, make sure that the policy applies to the app in which you are going to validate it.</span></span>
  
1. <span data-ttu-id="c4363-109">ב[מרכז הניהול](https://portal.office.com) של Microsoft 365 Business, עבור אל **פריטי מדיניות** \> **ערוך מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="c4363-109">In the Microsoft 365 Business [admin center](https://portal.office.com) go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="c4363-110">בחר **מדיניות יישום עבור Android** עבור ההגדרות שיצרת בעת ההתקנה, או מדיניות אחרת שיצרת, וודא שהיא נאכפת עבור Outlook לדוגמה.</span><span class="sxs-lookup"><span data-stu-id="c4363-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it is enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="c4363-112">אימות של 'דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office'</span><span class="sxs-lookup"><span data-stu-id="c4363-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="c4363-113">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **בקרת גישה למסמכי Office**, הרחב את **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים**, וודא שהאפשרות **דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office** מוגדרת ל **מופעל**.</span><span class="sxs-lookup"><span data-stu-id="c4363-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="c4363-115">במכשיר ה- Android של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="c4363-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="c4363-116">תתבקש גם להזין מספר זיהוי אישי או להשתמש בטביעת אצבע.</span><span class="sxs-lookup"><span data-stu-id="c4363-116">You will also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="c4363-118">אימות של 'אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה'</span><span class="sxs-lookup"><span data-stu-id="c4363-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="c4363-119">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **בקרת גישה למסמכי Office**, הרחב את **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים**, וודא שהאפשרות **אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה** מוגדרת למספר כלשהו - המספר מוגדר ל- 5 כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="c4363-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number - this is 5 by default.</span></span> 
  
1. <span data-ttu-id="c4363-120">במכשיר ה- Android של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="c4363-120">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="c4363-p101">הזן מספר זיהוי אישי שגוי כמספר הפעמים שצוין על-ידי המדיניות. תראה הודעה המציינת **הגעת למגבלת נסיונות מספר הזיהוי האישי** כדי לאפס את קוד ה- PIN.</span><span class="sxs-lookup"><span data-stu-id="c4363-p101">Enter an incorrect PIN as many times as specified by the policy. You will see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="c4363-p102">לחץ על **איפוס מספר זיהוי אישי**. תתבקש להיכנס עם אישורי Microsoft 365 Business של המשתמש ולאחר מכן תידרש להגדיר מספר זיהוי אישי חדש.</span><span class="sxs-lookup"><span data-stu-id="c4363-p102">Press **Reset PIN**. You will be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="c4363-126">אימות של 'כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business'</span><span class="sxs-lookup"><span data-stu-id="c4363-126">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="c4363-127">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **הגנה מפני מכשירים שאבדו או נגנבו**, הרחב את **הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים**, וודא שהאפשרות **כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business** מוגדרת ל **מופעל**.</span><span class="sxs-lookup"><span data-stu-id="c4363-127">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="c4363-129">במכשיר ה- Android של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש והזן מספר זיהוי אישי במידת הצורך.</span><span class="sxs-lookup"><span data-stu-id="c4363-129">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="c4363-130">פתח הודעת דואר אלקטרוני המכילה קובץ מצורף והקש על סמל החץ למטה לצד המידע אודות הקובץ המצורף.</span><span class="sxs-lookup"><span data-stu-id="c4363-130">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="c4363-132">תראה **אין אפשרות לשמור במכשיר** בתחתית המסך.</span><span class="sxs-lookup"><span data-stu-id="c4363-132">You will see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="c4363-134">[!הערה] שמירה ב- OneDrive for Business אינה זמינה עבור Android בשלב זה, לכן תוכל לראות רק ששמירה מקומית נחסמת.</span><span class="sxs-lookup"><span data-stu-id="c4363-134">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="c4363-135">אימות של 'דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך'</span><span class="sxs-lookup"><span data-stu-id="c4363-135">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="c4363-136">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **בקרת גישה למסמכי Office**, הרחב את **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים**, וודא שהאפשרות **דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך** מוגדרת למספר דקות כלשהו - המספר מוגדר ל- 30 דקות כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="c4363-136">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes - this is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="c4363-137">במכשיר ה- Android של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש והזן מספר זיהוי אישי במידת הצורך.</span><span class="sxs-lookup"><span data-stu-id="c4363-137">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="c4363-p103">כעת אתה אמור לראות את תיבת הדואר הנכנס של Outlook. הנח למכשיר ה- Android ואל תיגע בו במשך 30 דקות לפחות (או פרק זמן אחר, ארוך יותר מזה שצוין במדיניות). סביר להניח שהמכשיר יהפוך למעומעם.</span><span class="sxs-lookup"><span data-stu-id="c4363-p103">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="c4363-141">גש מחדש ל- Outlook במכשיר ה- Android.</span><span class="sxs-lookup"><span data-stu-id="c4363-141">Re-access Outlook on the Android device.</span></span>
    
4. <span data-ttu-id="c4363-142">תתבקש להזין את מספר הזיהוי האישי שלך לפני שתוכל לגשת ל- Outlook שוב.</span><span class="sxs-lookup"><span data-stu-id="c4363-142">You will be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="c4363-143">אימות של 'הגן על קבצי עבודה באמצעות הצפנה'</span><span class="sxs-lookup"><span data-stu-id="c4363-143">Validate Protect work files with encryption</span></span>

<span data-ttu-id="c4363-144">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **הגנה מפני מכשירים שאבדו או נגנבו**, הרחב את **הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים**, וודא שהאפשרות **הגן על קבצי עבודה באמצעות הצפנה** מוגדרת ל **מופעל** והאפשרות **כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business** מוגדרת ל **מבוטל**.</span><span class="sxs-lookup"><span data-stu-id="c4363-144">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="c4363-145">במכשיר ה- Android של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש והזן מספר זיהוי אישי במידת הצורך.</span><span class="sxs-lookup"><span data-stu-id="c4363-145">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="c4363-146">פתח הודעת דואר אלקטרוני המכילה כמה קבצים מצורפים של תמונות.</span><span class="sxs-lookup"><span data-stu-id="c4363-146">Open an email which contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="c4363-147">הקש על סמל החץ למטה לצד מידע אודות הקובץ המצורף כדי לשמור אותו.</span><span class="sxs-lookup"><span data-stu-id="c4363-147">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="c4363-p104">ייתכן שתתבקש לאפשר ל- Outlook לגשת לתמונות, למדיה ולקבצים במכשיר שלך. הקש על **אפשר**.</span><span class="sxs-lookup"><span data-stu-id="c4363-p104">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="c4363-151">בחלק התחתון של המסך, בחר **שמור במכשיר** ולאחר מכן פתח את האפליקציה **גלריה**.</span><span class="sxs-lookup"><span data-stu-id="c4363-151">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="c4363-p105">אתה אמור לראות תמונה מוצפנת (או יותר, אם שמרת קבצים מצורפים מרובים של תמונות) ברשימה. היא עשויה להופיע ברשימת התמונות כריבוע אפור עם סימן קריאה לבן בתוך עיגול לבן, במרכז הריבוע האפור.</span><span class="sxs-lookup"><span data-stu-id="c4363-p105">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="iostab"></a>[<span data-ttu-id="c4363-155">iOS</span><span class="sxs-lookup"><span data-stu-id="c4363-155">iOS</span></span>](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="c4363-156">בדיקה שהגדרות הגנה על יישומים פועלות במכשירי המשתמשים</span><span class="sxs-lookup"><span data-stu-id="c4363-156">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="c4363-157">לאחר [קביעת תצורות של יישומים עבור מכשירי iOS](app-protection-settings-for-android-and-ios.md) כדי להגן על יישומים, ניתן לבצע את השלבים הבאים כדי לאמת שההגדרות שבחרת פועלות.</span><span class="sxs-lookup"><span data-stu-id="c4363-157">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="c4363-158">תחילה, ודא שהמדיניות חלה על היישום שבו אתה עומד לאמת אותה.</span><span class="sxs-lookup"><span data-stu-id="c4363-158">First, make sure that the policy applies to the app in which you are going to validate it.</span></span>
  
1. <span data-ttu-id="c4363-159">ב[מרכז הניהול](https://portal.office.com) של Microsoft 365 Business, עבור אל **פריטי מדיניות** \> **ערוך מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="c4363-159">In the Microsoft 365 Business [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="c4363-160">בחר **מדיניות יישום עבור iOS** עבור ההגדרות שיצרת בעת ההגדרה, או מדיניות אחרת שיצרת, וודא שהיא נאכפת עבור Outlook, לדוגמה:</span><span class="sxs-lookup"><span data-stu-id="c4363-160">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it is enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="c4363-162">אימות של 'דרוש מספר זיהוי אישי כדי לגשת ליישומי Office'</span><span class="sxs-lookup"><span data-stu-id="c4363-162">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="c4363-163">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **בקרת גישה למסמכי Office**, הרחב את **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים**, וודא שהאפשרות **דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office** מוגדרת ל **מופעל**.</span><span class="sxs-lookup"><span data-stu-id="c4363-163">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="c4363-165">במכשיר ה- iOS של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="c4363-165">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="c4363-166">תתבקש גם להזין מספר זיהוי אישי או להשתמש בטביעת אצבע.</span><span class="sxs-lookup"><span data-stu-id="c4363-166">You will also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="c4363-168">אימות של 'אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה'</span><span class="sxs-lookup"><span data-stu-id="c4363-168">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="c4363-169">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **בקרת גישה למסמכי Office**, הרחב את **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים**, וודא שהאפשרות **אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה** מוגדרת למספר כלשהו - המספר מוגדר ל- 5 כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="c4363-169">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number - this is 5 by default.</span></span> 
  
1. <span data-ttu-id="c4363-170">במכשיר ה- iOS של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="c4363-170">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="c4363-p106">הזן מספר זיהוי אישי שגוי כמספר הפעמים שצוין על-ידי המדיניות. תראה הודעה המציינת **הגעת למגבלת נסיונות מספר הזיהוי האישי** כדי לאפס את קוד ה- PIN.</span><span class="sxs-lookup"><span data-stu-id="c4363-p106">Enter an incorrect PIN as many times as specified by the policy. You will see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="c4363-p107">לחץ על **אישור**. תתבקש להיכנס עם אישורי Microsoft 365 Business של המשתמש ולאחר מכן תידרש להגדיר מספר זיהוי אישי חדש.</span><span class="sxs-lookup"><span data-stu-id="c4363-p107">Press **OK**. You will be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="c4363-176">אימות של 'כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business'</span><span class="sxs-lookup"><span data-stu-id="c4363-176">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="c4363-177">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **הגנה מפני מכשירים שאבדו או נגנבו**, הרחב את **הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים**, וודא שהאפשרות **כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business** מוגדרת ל **מופעל**.</span><span class="sxs-lookup"><span data-stu-id="c4363-177">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="c4363-179">במכשיר ה- iOS של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש והזן קוד זיהוי אישי במידת הצורך.</span><span class="sxs-lookup"><span data-stu-id="c4363-179">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="c4363-180">פתח הודעת דואר אלקטרוני המכילה קובץ מצורף, פתח את הקובץ המצורף ובחר **שמור** בתחתית המסך.</span><span class="sxs-lookup"><span data-stu-id="c4363-180">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="c4363-p108">אתה אמור לראות אפשרות רק עבור OneDrive for Business. אם לא, הקש על **הוספת חשבון** ובחר **OneDrive for Business** מתוך המסך **הוספת חשבון אחסון**. ספק את Microsoft 365 Business של משתמש הקצה כדי להיכנס כאשר תתבקש לעשות זאת.</span><span class="sxs-lookup"><span data-stu-id="c4363-p108">You should only see an option for OneDrive for Business. If not If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen. Provide the end user's Microsoft 365 Business to sign in when prompted.</span></span> 
    
    <span data-ttu-id="c4363-185">הקש על **שמור** ובחר **OneDrive for Business**.</span><span class="sxs-lookup"><span data-stu-id="c4363-185">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="c4363-186">אימות של 'דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך'</span><span class="sxs-lookup"><span data-stu-id="c4363-186">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="c4363-187">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **בקרת גישה למסמכי Office**, הרחב את **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים**, וודא שהאפשרות **דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך** מוגדרת למספר דקות כלשהו - המספר מוגדר ל- 30 דקות כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="c4363-187">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes - this is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="c4363-188">במכשיר ה- iOS של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש והזן קוד זיהוי אישי במידת הצורך.</span><span class="sxs-lookup"><span data-stu-id="c4363-188">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="c4363-p109">כעת אתה אמור לראות את תיבת הדואר הנכנס של Outlook. הנח למכשיר ה- iOS ואל תיגע בו במשך 30 דקות לפחות (או פרק זמן אחר, ארוך יותר מזה שצוין במדיניות). סביר להניח שהמכשיר יהפוך למעומעם.</span><span class="sxs-lookup"><span data-stu-id="c4363-p109">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="c4363-192">גש מחדש ל- Outlook במכשיר ה- iOS.</span><span class="sxs-lookup"><span data-stu-id="c4363-192">Re-access Outlook on the iOS device.</span></span>
    
4. <span data-ttu-id="c4363-193">תתבקש להזין את מספר הזיהוי האישי שלך לפני שתוכל לגשת ל- Outlook שוב.</span><span class="sxs-lookup"><span data-stu-id="c4363-193">You will be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="c4363-194">אימות של 'הגן על קבצי עבודה באמצעות הצפנה'</span><span class="sxs-lookup"><span data-stu-id="c4363-194">Validate Protect work files with encryption</span></span>

<span data-ttu-id="c4363-195">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **הגנה מפני מכשירים שאבדו או נגנבו**, הרחב את **הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים**, וודא שהאפשרות **הגן על קבצי עבודה באמצעות הצפנה** מוגדרת ל **מופעל** והאפשרות **כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business** מוגדרת ל **מבוטל**.</span><span class="sxs-lookup"><span data-stu-id="c4363-195">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="c4363-196">במכשיר ה- iOS של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש והזן קוד זיהוי אישי במידת הצורך.</span><span class="sxs-lookup"><span data-stu-id="c4363-196">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="c4363-197">פתח הודעת דואר אלקטרוני המכילה כמה קבצים מצורפים של תמונות.</span><span class="sxs-lookup"><span data-stu-id="c4363-197">Open an email which contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="c4363-198">הקש על הקובץ המצורף ולאחר מכן הקש על האפשרות **שמור** מתחתיו.</span><span class="sxs-lookup"><span data-stu-id="c4363-198">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="c4363-p110">פתח את היישום **תמונות** מתוך מסך הבית. אתה אמור לראות תמונה מוצפנת (או יותר, אם שמרת קבצים מצורפים מרובים של תמונות) שמורה, אך מוצפנת.</span><span class="sxs-lookup"><span data-stu-id="c4363-p110">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---

