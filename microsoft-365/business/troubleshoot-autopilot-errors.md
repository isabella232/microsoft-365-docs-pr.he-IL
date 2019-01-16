---
title: פתרון בעיות של שגיאות במכשיר AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: troubleshooting
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: למד כיצד לפתור בעיות של שגיאות קבצים בהתקן AutoPilot.
ms.openlocfilehash: 9b8d8ab424dd3189ff5c228dab8f5c513ff5dafc
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982744"
---
# <a name="troubleshoot-autopilot-device-errors"></a>פתרון בעיות של שגיאות במכשיר AutoPilot

## <a name="device-file-error-messages"></a>הודעות שגיאה של קובץ התקן

מידע הנה על חלק מן השגיאות עשוי לראות בעת עבודה עם קבצים בהתקן AutoPilot בעסק 365 של Microsoft. 
  
|**קוד שגיאה**|**תיקון כדי לנסות**|
|:-----|:-----|
|גוף הבקשה לא חוקי  <br/> |שגיאה זו אמור לקרות רק לעתים רחוקות, אם אתה רואה שגיאה זו, נסה את הפעולה שוב.  <br/> |
|ערך ה-hash של החומרה עבור התקן אינו נכון.  <br/> |אם אתה רואה שגיאה זו, משמעות הדבר היא כי הערך שסיפקת בקובץ CSV עבור קוד hash של החומרה של התקן אחד אינו נכון. תחילה, ודא כי הערך הוקלד כראוי. אם אתה סבור כי הערך נכון, אך עדיין קורה שגיאה זו, בקש עזרה ספק החומרה שלך.  <br/> |
|התקן שהוקצו דייר אחר  <br/> |אם אתה רואה שגיאה זו, משמעות הדבר היא כי הערך שסיפקת בקובץ CSV עבור המספר הסידורי או את מפתח המוצר של התקן אחד או יותר אינו נכון. תחילה, ודא כי הערך הוקלד כראוי. אם אתה סבור כי הערך נכון, אך עדיין קורה שגיאה זו, בקש עזרה ספק החומרה שלך.  <br/> |
|קובץ ה-CSV מכילה מספר סידורי לא חוקי או מפתח מוצר  <br/> |אם אתה רואה שגיאה זו, פירוש הדבר ההתקן שאתה במהלך ניסיון לרשום כבר רשום על-ידי ארגון אחר. כדי לפתור בעיה זו, בקש ספק החומרה שלך לקבלת עזרה.  <br/> |
|התקן זה אינו נתמך עבור תוכנית ההתקנה באמצעות AutoPilot  <br/> | שגיאה זו פירושה שההתקן אינו עומד בדרישות הפריסה AutoPilot. התקנים עליך לעמוד בדרישות אלה:  <br/>  Windows ,10 גירסה 1703 ואילך.  <br/>  מכשירים חדשים שאינם נחשבים כמוצר Windows מוכן לשימוש.  <br/> |
|התקן לא נמצא  <br/> |שגיאה זו פירושה כי התקן אחד או יותר בקובץ CSV שלך אינו רשום לארגון שלך. כדי לפתור בעיה זו, בקש ספק החומרה שלך לקבלת עזרה.  <br/> |
   