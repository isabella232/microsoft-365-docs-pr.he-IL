---
title: שימוש במדריך שלב אחר שלב להוספת מכשירים ופרופיל של Autopilot
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: למד כיצד להשתמש בטייס אוטומטי של Windows כדי להגדיר התקנים חדשים של Windows 10 עבור העסק שלך כך שהם מוכנים לשימוש בעובדים.
ms.openlocfilehash: de14012ebf9e7cdd22e41505f316ab665773c670
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165880"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>שימוש במדריך שלב אחר שלב להוספת מכשירים ופרופיל של Autopilot

באפשרותך להשתמש בטייס אוטומטי של Windows כדי להגדיר windows **חדש** 10 התקנים עבור העסק שלך כך שהם מוכנים לשימוש כאשר אתה נותן אותם לעובדים שלך.
  
## <a name="device-requirements"></a>דרישות המכשירים

על התקנים לעמוד בדרישות הבאות:
  
- Windows 10, גירסה 1703 ואילך
    
- מכשירים חדשים שלא עברו חוויה מחוץ לקופסא של Windows
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>שימוש במדריך ההתקנה ליצירת מכשירים ופרופילים

[![תווית המיידעת אותך שמרכז הניהול משתנה ושניתן למצוא פרטים נוספים ב- aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

אם עדיין לא יצרת קבוצות או פרופילים של התקנים, הדרך הטובה ביותר להתחיל היא באמצעות המדריך צעד-אחר-צעד. באפשרותך גם [להוסיף התקנים](create-and-edit-autopilot-devices.md) [ולהקצות אליהם פרופילים](create-and-edit-autopilot-profiles.md) מבלי להשתמש במדריך. 
  
1. <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. לך למרכז המנהלה

2. בחלונית הניווט השמאלית, בחר באפשרות **התקנים** \> **טייס אוטומטי**.

    ![במרכז הניהול, בחר התקנים ולאחר מכן טייס אוטומטי.](../media/AutoPilot.png)
  
2. בעמוד **הטייס האוטומטי** , לחץ או הקש על **התחל מדריך**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. בקובץ **העלאה. csv עם רשימת ההתקנים** , אתר את המיקום שבו הכנת את הרשימה. קובץ CSV ולאחר מכן **פתח את** \> **הבא**. הקובץ חייב לכלול שלוש כותרות:
    
    - עמודה א: מספר סידורי של המכשיר
    
    - עמודה ב: מזהה המוצר של Windows
    
    - עמודה ג: קוד Hash של החומרה
    
    אתה יכול לקבל את המידע הזה מספק החומרה שלך, או שאתה יכול להשתמש [בסקריפט לקבל-Windowsautopilinfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) כדי ליצור קובץ CSV. 
    
    למידע נוסף, ראה [קובץ CSV עם רשימת מכשירים](https://docs.microsoft.com/microsoft-365/admin/misc/device-list). באפשרותך גם להוריד קובץ לדוגמה בדף **העלאת קובץ ‎.csv עם רשימת מכשירים**. 
    
4. בדף **הקצאת פרופיל** , באפשרותך לבחור פרופיל קיים או ליצור דף חדש. אם עדיין אין לך אחד, תתבקש ליצור אחד. 
    
    פרופיל הוא אוסף הגדרות שניתן להחיל על מכשיר בודד או על קבוצה של מכשירים.
    
    תכונות ברירת המחדל נדרשות ומוגדרות באופן אוטומטי. תכונות ברירת המחדל הן:
    
    - לדלג קורטנה, OneDrive, ו-OEM רישום.
    
    - יצירת חוויית כניסה עם מותג החברה.
    
    - חבר את המכשירים שלך לחשבונות מדריך הפעלה התכלת, ורשום אותם באופן אוטומטי כדי שינוהל על-ידי Microsoft 365 Business Premium.
    
    לקבלת מידע נוסף, ראה [אודות הגדרות פרופיל טייס אוטומטי](autopilot-profile-settings.md). 
    
5. שאר ההגדרות הן **דלג על הגדרות פרטיות** ו **אל תאפשר למשתמש להפוך למנהל המערכת המקומי**. שתי הגדרות אלה מוגדרות למצב **כבוי** כברירת מחדל. 
    
    בחר **הבא**.
    
6. **סיימת** מציין שהפרופיל שיצרת (או בחרת) יוחל על קבוצת ההתקנים שיצרת על-ידי טעינת רשימת ההתקנים. ההגדרות ייכנסו לתוקף כאשר משתמשי ההתקן ייכנסו בשלב הבא. בחר **סגור**.
    
