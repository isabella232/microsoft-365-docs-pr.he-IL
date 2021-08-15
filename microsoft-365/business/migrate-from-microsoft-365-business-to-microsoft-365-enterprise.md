---
title: מעבר מ- Microsoft 365 Business ל- Microsoft 365 E3
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
description: למד כיצד להעביר את העסק שלך Microsoft 365 Business Premium אל Microsoft 365 E3.
ms.openlocfilehash: d3030518f7f4467c7b2e16897dc7b100764d9d5a36c50169b58f1adcd7bef209
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53837626"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>מעבר מ- Microsoft 365 Business Premium אל Microsoft 365 E3

Microsoft 365 Business Premium כולל את כל מה שאתה צריך עבור העסק הקטן שלך, המשלב את יישומי הפרודוקטיביות מבוססי הענן הטובים ביותר מסוגם עם ניהול מכשירים ואבטחה פשוטים המאפשרים לעובדים שלך לעשות את העבודה הטובה ביותר שלהם. עם זאת, במקרים מסוימים, ייתכן שתצטרך להעביר את המנוי Microsoft 365 Business Premium שלך Microsoft 365 E3.

לדוגמה, העסק שלך גדל וצרכים יותר מ- 300 רשיונות (מזל טוב, דרך אגב).

לחלופין, העסק שלך זקוק לתכונות ארגוניות, כגון יישומי Microsoft 365 לארגונים, Windows 10 Enterprise E3 או Enterprise Client Access (CALs).

השדרוג קל: באפשרותך להתחיל את השדרוג [ממרכז הניהול.](../commerce/subscriptions/upgrade-to-different-plan.md) כל הנתונים והתצורה שלך במנוי הנוכחי שלך נשמרים. אין לך מה לעשות כדי להתכונן להעברה ולא לעשות דבר לאחר מכן, למעט לנצל את התכונות החדשות.

> [!NOTE]
> באפשרותך גם להשתמש במנוי Microsoft 365 Business Premium עבור עד 300 מושבים, לקבל מנוי Microsoft 365 E3 עבור יותר מ- 300 מושבים. עם זאת, Microsoft Defender עבור Office 365 אינו כלול ב- Microsoft 365 E3. לקבלת הגנה ממשכת על איומים, עליך להוסיף את Defender Office 365 עבור רשיונות נוספים, כך שכל המשתמשים בטווח של Defender עבור Office 365 שלך מורשים.

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>הבדלים בין Microsoft 365 Business Premium לבין Microsoft 365 Enterprise

טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium לבין Microsoft 365 E3.

| תכונה    | תמיכה Microsoft 365 Business Premium    | תמיכה Microsoft 365 E3 |
|:-------|:-----|:-----|
| **מקומי**        | | |
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3|
| Office אפליקציות*    | [יישומי Microsoft 365 לעסקים](#office-365-business)    | יישומי Microsoft 365 עבור ארגונים |
| **יישומי פרודוקטיביות בענן**        | | |
| Exchange Online ו- Outlook    | מגבלת אחסון של 50 GB לכל תיבת דואר ואחסון Exchange Online בארכיון    | מגבלת אחסון של 100 GB לכל תיבת דואר ואחסון Exchange Online בארכיון |
| Teams    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| OneDrive for Business    | מגבלת אחסון של 1 TB לכל משתמש    | ללא הגבלה |
| Yammer, SharePoint Online, Planner, Stream    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| **הגנה מפני איומים**        | | |
| יכולות הפחתת פני השטח של תקיפה    | [ראה רשימה זו](#threat-protection) | ניהול ארגוני של בידוד מבוסס-חומרה עבור Microsoft Edge |
| Defender for Office 365 תוכנית 1 | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | לא כלול, אך ניתן להוסיף אותו |
| **ניהול זהויות**        | | |
| איפוס סיסמה בשירות עצמי עבור חשבונות היברידיים של Azure Active Directory (Azure AD), אימות רב-גורמי של Azure AD (MFA), Access מותן, writeback באמצעות סיסמה עבור זהויות מקומיות|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| גילוי יישום ענן, Azure AD התחברות תקינות    |     | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| Azure AD Office 365 יחיד Sign-On (SSO): 10 אפליקציות לכל משתמש (אפליקציות Gallery SaaS כגון Salesforce)* | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| Azure AD Premium SSO 1: ללא הגבלה (יישומים מקומיים באמצעות Azure AD Application Proxy ואפליקציות שאינן גלריה באמצעות תבניות Self-Service שילוב יישומים)    |     | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| **ניהול מכשירים ואפליקציות**        | | |
| Microsoft Intune, Windows אוטומטי|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
|Virtual Desktop Access (VDA)    |  |     ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
|Windows Virtual Desktop (WVD)    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png) |     ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
|הפעלת מחשב משותפת (SCA)    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png) |     ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| חבילת מיטוב שולחן העבודה של Microsoft    | |     ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| **הגנה על מידע**        | | |
| Office 365 מניעת אובדן נתונים, תוכנית Azure Information Protection 1    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| הגנה על פרטי חלון עבור DLP של נקודת קצה    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| **לקוח Access רשיון (זכויות CAL)**    | | |
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows ניהול זכויות)| |         ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| **תאימות**        | | |
| אחסון דואר אלקטרוני בארכיון ללא הגבלה    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| מנהל תאימות    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| גילוי אלקטרוני    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| חסימה במקום והמתנה לתביעה משפטית    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
| תגיות שמירה ומדיניות שמירה של ניהול רשומות העברת הודעות (MRM)    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Microsoft 365 E3](../media/check-mark.png) |
||||

\* משתמשים שהוקצו להם גישה לאפליקציות SaaS יכולים לקבל גישת SSO ל- 10 יישומים לכל אדם. מנהלי מערכת יכולים לקבוע את התצורה של SSO ולשנות גישת משתמש לאפליקציות SaaS שונות, אך גישת SSO מותרת רק עבור 10 יישומים לכל משתמש בכל פעם. כל Office 365 היישומים נספרים כיישום יחיד.

## <a name="migration"></a>העברה

כדי לעבור, עבוד עם השותף שלך כדי להעביר Microsoft 365 Business Premium המנוי והרשיון שלך למנוי מתאים Microsoft 365 E3 עם הרשיונות שלו.

הסעיפים הבאים מתארים אילו שינויים עליך לבצע, אם יש, ומה ניתן לבצע לאחר ההעברה.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365 ונתונים של מנוי

אין צורך לבצע שינויים כלשהם במנוי או בנתונים הנוכחיים שלך לפני ההעברה, הכוללים:

- תצורת מנוי, כגון שמות תחומי DNS.
- חשבונות משתמשים וקבוצתיים והגדרות אימות, כגון אימות רב גורמי או פריטי מדיניות גישה מותנים.
- תצורות שירות פרודוקטיביות והנתונים שלהן, כגון Teams, Exchange Online דואר, SharePoint Online, תיקיות OneDrive for Business ומחברות OneNote אחרות.

כעת המשתמשים שלך יכולים ליהנות מאחסון בלתי מוגבל בתיבות הדואר Exchange Online ותיקיות OneDrive for Business שלך.

באפשרותך להתחיל להשתמש בגילוי יישומי ענן, ב- Azure AD התחברות תקינות וב- SSO עבור יותר מ- 10 יישומים.

<a name="threat-protection"></a>
### <a name="threat-protection"></a>הגנה מפני איומים

Windows 10 Business כולל הגנות אלה:

- אכיפת תקינות של תהליך אתחול מערכת ההפעלה
- אכיפת תקינות של רכיבי הפעלה רגישים
- פגיעות מתקדמת וניצול של אפס ימים
- הגנת רשת מבוססת מוניטין עבור Microsoft Edge, Internet Explorer ו- Chrome
- חומת אש מבוססת מארח
- הפחתת הסיכון של תוכנות כופר
- בידוד מבוסס חומרה עבור Microsoft Edge
- בקרת יישומים מופעלת על-ידי שרת האבטחה Graph
- בקרת התקן (USB)
- הגנת רשת עבור איומים מבוססי אינטרנט
- כללי מניעת חדירה מארחים

Windows 10 Enterprise E3 כולל גם ניהול ארגוני של בידוד מבוסס חומרה עבור Microsoft Edge.

> [!NOTE]
> משתמשים שהועברו ל- Microsoft 365 E3 יידרשו ל- Microsoft Defender עבור Office 365 עבור המשך הגנה מפני איומים. הקפד לרכוש Defender נוסף עבור Office 365 רישוי, כך שכל המשתמשים בטווח של Defender עבור Office 365 שלך מורשים.

### <a name="device-management-with-intune"></a>ניהול מכשירים עם Intune

אין צורך לבצע שינויים בתצורת Intune הנוכחית לפני המעבר, הכוללת מכשירים והגדרות מכשירים ואפליקציות רשומים.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium כולל Windows 10 Business, ש באפשרותך להתקין באמצעות Windows AutoPilot. בעת העברה ל- Microsoft 365 E3, כל רשיון משתמש כולל Windows 10 Enterprise E3, שברצונך גם להתקין באמצעות Windows Autopilot.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>יישומי Microsoft 365 לעסקים

לקוח יישומי Microsoft 365 לעסקים שלך המותקן במכשירים שלך יתחיל להשתמש באופן אוטומטי בתכונות של יישומי Microsoft 365 לארגונים. לאחר ההעברה, באפשרותך כעת להשתמש ב:

- תמיכה במדיניות קבוצתית
- השוואה וחקירה של גיליון אלקטרוני
- בינה עסקית
