---
title: מעבר אל Microsoft 365 Business מ- Office 365 E3
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
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
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: למד כיצד להעביר את העסק שלך Microsoft 365 Business Premium מ- Office 365 E3.
ms.openlocfilehash: f08b054473fdd63ec2372e81c776a1b64f89fe9d
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/06/2021
ms.locfileid: "52244835"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>מעבר מ- Office 365 E3 Microsoft 365 Business Premium

Microsoft 365 Business Premium כולל את כל מה שאתה צריך עבור העסק הקטן שלך, המשלב את יישומי הפרודוקטיביות מבוססי הענן הטובים מסוגם עם ניהול מכשירים ואבטחה פשוטים. אם יש לך כעת Office 365 E3, אך אין לך יותר מ- 300 עובדים, שקול לעבור ל- Microsoft 365 Business Premium לקבלת תכונות אבטחה נוספות.

העברה היא קלה: תחילה עליך להחליף רשיונות וכל הנתונים ומידע המשתמש שלך במנוי הנוכחי שלך נשמרים. לאחר ההעברה, יהיה עליך להגדיר את התכונות שנוספו ב- Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>הבדלים בין Office 365 E3 לבין Microsoft 365 Business Premium

טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium לבין Office 365 E3.

| תכונה    | תמיכה Microsoft 365 Business Premium    | תמיכה ב- Office 365 E3 | 
|:-------|:-----|:-----|
| **מקומי**        | | | 
| Office<sup>1</sup>    | יישומי Microsoft 365 לעסקים    | יישומי Microsoft 365 עבור ארגונים | 
| **יישומי פרודוקטיביות בענן**        | | | 
| Exchange Online ו- Outlook    | מגבלת שטח אחסון של 50 GB לכל תיבת דואר אחסון בארכיון של Exchange Online    | מגבלת שטח אחסון של 100 GB לכל תיבת דואר אחסון בארכיון של Exchange Online | 
| Teams    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) | 
| OneDrive for Business    | מגבלת אחסון של 1 TB לכל משתמש    | ללא הגבלה | 
| Yammer, SharePoint Online, Planner, Stream    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) | 
| MileIQ    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **הגנה מפני איומים**        | | | 
| Defender for Office 365 תוכנית 1 | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | לא כלול, אך ניתן להוסיף אותו | 
| **ניהול זהויות**        | | | 
| איפוס סיסמה בשירות עצמי עבור חשבונות היברידיים של Azure Active Directory (Azure AD), אימות רב-גורמי של Azure AD (MFA), Access מותן, writeback באמצעות סיסמה עבור זהויות מקומיות|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| **ניהול מכשירים ואפליקציות**        | | |
| Microsoft Intune, Windows AutoPilot|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| הפעלת מחשב משותף|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png)| 
| שדרוג זכויות Windows 10 Pro מתוך Win 7/8.1 Pro רשיונות|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    || 
| **הגנה על מידע**        | | |
|Office 365 מניעת אובדן נתונים|    ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)|![כלול ב- Office 365 E3](../media/check-mark.png)|
|Azure Information Protection Plan 1, BitLocker אכיפה|![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)||
|Azure Information Protection Plan 1, תוויות רגישות|![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)||
|**לקוח Access רשיון (זכויות CAL)**|||
|Enterprise CAL Suite (Exchange, SharePoint, Skype)||![כלול ב- Office 365 E3](../media/check-mark.png)|

<sup>1</sup> גירסת Microsoft 365 Business Premium של יישומי Office אינה כוללת הפעלת עוצמת קול באמצעות מדיניות קבוצתית, מדידת שימוש ביישומים, פקדים לעדכון, השוואה וחקירה של גיליון אלקטרוני או בינה עסקית.

## <a name="migration"></a>העברה

כדי להעביר את המנוי שלך, ראה [שינוי תוכניות באופן](../commerce/subscriptions/change-plans-manually.md) ידני לקבלת הוראות אם ברצונך להעביר רק כמה אנשים Microsoft 365 Business Premium. באפשרותך גם לשדרג [את כולם באופן](../commerce/subscriptions/upgrade-to-different-plan.md)אוטומטי, או לעבוד עם שותף כדי להעביר את המנוי והרשיון שלך ל- E3 למנוי Microsoft 365 Business Premium שלך.
הסעיפים הבאים מתארים את השינויים שתצטרך לבצע, אם יש, ומה ניתן לעשות לאחר ההעברה.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 תצורה ונתונים של מנוי E3
אין צורך לבצע שינויים כלשהם במנוי או בנתונים הנוכחיים שלך לפני המעבר, הכולל:

- תצורת מנוי, כגון רשומות DNS ושמות תחומים.
- חשבונות משתמשים וקבוצתיים והגדרות אימות, כגון אימות רב גורמי או פריטי מדיניות גישה מותנים.
- תצורות שירות פרודוקטיביות והנתונים שלהן, כגון Teams, Exchange Online דואר, SharePoint Online, תיקיות OneDrive for Business ומחברות OneNote אחרות.
- Office יתונו באופן אוטומטי. Office 365 רישוי מודרני יבדוק את הקצאת הרשיונות של המשתמש כל 72 שעות ותמיר Office יישומים לגירסה התואמת למנוי המשתמש.

### <a name="windows-10"></a>Windows 10

אם Windows שלך עדיין לא נמצא בעדכון Windows Pro הבורא, שדרג אותם [לעדכון Windows Pro ליוצרים](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>הגדרת פריטי מדיניות להגנה על מכשירים וקבצים של משתמשים

> [!NOTE]
> אם תגדיר Office 365 והתקנים של MDM, מכשירים אלה יופיעו בדף **מכשירים** במרכז Microsoft 365 הניהול. כל פריטי המדיניות שתגדיר יופיעו ברשימת פריטי המדיניות הקלאסיים [בפורטל Intune](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).

לאחר הקצאת רשיונות ל- Microsoft 365 Business Premium, באפשרותך להתחיל להגן על המכשירים והקבצים של המשתמשים.

אם שידרגת את כל האנשים בארגון שלך Microsoft 365 Business Premium, תראה את אשף ההגדרה בדף הבית, ופעל בהתאם להגדרה [Microsoft 365 Business Premium בשלבי](set-up.md) אשף ההגדרה כדי להגן על קבצים ומכשירים ניידים.

באפשרותך גם להשלים שלבים אלה בדף מכשירים:
  
1. במרכז הניהול, בסרגל הניווט הימני, עבור אל **מדיניות** \> **מכשירים**.
    
2. בדף מדיניות **מכשיר,** בחר **הוסף**.
    
3. בחלונית **הוספת** מדיניות, תן למדיניות שם ולאחר מכן בחר **סוג מדיניות** מהרשימה הנפתחת. 
    
     באפשרותך להגדיר מדיניות יישומים להגנה על קבצים במכשירי Android ו- iPhone, וכן Windows 10, וכן להגדיר מדיניות תצורה של מכשיר עבור מכשירי Windows 10 חברה. עיין בקישורים הבאים לקבלת פרטים:
    
  - [קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS](app-protection-settings-for-android-and-ios.md)
    
  - [קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [הגדרת הגדרות הגנה על מכשיר עבור Windows 10 אישיים](protection-settings-for-windows-10-pcs.md)
  
4. לאחר הגדרת מדיניות, אתה והעובדים שלך יכולים להגדיר מכשירים:
    
  - ראה [הגדרת Windows עבור משתמשים Microsoft 365 Business Premium לקבלת](set-up-windows-devices.md) שלבים עבור Windows אחרים. 
    
  - ראה [הגדרת מכשירים ניידים עבור Microsoft 365 Business Premium עבור](set-up-mobile-devices.md) שלבים עבור טלפונים ומכשירי iPhone של Android. 
  
### <a name="mailbox-size"></a>גודל תיבת דואר

Microsoft 365 Business Premium יש מגבלת אחסון של 50 GB כאשר היא משתמשת Exchange Online תוכנית 1. בעת המעבר ל- Microsoft 365 Business Premium, אם אחד מהמשתמשים שלך חורג מ- 50 GB של שטח אחסון בתיבות דואר, מומלץ להקצות למשתמש זה תוכנית Exchange Online תוכנית 2 ולהסיר את תוכנית Exchange Online 1, כי לא ניתן להקצות את שניהם.


### <a name="threat-protection"></a>הגנה מפני איומים

לאחר המעבר ל- Microsoft 365 Business Premium, יש לך את Defender Office 365. עיין [ב- Microsoft Defender לקבלת Office 365 לקבלת](../security/office-365-security/defender-for-office-365.md) מבט כולל. כדי להגדיר, ראה [הגדרת קישורים בטוחים](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [הגדרת](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)קבצים מצורפים בטוחים והגדרת מניעת דיוג [ב- Defender עבור Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).

### <a name="sensitivity-labels"></a>תוויות רגישות

כדי להתחיל להשתמש בתוויות רגישות, ראה [מבט כולל על תוויות רגישות](../compliance/sensitivity-labels.md) [ויצירה וניהול של תוויות רגישות](../business-video/create-sensitivity-labels.md) וידאו.
