---
title: אימות הגדרות הגנה של אפליקציות במחשבי Windows 10
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: אמת את הגדרות ההגנה העסקית של Microsoft 365 Business Premium בהתקנים של Windows 10 וודא שלמשתמשים אין אפשרות להעתיק נתוני חברה לקבצים אישיים או ליישומים שאינם מנוהלים.
ms.openlocfilehash: 589d2fc25cc1425a775523595881660cc03e152e
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403389"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>אימות הגדרות הגנה של אפליקציות במחשבי Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>ודא שמשתמשים אינם יכולים להעתיק נתונים של החברה לקבצים אישיים במכשירים של החברה

לאחר שאתה [מגדיר מדיניות הגנה על אפליקציות](protection-settings-for-windows-10-devices.md), עשויות לחלוף כמה שעות בטרם המדיניות תיכנס לתוקף במכשירים של המשתמשים. אם **הפעלת את** **הנתונים של החברה ' מנע ממשתמשים להעתיק ' לקבצים אישיים ולאלץ אותם לשמור קבצי עבודה בכונן אחד עבור** הגדרות עסקיות עבור התקנים בבעלות חברה, באפשרותך לבדוק זאת בהתקן המשתמש לאחר ההתחברות למודעה ולחתימה ב-. 
  
 **אימות הגדרות חיבור**
  
1. לאחר שתתחבר עם האישורים של microsoft 365 הפרמיה העסקית ותתחבר לתכלת כמתואר [בהגדרת windows התקנים עבור משתמשי Premium של משתמשים עסקיים של microsoft 365](set-up-windows-devices.md), עבור לחשבונות **של windows הגדרות** \> **Accounts** \> **גישה לעבודה או לבית הספר**. בחר \<tenant name\>ולאחר מכן בחר **מידע**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. בעמוד **מנוהל על-ידי** \<tenant name\> , באפשרותך לראות את **מידע החיבור** הכולל **כתובת שרת ניהול** כמו האפשרות המוצגת באיור הבא. 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **ודא שלא ניתן להדביק נתוני חברה ביישום שאינו מנוהל**
  
1. פתח את Outlook 2016 שהותקן על ידי מיקרוסופט 365 עסקים Premium.
    
2. פתח הודעת דואר אלקטרוני והעתק חלק מהתוכן שלה.
    
    פתח את 'פנקס רשימות' ונסה להדביק את התוכן.
    
    תקבל שגיאה המציינת כי ליישום אין אפשרות לגשת לתוכן.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    עם זאת, תוכל להדביק את אותו תוכן ב- Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>ודא שמשתמשים אינם יכולים להעתיק נתונים של החברה לקבצים אישיים במכשירים אישיים

 **אימות הגדרות חיבור**
  
1. בהתקן האישי של windows 10 שבו אתה מחובר כמשתמש מקומי, עבור אל ' **הגדרות Windows**' ולחץ על הלחצן עבודה או על הקשה על **חשבונות** \> **גישה**.
    
2. תחת **גישה לחשבון בעבודה או בבית ספר**, בחר **התחבר**.
    
3. הזן את האישור שלך ב-Microsoft 365 Business Premium לתוך **הגדרת כניסה לעבודה או לחשבון בית ספר** \> **Sign in**.
    
4. בדף **גישה לחשבון בעבודה או בבית ספר**, בחר את ה **חשבון בעבודה או בבית ספר** ולאחר מכן בחר **פרטים**.
    
    ![לחץ או הקש על מידע בתיבת הדו עבודה או חשבון בית ספר.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. בדף **עבודה או בית ספר של Access** , באפשרותך לראות את **מידע החיבור** הכולל **כתובת שרת ניהול** כגון האחת המוצגת באיור הבא, וכוללת את המילים *wip* *ואמא* בתוך. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **ודא שלא ניתן להדביק נתוני חברה ביישום שאינו מנוהל**
  
1. פתח את Outlook 2016 והוסף את חשבון Premium לעסקים של Microsoft 365 במידת הצורך והיכנס באמצעות האישורים העסקיים של Microsoft 365 Premium.
    
2. פתח הודעת דואר אלקטרוני והעתק חלק מהתוכן שלה.
    
    פתח את 'פנקס רשימות' ונסה להדביק את התוכן.
    
    תקבל שגיאה המציינת ש-App אינו יכול לגשת לתוכן.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    עם זאת, תוכל להדביק את אותו תוכן ב- Word 2016.
    

