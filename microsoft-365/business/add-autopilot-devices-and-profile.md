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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: למד כיצד להשתמש ב-Windows באופן אוטומטי כדי להגדיר מכשירים חדשים של Windows 10 עבור העסק שלך, כך שהם יהיו מוכנים לשימוש בעובדים.
ms.openlocfilehash: f263cc90656ae5e7be1a89e3c7f56bfb2d0e3651
ms.sourcegitcommit: 3b369a44b71540c8b8214ce588a7aa6f47c3bb1e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/04/2021
ms.locfileid: "50099749"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>שימוש במדריך שלב אחר שלב להוספת מכשירים ופרופיל של Autopilot

באפשרותך להשתמש ב-Windows בטייס אוטומטי כדי להגדיר מכשירים **חדשים** של windows 10 עבור העסק שלך, כך שהם יהיו מוכנים לשימוש כאשר אתה מעניק אותם לעובדים שלך.
  
## <a name="device-requirements"></a>דרישות המכשירים

המכשירים חייבים לעמוד בדרישות אלה:
  
- Windows 10, גירסה 1703 ואילך
    
- מכשירים חדשים שאינם מותקנים בחוויית Windows out-of-box
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>שימוש במדריך ההתקנה ליצירת מכשירים ופרופילים

[![תווית המיידעת אותך שמרכז הניהול משתנה ושניתן למצוא פרטים נוספים ב- aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

אם עדיין לא יצרת קבוצות מכשירים או פרופילים, הדרך הטובה ביותר להתחיל היא באמצעות מדריך שלב אחר שלב. באפשרותך גם [להוסיף מכשירים](create-and-edit-autopilot-devices.md) ולהקצות להם [פרופילים](create-and-edit-autopilot-profiles.md) ללא שימוש במדריך. 
  
1. עבור אל מרכז הניהול ב <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> -.

2. בחלונית הניווט הימנית, בחר **מכשירים** \> **טייס אוטומטי**.

    ![במרכז הניהול, בחר התקנים ולאחר מכן לחץ על אוטומטי.](../media/AutoPilot.png)
  
2. בדף **הטייס האוטומטי** , לחץ או הקש על **התחל מדריך**.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. בדף **העלאת קובץ. csv עם רשימת מכשירים** , אתר את המיקום שבו אתה מוכן. קובץ CSV ולאחר מכן **פתח את** \> **הבא**. הקובץ חייב לכלול שלוש כותרות:
    
    - עמודה א: מספר סידורי של המכשיר
    
    - עמודה ב: מזהה המוצר של Windows
    
    - עמודה ג: קוד Hash של החומרה
    
    באפשרותך לקבל מידע זה מספק החומרה, או להשתמש [בסקריפט get-Windowsautopilotinfohttps PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) כדי ליצור קובץ CSV. 
    
    למידע נוסף, ראה [קובץ CSV עם רשימת מכשירים](https://docs.microsoft.com/microsoft-365/admin/misc/device-list). באפשרותך גם להוריד קובץ לדוגמה בדף **העלאת קובץ ‎.csv עם רשימת מכשירים**. 
    
> [!NOTE]
> קובץ script זה משתמש ב-WMI כדי לאחזר מאפיינים הדרושים עבור לקוח כדי לרשום מכשיר באמצעות הטייס האוטומטי של Windows. שים לב שהוא נורמלי עבור קובץ ה-CSV שנוצר כדי לא לאסוף ערך של מזהה מוצר של Windows (PKID) מאחר שאין צורך לרשום מכשיר וPKID להיות NULL ב-CSV של הפלט הוא בסדר גמור. רק המספר הסידורי וגיבוב החומרה יאוכלסו.
    
4. בדף **הקצאת פרופיל** , באפשרותך לבחור פרופיל קיים או ליצור פרופיל חדש. אם עדיין אין לך אחד, תתבקש ליצור אחד. 
    
    פרופיל הוא אוסף הגדרות שניתן להחיל על מכשיר בודד או על קבוצה של מכשירים.
    
    תכונות ברירת המחדל נדרשות ומוגדרות באופן אוטומטי. תכונות ברירת המחדל הן:
    
    - דלג על Cortana, OneDrive ורישום OEM.
    
    - יצירת חוויית כניסה עם מותג החברה.
    
    - חבר את המכשירים שלך לחשבונות התכלת של Active Directory ורשום אותם באופן אוטומטי כדי לנהל אותם על-ידי Microsoft 365 Business Premium.
    
    לקבלת מידע נוסף, ראה [אודות הגדרות פרופיל טייס אוטומטי](autopilot-profile-settings.md). 
    
5. שאר ההגדרות הן **דלג על הגדרות פרטיות** ו **אל תאפשר למשתמש להפוך למנהל המערכת המקומי**. שתי הגדרות אלה מוגדרות למצב **כבוי** כברירת מחדל. 
    
    בחר **הבא**.
    
6. **סיימת** מציינת שהפרופיל שיצרת (או שבחרת) יוחל על קבוצת ההתקנים שיצרת על-ידי העלאת רשימת המכשירים. ההגדרות ייכנסו לתוקף כאשר משתמשי המכשיר ייכנסו לשלב הבא. בחר **סגור**.
    
