---
title: שימוש במדריך שלב אחר שלב להוספת מכשירים ופרופיל של Autopilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: למד כיצד להשתמש AutoPilot של Windows כדי להתקין התקנים חדשים של Windows 10 עבור העסק שלך.
ms.openlocfilehash: e0802ddcc0964d0b8d102f7dbdb9116b33cdcf58
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277114"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>שימוש במדריך שלב אחר שלב להוספת מכשירים ופרופיל של Autopilot

באפשרותך להשתמש ב- Windows Autopilot כדי להגדיר מכשירים חדשים של Windows 10 עבור העסק שלך, כך שהם יהיו מוכנים לשימוש פרודוקטיבי ברגע שתספק אותם לעובדים שלך.
  
## <a name="device-requirements"></a>דרישות המכשירים

המכשירים צריכים לעמוד בדרישות אלה:
  
- Windows ,10 גירסה 1703 ואילך.
    
- מכשירים חדשים שאינם נחשבים כמוצר Windows מוכן לשימוש.
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>שימוש במדריך ההתקנה ליצירת מכשירים ופרופילים

אם עדיין לא יצרת קבוצות מכשירים או פרופילים, הדרך הטובה ביותר להתחיל היא באמצעות מדריך צעד-אחר-צעד, אך תוכל גם [להוסיף מכשירים](create-and-edit-autopilot-devices.md) ו [להקצות להם פרופילים](create-and-edit-autopilot-profiles.md) מבלי להשתמש במדריך. 
  
1. במרכז הניהול של Microsoft 365 Business, אתר כרטיס **פעולות מכשיר** ובחר **פרוס את Windows באמצעות AutoPilot**.
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. בכרטיסיה **הכנת Windows**, לחץ או הקש על **מדריך התחלה**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. בדף **העלאת קובץ ‎.csv עם רשימת מכשירים**, אתר את המיקומים שבהם נמצא קובץ ה- ‎.CSV המוכן, ולאחר מכן לחץ על **פתח** \> **הבא**. הקובץ אמור להכיל שלוש כותרות:
    
  - עמודה א: מספר סידורי של המכשיר
    
  - עמודה ב: מזהה המוצר של Windows
    
  - עמודה ג: קוד Hash של החומרה
    
    ניתן לקבל מידע זה מספק החומרה, או להשתמש ב[קובץ Script של PowerShell, ‏Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) שייצור קובץ csv. 
    
    למידע נוסף, ראה [קובץ CSV עם רשימת מכשירים](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). באפשרותך גם להוריד קובץ לדוגמה בדף **העלאת קובץ ‎.csv עם רשימת מכשירים**. 
    
4. בדף **הקצאת פרופיל**, תוכל לבחור פרופיל קיים או ליצור פרופיל חדש. אם עדיין אין לך חשבון, תתבקש ליצור חשבון חדש. 
    
    פרופיל הוא אוסף הגדרות שניתן להחיל על מכשיר בודד או על קבוצה של מכשירים.
    
    תכונות ברירת המחדל נדרשות ויוגדרו באופן אוטומטי. תכונות ברירת המחדל הן:
    
  - דילוג על רישום Cortana‏, OneDrive ו- OEM.
    
  - יצירת חוויית כניסה עם מותג החברה.
    
  - המכשירים שלך עומדים להתחבר לחשבונות Azure Active Directory ולהירשם באופן אוטומטי לניהול על-ידי Microsoft 365 Business.
    
    לקבלת מידע נוסף, ראה
    
    [אודות ההגדרות של פרופיל AutoPilot](autopilot-profile-settings.md) . 
    
5. שאר ההגדרות הן **דלג על הגדרות פרטיות** ו **אל תאפשר למשתמש להפוך למנהל המערכת המקומי**. שתי הגדרות אלה מוגדרות למצב **כבוי** כברירת מחדל. 
    
    בחר **הבא**.
    
6. הדף **סיום** מציין שהפרופיל שיצרת (או בחרת) יוחל על קבוצת המכשירים שיצרת על-ידי העלאת רשימת המכשירים. הגדרות אלה ייכנסו לתוקף בפעם הבאה שמשתמשי המכשיר ייכנסו אליו. בחר **סגור**.
    