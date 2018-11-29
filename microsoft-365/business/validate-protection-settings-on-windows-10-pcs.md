---
title: אימות הגדרות הגנה של אפליקציות במחשבי Windows 10
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
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: למד כיצד לאמת את הגדרות ההגנה app עסקיים 365 Microsoft ב- Windows 10 התקנים.
ms.openlocfilehash: f00dd380103ad9498d77b0e8814bace3de168df4
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983294"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>אימות הגדרות הגנה של אפליקציות במחשבי Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>ודא שמשתמשים אינם יכולים להעתיק נתונים של החברה לקבצים אישיים במכשירים של החברה

לאחר שאתה [מגדיר מדיניות הגנה על אפליקציות](protection-settings-for-windows-10-devices.md), עשויות לחלוף כמה שעות בטרם המדיניות תיכנס לתוקף במכשירים של המשתמשים. אם **הפעלת** את ההגדרה **מנע ממשתמשים להעתיק נתוני חברה לקבצים אישיים וכפה עליהם לשמור קבצי עבודה ב- OneDrive for Business** עבור מכשירים השייכים לחברה, תוכל לבדוק זאת במכשירים של המשתמשים לאחר שהם יתחברו ל- Azure AD ויבצעו כניסה. 
  
 **אימות הגדרות חיבור**
  
1. לאחר להיכנס באמצעות אישורי Microsoft 365 עסקיים להתחבר AD תכלת הרקיע כפי שמתואר [להגדיר התקנים של Windows עבור משתמשים עסקיים 365 של Microsoft](set-up-windows-devices.md), עבור אל **ההגדרות של Windows** \> **חשבונות** \> **Access בעבודה או בבית הספר **. בחר **מחובר \<שם הדייר\> AD תכלת הרקיע**, ולאחר מכן בחר **מידע**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. בדף **מנוהל על-ידי** \<שם הדייר\>, תוכל לראות את **פרטי החיבור** הכוללים **כתובת שרת ניהול** כמו זו המוצגת באיור הבא. 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **ודא שלא ניתן להדביק נתוני חברה באפליקציה שאינה מנוהלת**
  
1. פתח את Outlook 2016 שהותקן על-ידי Microsoft 365 Business.
    
2. פתח הודעת דואר אלקטרוני והעתק חלק מהתוכן שלה.
    
    פתח את 'פנקס רשימות' ונסה להדביק את התוכן.
    
    תקבל שגיאה המציינת שהאפליקציה אינה יכולה לגשת לתוכן.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    עם זאת, תוכל להדביק את אותו תוכן ב- Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>ודא שמשתמשים אינם יכולים להעתיק נתונים של החברה לקבצים אישיים במכשירים אישיים

 **אימות הגדרות חיבור**
  
1. במכשיר Windows 10 האישי שבו אתה מחובר בתור משתמש מקומי, עבור אל **הגדרות Windows** ולחץ או הקש על **חשבונות** \> **גישה לחשבון בעבודה או בבית ספר**.
    
2. תחת **גישה לחשבון בעבודה או בבית ספר**, בחר **התחבר**.
    
3. הזן את אישור Microsoft 365 Business שלך בתיבת הדו-שיח **הגדר חשבון בעבודה או בבית ספר** \> **כניסה**.
    
4. בדף **גישה לחשבון בעבודה או בבית ספר**, בחר את ה **חשבון בעבודה או בבית ספר** ולאחר מכן בחר **פרטים**.
    
    ![Click or tap Info on the Work or school account dalog.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. בדף **גישה לחשבון עבודה או בית ספר**, תוכל לראות את **פרטי החיבור** הכוללים **כתובת שרת ניהול** כמו זו המוצגת באיור הבא, וכן כוללים את המילים  *wip*  ו-  *mam*  . 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **ודא שלא ניתן להדביק נתוני חברה באפליקציה שאינה מנוהלת**
  
1. פתח את Outlook 2016 והוסף את חשבון Microsoft 365 Business שלך, אם נדרש; לאחר מכן, היכנס עם אישורי Microsoft 365 Business שלך.
    
2. פתח הודעת דואר אלקטרוני והעתק חלק מהתוכן שלה.
    
    פתח את 'פנקס רשימות' ונסה להדביק את התוכן.
    
    תקבל שגיאה המציינת שהאפליקציה אינה יכולה לגשת לתוכן.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    עם זאת, תוכל להדביק את אותו תוכן ב- Word 2016.
    

