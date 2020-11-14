---
title: העברה מ-Microsoft 365 Business אל Microsoft 365 E3
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
ms.openlocfilehash: 2b15d20e3ae1ad0bef871b139e61abf3ba260729
ms.sourcegitcommit: 34ebec8e2bd54ba3d4ccfd9724797665c965c17f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/13/2020
ms.locfileid: "49071426"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>העברה מ-Microsoft 365 Business Premium ל-Microsoft 365 E3

Microsoft 365 Business Premium כולל את כל מה שדרוש לך עבור העסק הקטן שלך, תוך שילוב יישומי הפרודוקטיביות המבוססים על ענן ברמה הטובה ביותר עם ניהול מכשירים ואבטחה פשוטים המאפשרים לעובדים לבצע את עבודתם הטובה ביותר. עם זאת, במקרים מסוימים, ייתכן שיהיה עליך להעביר את מנוי Microsoft 365 Business Premium שלך ל-Microsoft 365 E3. 

לדוגמה, העסק שלך גדל וזקוק ליותר מ-300 רשיונות (מזל טוב, דרך אגב).

לחלופין, העסק שלך זקוק לתכונות ארגוניות, כגון יישומי Microsoft 365 עבור enterprise, Windows 10 Enterprise E3 או רשיונות של גישת לקוח ארגוניים (רשיונות גישת לקוח).

שדרוג קל: באפשרותך להפעיל את השדרוג [ממרכז הניהול](../commerce/subscriptions/upgrade-to-different-plan.md). כל הנתונים והתצורה במנוי הנוכחי שלך נשמרים. אין לך מה לעשות כדי להתכונן להעברה ואין מה לעשות לאחר מכן, למעט לנצל את התכונות החדשות.

>[!Note]
>באפשרותך גם להשתמש במנוי של Microsoft 365 Business Premium עבור עד 300 מושבים ולקבל מנוי של Microsoft 365 E3 עבור יותר מ-300 מושבים. עם זאת, Microsoft Defender עבור Office 365 אינו כלול ב-Microsoft 365 E3. לצורך הגנת האיום המתמשכת, עליך להוסיף רשיונות נוספים של Defender עבור Office 365 כך שכל המשתמשים בטווח של המגן שלך עבור משטרת Office 365 יהיו בעלי רשיון.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>הבדלים בין Microsoft 365 Business Premium ו-Microsoft 365 Enterprise

טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium ו-Microsoft 365 E3.

| תכונה    | תמיכה ב-Microsoft 365 Business Premium    | תמיכה ב-Microsoft 365 E3 | 
|:-------|:-----|:-----|
| **מקומי**        | | | 
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3| 
| יישומי Office *    | [אפליקציות Microsoft 365 לעסקים](#office-365-business)    | יישומי Microsoft 365 עבור ארגונים | 
| **אפליקציות לפרודוקטיביות בענן**        | | | 
| Exchange Online ו-Outlook    | מגבלת אחסון של 50 GB לכל תיבת דואר ואחסון בארכיון באופן בלתי מוגבל של Exchange Online    | מגבלת אחסון של 100 GB לכל תיבת דואר ואחסון בארכיון באופן בלתי מוגבל של Exchange Online | 
| Teams    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| OneDrive for Business    | מגבלת אחסון של 1 TB לכל משתמש    | גבלה | 
| קטרת, SharePoint Online, מתכנן תכנון, זרם    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| MileIQ    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **הגנה מפני איום**        | | | 
| יכולות הפחתת משטח התקפה    | [הצגת רשימה זו](#threat-protection) | ניהול ארגוני של בידוד מבוסס חומרה עבור Microsoft Edge | 
| Defender עבור Office 365 תוכנית 1 | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | לא כלול, אך ניתן להוסיף אותו | 
| **ניהול זהויות**        | | | 
| איפוס סיסמה בשירות עצמי עבור חשבונות היברידית תכלת Active Directory (תכלת לספירה), הודעות מרובות-גורמי אימות (מכשפות אחרות), גישה מותנית, סיסמה writeback עבור זהויות מקומיות|     ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| גילוי אפליקציית הענן, התחברות בריאות של תכלת    |     | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| אפליקציות של הודעות מיידיות של Office 365 בודדות Sign-On (SSO): 10 אפליקציות לכל משתמש (גלריה סאס apps כגון Salesforce) * | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| Self-Service שילוב מוגבל של הודעות מיידיות באפליקציות מקומיות באמצעות מכ    |     | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| **ניהול מכשירים ויישומים**        | | | 
| Microsoft intune, Windows טייס אוטומטי|     ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
|גישה לשולחן עבודה וירטואלי (VDA)    |  |     ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
|שולחן העבודה של Windows Virtual (WVD)    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png) |     ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
|הפעלת מחשב משותף (SCA)    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png) |     ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| חבילת אופטימיזציה לשולחן העבודה של Microsoft    | |     ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| **הגנה על מידע**        | | | 
| מניעת אובדן נתונים של Office 365, מניעת הגנה על מידע תכלת 1    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| הגנה על מידע חלון עבור DLP של נקודת קצה    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| **רשיון גישת לקוח (זכויות CAL)**    | | |     
| חבילת CAL של Enterprise (Exchange, SharePoint, Skype, Windows, מנהל התצורה של נקודות קצה של Microsoft, ניהול זכויות של Windows)| |         ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| **תאימות**        | | | 
| אחסון בארכיון של דואר אלקטרוני בלתי מוגבל    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| מנהל תאימות    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| גילוי אלקטרוני    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| חסימה מקומית וחסימה לצורך תביעה משפטית    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
| תגי שמירה של ניהול רשומות של העברת הודעות (MRM) ומדיניות שמירה    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Microsoft 365 E3](../media/check-mark.png) | 
||||

\* משתמשים שהוקצו להם גישה לאפליקציות של SaaS יכולים לקבל גישה ל-SSO עד 10 אפליקציות. מנהלי מערכת יכולים לקבוע את התצורה של SSO ולשנות את גישת המשתמש ליישומים שונים של SaaS, אך גישת SSO מותרת רק עבור 10 אפליקציות לכל משתמש בכל פעם. כל יישומי Office 365 נספרים כאפליקציה אחת.

## <a name="migration"></a>העברה

כדי להעביר, עבוד עם השותף שלך כדי להעביר את מנוי Microsoft 365 Business Premium ורשיונות למנוי מתאים של Microsoft 365 E3 עם הרשיונות שלו.

הסעיפים הבאים מתארים אילו שינויים עליך לבצע, אם בכלל, ומה ניתן לעשות לאחר ההעברה.

### <a name="microsoft-365-subscription-configuration-and-data"></a>תצורת מנוי ונתונים של Microsoft 365

אין צורך לבצע שינויים במנוי או בנתונים הנוכחיים לפני ההעברה, הכוללת:

- תצורת מנוי, כגון שמות תחומים של DNS.
- חשבונות משתמשים וקבוצות והגדרות אימות, כגון אימות רב-גורמי או מדיניות גישה מותנית.
- תצורות שירות פרודוקטיביות והנתונים שלהם, כגון Teams, תיבות דואר של Exchange Online, אתרי SharePoint Online, תיקיות OneDrive for Business ומחברות OneNote.

כעת המשתמשים יכולים ליהנות משטח אחסון בלתי מוגבל בתיקיות ' תיבות דואר של Exchange Online ' OneDrive for Business '.

באפשרותך להתחיל להשתמש בגילוי של אפליקציית הענן, לחבר את בריאות התכלת ולהשתמש ב-SSO עבור יותר מ-10 אפליקציות.

>[!Note]
>משתמשים שהועברו ל-Microsoft 365 E3 אינם יכולים עוד להשתמש ב-MileIQ.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>הגנה מפני איום

Windows 10 Business כולל הגנות אלה:

- אכיפת תקינות של תהליך אתחול מערכת ההפעלה
- אכיפת תקינות של רכיבי הפעלה רגישים
- פגיעות מתקדמת וגורמים מקלים לניצול של אפס ימים
- הגנה על רשת מבוססת מוניטין עבור Microsoft Edge, Internet Explorer ו-Chrome
- חומת אש מבוססת מארח
- מזעור Ransomware
- בידוד מבוסס חומרה עבור Microsoft Edge
- בקרת יישומים מופעלת על-ידי גרף האבטחה החכם
- פקד מכשיר (USB)
- הגנה על הרשת עבור איומים מבוססי-אינטרנט
- כללי מניעת החדירה למארח

Windows 10 Enterprise E3 כולל גם ניהול ארגוני של בידוד מבוסס חומרה עבור Microsoft Edge.

>[!Note]
>משתמשים שהועברו ל-Microsoft 365 E3 ידרשו מכל אחד מהם לדרוש רשיון של Microsoft Defender עבור Office 365 לצורך הגנה על האיום המתמשך. הקפד לרכוש רשיונות נוספים של Defender עבור Office 365 כך שכל המשתמשים בטווח של המגן שלך עבור משטרת Office 365 יהיו בעלי רשיון. 
>

### <a name="device-management-with-intune"></a>ניהול מכשירים עם כוונון

אין צורך לבצע שינויים בקביעת התצורה הנוכחית של ' שינוי כיוון ' לפני ההעברה, הכוללת התקנים רשומים והגדרות התקן ואפליקציה.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium כולל את Windows 10 Business, שניתן להתקין באמצעות Windows טייס אוטומטי. כאשר אתה מעביר ל-Microsoft 365 E3, כל רשיון משתמש כולל את Windows 10 Enterprise E3, שניתן גם להתקין באמצעות Windows טייס אוטומטי.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>אפליקציות Microsoft 365 לעסקים

לקוח Microsoft 365 Apps לעסקים המותקן במכשירים שלך יתחיל להשתמש באופן אוטומטי בתכונות של יישומי Microsoft 365 עבור הארגון. לאחר ההעברה, כעת באפשרותך להשתמש ב:

 - הפעלת עוצמת הקול במסגרת מדיניות קבוצתית
 - טלמטריה באפליקציות
 - פקדי עדכון
 - השוואה בין גליונות אלקטרוניים ובירורים
 - בינה עסקית

