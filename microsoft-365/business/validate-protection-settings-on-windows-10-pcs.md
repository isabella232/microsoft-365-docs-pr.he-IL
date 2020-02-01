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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: למד כיצד לאמת את הגדרות הגנת היישום העסקי של Microsoft 365 בהתקני Windows 10.
ms.openlocfilehash: 6573519ee2fe2d1eb82545755fa98b8c018e08ff
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594994"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>אימות הגדרות הגנה של אפליקציות במחשבי Windows 10

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>ודא שמשתמשים אינם יכולים להעתיק נתונים של החברה לקבצים אישיים במכשירים של החברה

לאחר שאתה [מגדיר מדיניות הגנה על אפליקציות](protection-settings-for-windows-10-devices.md), עשויות לחלוף כמה שעות בטרם המדיניות תיכנס לתוקף במכשירים של המשתמשים. אם **הפעלת את** **הנתונים של החברה ' מנע ממשתמשים להעתיק ' לקבצים אישיים ולאלץ אותם לשמור קבצי עבודה בכונן אחד עבור** הגדרות עסקיות עבור התקנים בבעלות חברה, באפשרותך לבדוק זאת בהתקן המשתמש לאחר ההתחברות למודעה ולחתימה ב-. 
  
 **אימות הגדרות חיבור**
  
1. After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. בדף ' **מנוהל על-ידי** \<שם\> דייר ', באפשרותך לראות את **מידע החיבור** הכולל **כתובת שרת ניהול** כמו זו המוצגת באיור הבא. 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **ודא שלא ניתן להדביק נתוני חברה ביישום שאינו מנוהל**
  
1. פתח את Outlook 2016 שהותקן על-ידי Microsoft 365 Business.
    
2. פתח הודעת דואר אלקטרוני והעתק חלק מהתוכן שלה.
    
    פתח את 'פנקס רשימות' ונסה להדביק את התוכן.
    
    תקבל שגיאה המציינת כי ליישום אין אפשרות לגשת לתוכן.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    עם זאת, תוכל להדביק את אותו תוכן ב- Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>ודא שמשתמשים אינם יכולים להעתיק נתונים של החברה לקבצים אישיים במכשירים אישיים

 **אימות הגדרות חיבור**
  
1. בהתקן האישי של windows 10 שבו אתה מחובר כמשתמש מקומי, עבור אל **הגדרות Windows**ולחץ או הקש על **חשבון** \> **גישה לעבודה או בית ספר**.
    
2. תחת **גישה לחשבון בעבודה או בבית ספר**, בחר **התחבר**.
    
3. הזן את אישור Microsoft 365 Business שלך בתיבת הדו-שיח **הגדר חשבון בעבודה או בבית ספר** \> **כניסה**.
    
4. בדף **גישה לחשבון בעבודה או בבית ספר**, בחר את ה **חשבון בעבודה או בבית ספר** ולאחר מכן בחר **פרטים**.
    
    ![לחץ או הקש על מידע בתיבת הדו עבודה או חשבון בית ספר.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. בדף **עבודה או בית ספר של Access** , באפשרותך לראות את **מידע החיבור** הכולל **כתובת שרת ניהול** כגון האחת המוצגת באיור הבא, וכוללת את המילים *wip* *ואמא* בתוך. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **ודא שלא ניתן להדביק נתוני חברה ביישום שאינו מנוהל**
  
1. פתח את Outlook 2016 והוסף את חשבון Microsoft 365 Business שלך, אם נדרש; לאחר מכן, היכנס עם אישורי Microsoft 365 Business שלך.
    
2. פתח הודעת דואר אלקטרוני והעתק חלק מהתוכן שלה.
    
    פתח את 'פנקס רשימות' ונסה להדביק את התוכן.
    
    תקבל שגיאה המציינת ש-App אינו יכול לגשת לתוכן.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    עם זאת, תוכל להדביק את אותו תוכן ב- Word 2016.
    

