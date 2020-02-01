---
title: אימות הגדרות הגנה app על אנדרואיד או מכשירי iOS
f1.keywords:
- NOCSH
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
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: Learn how to validate the Microsoft 365 Business app protection settings in your Android or iOS devices.
ms.openlocfilehash: 47ce137f785c595992886c756ad85b80957272fe
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594974"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a>אימות הגדרות הגנה app על אנדרואיד או מכשירי iOS

בצע את ההוראות בסעיפים הבאים כדי לאמת הגדרות הגנה app על אנדרואיד או מכשירי iOS.
  
## <a name="android"></a>אנדרואיד
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a>בדוק שהגדרות הגנת היישום עובדות על התקני משתמש

לאחר [קביעת תצורות של יישומים עבור מכשירי Android](app-protection-settings-for-android-and-ios.md) כדי להגן על יישומים, ניתן לבצע את השלבים הבאים כדי לאמת שההגדרות שבחרת פועלות. 
  
ראשית, ודא שהמדיניות חלה על היישום שבו אתה עומד לאמת אותו.
  
1. ב[מרכז הניהול](https://portal.office.com) של Microsoft 365 Business, עבור אל **פריטי מדיניות** \> **ערוך מדיניות**.
    
2. בחר **מדיניות יישום עבור Android** עבור ההגדרות שיצרת בתוכנית ההתקנה, או מדיניות אחרת שיצרת וודא שהיא נאכפת עבור Outlook, לדוגמה. 
    
    ![Shows all the apps for which this policy protects files.](media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a>אימות של 'דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office'

בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **בקרת גישה למסמכי Office**, הרחב את **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים**, וודא שהאפשרות **דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office** מוגדרת ל **מופעל**.
  
![ודא שדרוש ל-PIN או טביעת אצבע כדי לגשת ליישומי Office מוגדר כופעל.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. במכשיר ה- Android של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש.
    
2. תתבקש גם להזין PIN או להשתמש בטביעת אצבע.
    
    ![Enter a PIN on your Android device to access Office apps.](media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a>אימות של 'אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה'

בחלונית ' **עריכת מדיניות** ', בחר ' **עריכה** ' לצד **בקרת גישה למסמכי Office**, הרחב את **ניהול האופן שבו משתמשים ניגשים לקבצי OFFICE בהתקנים ניידים**וודא **שפין איפוס לאחר מספר הנסיונות הכושלים** מוגדר כמספר מסוים. . זה 5 כברירת מחדל 
  
1. במכשיר ה- Android של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש.
    
2. הזן מספר זיהוי אישי שגוי כמספר הפעמים שצוין על-ידי המדיניות. תראה הודעה שמציינת את **מגבלת ניסיון של pin הושגה** כדי לאפס את ה-PIN. 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. לחץ על **איפוס מספר זיהוי אישי**. תתבקש להיכנס עם האישורים העסקיים של Microsoft 365 של המשתמש ולאחר מכן להגדיר PIN חדש.
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a>אימות של 'כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business'

בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **הגנה מפני מכשירים שאבדו או נגנבו**, הרחב את **הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים**, וודא שהאפשרות **כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business** מוגדרת ל **מופעל**.
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. במכשיר ה- Android של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש והזן מספר זיהוי אישי במידת הצורך.
    
2. פתח הודעת דואר אלקטרוני המכילה קובץ מצורף והקש על סמל החץ למטה לצד המידע אודות הקובץ המצורף.
    
    ![Tap the down arrow next to an attachment to try to save it.](media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    תראה **אין אפשרות לשמור את ההתקן** בתחתית המסך. 
    
    ![Warning text that indicates cannot save a file locally to an Android.](media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > [!הערה] שמירה ב- OneDrive for Business אינה זמינה עבור Android בשלב זה, לכן תוכל לראות רק ששמירה מקומית נחסמת. 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a>אימות של 'דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך'

בחלונית **המדיניות edit** , בחר באפשרות **ערוך** לצד **בקרת גישה למסמכי Office**, הרחב את **ניהול האופן שבו משתמשים ניגשים לקבצי Office בהתקנים ניידים**וודא **שדרוש למשתמשים להיכנס שוב לאחר שיישומי office לא היו במצב פעיל** מוגדר כמספר דקות מסוים. . זה 30 דקות כברירת מחדל 
  
1. במכשיר ה- Android של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש והזן מספר זיהוי אישי במידת הצורך.
    
2. כעת אתה אמור לראות את תיבת הדואר הנכנס של Outlook. הנח למכשיר ה- Android ואל תיגע בו במשך 30 דקות לפחות (או פרק זמן אחר, ארוך יותר מזה שצוין במדיניות). סביר להניח שהמכשיר יהפוך למעומעם.
    
3. גש שוב ל-Outlook בהתקן האנדרואיד.
    
4. תתבקש להזין את ה-PIN שלך לפני שתוכל לגשת שוב ל-Outlook.
    
### <a name="validate-protect-work-files-with-encryption"></a>אימות של 'הגן על קבצי עבודה באמצעות הצפנה'

בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **הגנה מפני מכשירים שאבדו או נגנבו**, הרחב את **הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים**, וודא שהאפשרות **הגן על קבצי עבודה באמצעות הצפנה** מוגדרת ל **מופעל** והאפשרות **כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business** מוגדרת ל **מבוטל**.
  
1. במכשיר ה- Android של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש והזן מספר זיהוי אישי במידת הצורך.
    
2. פתח דואר אלקטרוני המכיל קבצים מצורפים אחדים של קובץ תמונה.
    
3. הקש על סמל החץ למטה לצד מידע אודות הקובץ המצורף כדי לשמור אותו.
    
    ![Tap the down arrow to save the figure file to the Android device.](media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. ייתכן שתתבקש לאפשר ל- Outlook לגשת לתמונות, למדיה ולקבצים במכשיר שלך. הקש על **אפשר**.
    
5. בחלק התחתון של המסך, בחר **שמור במכשיר** ולאחר מכן פתח את האפליקציה **גלריה**. 
    
6. אתה אמור לראות תמונה מוצפנת (או יותר, אם שמרת קבצים מצורפים מרובים של תמונות) ברשימה. היא עשויה להופיע ברשימת התמונות כריבוע אפור עם סימן קריאה לבן בתוך עיגול לבן, במרכז הריבוע האפור.
    
    ![An encrypted image file in the Gallery app.](media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="ios"></a>iOS
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a>בדיקה שהגדרות הגנה על יישומים פועלות במכשירי המשתמשים

לאחר [קביעת תצורות של יישומים עבור מכשירי iOS](app-protection-settings-for-android-and-ios.md) כדי להגן על יישומים, ניתן לבצע את השלבים הבאים כדי לאמת שההגדרות שבחרת פועלות. 
  
ראשית, ודא שהמדיניות חלה על היישום שבו אתה עומד לאמת אותו.
  
1. ב[מרכז הניהול](https://portal.office.com) של Microsoft 365 Business, עבור אל **פריטי מדיניות** \> **ערוך מדיניות**.
    
2. בחר **מדיניות יישום עבור iOS** עבור ההגדרות שיצרת בתוכנית ההתקנה, או מדיניות אחרת שיצרת וודא שהיא נאכפת עבור Outlook לדוגמה. 
    
    ![Shows all the apps for which this policy protects files.](media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a>אימות של 'דרוש מספר זיהוי אישי כדי לגשת ליישומי Office'

בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **בקרת גישה למסמכי Office**, הרחב את **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים**, וודא שהאפשרות **דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office** מוגדרת ל **מופעל**.
  
![ודא שדרוש ל-PIN או טביעת אצבע כדי לגשת ליישומי Office מוגדר כופעל.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. במכשיר ה- iOS של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש.
    
2. תתבקש גם להזין PIN או להשתמש בטביעת אצבע.
    
    ![Enter a PIN on your IOS device to access Office apps.](media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a>אימות של 'אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה'

בחלונית ' **עריכת מדיניות** ', בחר ' **עריכה** ' לצד **בקרת גישה למסמכי Office**, הרחב את **ניהול האופן שבו משתמשים ניגשים לקבצי OFFICE בהתקנים ניידים**וודא **שפין איפוס לאחר מספר הנסיונות הכושלים** מוגדר כמספר מסוים. . זה 5 כברירת מחדל 
  
1. במכשיר ה- iOS של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש.
    
2. הזן מספר זיהוי אישי שגוי כמספר הפעמים שצוין על-ידי המדיניות. תראה הודעה שמציינת את **מגבלת ניסיון של pin הושגה** כדי לאפס את ה-PIN. 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. לחץ על **אישור**. תתבקש להיכנס עם האישורים העסקיים של Microsoft 365 של המשתמש ולאחר מכן להגדיר PIN חדש.
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a>אימות של 'כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business'

בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **הגנה מפני מכשירים שאבדו או נגנבו**, הרחב את **הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים**, וודא שהאפשרות **כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business** מוגדרת ל **מופעל**.
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. במכשיר ה- iOS של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש והזן קוד זיהוי אישי במידת הצורך.
    
2. פתח הודעת דואר אלקטרוני המכילה קובץ מצורף, פתח את הקובץ המצורף ובחר **שמור** בתחתית המסך. 
    
    ![Tap the Save option after you open an attachment to try to save it.](media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. אתה אמור לראות אפשרות רק עבור OneDrive for Business. אם לא, הקש על **הוסף חשבון** ובחר **בכונן Onedrive עבור עסקים** מהמסך **הוספת חשבון אחסון** . ספק את Microsoft 365 Business של משתמש הקצה כדי להיכנס כאשר תתבקש לעשות זאת. 
    
    הקש על **שמור** ובחר **OneDrive for Business**.
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a>אימות של 'דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך'

בחלונית **המדיניות edit** , בחר באפשרות **ערוך** לצד **בקרת גישה למסמכי Office**, הרחב את **ניהול האופן שבו משתמשים ניגשים לקבצי Office בהתקנים ניידים**וודא **שדרוש למשתמשים להיכנס שוב לאחר שיישומי office לא היו במצב פעיל** מוגדר כמספר דקות מסוים. . זה 30 דקות כברירת מחדל 
  
1. במכשיר ה- iOS של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש והזן קוד זיהוי אישי במידת הצורך.
    
2. כעת אתה אמור לראות את תיבת הדואר הנכנס של Outlook. הנח למכשיר ה- iOS ואל תיגע בו במשך 30 דקות לפחות (או פרק זמן אחר, ארוך יותר מזה שצוין במדיניות). סביר להניח שהמכשיר יהפוך למעומעם.
    
3. גישה ל-Outlook בהתקן iOS שוב.
    
4. תתבקש להזין את ה-PIN שלך לפני שתוכל לגשת שוב ל-Outlook.
    
### <a name="validate-protect-work-files-with-encryption"></a>אימות של 'הגן על קבצי עבודה באמצעות הצפנה'

בחלונית **ערוך מדיניות**, בחר **ערוך** לצד **הגנה מפני מכשירים שאבדו או נגנבו**, הרחב את **הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים**, וודא שהאפשרות **הגן על קבצי עבודה באמצעות הצפנה** מוגדרת ל **מופעל** והאפשרות **כפה על משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business** מוגדרת ל **מבוטל**.
  
1. במכשיר ה- iOS של המשתמש, פתח את Outlook והיכנס באמצעות אישורי Microsoft 365 Business של המשתמש והזן קוד זיהוי אישי במידת הצורך.
    
2. פתח דואר אלקטרוני המכיל קבצים מצורפים אחדים של קובץ תמונה.
    
3. הקש על הקובץ המצורף ולאחר מכן הקש על האפשרות **שמור** מתחתיו. 
    
4. פתח את היישום **תמונות** מתוך מסך הבית. אתה אמור לראות תמונה מוצפנת (או יותר, אם שמרת קבצים מצורפים מרובים של תמונות) שמורה, אך מוצפנת. 
    
---

