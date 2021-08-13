---
title: התכונן Office הלקוח על-ידי Microsoft 365 לעסקים
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: למד כיצד להתקין באופן אוטומטי את יישומי גירסת 32 Office במחשבי Windows 10 ולעדכן אותם.
ms.openlocfilehash: 134d5f2918e3f28c2025b282b9ae0325b64fe0474ae8123d0637bb43c4730c55
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53803549"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>התכונן Office הלקוח על-ידי Microsoft 365 לעסקים

מאמר זה חל על Microsoft 365 Business Premium.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>הכנה להתקנה אוטומטית של יישומי Office במחשבי לקוח

באפשרותך להשתמש ב- Microsoft 365 Business Premium כדי להתקין באופן אוטומטי את יישומי גירסת 32 Office במחשבי Windows 10 ולהתעדכן בהם עם עדכונים.
  
ההתקנה האוטומטית פועלת בצורה הטובה ביותר אם המחשב של משתמש הקצה Windows 10 Business ו:
  
- הוא אינו כולל יישומים שולחניים קיימים של Office (‏Word, ‏Excel, ‏PowerPoint, ‏Outlook, ‏OneNote, ‏Publisher, ‏Access ו- OneDrive).
    
    או
    
- מותקנת בו גירסה קיימת של Office מסוג 'לחץ והפעל'.
    
כדי לקבוע אם יש לך גירסת 'לחץ והפעל' של Office, בכל יישום של Office, עבור אל **קובץ** \> **חשבון** ( **חשבון Office** ב- Outlook). אם אתה רואה **Office כפי** שמוצג באיור הבא, ההתקנה ת בוצע באמצעות 'לחץ הפעל'. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **מי יתרונות מתכונה זו**
  
משתמש קצה שהמחשב שלו:
  
- **כולל** Windows 10 Business משתמש, רשיון Microsoft 365 עבור העסק, עדכון Windows 10 ליוצרים ומצורף ל- Azure Active Directory. 
    
- **אין לו אפליקציות של** 64 Office (לדוגמה: Word, Excel, PowerPoint). אם אפליקציות Office של 64 סיביות נדרשות, תכונה זו אינה מתאימה מכיוון שאין תמיכה בהפצת גירסת 'לחץ הפעל' של 64 סיביות של Office ממסוף הניהול של Microsoft 365 לעסקים. 
    
- **אינו כולל** יישומים עצמאיים של Windows Installer (MSI) 2016 (לדוגמה, Visio או Project). Microsoft 365 עבור שדרוגים עסקיים Office לגירסה 'לחץ הפעל' של Office 2016 וזה לא עובד עם אפליקציות עצמאיות של Office 2016 MSI. 
    
הטבלה הבאה מציגה את הפעולה שמשתמשי הקצה/מנהלי המערכת עשויים לנקוט, בהתאם למצב ההתחלה שלהם, כדי לקבל גירסת 'לחץ הפעל' מוצלחת של 32 סיביות של פריסת Office ממסוף הניהול של Microsoft 365 לעסקים.<br/>


|הפעלת מצב ההתקנה של Office|פעולה יש לבצע לפני Microsoft 365 לעסקים Office התקנה|מצב סיום|
|:-----|:-----|:-----|
|לא הותקנה חבילת Office  <br/> |ללא  <br/> |Office 2016 גירסת 32 סיביות מותקנת באמצעות 'לחץ הפעל'  <br/> |
|גירסת 'לחץ והפעל' קיימת של Office מסוג 32 סיביות (2016 או גירסה קודמת) וללא יישומים עצמאיים  <br/> |ללא  <br/> |שדרוג לגירסת 'לחץ והפעל' האחרונה של Office 2016 מסוג 32 סיביות, לפי הצורך **\*** <br/> |
|גירסת 32 סיביות קיימת של 'לחץ הפעל' של Office ו'לחץ על הפעלה' של 32 סיביות או 64 סיביות Office עצמאיות (לדוגמה, Visio, Project)  <br/> |ללא  <br/> |אפליקציות עצמאיות אינן מושפעות. שדרוג החבילה לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות  <br/> |
|גירסת 'לחץ והפעל' קיימת של Office מסוג 32 סיביות ויישומי Office עצמאיים של MSI מסוג 32 או 64 סיביות (למעט 2016)  <br/> |ללא  <br/> |אפליקציות עצמאיות אינן מושפעות. שדרוג החבילה לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות  <br/> |
|גירסת 'לחץ והפעל' קיימת של Office מסוג 64 סיביות  <br/> |הסרת ההתקנה של אפליקציות Office של 64 סיביות, אם זה בסדר להחליף אותן באפליקציות של 32 Office סיביות  <br/> |אם אתה מסיר את יישומי Office מסוג 64 סיביות, גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות מותקנת  <br/> |
|התקנת MSI קיימת של Office 2016 עם או בלי יישומים עצמאיים  <br/> |הסרת התקנה של MSI Office 2016.  <br/> |מותקנת גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות. ללא שינוי ביישומים עצמאיים  <br/> |
|התקנת MSI קיימת של Office 2013 (או גירסה קודמת) ו/או יישומי Office עצמאיים  <br/> |ללא  <br/> |גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות עם התקנת MSI Office קיימת מראש (ויישומים עצמאיים) מתקיימות זו לצד זו  <br/> |
||||
   
 **(\*) הערה:** לא מתקיים שדרוג לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות עקב באג ידוע. מתבצע תיקון. 
  
