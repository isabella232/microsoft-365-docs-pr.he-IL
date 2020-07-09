---
title: העברה ל-Microsoft 365 Business מ-Office 365 E3
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: למד כיצד להעביר את העסק שלך ל-Microsoft 365 Business Premium מ-Office 365 E3.
ms.openlocfilehash: d72f0c52a745ff973868b6fdaa95efa1a37a3dbd
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/18/2020
ms.locfileid: "45081836"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>הגירה מ-Office 365 E3 ל-Microsoft 365 עסקים פרימיום 

Microsoft 365 Business Premium יש את כל מה שאתה צריך עבור העסק הקטן שלך, שילוב של יישומי הפרודוקטיביות המבוססת על ענן ברמה הטובה ביותר עם ניהול התקנים פשוטים ואבטחה. אם יש לך כרגע מנוי של Office 365 E3, אך אין ברשותך יותר מ-300 עובדים, שקול לעבור ל-Microsoft 365 Business Premium לקבלת תכונות אבטחה נוספות.

ההעברה קלה: תחילה אתה מחליף רישיונות וכל הנתונים ופרטי המשתמש שלך במנוי הנוכחי שלך נשמרים. לאחר ההעברה, יהיה עליך להגדיר את התכונות הנוספות ב-Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>הבדלים בין Office 365 E3 ו-Microsoft 365 עסקים Premium

טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium ו-Office 365 E3.

| תכונה    | תמיכה ב-Microsoft 365 עסקים פרימיום    | תמיכה ב-Office 365 E3 | 
|:-------|:-----|:-----|
| **מקומי**        | | | 
| יישומים משרדיים<sup>1</sup>    | מיקרוסופט 365 אפליקציות לעסקים    | מיקרוסופט 365 Apps עבור הארגון | 
| **אפליקציות לפרודוקטיביות בענן**        | | | 
| Exchange Online ו-Outlook    | 50 ג'יגה-בתים של מגבלת אחסון עבור תיבת דואר ובלתי מוגבל לארכיון Exchange Online    | 100 ג'יגה-בתים של מגבלת אחסון עבור תיבת דואר ובלתי מוגבל לארכיון Exchange Online | 
| צוותים    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png) | 
| OneDrive for Business    | 1 TB מגבלת אחסון לכל משתמש    | גבלה | 
| Yammer, SharePoint מקוון, מתכנן, זרם    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png) | 
| מרכז הצוות    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png) | 
| מנהל הלקוחות של Outlook, MileIQ    | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | | 
| **הגנה מפני איומים**        | | | 
| תוכנית הגנת האיומים המתקדמת של Office 365 (ATP) 1 | ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | לא כלול, אבל ניתן להוסיף על | 
| **ניהול זהויות**        | | | 
| איפוס סיסמה של שירות עצמי עבור חשבונות היברידית של התכלת הפעילה (כחול לספירה), אימות מרובה-גורמים (משרד המידע), גישה מותנית, סיסמה שתכתוב עבור זהויות מקומיות|     ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    |  | 
| **ניהול התקנים ואפליקציות**        | | |
| מיקרוסופט Intune, Windows טייס אוטומטי|     ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    |  |
| הפעלת מחשב משותף|     ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png)| 
| זכויות שדרוג ל-Windows 10 Pro מ-Win 7/8.1 Pro רשיונות|     ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)    || 
| **הגנה מפני מידע**        | | |
|מניעת אובדן נתונים של Office 365|    ![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)|![כלול ב-Office 365 E3](../media/check-mark.png)|
|התוכנית להגנה מפני מידע תכלת 1, אכיפה של Bitlocker|![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)||
|שיטת הגנת מידע תכלת, תוויות רגישות|![כלולים עם מיקרוסופט 365 עסקים פרימיום](../media/check-mark.png)||
|**רשיון גישת לקוח (זכויות CAL)**|||
|סוויטת CAL ארגונית (Exchange, SharePoint, סקייפ)||![כלול ב-Office 365 E3](../media/check-mark.png)|

<sup>1</sup> מיקרוסופט 365 עסקים Premium גירסה של יישומי המשרד אינו כולל הפעלת אמצעי אחסון באמצעות מדיניות קבוצתית, apps טלמטריה, עדכון פקדים, גיליון אלקטרוני להשוות ולברר, או בינה עסקית.

## <a name="migration"></a>העברה

כדי להעביר את המנוי שלך, ראה [שינוי תוכניות באופן ידני](../commerce/subscriptions/change-plans-manually.md) לקבלת הוראות אם ברצונך להעביר רק כמה אנשים ל-Microsoft 365 Business Premium. באפשרותך גם [לשדרג את כולם באופן אוטומטי](../commerce/subscriptions/upgrade-to-different-plan.md), או לעבוד עם שותף כדי להעביר את מנוי ה-E3 והרשיונות שלך למנוי של Microsoft Business Premium של מיקרוסופט 365.
הסעיפים הבאים מתארים את השינויים שעליך לבצע, אם בכלל, ומה באפשרותך לעשות לאחר ההעברה.

### <a name="office-365-e3-subscription-configuration-and-data"></a>תצורה ונתונים של מנויים ב-Office 365 E3
אין צורך לבצע שינויים כלשהם במנוי או בנתונים הנוכחיים לפני ההעברה, הכוללת:

- תצורת מנוי, כגון רשומות DNS ושמות תחומים.
- חשבונות משתמש וקבוצה והגדרות אימות, כגון אימות מרובה גורמים או מדיניות גישה מותנית.
- תצורות שירות של פרודוקטיביות והנתונים שלהם, כגון צוותים, תיבות דואר של Exchange Online, אתרים מקוונים של SharePoint, OneDrive עבור תיקיות עסקיות ומחברות של OneNote.
- יישומי Office יגודלם באופן אוטומטי. הרישוי המודרני של Office 365 יבדוק את הקצאת הרשיון של המשתמש כל 72 שעות וימיר יישומי Office לגירסה התואמת למנוי המשתמש.

### <a name="windows-10"></a>ווינדוס 10

אם Windows שברשותך אינו נמצא כבר בעדכון Windows Pro Creator, [שדרג אותם לעדכון יוצרי Windows pro](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>כוונן פריטי מדיניות כדי להגן על התקני משתמש וקבצים

> [!NOTE]
> אם תגדיר מדיניות והתקנים של Office 365 MDM, התקנים אלה יפורטו בדף **ההתקנים** במרכז הניהול של Microsoft 365. כל פריטי המדיניות שתגדיר יופיעו ברשימת המדיניות הקלאסית [בפורטל Intune](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).

לאחר שהקצית רשיונות ל-Microsoft 365 Business Premium, באפשרותך להתחיל להגן על ההתקנים והקבצים של המשתמשים.

אם שדרגת את כל האנשים בארגון שלך ל-Microsoft 365 Business Premium, תראה את אשף ההגדרה בדף הבית, ותוכל לעקוב אחר [הגדרת Microsoft 365 Business Premium בשלבי אשף ההתקנה](set-up.md) כדי להגן על קבצים ומכשירים ניידים.

באפשרותך גם להשלים שלבים אלה בדף ' התקנים ':
  
1. במרכז הניהול, בניווט השמאלי, עבור אל **Devices** \> **מדיניות**התקנים.
    
2. בדף ' **מדיניות התקן** ', בחר באפשרות ' **הוסף**'.
    
3. בחלונית **המדיניות הוסף** את שם המדיניות ולאחר מכן בחר **סוג מדיניות** מהרשימה הנפתחת. 
    
     באפשרותך להגדיר מדיניות יישומים להגנה על קבצים בהתקני Android ו-iPhone, כמו גם ב-Windows 10, ובאפשרותך להגדיר מדיניות תצורת התקנים עבור התקנים של Windows 10 השייכים לחברה. לפרטים, עיין בקישורים הבאים:
    
  - [קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS](app-protection-settings-for-android-and-ios.md)
    
  - [קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [הגדרת הגדרות הגנת התקן עבור מחשבי Windows 10](protection-settings-for-windows-10-pcs.md)
  
4. לאחר הגדרת פריטי מדיניות, אתה ועובדיך יכולים להגדיר התקנים:
    
  - ראה [הגדרת התקני windows עבור משתמשי Microsoft Business Premium 365](set-up-windows-devices.md) עבור שלבים עבור התקני windows. 
    
  - ראה [הגדרת התקנים ניידים עבור Microsoft 365 Business Premium משתמשים](set-up-mobile-devices.md) עבור שלבים עבור טלפונים אנדרואיד ו-iphone. 

### <a name="threat-protection"></a>הגנה מפני איומים

לאחר הגירה ל-Microsoft 365 Business Premium, יש לך Office 365 ATP. לקבלת סקירה, ראה [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) . כדי להגדיר, ראה [הגדרת קישורים בטוחים של atp](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [הגדר קבצים מצורפים של atp בטוחים](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5) [והגדר את האנטי-דיוג של atp](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).

### <a name="sensitivity-labels"></a>תוויות רגישות

כדי להתחיל להשתמש בתוויות רגישות, ראה [מבט כולל על תוויות רגישות](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) [ויצירה וניהול של תוויות רגישות](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) וידאו.
