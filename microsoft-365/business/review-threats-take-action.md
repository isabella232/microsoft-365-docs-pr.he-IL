---
title: סקירה של איומים שזוהו ופעולה
f1.keywords: NOCSH
ms.author: sharik
author: SKjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- Adm_O365
- Adm_TOC
ms.custom: AdminSurgePortfolio
search.appverid: MET150
description: למד כיצד לסקור ולנהל איומים שזוהו על-ידי אנטי-וירוס של Microsoft Defender במכשירי Windows 10 שלך.
ms.openlocfilehash: 15e99fb75e4a3ac1af842ca7d0b900e02cbc6bd4
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "53465413"
---
# <a name="review-detected-threats-and-take-action"></a>סקירה של איומים שזוהו ופעולה

ברגע שתזהה קובץ או תוכנה זדוניים, אנטי-וירוס של Microsoft Defender אותו וימנע ממנו לפעול. כאשר הגנה מועברת בענן מופעלת, איומים שזוהו לאחרונה מתווספים למנוע האנטי-וירוס והאנטי-תוכנות זדוניות כך שהמכשירים והמשתמשים האחרים שלך מוגנים גם הם.

אנטי-וירוס של Microsoft Defender מזהה ומגן מפני סוגי האיומים הבאים:

- וירוסים, תוכנות זדוניות ואיומים מבוססי אינטרנט במכשירים
- ניסיונות דיוג
- ניסיונות גניבת נתונים

כמקצוען IT/מנהל מערכת, באפשרותך להציג מידע אודות זיהויי Windows 10 במכשירים [שנרשמו ל- Intune](/mem/intune/enrollment/device-enrollment) ב- מרכז הניהול של Microsoft 365. תראה מידע סיכום, כגון:

- כמה מכשירים זקוקים להגנה מפני אנטי-וירוס
- כמה מכשירים אינם תואמים למדיניות אבטחה
- כמה איומים פעילים, מקלים או נפתרים כעת

קיימות כמה אפשרויות כדי להציג מידע ספציפי אודות זיהויי איומים ומכשירים:

- הדף **'מכשירים** פעילים' <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">מרכז הניהול של Microsoft 365</a>. ראה [ניהול זיהויי איומים בדף 'מכשירים פעילים'](#manage-threat-detections-on-the-active-devices-page) במאמר זה.
- הדף **'איומים פעילים'** <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">מרכז הניהול של Microsoft 365</a>. ראה [ניהול זיהויי איומים בדף 'איומים פעילים'](#manage-threat-detections-on-the-active-threats-page) במאמר זה.
- הדף **אנטי-וירוס** <a href="https://go.microsoft.com/fwlink/p/?linkid=2150463" target="_blank">ב- Microsoft Endpoint Manager</a>. ראה [ניהול זיהויי איומים Microsoft Endpoint Manager](#manage-threat-detections-in-microsoft-endpoint-manager) במאמר זה.

כדי ללמוד עוד, ראה [איומים שזוהו על-ידי אנטי-וירוס של Microsoft Defender](threats-detected-defender-av.md).

## <a name="manage-threat-detections-on-the-active-devices-page"></a>ניהול זיהויי איומים בדף **'מכשירים פעילים'**

ההליך הבא חל על לקוחות שיש להם Microsoft 365 Business Premium.

1. עבור אל מרכז הניהול של Microsoft 365 ב <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> והירשם.

2. בדף הניווט, בחר **מכשירים**  >  **פעילים מכשירים**. תראה רשימה של מכשירים ופרטים פעילים, כגון מצב הגנה, מצב הגנה של אנטי-וירוס (AV) ומספר האיומים הפעילים שזוהו.

3. בחר מכשיר כדי להציג פרטים נוספים אודות מכשיר זה ופעולות זמינות. תפריט נשלף נפתח עם המלצות ופעולות זמינות, כגון מדיניות עדכון **,** עדכון **אנטי-וירוס**, **הפעל סריקה מהירה**, הפעל **סריקה** מלאה ועוד.

## <a name="manage-threat-detections-on-the-active-threats-page"></a>ניהול זיהויי איומים **בדף 'איומים פעילים'**

ההליך הבא חל על לקוחות שיש להם Microsoft 365 Business Premium. [Windows 10 מכשירים חייבים להיות מאובטחים](./secure-win-10-pcs.md) [ונרשמו ב- Intune](/mem/intune/enrollment/windows-enrollment-methods).

> [!NOTE]
> הכרטיס **אנטי-וירוס של Microsoft Defender** **והדף 'איומים פעילים'** מגולגלים בשלבים, ולכן ייתכן שלא תוכל לגשת אליהם באופן מיידי.

1. עבור אל מרכז הניהול של Microsoft 365 ב <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> והירשם.

2. בכרטיס **אנטי-וירוס של Microsoft Defender,** בחר **הצג איומים פעילים**. (לחלופין, בחלונית הניווט, בחר **תקינות**  >  **איומים & אנטי-וירוס**.)

3. בדף **איומים פעילים,** בחר איום שזוהה כדי לקבל מידע נוסף עליו. נפתח חלון נשלף עם פרטים אודות איום זה, כולל המכשירים המושפעים.

4. בתפריט נשלף, בחר מכשיר כדי להציג פעולות זמינות, כגון מדיניות **עדכון**, עדכון **אנטי-וירוס**, **הפעל סריקה** מהירה ועוד.

## <a name="actions-you-can-take"></a>פעולות שתוכל לבצע

בעת הצגת פרטים אודות איומים או מכשירים ספציפיים, תראה המלצות ופעולות אחד או יותר שתוכל לבצע. הטבלה הבאה מתארת פעולות שאתה עשוי לראות.<br><br>

| פעולה | תיאור |
|--|--|
| קביעת תצורה של הגנה | יש לקבוע את תצורת מדיניות ההגנה על איומים שלך. בחר את הקישור כדי לעבור לדף תצורת המדיניות שלך.<br><br>זקוק לעזרה? ראה [ניהול אבטחת מכשירים עם מדיניות אבטחה של נקודות קצה ב- Microsoft Intune](/mem/intune/protect/endpoint-security-policy). |
| מדיניות עדכון | יש לעדכן או להגדיר את מדיניות האנטי-וירוס ומדיניות ההגנה בזמן אמת. בחר את הקישור כדי לעבור לדף תצורת המדיניות.<br><br>זקוק לעזרה? ראה [ניהול אבטחת מכשירים עם מדיניות אבטחה של נקודות קצה ב- Microsoft Intune](/mem/intune/protect/endpoint-security-policy). |
| הפעלת סריקה מהירה | הפעלת סריקת אנטי-וירוס מהירה במכשיר, התמקדות במיקום משותף שבו תוכנות זדוניות עשויים להיות רשומים, כגון מפתחות רישום ותיקיות אתחול Windows ידועות. |
| הפעל סריקה מלאה | הפעלת סריקת אנטי-וירוס מלאה במכשיר, התמקדות במיקום משותף שבו תוכנות זדוניות עשויים להיות רשומים, כולל כל קובץ ותיקיה במכשיר. התוצאות נשלחות [אל Microsoft Endpoint Manager](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager). |
| עדכון אנטי-וירוס | דורש מהמכשיר לקבל עדכוני [בינה אבטחה עבור אנטי-וירוס](https://go.microsoft.com/fwlink/?linkid=2149926) והגנה מפני תוכנות זדוניות. |
| הפעל מחדש את המכשיר | כפה על Windows 10 מחדש תוך חמש דקות.<br><br>**חשוב:** הבעלים או המשתמש של המכשיר לא יתו באופן אוטומטי על ההפעלה מחדש, והוא עלול לאבד עבודה שלא נשמרה. |

## <a name="manage-threat-detections-in-microsoft-endpoint-manager"></a>ניהול זיהויי איומים Microsoft Endpoint Manager

באפשרותך להשתמש ב- Microsoft Endpoint Manager כדי לנהל זיהויי איומים. Windows 10 אלה חייבים להיות [רשומים ב- Intune](/mem/intune/enrollment/windows-enrollment-methods) (חלק Microsoft Endpoint Manager).

1. עבור אל Microsoft Endpoint Manager הניהול של מרכז <a href="https://go.microsoft.com/fwlink/p/?linkid=2150463" target="_blank">https://endpoint.microsoft.com</a> הניהול והירשם.

2. בחלונית הניווט, בחר **אבטחת נקודת קצה**.

3. תחת **ניהול**, בחר **אנטי-וירוס**. תראה כמה כרטיסיות, כגון סיכום **,** **Windows 10** קצה לא בריאים ונקודות **Windows 10 תוכנות זדוניות.**

4. סקור את המידע על הכרטיסיות הזמינות ולאחר מכן בצע כל פעולה נדרשת.

לדוגמה, נניח שהתקנים מפורטים בכרטיסיה **Windows 10 זוהתה תוכנה זדונית.** בעת בחירת מכשיר, יהיו לך פעולות מסוימות זמינות, כגון הפעלה מחדש , סריקה **מהירה** **,** **סריקה מלאה**, **סינכרון** או **עדכון חתימות**. בחר פעולה עבור מכשיר זה.

הטבלה הבאה מתארת את הפעולות שאתה עשוי לראות Microsoft Endpoint Manager.<br><br>

| פעולה | תיאור |
|--|--|
| הפעל מחדש | כפה על Windows 10 מחדש תוך חמש דקות.<br><br>**חשוב:** הבעלים או המשתמש של המכשיר לא יתו באופן אוטומטי על ההפעלה מחדש, והוא עלול לאבד עבודה שלא נשמרה. |
| סריקה מהירה | הפעלת סריקת אנטי-וירוס מהירה במכשיר, התמקדות במיקום משותף שבו תוכנות זדוניות עשויים להיות רשומים, כגון מפתחות רישום ותיקיות אתחול Windows ידועות. התוצאות נשלחות [אל Microsoft Endpoint Manager](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager). |
| סריקה מלאה | הפעלת סריקת אנטי-וירוס מלאה במכשיר, התמקדות במיקום משותף שבו תוכנות זדוניות עשויים להיות רשומים, כולל כל קובץ ותיקיה במכשיר. התוצאות נשלחות [אל Microsoft Endpoint Manager](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager). |
| סינכרון | נדרש מכשיר כדי לבצע צ'ק-אין עם Intune (חלק Microsoft Endpoint Manager). כאשר המכשיר מחובר, המכשיר מקבל את כל הפעולות או פריטי המדיניות הממתנים שהוקצו למכשיר. |
| עדכון חתימות | דורש מהמכשיר לקבל עדכוני [בינה אבטחה עבור אנטי-וירוס](https://go.microsoft.com/fwlink/?linkid=2149926) והגנה מפני תוכנות זדוניות. |

> [!TIP]
> לקבלת מידע נוסף, ראה [פעולות מרוחקות עבור מכשירים](/mem/intune/protect/endpoint-security-manage-devices#remote-actions-for-devices).

## <a name="how-to-submit-a-file-for-malware-analysis"></a>כיצד לשלוח קובץ לניתוח תוכנות זדוניות

אם יש לך קובץ שאתה סבור שהחמיץ או סווג באופן שגוי כתוכנה זדונית, באפשרותך לשלוח קובץ זה ל- Microsoft לצורך ניתוח תוכנות זדוניות. משתמשים ומנהלי IT יכולים לשלוח קובץ לניתוח. בקר [https://www.microsoft.com/wdsi/filesubmission](https://www.microsoft.com/wdsi/filesubmission) ב- .