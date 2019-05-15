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
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: למד כיצד להתקין את יישומי Office של 32 סיביות במחשבים Windows 10 וכיצד במצב עדכני.
ms.openlocfilehash: 20269c493b0e3b5a7deb56a24a5e1a9583ef9d0a
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074649"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>הכנה לפריסת לקוח של Office על-ידי Microsoft 365 Business

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>הכנה להתקנה אוטומטית של יישומי Office במחשבי לקוח

באפשרותך להשתמש ב- Microsoft 365 Business כדי להתקין באופן אוטומטי את יישומי Office בגירסת 32 סיביות במחשבי Windows 10 ולהבטיח שהם עדכניים תמיד בעזרת עדכונים.
  
מוטב שהמחשב של משתמש הקצה יופעל באמצעות Windows 10 Business וכן:
  
- הוא אינו כולל יישומים שולחניים קיימים של Office (‏Word, ‏Excel, ‏PowerPoint, ‏Outlook, ‏OneNote, ‏Publisher, ‏Access ו- OneDrive).
    
    או
    
- מותקנת בו גירסה קיימת של Office מסוג 'לחץ והפעל'.
    
כדי לקבוע אם יש לך גירסת 'לחץ והפעל' של Office, בכל יישום של Office, עבור אל **קובץ** \> **חשבון** ( **חשבון Office** ב- Outlook). אם אתה רואה 'עדכוני Office' כפי שמוצג באיור הבא, פירוש הדבר שההתקנה בוצעה באמצעות 'לחץ והפעל'. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **מי יפיק תועלת מתכונה זו**
  
משתמש קצה שהמחשב שלו:
  
- **כולל** רשיון משתמש של Windows 10 Business, רשיון פעיל של Microsoft 365 Business, עדכון Windows 10 ליוצרים ושהמחשב שלו מצורף ל- Azure Active Directory. 
    
- **אינו כולל** יישומי Office בגירסת 64 סיביות (לדוגמה: Word,‏ Excel,‏ Powerpoint). אם יישומי Office בגירסת 64 סיביות נדרשים, תכונה זו אינה מתאימה כיוון שאין תמיכה בהפעלה של גירסת 64 סיביות מסוג 'לחץ והפעל' של Office 2016 ממסוף הניהול של Microsoft 365 Business. 
    
- **אינו כולל** יישומים עצמאיים של Windows Installer (MSI) 2016 (לדוגמה, Visio או Project). Microsoft 365 Business משדרג את Office לגירסת 'לחץ והפעל' של Office 2016 וזו אינה מתאימה ליישומים עצמאיים של Office 2016 MSI. 
    
הטבלה הבאה מפרטת את הפעולה שייתכן שמשתמשי הקצה/מנהלי המערכת יצטרכו לנקוט, בהתאם למצב ההתחלתי שלהם, כדי להשיג גירסת 'לחץ והפעל' מוצלחת בת 32 סיביות של פריסת Office ממסוף הניהול של Microsoft 365 Business.
  
|**הפעלת מצב ההתקנה של Office**|**הפעולה שיש לנקוט לפני התקנת Office עבור Microsoft 365 Business**|**מצב סיום**|
|:-----|:-----|:-----|
|לא הותקנה חבילת Office  <br/> |ללא  <br/> |Office 2016 בגירסת 32 סיביות הותקן באמצעות 'לחץ והפעל'  <br/> |
|גירסת 'לחץ והפעל' קיימת של Office מסוג 32 סיביות (2016 או גירסה קודמת) וללא יישומים עצמאיים  <br/> |ללא  <br/> |שדרוג לגירסת 'לחץ והפעל' האחרונה של Office 2016 מסוג 32 סיביות, לפי הצורך **\*** <br/> |
|גירסת 'לחץ והפעל' קיימת של Office מסוג 32 סיביות או יישומי Office עצמאיים מסוג 32 או 64 סיביות (למשל Visio, ‏Project)  <br/> |ללא  <br/> |יישומים עצמאיים אינם מושפעים. שדרוג החבילה לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות  <br/> |
|גירסת 'לחץ והפעל' קיימת של Office מסוג 32 סיביות ויישומי Office עצמאיים של MSI מסוג 32 או 64 סיביות (למעט 2016)  <br/> |ללא  <br/> |יישומים עצמאיים אינם מושפעים. שדרוג החבילה לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות  <br/> ||||
|גירסת 'לחץ והפעל' קיימת של Office מסוג 64 סיביות  <br/> |הסרת התקנה של יישומי Office מסוג 64 סיביות, אם זה בסדר להחליף אותה ביישומי Office מסוג 32 סיביות  <br/> |אם אתה מסיר את יישומי Office מסוג 64 סיביות, גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות מותקנת  <br/> |
|התקנת MSI קיימת של Office 2016 עם או בלי יישומים עצמאיים  <br/> |הסרת התקנה של MSI Office 2016.  <br/> |מותקנת גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות. ללא שינוי ביישומים עצמאיים  <br/> |
|התקנת MSI קיימת של Office 2013 (או גירסה קודמת) ו/או יישומי Office עצמאיים  <br/> |ללא  <br/> |גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות עם התקנת MSI Office קיימת מראש (ויישומים עצמאיים) מתקיימות זו לצד זו  <br/> |
||||
   
 **(\*) הערה:** לא מתקיים שדרוג לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות עקב באג ידוע. הבעיה תיפתר בקרוב. 
  


