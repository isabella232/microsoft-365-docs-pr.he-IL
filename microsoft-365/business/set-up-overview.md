---
title: מבט כולל על הגדרה
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: למד את שלבי ההגדרה עבור Microsoft 365 Business Premium, החל ממנוי, כדי להוסיף תחום ומשתמשים, כדי להגדיר מדיניות אבטחה ועוד.
ms.openlocfilehash: 9d92aefb3b5666bb7c2fd2e13c9a00f074f107a7
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912489"
---
# <a name="overview-of-setup"></a>מבט כולל על הגדרה

צפה בסרטון וידאו קצר אודות הגדרת Premium של Microsoft 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

אם סרטון וידאו זה היה שימושי עבורך, עיין ב[סדרת ההדרכה המלאה עבור עסקים קטנים ומשתמשים חדשים ב- Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

ניתן לבצע את רוב שלבי ההגדרה בהגדרה המודרכת, אך גם האפשרויות האחרות מפורטות.

## <a name="step-1-add-your-domain-and-users"></a>שלב 1: הוספת התחום והמשתמשים שלך

   - **[הוסף את התחום שלך](set-up.md#add-your-domain-to-personalize-sign-in)** (אם רכשת את התחום שלך במהלך [ההרשמה](sign-up.md), שלב זה כבר מתבצע.)

   - **הוספת משתמשים**. באפשרותך להוסיף משתמשים בכל אחת משלוש הדרכים הבאות:
        - בהגדרה [מודרכת](set-up.md#add-users-in-the-wizard).
        - השתמש בסינכרון מדריכי כתובות כדי [להוסיף משתמשים באמצעות תכלת AD Connect](../enterprise/set-up-directory-synchronization.md) אם יש לך Active directory מקומי.
        - באפשרותך גם [להוסיף משתמשים בהמשך](../admin/add-users/add-users.md) מרכז הניהול.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>שלב 2: הגדרת מדיניות אבטחה וקביעת תצורה של מכשירים 

  - השתמש [בהגדרה המודרכת](set-up.md#protect-your-organization) כדי לקבוע את תצורת מדיניות ההתקן. 
  - באפשרותך גם להוסיף או לערוך אותם מאוחר יותר [במרכז הניהול](view-policies-and-devices.md) [ובפורטל של המנגינה](/intune/tutorial-walkthrough-intune-portal).
  - אשף ההגדרה יגדיר גם הגדרות איום בסיסיות והגדרות מניעת אובדן נתונים.
  
  בנוסף להגדרות האבטחה באשף ההתקנה, באפשרותך להגדיל את האבטחה על-ידי הוספת ההגדרות הבאות:

- **הגנה מפני תוכנות זדוניות של דואר אלקטרוני**
- **אנטי-דיוג ב-Defender עבור Office 365**
- **אחסון בארכיון של Exchange Online**
- **תכלת הגנה על מידע (Plan1**)

כדי להתחיל, ראה [הגדלת הגנת האיום](increase-threat-protection.md) [והגדרת תכונות תאימות](set-up-compliance.md).

ראה גם [את 10 הדרכים המובילות לאבטח את Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) עבור כביש-מפת שיטות האבטחה הטובות ביותר.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>שלב 3: הגדרה וניהול של מכשירי Windows 10

לאחר שתשלים את ההגדרה המודרכת, תרצה להגן על כל מחשבי Windows 10 בארגון שלך.
  
- Windows 10 Pro הוא [תנאי](pre-requisites-for-data-protection.md) מחייב עבור Microsoft 365 Business Premium, אך אם יש לך Windows 7 Pro, Windows 8 Pro או Windows 8.1 pro, המנוי שלך מעניק לך [שדרוג ל-windows 10 pro](./upgrade-to-windows-pro-creators-update.md).
- בצע את השלבים [במחשבי pc מאובטחים של windows 10](secure-win-10-pcs.md) כדי להגדיר מדיניות עבור מכשירי windows 10.

בעת הצטרפות למכשיר של Windows 10 ל-תכלת לספירה, המדיניות שהגדרת עבור מחשבי Windows 10 מוחלת עליו. לקבלת מידע נוסף, ראה [הגדרת מכשירי Windows עבור משתמשי Microsoft 365](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>שלב 4: התקנת יישומי Microsoft 365 for business
- באפשרותך להתקין באופן אוטומטי את Office במכשירי Windows באמצעות [אשף ההגדרה](set-up.md#deploy-office-365-client-apps).
- אפשר למשתמשים [להתקין אפליקציות של Office](/office365/admin/setup/install-applications) עבור Windows ומכשירים.
     
## <a name="advanced"></a>מתקדם
- **שימוש בטייס אוטומטי כדי להגדיר מכשירים חדשים**
            
     באפשרותך להשתמש ב- [Windows](add-autopilot-devices-and-profile.md) באופן אוטומטי כדי לקבוע מראש באופן אוטומטי את תצורתם של מכשירי Windows 10 **חדשים** עבור משתמש, אך ייתכן שיהיה לך קל יותר להשיג [שותף](https://www.microsoft.com/solution-providers/search) שיכול לעשות זאת עבורך. באפשרותך גם לעבור אל [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)ולבקש ממומחה טכנולוגיית הענן להגדיר מכשירים חדשים שאתה רוכש.

- **גישה למשאבים מקומיים**

     - אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business Premium כדי להגן על מכשירי Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים הדורשים אימות מקומי. בצע את השלבים המפורטים במאמר [הפיכת מכשירי Windows 10 המצורפים לתחום למנוהל על-ידי Microsoft 365 Business Premium](manage-windows-devices.md) כדי להגדיר זאת. זוהי השיטה המועדפת, והמכשירים במצב זה נקראים מכשירים היברידיים של תכלת לספירה.

    - אם לעסק שלך יש מדריך Active Directory מקומי המכיל משאבים מקומיים (כגון מיקומים משותפים ומדפסות של קבצים), באפשרותך להעניק למכשירים המצורפים שלך מכשירים המצורפים למשאבים אלה על-ידי ביצוע השלבים הבאים: [גישה למשאבים מקומיים 365 באמצעות מכשיר תכלת לפני הצטרפות](access-resources.md)

## <a name="see-also"></a>ראה גם

[סרטוני וידאו של הדרכה של Microsoft 365 for business](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)