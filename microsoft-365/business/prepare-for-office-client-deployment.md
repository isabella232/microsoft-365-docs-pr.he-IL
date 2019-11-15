---
title: הכנה לפריסת לקוח של Office על-ידי Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: למד כיצד להתקין באופן אוטומטי את יישומי Office 32-bit במחשבי Windows 10 ולעדכן אותם.
ms.openlocfilehash: 09857ddeb28e953da07979045a65f6b91925aeaf
ms.sourcegitcommit: 2c2248b03f7753d64490f2f7e56ec644a235b65a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/15/2019
ms.locfileid: "38640768"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>הכנה לפריסת לקוח של Office על-ידי Microsoft 365 Business

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>הכנה להתקנה אוטומטית של יישומי Office במחשבי לקוח

באפשרותך להשתמש ב-Microsoft 365 Business כדי להתקין באופן אוטומטי את יישומי Office מסוג 32-bit במחשבי Windows 10 ולשמור אותם עדכניים באמצעות עדכונים.
  
ההתקנה האוטומטית פועלת באופן הטוב ביותר אם המחשב של משתמש הקצה הוא ב-Windows 10 Business ו:
  
- הוא אינו כולל יישומים שולחניים קיימים של Office (‏Word, ‏Excel, ‏PowerPoint, ‏Outlook, ‏OneNote, ‏Publisher, ‏Access ו- OneDrive).
    
    או
    
- מותקנת בו גירסה קיימת של Office מסוג 'לחץ והפעל'.
    
כדי לקבוע אם יש לך גירסת 'לחץ והפעל' של Office, בכל יישום של Office, עבור אל **קובץ** \> **חשבון** ( **חשבון Office** ב- Outlook). אם אתה רואה **עדכונים של Office** כפי שמוצג באיור הבא, ההתקנה נעשתה על-ידי שימוש בלחיצה-להפעלה. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **שנהנה מתכונה זו**
  
משתמש קצה שהמחשב שלו:
  
- **כולל** רשיון משתמש של Windows 10 Business, רשיון פעיל של Microsoft 365 Business, עדכון Windows 10 ליוצרים ושהמחשב שלו מצורף ל- Azure Active Directory. 
    
- אין **ברשותך** יישומי Office 64-bit (לדוגמה: Word, Excel, PowerPoint). אם 64-bit apps Office נדרשים, תכונה זו אינה מתאימה בכלל, משום שאין תמיכה בהפעלת גירסה 64-bit 2016 לחץ-להפעלה של Office מתוך מסוף מנהל העסקים של Microsoft 365. 
    
- **אינו כולל** יישומים עצמאיים של Windows Installer (MSI) 2016 (לדוגמה, Visio או Project). Microsoft 365 עסקים שדרוגים Office לגירסת הלחיצה-אל-הפעל של Office 2016 ושאינה פועלת עם יישומים עצמאיים של Office 2016 MSI. 
    
הטבלה הבאה מציגה את הפעולה שייתכן שמשתמשי הקצה/מנהלים יצטרכו לבצע, בהתאם למצב ההתחלה שלהם, לקבל גירסה מוצלחת של 32 סיביות להפעלה של פריסת Office ממסוף הניהול העסקי של Microsoft 365.
  
|**הפעלת מצב ההתקנה של Office**|**הפעולה שיש לנקוט לפני התקנת Office עבור Microsoft 365 Business**|**מצב סיום**|
|:-----|:-----|:-----|
|לא הותקנה חבילת Office  <br/> |ללא  <br/> |Office 2016 32-bit מותקן באמצעות ' לחץ להפעלה '  <br/> |
|גירסת 'לחץ והפעל' קיימת של Office מסוג 32 סיביות (2016 או גירסה קודמת) וללא יישומים עצמאיים  <br/> |ללא  <br/> |שדרוג לגירסת 'לחץ והפעל' האחרונה של Office 2016 מסוג 32 סיביות, לפי הצורך **\*** <br/> |
|גירסת לחיצה על הפעלה מסוג 32-bit של Office ולחיצה-להפעלה קיימת, 32-bit או 64-bit של יישומי Office עצמאיים (לדוגמה, Visio, Project)  <br/> |ללא  <br/> |יישומים עצמאיים אינם מושפעים. שדרוג החבילה לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות  <br/> |
|גירסת 'לחץ והפעל' קיימת של Office מסוג 32 סיביות ויישומי Office עצמאיים של MSI מסוג 32 או 64 סיביות (למעט 2016)  <br/> |ללא  <br/> |יישומים עצמאיים אינם מושפעים. שדרוג החבילה לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות  <br/> ||||
|גירסת 'לחץ והפעל' קיימת של Office מסוג 64 סיביות  <br/> |הסר את ההתקנה של יישומי Office 64-bit, אם זה בסדר להחליף אותם ביישומי Office בעלי 32 סיביות  <br/> |אם אתה מסיר את יישומי Office מסוג 64 סיביות, גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות מותקנת  <br/> |
|התקנת MSI קיימת של Office 2016 עם או בלי יישומים עצמאיים  <br/> |הסרת התקנה של MSI Office 2016.  <br/> |מותקנת גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות. ללא שינוי ביישומים עצמאיים  <br/> |
|התקנת MSI קיימת של Office 2013 (או גירסה קודמת) ו/או יישומי Office עצמאיים  <br/> |ללא  <br/> |גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות עם התקנת MSI Office קיימת מראש (ויישומים עצמאיים) מתקיימות זו לצד זו  <br/> |
||||
   
 **(\*) הערה:** לא מתקיים שדרוג לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות עקב באג ידוע. . התיקון מתבצע 
  