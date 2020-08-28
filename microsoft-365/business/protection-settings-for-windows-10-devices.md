---
title: עריכה או הגדרה של הגדרות הגנה של יישומים עבור מכשירי Windows 10
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
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
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: למד כיצד ליצור או לערוך מדיניות של ניהול יישומים ולהגן על קבצי עבודה במכשירי Windows 10 אישיים של משתמשים.
ms.openlocfilehash: f85a59649e43c141b62091337b842a490d411833
ms.sourcegitcommit: abf63669daf12993ad3353e4b578f41c8910b20f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/27/2020
ms.locfileid: "47289198"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a>הגדרה או עריכה של הגדרות הגנה של יישומים עבור מכשירי Windows 10

מאמר זה חל על Microsoft 365 Business Premium.

## <a name="edit-an-app-management-policy-for-windows-10"></a>עריכת מדיניות ניהול יישומים עבור Windows 10

1. עבור אל מרכז הניהול ב <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> -.     
2. בסרגל הניווט הימני **Devices** , בחר \> **מדיניות** מכשירים.
1. בחר מדיניות קיימת של Windows app ולאחר מכן **ערוך**.
1. בחר **ערוך** לצד הגדרה שברצונך לשנות ולאחר מכן **שמור**.

## <a name="create-an-app-management-policy-for-windows-10"></a>יצירת מדיניות לניהול יישומים עבור Windows 10

אם למשתמשים שלך יש מכשירים אישיים של Windows 10 שהם מבצעים דרכם משימות עבודה, באפשרותך להגן על הנתונים שלך גם במכשירים אלה.
  
1. עבור אל מרכז הניהול ב <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> -. 
2. בסרגל הניווט הימני **Devices** , בחר באפשרות \> הוסף **מדיניות** מכשירים \> **Add**.
3. בחלונית **הוסף מדיניות**, הזן שם ייחודי עבור מדיניות זו. 
4. תחת **סוג מדיניות**, בחר **ניהול יישומים עבור Windows 10**.
5. תחת **סוג מכשיר**, בחר **אישית** או **חברה בבעלות**.
6. האפשרות **הצפן קבצי עבודה** מופעלת באופן אוטומטי. 
7. קבע את ההגדרה **מנע ממשתמשים להעתיק נתוני חברה לקבצים אישיים וכפה עליהם לשמור קבצי עבודה ב- OneDrive for Business** למצב **מופעל** אם אינך מעוניין שהמשתמשים ישמרו קבצי עבודה במחשב שלהם. 
9. הרחב את **שחזור הנתונים במכשירי Windows**. **מומלץ להפעיל**אותה.
    לפני שתוכל לנווט אל מיקום האישור של סוכן שחזור הנתונים, עליך תחילה ליצור את האישור. לקבלת הוראות, ראה [יצירה ואימות של אישור סוכן שחזור נתונים (EFS) של מערכת קבצים מצפינה (EFS](https://go.microsoft.com/fwlink/p/?linkid=853700)).
    
    כברירת מחדל, קבצי עבודה מוצפנים באמצעות מפתח סודי שמאוחסן במכשיר ומשויך לפרופיל של המשתמש. רק המשתמש יכול לפתוח ולפענח את הקובץ. עם זאת, במקרה של אובדן המכשיר או הסרת משתמש, הקובץ יכול להיתקע במצב מוצפן. מנהל מערכת יכול להשתמש באישור סוכן שחזור נתונים (DRA) כדי לפענח את הקובץ.
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. הרחב את **ההגנה על מיקומים נוספים ברשת ובענן** אם ברצונך להוסיף תחומים נוספים או מיקומים של SharePoint Online כדי לוודא שהקבצים בכל היישומים הרשומים מוגנים. אם עליך להזין יותר מפריט אחד עבור שדה כלשהו, השתמש בנקודה-פסיק (;) בין הפריטים.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. לאחר מכן החלט **מי יקבל הגדרות אלה?** אם אינך מעוניין להשתמש בקבוצת האבטחה המוגדרת כברירת מחדל **כל המשתמשים**, בחר **שינוי**, בחר את קבוצות האבטחה שיקבלו הגדרות אלה \> **בחר**.
12. לבסוף, בחר **הוסף** כדי לשמור את המדיניות והקצה אותה למכשירים. 
