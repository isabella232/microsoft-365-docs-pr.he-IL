---
title: עריכה או הגדרה של הגדרות הגנה על יישומים עבור Windows 10 אחרים
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: למד כיצד ליצור או לערוך מדיניות ניהול יישומים ולהגן על קבצי עבודה במכשירים האישיים של המשתמשים Windows 10 שלך.
ms.openlocfilehash: 6d38d1765e0a331516b2261870112d530ab4ee50f24c6defba95964ea4d9dcfa
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53852643"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a>הגדרה או עריכה של הגדרות הגנה על יישומים עבור Windows 10 אחרים

מאמר זה חל על Microsoft 365 Business Premium.

## <a name="edit-an-app-management-policy-for-windows-10"></a>עריכת מדיניות ניהול יישומים עבור Windows 10

1. עבור אל מרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> ב- .     
2. בסרגל הניווט הימני, בחר **מדיניות** \> **מכשירים** .
1. בחר מדיניות קיימת של Windows אפליקציה ולאחר מכן **ערוך**.
1. בחר **ערוך** לצד הגדרה שברצונך לשנות ולאחר מכן **שמור**.

## <a name="create-an-app-management-policy-for-windows-10"></a>יצירת מדיניות לניהול יישומים עבור Windows 10

אם למשתמשים שלך יש מכשירים אישיים של Windows 10 שהם מבצעים דרכם משימות עבודה, באפשרותך להגן על הנתונים שלך גם במכשירים אלה.
  
1. עבור אל מרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> ב- . 
2. בסרגל הניווט הימני, בחר **מדיניות** \> **מכשירים** \> **הוסף**.
3. בחלונית **הוסף מדיניות**, הזן שם ייחודי עבור מדיניות זו. 
4. תחת **סוג מדיניות**, בחר **ניהול יישומים עבור Windows 10**.
5. תחת **סוג מכשיר**, בחר אישי **או** **בבעלות חברה.**
6. האפשרות **הצפן קבצי עבודה** מופעלת באופן אוטומטי. 
7. קבע את ההגדרה **מנע ממשתמשים להעתיק נתוני חברה לקבצים אישיים וכפה עליהם לשמור קבצי עבודה ב- OneDrive for Business** למצב **מופעל** אם אינך מעוניין שהמשתמשים ישמרו קבצי עבודה במחשב שלהם. 
9. הרחב **את שחזור נתונים במכשירי Windows אחרים.** מומלץ להפעיל **אותו.**
    לפני שתוכל לנווט אל מיקום האישור של סוכן שחזור הנתונים, עליך תחילה ליצור את האישור. לקבלת הוראות, ראה יצירה ואימות של אישור סוכן שחזור נתונים (DRA) של מערכת קבצים [מצפינה (EFS).](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)
    
    כברירת מחדל, קבצי עבודה מוצפנים באמצעות מפתח סודי שמאוחסן במכשיר ומשויך לפרופיל של המשתמש. רק המשתמש יכול לפתוח ולפענח את הקובץ. עם זאת, במקרה של אובדן המכשיר או הסרת משתמש, הקובץ יכול להיתקע במצב מוצפן. מנהל מערכת יכול להשתמש באישור סוכן שחזור נתונים (DRA) כדי לפענח את הקובץ.
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. הרחב **את הגן על מיקומי רשת** וענן נוספים אם ברצונך להוסיף תחומים נוספים או SharePoint מיקומים מקוונים כדי לוודא שהקבצים בכל האפליקציות המפורטות מוגנים. אם עליך להזין יותר מפריט אחד עבור שדה כלשהו, השתמש בנקודה-פסיק (;) בין הפריטים.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. לאחר מכן החלט **מי יקבל הגדרות אלה?** אם אינך מעוניין להשתמש בקבוצת האבטחה המוגדרת כברירת מחדל **כל המשתמשים**, בחר **שינוי**, בחר את קבוצות האבטחה שיקבלו הגדרות אלה \> **בחר**.
12. לבסוף, בחר **הוסף** כדי לשמור את המדיניות והקצה אותה למכשירים.