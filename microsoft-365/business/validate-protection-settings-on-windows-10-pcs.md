---
title: אימות הגדרות הגנה של אפליקציות במחשבי Windows 10
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: אמת Microsoft 365 Business Premium הגנה על אפליקציות Windows 10 ואמת שמשתמשים אינם יכולים להעתיק נתוני חברה לקבצים אישיים או ליישומים שאינם מנוהלים.
ms.openlocfilehash: ab084ded5ef052a7b85839f0debb96eb1bc5bdf332230293613396825c7263f0
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53861717"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>אימות הגדרות הגנה של אפליקציות במחשבי Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>ודא שמשתמשים אינם יכולים להעתיק נתונים של החברה לקבצים אישיים במכשירים של החברה

לאחר שאתה [מגדיר מדיניות הגנה על אפליקציות](protection-settings-for-windows-10-devices.md), עשויות לחלוף כמה שעות בטרם המדיניות תיכנס לתוקף במכשירים של המשתמשים. אם הפכת את **ההגדרה** מנע ממשתמשים להעתיק נתוני חברה לקבצים אישיים ולאלץ אותם לשמור קבצי **עבודה ב- OneDrive for Business** עבור מכשירים בבעלות החברה, באפשרותך לבדוק זאת במכשיר של המשתמש לאחר שהם התחברו ל- Azure AD והינם מחוברים. 
  
 **אימות הגדרות חיבור**
  
1. לאחר שתיתחבר באמצעות Microsoft 365 Business Premium ותתחבר ל- Azure AD כמתואר במאמר [הגדרת Windows עבור משתמשי Microsoft 365 Business Premium](set-up-windows-devices.md), עבור אל Windows הגדרות  \> **חשבונות** Access עבודה או \> **בית ספר**. בחר **מחובר \<tenant name\> ל- Azure AD** ולאחר מכן בחר **מידע**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. בדף **מנוהל על-ידי,** באפשרותך לראות את פרטי החיבור הכוללים כתובת \<tenant name\> שרת **ניהול,** כמו זו המוצגת באיור הבא.  
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **ודא שלא ניתן להדביק נתוני חברה באפליקציה לא מנוהלת**
  
1. פתח Outlook 2016 שהותקן על-ידי Microsoft 365 Business Premium.
    
2. פתח הודעת דואר אלקטרוני והעתק חלק מהתוכן שלה.
    
    פתח את 'פנקס רשימות' ונסה להדביק את התוכן.
    
    תקבל שגיאה המציין שלאפליקציה אין אפשרות לגשת לתוכן.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    עם זאת, תוכל להדביק את אותו תוכן ב- Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>ודא שמשתמשים אינם יכולים להעתיק נתונים של החברה לקבצים אישיים במכשירים אישיים

 **אימות הגדרות חיבור**
  
1. במכשיר Windows 10 האישי שלך שבו אתה מחובר כמשתמש מקומי, עבור **אל Windows הגדרות** ולאחר מכן לחץ או הקש על **חשבונות** Access בעבודה או \> **בבית ספר**.
    
2. תחת **גישה לחשבון בעבודה או בבית ספר**, בחר **התחבר**.
    
3. הזן את Microsoft 365 Business Premium האישור שלך בתיבת **הדו-שיח הגדרת חשבון בעבודה או בבית ספר** \> **היכנס.**
    
4. בדף **גישה לחשבון בעבודה או בבית ספר**, בחר את ה **חשבון בעבודה או בבית ספר** ולאחר מכן בחר **פרטים**.
    
    ![לחץ או הקש על מידע בתיבת הדו-שיח חשבון בעבודה או בבית ספר.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. בדף **Access בעבודה** או בבית ספר, באפשרותך  לראות את פרטי החיבור הכוללים כתובת **שרת** ניהול, כמו זו המוצגת באיור הבא, וכוללת את המילים *wip* *ו- mam* בתוך. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **ודא שלא ניתן להדביק נתוני חברה באפליקציה לא מנוהלת**
  
1. פתח Outlook 2016 והוסף את Microsoft 365 Business Premium שלך במקרה הצורך והירשם באמצעות אישורי Microsoft 365 Business Premium שלך.
    
2. פתח הודעת דואר אלקטרוני והעתק חלק מהתוכן שלה.
    
    פתח את 'פנקס רשימות' ונסה להדביק את התוכן.
    
    תקבל שגיאה שמציין ש- App לא יכול לגשת לתוכן.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    עם זאת, תוכל להדביק את אותו תוכן ב- Word 2016.
    

