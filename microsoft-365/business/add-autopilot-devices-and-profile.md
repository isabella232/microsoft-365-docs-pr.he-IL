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
ms.openlocfilehash: 8c4a14b4b9dcbf7a30c1e6e0bdd53418a1ab8a03
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660670"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>שימוש במדריך שלב אחר שלב להוספת מכשירים ופרופיל של Autopilot

באפשרותך להשתמש AutoPilot של Windows כדי להגדיר התקנים 10 חלונות **חדשים** עבור העסק שלך, כך הם מוכנים לשימוש יעיל ברגע שתיתן לו את העובדים שלך.
  
## <a name="device-requirements"></a>דרישות המכשירים

המכשירים צריכים לעמוד בדרישות אלה:
  
- Windows ,10 גירסה 1703 ואילך.
    
- מכשירים חדשים שאינם נחשבים כמוצר Windows מוכן לשימוש.
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>שימוש במדריך ההתקנה ליצירת מכשירים ופרופילים

![כרזה המצביעים על https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

אם עדיין לא יצרת קבוצות מכשירים או פרופילים, הדרך הטובה ביותר להתחיל היא באמצעות מדריך צעד-אחר-צעד, אך תוכל גם [להוסיף מכשירים](create-and-edit-autopilot-devices.md) ו [להקצות להם פרופילים](create-and-edit-autopilot-profiles.md) מבלי להשתמש במדריך. 
  
1. עבור אל מרכז admin ב <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.

2. בסרגל ניווט השמאלי לבחור **התקנים** \> **AutoPilot**.

    ![במרכז admin לבחור התקנים ולאחר מכן AutoPilot.](media/AutoPilot.png)
  
2. בדף **AutoPilot** , לחץ או הקש על **מדריך התחלה**.
    
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
    