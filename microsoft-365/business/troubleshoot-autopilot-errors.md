---
title: פתרון בעיות עבור שגיאות במכשיר AutoPilot
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: troubleshooting
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: למד כיצד לפתור שגיאות שייתכן שתראה בעת עבודה עם קבצי התקן טייס אוטומטי ב-Microsoft 365 Business.
ms.openlocfilehash: 7569f18097a1f5959b3dd491958c78886e1e05d6
ms.sourcegitcommit: 41c0bc5cf50f4ca63b4286d1ea0f58ab82984b7a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2020
ms.locfileid: "42547470"
---
# <a name="troubleshoot-autopilot-device-errors"></a>פתרון בעיות עבור שגיאות במכשיר AutoPilot

## <a name="device-file-error-messages"></a>הודעות שגיאה של קובץ התקן

להלן מידע על חלק מהשגיאות שייתכן שתראה בעת עבודה עם קבצי התקן טייס אוטומטי ב-Microsoft 365 Business. 
  
|**קוד שגיאה**|**תקן כדי לנסות**|
|:-----|:-----|
|גוף בקשה לא חוקי  <br/> |שגיאה זו אמורה להתרחש לעתים רחוקות, אם אתה רואה שגיאה זו, נסה את הפעולה שנית.  <br/> |
|ערך hash של חומרה עבור התקן אינו נכון.  <br/> |אם אתה רואה שגיאה זו, משמעות הדבר היא שהערך שסיפקת בקובץ ה-CSV עבור קוד ה-hash של התקן אחד אינו נכון. תחילה, ודא שהערך הוקלד בצורה נכונה. אם אתה סבור שהערך נכון, אך שגיאה זו עדיין מתרחשת, שאל את ספק החומרה שלך לקבלת עזרה.  <br/> |
|התקן שהוקצה לדייר אחר  <br/> |אם אתה רואה שגיאה זו, משמעות הדבר היא שהערך שסיפקת בקובץ ה-CSV עבור המספר הסידורי או מפתח המוצר של התקן אחד או יותר אינו נכון. תחילה, ודא שהערך הוקלד בצורה נכונה. אם אתה סבור שהערך נכון, אך שגיאה זו עדיין מתרחשת, שאל את ספק החומרה שלך לקבלת עזרה.  <br/> |
|קובץ ה-CSV מכיל מספר סידורי או מפתח מוצר לא חוקי  <br/> |אם אתה רואה שגיאה זו, משמעות הדבר היא שההתקן שאתה מנסה לרשום כבר רשום על-ידי ארגון אחר. כדי לתקן שגיאה זו, שאל את ספק החומרה שלך לקבלת עזרה.  <br/> |
|התקן זה אינו נתמך עבור התקנה באמצעות טייס אוטומטי  <br/> | שגיאה זו פירושה שההתקן אינו עומד בדרישות הפריסה של טייס אוטומטי. המכשירים צריכים לעמוד בדרישות אלה:  <br/>  Windows ,10 גירסה 1703 ואילך.  <br/>  מכשירים חדשים שלא התבצעה באמצעות הניסיון היוצא מהקופסה של Windows.  <br/> |
|ההתקן לא נמצא  <br/> |שגיאה זו פירושה שהתקן אחד או יותר בקובץ ה-CSV אינו רשום לארגון שלך. כדי לתקן זאת, בקש עזרה מספק החומרה שלך.  <br/> |
