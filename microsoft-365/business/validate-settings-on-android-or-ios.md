---
title: אימות הגדרות הגנה על יישומים במכשירי Android או iOS
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: למד כיצד לאמת את הגדרות ההגנה Microsoft 365 Business Premium אפליקציה במכשירי Android או iOS שלך.
ms.openlocfilehash: 43e74b548711550090021c39096b1647cee9e039
ms.sourcegitcommit: 0d1b065c94125b495e9886200f7918de3bda40b3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339329"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="26926-103">אימות הגדרות הגנה על יישומים במכשירי Android או iOS</span><span class="sxs-lookup"><span data-stu-id="26926-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="26926-104">בצע את ההוראות בסעיפים הבאים כדי לאמת הגדרות הגנה על אפליקציות במכשירי Android או iOS.</span><span class="sxs-lookup"><span data-stu-id="26926-104">Follow the instructions in the following sections to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="android"></a><span data-ttu-id="26926-105">Android</span><span class="sxs-lookup"><span data-stu-id="26926-105">Android</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="26926-106">ודא שהגדרות ההגנה על היישום פועלות במכשירי משתמש</span><span class="sxs-lookup"><span data-stu-id="26926-106">Check that the app protection settings are working on user devices</span></span>

<span data-ttu-id="26926-107">לאחר [קביעת תצורות של יישומים עבור מכשירי Android](app-protection-settings-for-android-and-ios.md) כדי להגן על יישומים, ניתן לבצע את השלבים הבאים כדי לאמת שההגדרות שבחרת פועלות.</span><span class="sxs-lookup"><span data-stu-id="26926-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="26926-108">תחילה, ודא שהמדיניות חלה על היישום שבו אתה עומד לאמת אותה.</span><span class="sxs-lookup"><span data-stu-id="26926-108">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="26926-109">במרכז Microsoft 365 Business Premium [,](https://admin.microsoft.com)עבור אל **מדיניות עריכת** \> **מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="26926-109">In the Microsoft 365 Business Premium [admin center](https://admin.microsoft.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="26926-110">בחר **מדיניות יישומים עבור Android** עבור ההגדרות שיצרת בהגדרה, או מדיניות אחרת שיצרת וודא שהיא נאכפת עבור Outlook, לדוגמה.</span><span class="sxs-lookup"><span data-stu-id="26926-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook, for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](../media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="26926-112">אימות של 'דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office'</span><span class="sxs-lookup"><span data-stu-id="26926-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="26926-113">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **בקרת גישה למסמכי Office**, הרחב את **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים**, וודא שהאפשרות **דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office** מוגדרת ל **מופעל**.</span><span class="sxs-lookup"><span data-stu-id="26926-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![ודא שה- דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת לאפליקציות Office מוגדרות ל'הפעלה'.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="26926-115">במכשיר Android של המשתמש, פתח Outlook והירשם באמצעות אישורי Microsoft 365 Business Premium המשתמש.</span><span class="sxs-lookup"><span data-stu-id="26926-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="26926-116">תתבקש גם להזין מספר זיהוי אישי או להשתמש בטביעת אצבע.</span><span class="sxs-lookup"><span data-stu-id="26926-116">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](../media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="26926-118">אימות של 'אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה'</span><span class="sxs-lookup"><span data-stu-id="26926-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="26926-119">בחלונית **עריכת מדיניות,** בחר ערוך לצד **פקד גישה של Office** מסמכים , הרחב את נהל את אופן הגישה של משתמשים  **לקבצי Office** במכשירים ניידים ולאחר מכן ודא כי איפוס **מספר** הזיהוי האישי לאחר מספר הניסיונות שנכשלו מוגדר למספר מסויים.</span><span class="sxs-lookup"><span data-stu-id="26926-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="26926-120">זהו 5 כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="26926-120">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="26926-121">במכשיר Android של המשתמש, פתח Outlook והירשם באמצעות אישורי Microsoft 365 Business Premium המשתמש.</span><span class="sxs-lookup"><span data-stu-id="26926-121">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="26926-122">הזן מספר זיהוי אישי שגוי כמספר הפעמים שצוין על-ידי המדיניות.</span><span class="sxs-lookup"><span data-stu-id="26926-122">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="26926-123">תראה בקשה לפיה מספר הזיהוי האישי הגיע **למגבלת הניסיון לאיפוס** מספר הזיהוי האישי.</span><span class="sxs-lookup"><span data-stu-id="26926-123">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="26926-125">לחץ על **איפוס מספר זיהוי אישי**.</span><span class="sxs-lookup"><span data-stu-id="26926-125">Press **Reset PIN**.</span></span> <span data-ttu-id="26926-126">תתבקש להיכנס באמצעות אישורי Microsoft 365 Business Premium של המשתמש ולאחר מכן תידרש להגדיר מספר זיהוי אישי חדש.</span><span class="sxs-lookup"><span data-stu-id="26926-126">You'll be prompted to sign in with the user's Microsoft 365 Business Premium credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="26926-127">אימות של 'כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business'</span><span class="sxs-lookup"><span data-stu-id="26926-127">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="26926-128">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **הגנה מפני מכשירים שאבדו או נגנבו**, הרחב את **הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים**, וודא שהאפשרות **כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business** מוגדרת ל **מופעל**.</span><span class="sxs-lookup"><span data-stu-id="26926-128">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="26926-130">במכשיר Android של המשתמש, פתח Outlook והיכנס באמצעות אישורי Microsoft 365 Business Premium המשתמש והזן מספר זיהוי אישי לפי התבקש.</span><span class="sxs-lookup"><span data-stu-id="26926-130">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="26926-131">פתח הודעת דואר אלקטרוני המכילה קובץ מצורף והקש על סמל החץ למטה לצד המידע אודות הקובץ המצורף.</span><span class="sxs-lookup"><span data-stu-id="26926-131">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](../media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="26926-133">תראה שאין **אפשרות לשמור במכשיר** בחלק התחתון של המסך.</span><span class="sxs-lookup"><span data-stu-id="26926-133">You'll see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](../media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="26926-135">[!הערה] שמירה ב- OneDrive for Business אינה זמינה עבור Android בשלב זה, לכן תוכל לראות רק ששמירה מקומית נחסמת.</span><span class="sxs-lookup"><span data-stu-id="26926-135">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="26926-136">אימות של 'דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך'</span><span class="sxs-lookup"><span data-stu-id="26926-136">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="26926-137">בחלונית **עריכת מדיניות,** בחר ערוך לצד **פקד גישה של Office** מסמכים , הרחב את נהל את אופן הגישה של משתמשים  **לקבצי Office** במכשירים ניידים, ודא שדרוש מהמשתמשים להיכנס שוב לאחר **שאפליקציות Office** לא היו פעילות במשך כמה דקות.</span><span class="sxs-lookup"><span data-stu-id="26926-137">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="26926-138">זהו 30 דקות כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="26926-138">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="26926-139">במכשיר Android של המשתמש, פתח Outlook והיכנס באמצעות אישורי Microsoft 365 Business Premium המשתמש והזן מספר זיהוי אישי לפי התבקש.</span><span class="sxs-lookup"><span data-stu-id="26926-139">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="26926-p105">כעת אתה אמור לראות את תיבת הדואר הנכנס של Outlook. הנח למכשיר ה- Android ואל תיגע בו במשך 30 דקות לפחות (או פרק זמן אחר, ארוך יותר מזה שצוין במדיניות). סביר להניח שהמכשיר יהפוך למעומעם.</span><span class="sxs-lookup"><span data-stu-id="26926-p105">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="26926-143">Access Outlook שוב במכשיר Android.</span><span class="sxs-lookup"><span data-stu-id="26926-143">Access Outlook on the Android device again.</span></span>
    
4. <span data-ttu-id="26926-144">תתבקש להזין את מספר הזיהוי האישי שלך לפני שתוכל לגשת אל Outlook שוב.</span><span class="sxs-lookup"><span data-stu-id="26926-144">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="26926-145">אימות של 'הגן על קבצי עבודה באמצעות הצפנה'</span><span class="sxs-lookup"><span data-stu-id="26926-145">Validate Protect work files with encryption</span></span>

<span data-ttu-id="26926-146">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **הגנה מפני מכשירים שאבדו או נגנבו**, הרחב את **הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים**, וודא שהאפשרות **הגן על קבצי עבודה באמצעות הצפנה** מוגדרת ל **מופעל** והאפשרות **כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business** מוגדרת ל **מבוטל**.</span><span class="sxs-lookup"><span data-stu-id="26926-146">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="26926-147">במכשיר Android של המשתמש, פתח Outlook והיכנס באמצעות אישורי Microsoft 365 Business Premium המשתמש והזן מספר זיהוי אישי לפי התבקש.</span><span class="sxs-lookup"><span data-stu-id="26926-147">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="26926-148">פתח הודעת דואר אלקטרוני המכילה כמה קבצים מצורפים של תמונה.</span><span class="sxs-lookup"><span data-stu-id="26926-148">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="26926-149">הקש על סמל החץ למטה לצד מידע אודות הקובץ המצורף כדי לשמור אותו.</span><span class="sxs-lookup"><span data-stu-id="26926-149">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](../media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="26926-p106">ייתכן שתתבקש לאפשר ל- Outlook לגשת לתמונות, למדיה ולקבצים במכשיר שלך. הקש על **אפשר**.</span><span class="sxs-lookup"><span data-stu-id="26926-p106">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="26926-153">בחלק התחתון של המסך, בחר **שמור במכשיר** ולאחר מכן פתח את האפליקציה **גלריה**.</span><span class="sxs-lookup"><span data-stu-id="26926-153">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="26926-p107">אתה אמור לראות תמונה מוצפנת (או יותר, אם שמרת קבצים מצורפים מרובים של תמונות) ברשימה. היא עשויה להופיע ברשימת התמונות כריבוע אפור עם סימן קריאה לבן בתוך עיגול לבן, במרכז הריבוע האפור.</span><span class="sxs-lookup"><span data-stu-id="26926-p107">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](../media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="ios"></a><span data-ttu-id="26926-157">iOS</span><span class="sxs-lookup"><span data-stu-id="26926-157">iOS</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="26926-158">בדיקה שהגדרות הגנה על יישומים פועלות במכשירי המשתמשים</span><span class="sxs-lookup"><span data-stu-id="26926-158">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="26926-159">לאחר [קביעת תצורות של יישומים עבור מכשירי iOS](app-protection-settings-for-android-and-ios.md) כדי להגן על יישומים, ניתן לבצע את השלבים הבאים כדי לאמת שההגדרות שבחרת פועלות.</span><span class="sxs-lookup"><span data-stu-id="26926-159">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="26926-160">תחילה, ודא שהמדיניות חלה על היישום שבו אתה עומד לאמת אותה.</span><span class="sxs-lookup"><span data-stu-id="26926-160">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="26926-161">במרכז Microsoft 365 Business Premium [,](https://admin.microsoft.com)עבור אל **מדיניות עריכת** \> **מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="26926-161">In the Microsoft 365 Business Premium [admin center](https://admin.microsoft.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="26926-162">בחר **מדיניות יישום** עבור iOS עבור ההגדרות שיצרת בהגדרה, או מדיניות אחרת שיצרת וודא שהיא נאכפת עבור Outlook לדוגמה.</span><span class="sxs-lookup"><span data-stu-id="26926-162">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](../media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="26926-164">אימות של 'דרוש מספר זיהוי אישי כדי לגשת ליישומי Office'</span><span class="sxs-lookup"><span data-stu-id="26926-164">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="26926-165">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **בקרת גישה למסמכי Office**, הרחב את **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים**, וודא שהאפשרות **דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office** מוגדרת ל **מופעל**.</span><span class="sxs-lookup"><span data-stu-id="26926-165">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![ודא שה- דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת לאפליקציות Office מוגדרות ל'הפעלה'.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="26926-167">במכשיר iOS של המשתמש, פתח Outlook והירשם באמצעות אישורי Microsoft 365 Business Premium המשתמש.</span><span class="sxs-lookup"><span data-stu-id="26926-167">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="26926-168">תתבקש גם להזין מספר זיהוי אישי או להשתמש בטביעת אצבע.</span><span class="sxs-lookup"><span data-stu-id="26926-168">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](../media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="26926-170">אימות של 'אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה'</span><span class="sxs-lookup"><span data-stu-id="26926-170">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="26926-171">בחלונית **עריכת מדיניות,** בחר ערוך לצד **פקד גישה של Office** מסמכים , הרחב את נהל את אופן הגישה של משתמשים  **לקבצי Office** במכשירים ניידים ולאחר מכן ודא כי איפוס **מספר** הזיהוי האישי לאחר מספר הניסיונות שנכשלו מוגדר למספר מסויים.</span><span class="sxs-lookup"><span data-stu-id="26926-171">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="26926-172">זהו 5 כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="26926-172">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="26926-173">במכשיר iOS של המשתמש, פתח Outlook והירשם באמצעות אישורי Microsoft 365 Business Premium המשתמש.</span><span class="sxs-lookup"><span data-stu-id="26926-173">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="26926-174">הזן מספר זיהוי אישי שגוי כמספר הפעמים שצוין על-ידי המדיניות.</span><span class="sxs-lookup"><span data-stu-id="26926-174">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="26926-175">תראה בקשה לפיה מספר הזיהוי האישי הגיע **למגבלת הניסיון לאיפוס** מספר הזיהוי האישי.</span><span class="sxs-lookup"><span data-stu-id="26926-175">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="26926-177">לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="26926-177">Press **OK**.</span></span> <span data-ttu-id="26926-178">תתבקש להיכנס באמצעות אישורי Microsoft 365 Business Premium של המשתמש ולאחר מכן תידרש להגדיר מספר זיהוי אישי חדש.</span><span class="sxs-lookup"><span data-stu-id="26926-178">You'll be prompted to sign in with the user's Microsoft 365 Business Premium credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="26926-179">אימות של 'כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business'</span><span class="sxs-lookup"><span data-stu-id="26926-179">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="26926-180">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **הגנה מפני מכשירים שאבדו או נגנבו**, הרחב את **הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים**, וודא שהאפשרות **כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business** מוגדרת ל **מופעל**.</span><span class="sxs-lookup"><span data-stu-id="26926-180">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="26926-182">במכשיר iOS של המשתמש, פתח Outlook והיכנס באמצעות אישורי Microsoft 365 Business Premium של המשתמש והזן מספר זיהוי אישי לפי התבקש.</span><span class="sxs-lookup"><span data-stu-id="26926-182">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="26926-183">פתח הודעת דואר אלקטרוני המכילה קובץ מצורף, פתח את הקובץ המצורף ובחר **שמור** בתחתית המסך.</span><span class="sxs-lookup"><span data-stu-id="26926-183">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](../media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="26926-185">אתה אמור לראות אפשרות רק עבור OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="26926-185">You should only see an option for OneDrive for Business.</span></span> <span data-ttu-id="26926-186">אם לא, הקש **על הוסף חשבון** ובחר OneDrive for Business **במסך** **הוספת חשבון אחסון.**</span><span class="sxs-lookup"><span data-stu-id="26926-186">If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen.</span></span> <span data-ttu-id="26926-187">ספק למשתמש הקצה את Microsoft 365 Business Premium להיכנס כאשר תתבקש לעשות זאת.</span><span class="sxs-lookup"><span data-stu-id="26926-187">Provide the end user's Microsoft 365 Business Premium to sign in when prompted.</span></span> 
    
    <span data-ttu-id="26926-188">הקש על **שמור** ובחר **OneDrive for Business**.</span><span class="sxs-lookup"><span data-stu-id="26926-188">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="26926-189">אימות של 'דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך'</span><span class="sxs-lookup"><span data-stu-id="26926-189">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="26926-190">בחלונית **עריכת מדיניות,** בחר ערוך לצד **פקד גישה של Office** מסמכים , הרחב את נהל את אופן הגישה של משתמשים  **לקבצי Office** במכשירים ניידים, ודא שדרוש מהמשתמשים להיכנס שוב לאחר **שאפליקציות Office** לא היו פעילות במשך כמה דקות.</span><span class="sxs-lookup"><span data-stu-id="26926-190">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="26926-191">זהו 30 דקות כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="26926-191">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="26926-192">במכשיר iOS של המשתמש, פתח Outlook והיכנס באמצעות אישורי Microsoft 365 Business Premium של המשתמש והזן מספר זיהוי אישי לפי התבקש.</span><span class="sxs-lookup"><span data-stu-id="26926-192">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="26926-p113">כעת אתה אמור לראות את תיבת הדואר הנכנס של Outlook. הנח למכשיר ה- iOS ואל תיגע בו במשך 30 דקות לפחות (או פרק זמן אחר, ארוך יותר מזה שצוין במדיניות). סביר להניח שהמכשיר יהפוך למעומעם.</span><span class="sxs-lookup"><span data-stu-id="26926-p113">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="26926-196">Access Outlook שוב במכשיר iOS.</span><span class="sxs-lookup"><span data-stu-id="26926-196">Access Outlook on the iOS device again.</span></span>
    
4. <span data-ttu-id="26926-197">תתבקש להזין את מספר הזיהוי האישי שלך לפני שתוכל לגשת אל Outlook שוב.</span><span class="sxs-lookup"><span data-stu-id="26926-197">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="26926-198">אימות של 'הגן על קבצי עבודה באמצעות הצפנה'</span><span class="sxs-lookup"><span data-stu-id="26926-198">Validate Protect work files with encryption</span></span>

<span data-ttu-id="26926-199">בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **הגנה מפני מכשירים שאבדו או נגנבו**, הרחב את **הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים**, וודא שהאפשרות **הגן על קבצי עבודה באמצעות הצפנה** מוגדרת ל **מופעל** והאפשרות **כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business** מוגדרת ל **מבוטל**.</span><span class="sxs-lookup"><span data-stu-id="26926-199">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="26926-200">במכשיר iOS של המשתמש, פתח Outlook והיכנס באמצעות אישורי Microsoft 365 Business Premium של המשתמש והזן מספר זיהוי אישי לפי התבקש.</span><span class="sxs-lookup"><span data-stu-id="26926-200">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="26926-201">פתח הודעת דואר אלקטרוני המכילה כמה קבצים מצורפים של תמונה.</span><span class="sxs-lookup"><span data-stu-id="26926-201">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="26926-202">הקש על הקובץ המצורף ולאחר מכן הקש על האפשרות **שמור** מתחתיו.</span><span class="sxs-lookup"><span data-stu-id="26926-202">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="26926-p114">פתח את היישום **תמונות** מתוך מסך הבית. אתה אמור לראות תמונה מוצפנת (או יותר, אם שמרת קבצים מצורפים מרובים של תמונות) שמורה, אך מוצפנת.</span><span class="sxs-lookup"><span data-stu-id="26926-p114">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---

