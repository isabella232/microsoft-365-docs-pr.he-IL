---
title: שימוש במדריך שלב אחר שלב להוספת מכשירים ופרופיל של Autopilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: למד כיצד להשתמש ב Windows AutoPilot כדי להגדיר מכשירי Windows 10 חדשים עבור העסק שלך כך שהם מוכנים לשימוש של עובדים.
ms.openlocfilehash: f160ddcd1e41bd44c908ecc8bbd30a9819f76902
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/12/2021
ms.locfileid: "53393438"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>שימוש במדריך שלב אחר שלב להוספת מכשירים ופרופיל של Autopilot

באפשרותך להשתמש Windows AutoPilot כדי **להגדיר** מכשירי Windows 10 חדשים עבור העסק שלך כך שהם מוכנים לשימוש כאשר אתה נותן אותם לעובדים שלך.
  
## <a name="device-requirements"></a>דרישות המכשירים

מכשירים חייבים לעמוד בדרישות הבאות:
  
- Windows 10, גירסה 1703 ואילך
    
- מכשירים חדשים שלא עברו Windows חוויה מחוץ לקופסה
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>שימוש במדריך ההתקנה ליצירת מכשירים ופרופילים

אם עדיין לא יצרת קבוצות מכשירים או פרופילים, הדרך הטובה ביותר להתחיל היא באמצעות מדריך שלב אחר שלב. באפשרותך גם [להוסיף מכשירים](create-and-edit-autopilot-devices.md) [ולהקצות להם](create-and-edit-autopilot-profiles.md) פרופילים מבלי להשתמש במדריך. 
  
1. עבור אל מרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> ב- .

2. בחלונית הניווט הימנית, בחר  \> **מכשירים AutoPilot**.

    ![במרכז הניהול, בחר מכשירים ולאחר מכן בחר AutoPilot.](../media/AutoPilot.png)
  
2. בדף **AutoPilot,** לחץ או הקש על **מדריך התחלה**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. בדף Upload .csv **עם רשימת מכשירים,** עבור אל מיקום שבו יש לך את קובץ .CSV מוכן ולאחר מכן **פתח את** \> **הבא**. לקובץ חייבות להיות שלוש כותרות:
    
    - עמודה א: מספר סידורי של המכשיר
    
    - עמודה ב: מזהה המוצר של Windows
    
    - עמודה ג: קוד Hash של החומרה
    
    באפשרותך לקבל מידע זה מספק החומרה שלך, או להשתמש בקובץ [ה- Script Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) כדי ליצור קובץ CSV. 
    
    למידע נוסף, ראה [קובץ CSV עם רשימת מכשירים](../admin/misc/device-list.md). באפשרותך גם להוריד קובץ לדוגמה בדף **העלאת קובץ ‎.csv עם רשימת מכשירים**. 
    
> [!NOTE]
> קובץ Script זה משתמש ב- WMI כדי לאחזר מאפיינים הדרושים ללקוח כדי לרשום מכשיר באמצעות Windows Autopilot. שים לב שקובץ ה- CSV שנוצר אינו אוסף ערך של מזהה מוצר (PKID) של Windows מאחר שקובץ זה אינו נדרש לרישום מכשיר, ו- PKID הוא NULL ב- CSV של הפלט. רק המספר הסידורי ו- Hash של החומרה יאוכלסו.
    
4. בדף **הקצאת פרופיל,** באפשרותך לבחור פרופיל קיים או ליצור פרופיל חדש. אם עדיין אין לך אחד, תתבקש ליצור אחד. 
    
    פרופיל הוא אוסף הגדרות שניתן להחיל על מכשיר בודד או על קבוצה של מכשירים.
    
    תכונות ברירת המחדל נדרשות ומוגדרות באופן אוטומטי. תכונות ברירת המחדל הן:
    
    - דלג Cortana, OneDrive ורישום OEM.
    
    - יצירת חוויית כניסה עם מותג החברה.
    
    - התחברות את המכשירים שלך לחשבונות Azure Active Directory ורשום אותם באופן אוטומטי כדי להיות מנוהלים על-ידי Microsoft 365 Business Premium.
    
    לקבלת מידע נוסף, ראה [אודות הגדרות פרופיל AutoPilot](autopilot-profile-settings.md). 
    
5. שאר ההגדרות הן **דלג על הגדרות פרטיות** ו **אל תאפשר למשתמש להפוך למנהל המערכת המקומי**. שתי הגדרות אלה מוגדרות למצב **כבוי** כברירת מחדל. 
    
    בחר **הבא**.
    
6. **סיימת מציין** שהפרופיל שיצרת (או בחרת) יוחל על קבוצת המכשירים שיצרת על-ידי העלאת רשימת המכשירים. ההגדרות יהיו בתוקף כאשר המשתמשים במכשיר יתו בפעם הבאה. בחר **סגור**.

## <a name="related-content"></a>תוכן קשור

[אודות הגדרות פרופיל AutoPilot](autopilot-profile-settings.md) (מאמר)\
[אפשרויות להגנה על המכשירים ותוני האפליקציה](../admin/devices/choose-device-security.md) שלך (מאמר)
