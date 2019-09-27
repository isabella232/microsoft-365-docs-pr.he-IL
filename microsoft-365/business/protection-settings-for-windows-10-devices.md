---
title: קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: למד כיצד ליצור מדיניות ניהול יישומים ולהגן על קבצי עבודה בהתקני Windows 10.
ms.openlocfilehash: 92cd3facbd3eabbfef674300abe0257c370294ea
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288414"
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
    
9. הרחב את **שחזר נתונים במכשירי Windows** ומומלץ להגדיר את האפשרות למצב **מופעל**.
    
    לפני שתוכל לנווט אל מיקום האישור של סוכן שחזור הנתונים, עליך תחילה ליצור את האישור. לקבלת הוראות עיין בנושא [יצירה ואימות של אישור מסוג מערכת קבצים מצפינה (EFS) סוכן שחזור נתונים (DRA)](https://go.microsoft.com/fwlink/p/?linkid=853700).
    
    כברירת מחדל, קבצי עבודה מוצפנים באמצעות מפתח סודי שמאוחסן במכשיר ומשויך לפרופיל של המשתמש. רק המשתמש יכול לפתוח ולפענח את הקובץ. עם זאת, במקרה של אובדן המכשיר או הסרת משתמש, הקובץ יכול להיתקע במצב מוצפן. מנהל מערכת יכול להשתמש באישור של סוכן שחזור נתונים (DRA) כדי לפענח את הקובץ.
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. הרחב את **הגן על מיקומים נוספים ברשת ובענן** אם ברצונך להוסיף תחומים נוספים או מיקומים נוספים של SharePoint Online כדי לוודא שהקבצים בכל היישומים המפורטים יהיו מוגנים. אם עליך להזין יותר מפריט אחד עבור שדה כלשהו, השתמש בנקודה-פסיק (;) בין הפריטים.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. לאחר מכן החלט **מי יקבל הגדרות אלה?** אם אינך מעוניין להשתמש בקבוצת האבטחה המוגדרת כברירת מחדל **כל המשתמשים**, בחר **שינוי**, בחר את קבוצות האבטחה שיקבלו הגדרות אלה \> **בחר**.
    
12. לבסוף, בחר **הוסף** כדי לשמור את המדיניות והקצה אותה למכשירים. 