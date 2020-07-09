---
title: העברה מ-Microsoft 365 Business ל-Microsoft 365 E3
f1.keywords:
- NOCSH
ms.author: josephd
author: JoeDavies-MSFT
manager: laurawi
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: למד כיצד להעביר את העסק שלך מ-Microsoft 365 Business Premium ל-Microsoft 365 E3.
ms.openlocfilehash: 6a795d96ccae7e054e7e52d4fd60a4e73b3c71dd
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/27/2020
ms.locfileid: "45081831"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>העברה מ-Microsoft 365 Business Premium ל-Microsoft 365 E3

Microsoft 365 Business Premium יש את כל מה שאתה צריך עבור העסק הקטן שלך, שילוב של יישומי הפרודוקטיביות המבוססת על ענן ברמה הטובה ביותר עם ניהול התקן פשוט ואבטחה המאפשרים לעובדים שלך לעשות את העבודה הטובה ביותר שלהם. עם זאת, במקרים מסוימים, ייתכן שיהיה עליך להעביר את מנוי ה-365 Business Premium של Microsoft למיקרוסופט 365 E3. 

לדוגמה, העסק שלך גדל וזקוק ליותר מ 300 רשיונות (ברכות, דרך אגב).

לחלופין, העסק שלך זקוק לתכונות ארגוניות, כגון Microsoft 365 Apps עבור הארגון, Windows 10-E3 Enterprise, או רשיונות גישת לקוח ארגוניים (Cal).

השדרוג הוא קל: באפשרותך להפעיל את השדרוג [ממרכז הניהול](../commerce/subscriptions/upgrade-to-different-plan.md). כל הנתונים והגדרות התצורה במנוי הנוכחי נשמרים. אין לך מה לעשות כדי להתכונן להגירה ולא לעשות כלום לאחר מכן, מלבד לנצל את התכונות החדשות.

>[!Note]
>באפשרותך גם להשתמש במנוי של Microsoft Business Premium 365 עבור עד 300 מושבים ולקבל מנוי של Microsoft 365 E3 עבור יותר מ-300 מושבים. עם זאת, Office 365 ATP אינו כלול ב-Microsoft 365 E3. לצורך הגנה על איום מתמשך, עליך להוסיף רשיונות Office 365 של ATP נוספים כך שכל המשתמשים בהיקף של מדיניות ה-ATP של Office 365 יהיו מורשים.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>הבדלים בין מיקרוסופט 365 עסקים Premium ו-Microsoft 365 Enterprise

טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium ו-Microsoft 365 E3.

| תכונה    | תמיכה ב-Microsoft 365 עסקים פרימיום    | תמיכה ב-Microsoft 365 E3 | 
|:-------|:-----|:-----|
| **מקומי**        | | | 
| ווינדוס 10    | העסק של חלונות 10  |     Windows 10 E3 ארגון| 
| יישומי Office *    | [מיקרוסופט 365 אפליקציות לעסקים](#office-365-business)    | מיקרוסופט 365 Apps עבור הארגון | 
| **אפליקציות לפרודוקטיביות בענן**        | | | 
| Exchange Online ו-Outlook    | 50 ג'יגה-בתים של מגבלת אחסון לכל תיבת דואר וארכיון Exchange Online בלתי מוגבל    | 100 ג'יגה-בתים של מגבלת אחסון לכל תיבת דואר וארכיון Exchange Online בלתי מוגבל | 
| צוותים    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| OneDrive for Business    | 1 TB מגבלת אחסון לכל משתמש    | גבלה | 
| Yammer, SharePoint מקוון, מתכנן, זרם    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| מנהל הלקוחות של Outlook, MileIQ    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | | 
| **הגנה מפני איומים**        | | | 
| יכולות הפחתת משטח התקפה    | [ראה רשימה זו](#threat-protection) | ניהול ארגוני של בידוד מבוסס חומרה עבור Microsoft Edge | 
| תוכנית הגנת האיומים המתקדמת של Office 365 (ATP) 1 | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | לא כלול, אבל ניתן להוסיף על | 
| **ניהול זהויות**        | | | 
| איפוס סיסמה של שירות עצמי עבור חשבונות היברידית של התכלת הפעילה (כחול לספירה), אימות מרובה-גורמים (משרד המידע), גישה מותנית, סיסמה שתכתוב עבור זהויות מקומיות|     ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| האפליקציה גילוי ענן, תכלת AD התחברות בריאות    |     | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| תכלת המשרד 365 אפליקציות כניסה יחידה (SSO): 10 יישומים לכל משתמש (גלריית יישומים מסוג SaaS כגון מערכת המחיר) * | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| תכלת AD פרימיום 1 SSO: אין מגבלה (יישומים מקומיים באמצעות התכלת AD היישום Proxy ויישומים שאינם הגלריה באמצעות שילוב עצמי יישום App תבניות)    |     | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| **ניהול התקנים ואפליקציות**        | | | 
| מיקרוסופט Intune, Windows טייס אוטומטי|     ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
|גישה לשולחן עבודה וירטואלי (VDA)    |  |     ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
|שולחן עבודה וירטואלי של Windows (WVD)    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png) |     ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
|הפעלה משותפת של מחשב (סקה)    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png) |     ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| חבילת אופטימיזציה לשולחן העבודה של Microsoft    | |     ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| **הגנה מפני מידע**        | | | 
| משרד 365 למניעת אובדן נתונים, תוכנית הגנת מידע תכלת 1    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| הגנה על מידע חלון עבור DLP של נקודת קצה    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| **רשיון גישת לקוח (זכויות CAL)**    | | |     
| סוויטת CAL של ארגון (Exchange, SharePoint, סקייפ, חלונות, מנהל תצורת נקודות קצה של מיקרוסופט, ניהול זכויות של Windows)| |         ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| **תאימות**        | | | 
| בארכיון דוא ל ללא הגבלה    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| תוצאת תאימות/מנהל תאימות    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| eDiscovery    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| חסימה במקום והחזקת ליטיגציה    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
| תגי שמירה של ניהול רשומות העברת הודעות (MRM) ומדיניות שמירה    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלולים ב-Microsoft 365 E3](../media/check-mark.png) | 
||||

\*משתמשים שהוקצו להם גישה ליישומי SaaS יכולים לקבל גישה ל-SSO עד 10 אפליקציות. מנהלים יכולים לקבוע את תצורת SSO ולשנות את גישת המשתמש ליישומי SaaS שונים, אך גישת SSO מותרת רק עבור 10 יישומים לכל משתמש בכל פעם. כל יישומי Office 365 נספרים כיישום יחיד.

## <a name="migration"></a>העברה

כדי להעביר, עבוד עם השותף שלך כדי להעביר את Microsoft 365 Business Premium למנוי ורישיונות למנוי מתאים של Microsoft 365 E3 עם הרישיונות שלה.

הסעיפים הבאים מתארים את השינויים שעליך לבצע, אם בכלל, ומה באפשרותך לעשות לאחר ההעברה.

### <a name="microsoft-365-subscription-configuration-and-data"></a>מיקרוסופט 365 תצורת מנויים ונתונים

אין צורך לבצע שינויים במנוי או בנתונים הנוכחיים לפני ההעברה, כולל:

- תצורת מנוי, כגון שמות תחומים של DNS.
- חשבונות משתמש וקבוצה והגדרות אימות, כגון אימות מרובה גורמים או מדיניות גישה מותנית.
- תצורות שירות של פרודוקטיביות והנתונים שלהם, כגון צוותים, תיבות דואר של Exchange Online, אתרים מקוונים של SharePoint, OneDrive עבור תיקיות עסקיות ומחברות של OneNote.

כעת, המשתמשים שלך יכולים ליהנות מאחסון בלתי מוגבל בתיבות הדואר של Exchange Online ובתיקיות עסקיות.

אתה יכול להתחיל להשתמש בגילוי קלאוד App, תכלת AD התחברות בריאות, ו-SSO עבור יותר מ 10 apps.

>[!Note]
>משתמשים שהועברו ל-Microsoft 365 E3 לא יכולים עוד להשתמש במנהל הלקוחות של Outlook ו-MileIQ.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>הגנה מפני איומים

Windows 10 Business כולל הגנות אלה:

- אכיפת התקינות של תהליך האתחול של מערכת ההפעלה
- אכיפת שלמות של רכיבי הפעלה רגישים
- פגיעות מתקדמת והגורמים המקלים על ניצול של אפס ימים
- הגנת רשת מבוססת מוניטין עבור Microsoft Edge, Internet Explorer וכרום
- חומת אש מבוססת-מארח
- הגורמים המקלים Ransomware
- בידוד מבוסס חומרה עבור Microsoft Edge
- בקרת יישומים המונעת על-ידי גרף האבטחה החכם
- בקרת התקן (USB)
- הגנת רשת עבור איומים מבוססי אינטרנט
- כללי מניעת חדירה למחשב

Windows 10 מארגון E3 כולל גם ניהול ארגוני של בידוד מבוסס חומרה עבור Microsoft Edge.

>[!Note]
>משתמשים שהועברו ל-Microsoft 365 E3 ידרשו רישיון של Office 365 ATP לצורך הגנה על האיום המתמשך. הקפד לרכוש רשיונות נוספים של Office 365 ATP כך שכל המשתמשים בטווח של מדיניות ה-ATP של Office 365 יהיו מורשים. 
>

### <a name="device-management-with-intune"></a>ניהול התקנים באמצעות Intune

אין צורך לבצע שינויים כלשהם בתצורת Intune הנוכחית לפני ההעברה, הכוללת התקנים רשומים והגדרות התקן ויישום.

### <a name="windows-10"></a>ווינדוס 10

מיקרוסופט 365 עסקים Premium כולל Windows 10 עסקים, אשר ניתן להתקין עם Windows טייס אוטומטי. כאשר אתה מעביר ל-Microsoft 365 E3, כל רשיון משתמש כולל Windows 10 Enterprise E3, אשר ניתן גם להתקין עם Windows טייס אוטומטי.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>מיקרוסופט 365 אפליקציות לעסקים

היישומים שלך ב-Microsoft 365 ללקוח עסקי המותקנים במכשירים שלך יתחילו באופן אוטומטי להשתמש בתכונות של Microsoft 365 Apps עבור הארגון. לאחר ההעברה, באפשרותך להשתמש כעת:

 - הפעלת אמצעי אחסון באמצעות מדיניות קבוצתית
 - טלמטריה אפליקציות
 - עדכן פקדים
 - גיליון אלקטרוני להשוות ולברר
 - בינה עסקית

