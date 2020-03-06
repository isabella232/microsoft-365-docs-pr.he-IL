---
title: קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: למד כיצד ליצור מדיניות ניהול יישומים ולהגן על קבצי עבודה בהתקני Windows 10 האישיים של המשתמשים שלך.
ms.openlocfilehash: ce389980ceb8bd889214404b0c48769380044bcf
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550206"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a>קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10

## <a name="create-an-app-management-policy-for-windows-10"></a>יצירת מדיניות לניהול יישומים עבור Windows 10

אם למשתמשים שלך יש מכשירים אישיים של Windows 10 שהם מבצעים דרכם משימות עבודה, באפשרותך להגן על הנתונים שלך גם במכשירים אלה.
  
1. <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. לך למרכז המנהלה 
    
2. בניווט השמאלי, בחר באפשרות **מדיניות** \> **** **התקנים** \> .

3. בחלונית **הוסף מדיניות**, הזן שם ייחודי עבור מדיניות זו. 
    
4. תחת **סוג מדיניות**, בחר **ניהול יישומים עבור Windows 10**.
    
5. תחת **סוג התקן**, בחר בבעלות **אישית** או **בחברה**.
    
6. האפשרות **הצפן קבצי עבודה** מופעלת באופן אוטומטי. 
    
7. קבע את ההגדרה **מנע ממשתמשים להעתיק נתוני חברה לקבצים אישיים וכפה עליהם לשמור קבצי עבודה ב- OneDrive for Business** למצב **מופעל** אם אינך מעוניין שהמשתמשים ישמרו קבצי עבודה במחשב שלהם. 
    
9. הרחב **שחזור נתונים בהתקני Windows**. **מומלץ**להדליק אותו.
    
    לפני שתוכל לנווט אל מיקום האישור של סוכן שחזור הנתונים, עליך תחילה ליצור את האישור. לקבלת הוראות, ראה [יצירה ואימות של אישור סוכן שחזור נתונים (DRA) של מערכת קבצים מצפינה (EFS](https://go.microsoft.com/fwlink/p/?linkid=853700)).
    
    כברירת מחדל, קבצי עבודה מוצפנים באמצעות מפתח סודי שמאוחסן במכשיר ומשויך לפרופיל של המשתמש. רק המשתמש יכול לפתוח ולפענח את הקובץ. עם זאת, במקרה של אובדן המכשיר או הסרת משתמש, הקובץ יכול להיתקע במצב מוצפן. מנהל יכול להשתמש באישור סוכן שחזור נתונים (DRA) כדי לפענח את הקובץ.
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. הרחב את **הגן על מיקומי רשת וענן נוספים** אם ברצונך להוסיף תחומים נוספים או מיקומים מקוונים של SharePoint כדי לוודא שהקבצים בכל היישומים המפורטים מוגנים. אם עליך להזין יותר מפריט אחד עבור שדה כלשהו, השתמש בנקודה-פסיק (;) בין הפריטים.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. לאחר מכן החלט **מי יקבל הגדרות אלה?** אם אינך מעוניין להשתמש בקבוצת האבטחה המוגדרת כברירת מחדל **כל המשתמשים**, בחר **שינוי**, בחר את קבוצות האבטחה שיקבלו הגדרות אלה \> **בחר**.
    
12. לבסוף, בחר **הוסף** כדי לשמור את המדיניות והקצה אותה למכשירים. 
