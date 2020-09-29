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
ms.openlocfilehash: f3f3894a2a5cb69f9f91825d89db4f4b857fac5c
ms.sourcegitcommit: 15be7822220041c25fc52565f1c64d252e442d89
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/28/2020
ms.locfileid: "48295289"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>העברה מ-Office 365 E3 ל-Microsoft 365 Business Premium 

Microsoft 365 Business Premium כולל את כל מה שדרוש לך עבור העסק הקטן שלך, תוך שילוב אפליקציות הפרודוקטיביות המבוססות על ענן ברמה הטובה ביותר עם ניהול מכשירים ואבטחה פשוטים. אם יש לך כעת מנוי של Office 365 E3, אך אין לך יותר מ-300 עובדים, שקול לעבור ל-Microsoft 365 Business Premium לקבלת תכונות אבטחה נוספות.

העברה קלה: תחילה עליך להחליף רשיונות וכל הנתונים ופרטי המשתמש שלך במנוי הנוכחי יישמרו. לאחר ההעברה, יהיה עליך להגדיר את התכונות שנוספו ב-Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>הבדלים בין Office 365 E3 ו-Microsoft 365 Business Premium

טבלה זו מציגה את ההבדלים בין Microsoft 365 Business Premium ו-Office 365 E3.

| תכונה    | תמיכה ב-Microsoft 365 Business Premium    | תמיכה ב-Office 365 E3 | 
|:-------|:-----|:-----|
| **מקומי**        | | | 
| יישומי Office<sup>1</sup>    | אפליקציות Microsoft 365 לעסקים    | Microsoft 365 Apps for enterprise | 
| **אפליקציות לפרודוקטיביות בענן**        | | | 
| Exchange Online ו-Outlook    | מגבלת אחסון של 50 GB לכל תיבת דואר ואחסון בארכיון באופן בלתי מוגבל של Exchange Online    | מגבלת אחסון של 100 GB לכל תיבת דואר ואחסון בארכיון באופן בלתי מוגבל של Exchange Online | 
| Teams    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png) | 
| OneDrive for Business    | מגבלת אחסון של 1 TB לכל משתמש    | גבלה | 
| קטרת, SharePoint Online, מתכנן תכנון, זרם    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png) | 
| Outlook Customer Manager, MileIQ    | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **הגנה מפני איום**        | | | 
| תוכנית מתקדמת של הגנה מפני איום של Office 365 (ATP) תוכנית 1 | ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | לא כלול, אך ניתן להוסיף אותו | 
| **ניהול זהויות**        | | | 
| איפוס סיסמה בשירות עצמי עבור חשבונות היברידית תכלת Active Directory (תכלת לספירה), הודעות מרובות-גורמי אימות (מכשפות אחרות), גישה מותנית, סיסמה writeback עבור זהויות מקומיות|     ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| **ניהול מכשירים ויישומים**        | | |
| Microsoft intune, Windows טייס אוטומטי|     ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| הפעלת מחשב משותף|     ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    | ![כלול ב-Office 365 E3](../media/check-mark.png)| 
| הרשאות שדרוג ל-Windows 10 Pro מ-Win 7/8.1 Pro רשיונות|     ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)    || 
| **הגנה על מידע**        | | |
|מניעת אובדן נתונים של Office 365|    ![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)|![כלול ב-Office 365 E3](../media/check-mark.png)|
|הגנה על מידע של תכלת בתוכנית 1, אכיפה של Bitlocker|![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)||
|הגנה על מידע ב-תכלת-תוכנית 1, תוויות רגישות|![כלול ב-Microsoft 365 Business Premium](../media/check-mark.png)||
|**רשיון גישת לקוח (זכויות CAL)**|||
|חבילת CAL של Enterprise (Exchange, SharePoint, Skype)||![כלול ב-Office 365 E3](../media/check-mark.png)|

<sup>1</sup> גירסת Microsoft 365 Business Premium של יישומי Office אינה כוללת הפעלת עוצמת הקול באמצעות מדיניות קבוצתית, טלמטריה ביישומים, פקדי עדכון, השוואה בין גליונות אלקטרוניים ובירורים או בינה עסקית.

## <a name="migration"></a>העברה

כדי להעביר את המנוי שלך, ראה [שינוי התוכניות באופן ידני](../commerce/subscriptions/change-plans-manually.md) לקבלת הוראות אם ברצונך להעביר רק כמה אנשים ל-Microsoft 365 Business Premium. באפשרותך גם [לשדרג את כולם באופן אוטומטי](../commerce/subscriptions/upgrade-to-different-plan.md), או לעבוד עם שותף כדי להעביר את מנוי E3 ואת הרשיונות למנוי של Microsoft 365 Business Premium.
הסעיפים הבאים מתארים את השינויים שעליך לבצע, אם בכלל, ומה ניתן לעשות לאחר ההעברה.

### <a name="office-365-e3-subscription-configuration-and-data"></a>תצורת המנוי והנתונים של Office 365 E3
אין צורך לבצע שינויים במנוי או בנתונים הנוכחיים לפני ההעברה, הכוללת:

- תצורת מנוי, כגון רשומות DNS ושמות תחומים.
- חשבונות משתמשים וקבוצות והגדרות אימות, כגון אימות רב-גורמי או מדיניות גישה מותנית.
- תצורות שירות פרודוקטיביות והנתונים שלהם, כגון Teams, תיבות דואר של Exchange Online, אתרי SharePoint Online, תיקיות OneDrive for Business ומחברות OneNote.
- יישומי Office יתבצעו בקנה מידה באופן אוטומטי. הרישוי המודרני של Office 365 יבדוק את משימת הרשיון של המשתמש כל 72 שעות וימיר את יישומי Office לגירסה התואמת למנוי המשתמש.

### <a name="windows-10"></a>Windows 10

אם החלונות שלך אינם נמצאים כבר בעדכון Windows Pro Creator, [שדרג אותם לעדכון Windows Pro creators](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>הגדרת מדיניות להגנה על התקני משתמשים וקבצים

> [!NOTE]
> אם תגדיר את מדיניות ומכשירים של Office 365 MDM, מכשירים אלה יופיעו בדף **מכשירים** במרכז הניהול של Microsoft 365. כל פריטי המדיניות שתגדיר יופיעו ברשימה של פריטי המדיניות הקלאסיים [בפורטל ' כוונון](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)'.

לאחר שהקצית רשיונות ל-Microsoft 365 Business Premium, באפשרותך להתחיל להגן על המכשירים והקבצים של המשתמשים.

אם שדרגת את כל המשתמשים בארגון שלך ל-Microsoft 365 Business Premium, תוכל לראות את אשף ההגדרה בדף הבית ולעקוב אחר [ההגדרה של Microsoft 365 Business Premium בשלבי אשף ההגדרה](set-up.md) כדי להגן על קבצים ומכשירים ניידים.

באפשרותך גם להשלים שלבים אלה בדף ' מכשירים ':
  
1. במרכז הניהול, בסרגל הניווט הימני, **Devices** עבור אל \> **פריטי מדיניות**של מכשירים.
    
2. בדף ' **פריטי מדיניות מכשיר** ', בחר **הוסף**.
    
3. בחלונית **הוספת מדיניות** , הענק שם למדיניות ולאחר מכן בחר **סוג מדיניות** מהרשימה הנפתחת. 
    
     באפשרותך להגדיר פריטי מדיניות של יישומים להגנה על קבצים במכשירי Android ו-iPhone, וכן Windows 10, ובאפשרותך להגדיר מדיניות תצורת מכשיר עבור מכשירי Windows 10 בבעלות החברה. עיין בקישורים הבאים לקבלת פרטים:
    
  - [קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS](app-protection-settings-for-android-and-ios.md)
    
  - [קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10](protection-settings-for-windows-10-devices.md)
    
  - [קביעת הגדרות הגנה על מכשירים עבור מחשבי Pc של Windows 10](protection-settings-for-windows-10-pcs.md)
  
4. לאחר הגדרת מדיניות, אתה והעובדים שלך יכולים להגדיר מכשירים:
    
  - ראה [הגדרת מכשירי windows עבור משתמשי Microsoft 365 Business Premium](set-up-windows-devices.md) לקבלת שלבים עבור מכשירי Windows. 
    
  - ראה [הגדרת מכשירים ניידים עבור משתמשי Microsoft 365 Business Premium](set-up-mobile-devices.md) לקבלת שלבים עבור טלפונים ומכשירי Iphone של Android. 
  
### <a name="mailbox-size"></a>גודל תיבת הדואר

Microsoft 365 Business Premium כולל מגבלת אחסון של 50 GB כאשר הוא משתמש ב-Exchange Online תוכנית 1. בעת המעבר ל-Microsoft 365 Business Premium, אם אחד מהמשתמשים שלך חורג מ-50 ג'יגה-בתים של אחסון תיבת הדואר, מומלץ להקצות למשתמש זה תוכנית Exchange Online 2 ולהסיר את Exchange Online Plan 1 מכיוון שלא ניתן להקצות את שניהם.


### <a name="threat-protection"></a>הגנה מפני איום

לאחר המעבר ל-Microsoft 365 Business Premium, יש לך Office 365 ATP. ראה [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) לקבלת מבט כולל. כדי להגדיר, ראה [הגדרת קישורים בטוחים של atp](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [הגדר קבצים מצורפים בטוחים של atp](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5) [והגדר את האנטי-דיוג של atp](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).

### <a name="sensitivity-labels"></a>תוויות רגישות

כדי להתחיל להשתמש בתוויות רגישות, ראה [מבט כולל על תוויות רגישות](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) ולאחר מכן [יצירה וניהול של וידאו וניהול של תוויות רגישות](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) .
