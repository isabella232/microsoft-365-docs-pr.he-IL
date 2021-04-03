---
title: פתרון בעיות עבור שגיאות במכשיר AutoPilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: למד כיצד לפתור שגיאות שאתה עשוי לראות בעת עבודה עם קבצי מכשיר AutoPilot ב- Microsoft 365 Business Premium.
ms.openlocfilehash: 1078ab74b07952e4bb565555a081b98ecce9db5c
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578086"
---
# <a name="troubleshoot-autopilot-device-errors"></a>פתרון בעיות עבור שגיאות במכשיר AutoPilot

## <a name="device-file-error-messages"></a>הודעות שגיאה של קובץ מכשיר

להלן מידע על חלק מהשגיאות שאתה עשוי לראות בעת עבודה עם קבצי מכשיר AutoPilot ב- Microsoft 365 Business Premium. 
  
|**קוד שגיאה**|**תקן כדי לנסות**|
|:-----|:-----|
|גוף בקשה לא חוקי  <br/> |שגיאה זו אמורה להתרחש לעתים רחוקות, אם אתה רואה שגיאה זו, נסה את הפעולה שוב.  <br/> |
|ערך Hash של חומרה עבור מכשיר אינו נכון.  <br/> |אם אתה רואה שגיאה זו, משמעות הדבר היא שהערך שסופק בקובץ ה- CSV עבור קוד ה- Hash של החומרה של מכשיר אחד אינו נכון. תחילה, ודא שהערך הוקלדה כראוי. אם אתה סבור שהערך נכון, אך שגיאה זו עדיין מתרחשת, בקש עזרה מספק החומרה.  <br/> |
|מכשיר שהוקצה לדייר אחר  <br/> |אם אתה רואה שגיאה זו, פירוש הדבר שהערך שסופק בקובץ ה- CSV עבור המספר הסידורי או מפתח המוצר של מכשיר אחד או יותר אינו נכון. תחילה, ודא שהערך הוקלדה כראוי. אם אתה סבור שהערך נכון, אך שגיאה זו עדיין מתרחשת, בקש עזרה מספק החומרה.  <br/> |
|קובץ ה- CSV מכיל מספר סידורי לא חוקי או מפתח מוצר לא חוקי  <br/> |אם אתה רואה שגיאה זו, פירוש הדבר שהמכשיר שאתה מנסה לרשום כבר רשום על-ידי ארגון אחר. כדי לפתור שגיאה זו, בקש עזרה מספק החומרה שלך.  <br/> |
|התקן זה אינו נתמך עבור הגדרה באמצעות AutoPilot  <br/> | שגיאה זו פירושה שההתקן אינו לעמוד בדרישות הפריסה של AutoPilot. המכשירים צריכים לעמוד בדרישות אלה:  <br/>  Windows ,10 גירסה 1703 ואילך.  <br/>  מכשירים חדשים שלא עברו את החוויה 'מחוץ ל- Windows'.  <br/> |
|המכשיר לא נמצא  <br/> |שגיאה זו פירושה שמכשיר אחד או יותר בקובץ ה- CSV שלך אינו רשום בארגון שלך. כדי לפתור בעיה זו, בקש עזרה מספק החומרה שלך.  <br/> |
