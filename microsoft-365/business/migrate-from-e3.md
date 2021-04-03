---
title: מעבר ל- Microsoft 365 Business מ- Office 365 E3
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
description: למד כיצד להעביר את העסק שלך ל- Microsoft 365 Business Premium מ- Office 365 E3.
ms.openlocfilehash: ffb82fa40f05383260ac1b97ed0bdf5f2f30c1df
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578326"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>העברה מ- Office 365 E3 ל- Microsoft 365 Business Premium

Microsoft 365 Business Premium כולל את כל מה שאתה צריך עבור העסק הקטן שלך, המשלב את יישומי הפרודוקטיביות מבוססי הענן הטובים ביותר מסוגם עם ניהול ואבטחה פשוטים של מכשירים. אם יש לך כעת מנוי Office 365 E3, אך אין לך יותר מ- 300 עובדים, שקול לעבור ל- Microsoft 365 Business Premium לקבלת תכונות אבטחה נוספות.

העברה היא קלה: תחילה עליך להחליף רשיונות וכל הנתונים ומידע המשתמש שלך במנוי הנוכחי שלך נשמרים. לאחר ההעברה, יהיה עליך להגדיר את התכונות שנוספו ב- Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>הבדלים בין Office 365 E3 לבין Microsoft 365 Business Premium

טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium לבין Office 365 E3.

| תכונה    | תמיכה ב- Microsoft 365 Business Premium    | תמיכה ב- Office 365 E3 | 
|:-------|:-----|:-----|
| **מקומי**        | | | 
| יישומי Office<sup>1</sup>    | יישומי Microsoft 365 לעסקים    | יישומי Microsoft 365 עבור ארגונים | 
| **יישומי פרודוקטיביות בענן**        | | | 
| Exchange Online ו- Outlook    | מגבלת אחסון של 50 GB לכל תיבת דואר ואחסון בארכיון בלתי מוגבל של Exchange Online    | מגבלת אחסון של 100 GB לכל תיבת דואר ואחסון בארכיון בלתי מוגבל של Exchange Online | 
| Teams    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) | 
| OneDrive for Business    | מגבלת אחסון של 1 TB לכל משתמש    | ללא הגבלה | 
| Yammer, SharePoint Online, Planner, Stream    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png) | 
| מנהל הלקוחות של Outlook    | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **הגנה מפני איומים**        | | | 
| Defender for Office 365 Plan 1 | ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | לא כלול, אך ניתן להוסיף אותו | 
| **ניהול זהויות**        | | | 
| איפוס סיסמה בשירות עצמי עבור חשבונות היברידיים של Azure Active Directory (Azure AD), אימות רב-גורמי של Azure AD (MFA), Access מותן, writeback באמצעות סיסמה עבור זהויות מקומיות|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| **ניהול מכשירים ואפליקציות**        | | |
| Microsoft Intune, Windows AutoPilot|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| הפעלת מחשב משותף|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב- Office 365 E3](../media/check-mark.png)| 
| זכויות שדרוג ל- Windows 10 Pro מ- Win 7/8.1 Pro|     ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)    || 
| **הגנה על מידע**        | | |
|מניעת אובדן נתונים של Office 365|    ![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)|![כלול ב- Office 365 E3](../media/check-mark.png)|
|Azure Information Protection Plan 1, אכיפת Bitlocker|![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)||
|Azure Information Protection Plan 1, תוויות רגישות|![כלול ב- Microsoft 365 Business Premium](../media/check-mark.png)||
|**לקוח Access רשיון (זכויות CAL)**|||
|Enterprise CAL Suite (Exchange, SharePoint, Skype)||![כלול ב- Office 365 E3](../media/check-mark.png)|

<sup>1</sup> גירסת Microsoft 365 Business Premium של יישומי Office אינה כוללת הפעלת עוצמת קול באמצעות מדיניות קבוצתית, מדידת שימוש ביישומים, פקדים לעדכון, השוואה וחקירה של גיליון אלקטרוני או בינה עסקית.

## <a name="migration"></a>העברה

כדי להעביר את המנוי שלך, ראה [שינוי תוכניות](../commerce/subscriptions/change-plans-manually.md) באופן ידני לקבלת הוראות אם ברצונך להעביר רק כמה אנשים ל- Microsoft 365 Business Premium. באפשרותך גם לשדרג [את כולם באופן אוטומטי,](../commerce/subscriptions/upgrade-to-different-plan.md)או לעבוד עם שותף כדי להעביר את המנוי והרשיון שלך ל- Microsoft 365 Business Premium.
הסעיפים הבאים מתארים את השינויים שתצטרך לבצע, אם יש, ומה ניתן לעשות לאחר ההעברה.

### <a name="office-365-e3-subscription-configuration-and-data"></a>קביעת תצורה ונתונים של מנוי Office 365 E3
אין צורך לבצע שינויים כלשהם במנוי או בנתונים הנוכחיים שלך לפני המעבר, הכולל:

- תצורת מנוי, כגון רשומות DNS ושמות תחומים.
- חשבונות משתמשים וקבוצתיים והגדרות אימות, כגון אימות רב גורמי או פריטי מדיניות גישה מותנים.
- תצורות שירות פרודוקטיביות והנתונים שלהם, כגון Teams, תיבות דואר של Exchange Online, אתרי SharePoint Online, תיקיות OneDrive for Business ומחברות OneNote.
- יישומי Office יתווו את קנה המידה באופן אוטומטי. רישוי מודרני של Office 365 יבדוק את הקצאת הרשיונות של המשתמש כל 72 שעות ותמיר יישומי Office לגירסה התואמת למנוי המשתמש.

### <a name="windows-10"></a>Windows 10

אם Windows שלך עדיין לא נמצא בעדכון Windows Pro Creator, [שדרג אותם לעדכון יוצרי Windows Pro](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>הגדרת פריטי מדיניות להגנה על מכשירים וקבצים של משתמשים

> [!NOTE]
> אם תגדיר פריטי מדיניות ומכשירי MDM של Office 365,  מכשירים אלה יופיעו בדף מכשירים במרכז הניהול של Microsoft 365. כל פריטי המדיניות שתגדיר יופיעו ברשימת פריטי המדיניות הקלאסיים [בפורטל Intune](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).

לאחר הקצאת רשיונות ל- Microsoft 365 Business Premium, באפשרותך להתחיל להגן על המכשירים והקבצים של המשתמשים.

אם שידרגת את כל האנשים בארגון שלך ל- Microsoft 365 Business Premium, תראה את אשף ההגדרה בדף הבית, ופעל בהתאם להגדרה [של Microsoft 365 Business Premium](set-up.md) בשלבי אשף ההגדרה כדי להגן על קבצים ומכשירים ניידים.

באפשרותך גם להשלים שלבים אלה בדף מכשירים:
  
1. במרכז הניהול, בסרגל הניווט הימני, עבור אל **מדיניות** \> **מכשירים**.
    
2. בדף מדיניות **מכשיר,** בחר **הוסף**.
    
3. בחלונית **הוספת** מדיניות, תן למדיניות שם ולאחר מכן בחר **סוג מדיניות** מהרשימה הנפתחת. 
    
     באפשרותך להגדיר מדיניות יישומים להגנה על קבצים במכשירי Android ו- iPhone, וכן Windows 10, וכן להגדיר מדיניות תצורה של מכשיר עבור מכשירי Windows 10 בבעלות החברה. עיין בקישורים הבאים לקבלת פרטים:
    
  - [קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS](app-protection-settings-for-android-and-ios.md)
    
  - [קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [הגדרת הגדרות הגנה על מכשיר עבור מחשבי Windows 10](protection-settings-for-windows-10-pcs.md)
  
4. לאחר הגדרת מדיניות, אתה והעובדים שלך יכולים להגדיר מכשירים:
    
  - ראה [הגדרת מכשירי Windows עבור משתמשי Microsoft 365 Business Premium לקבלת שלבים](set-up-windows-devices.md) עבור מכשירי Windows. 
    
  - ראה [הגדרת מכשירים ניידים עבור משתמשי Microsoft 365 Business Premium](set-up-mobile-devices.md) לקבלת שלבים עבור טלפונים ומכשירי iPhone של Android. 
  
### <a name="mailbox-size"></a>גודל תיבת דואר

Microsoft 365 Business Premium כולל מגבלת אחסון של 50 GB, כאשר היא משתמשת בתוכנית Exchange Online 1. בעת המעבר ל- Microsoft 365 Business Premium, אם אחד מהמשתמשים שלך חורג מאחסון תיבת דואר בנפח 50 GB, מומלץ להקצות למשתמש זה תוכנית Exchange Online 2 ולהסיר את תוכנית Exchange Online 1, כפי שלא ניתן להקצות את שניהם.


### <a name="threat-protection"></a>הגנה מפני איומים

לאחר המעבר ל- Microsoft 365 Business Premium, יש לך את Defender for Office 365. עיין [ב- Microsoft Defender עבור Office 365](../security/office-365-security/defender-for-office-365.md) לקבלת מבט כולל. כדי להגדיר, ראה [הגדרת קישורים בטוחים](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [הגדרת](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)קבצים מצורפים בטוחים והגדרת מניעת [דיוג ב- Defender עבור Office 365.](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)

### <a name="sensitivity-labels"></a>תוויות רגישות

כדי להתחיל להשתמש בתוויות רגישות, ראה [מבט כולל על תוויות רגישות](../compliance/sensitivity-labels.md) [ויצירה וניהול של תוויות רגישות](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) וידאו.
