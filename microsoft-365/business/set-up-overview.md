---
title: מבט כולל על הכיוונון
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: למד את שלבי ההתקנה עבור Microsoft 365 Business Premium, מהרשמה מנוי, כדי להוסיף קבוצת מחשבים ומשתמשים, כדי להגדיר מדיניות אבטחה ועוד.
ms.openlocfilehash: 8b26d423d4f62ee8f9ea4a61eb8f7efa72ee26cb
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43633354"
---
# <a name="overview-of-setup"></a>מבט כולל על הכיוונון

צפה בסרטון וידאו קצר אודות התקנת הפרמיה של Microsoft Business 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

אם סרטון וידאו זה היה שימושי עבורך, עיין ב[סדרת ההדרכה המלאה עבור עסקים קטנים ומשתמשים חדשים ב- Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

ניתן לבצע את רוב שלבי ההתקנה באשף ההתקנה, אך גם האפשרויות האחרות מפורטות.

## <a name="step-1-add-your-domain-and-users"></a>שלב 1: הוספת התחום שלך והמשתמשים

   - **[הוסף את התחום שלך](set-up.md#add-your-domain-to-personalize-sign-in)** (אם רכשת את התחום שלך במהלך [ההרשמה](sign-up.md), שלב זה כבר נעשה.)

    - **הוסיף משתמשים**. באפשרותך להוסיף משתמשים בכל אחת משלוש הדרכים:
        - באשף [wizard](set-up.md#add-users-in-the-wizard).
        - השתמש בסינכרון ספריות כדי [להוסיף משתמשים על-ידי שימוש בתכלת AD להתקשרות](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) אם ברשותך ספריה פעילה מקומית.
        - באפשרותך גם [להוסיף משתמשים בהמשך](add-users-m365b.md) מרכז הניהול.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>שלב 2: הגדרת מדיניות אבטחה וקביעת תצורה של התקנים 

  - השתמש [באשף ההתקנה](set-up.md#protect-your-organization) כדי לקבוע את התצורה של מדיניות התקנים. 
  - באפשרותך גם להוסיף או לערוך אותם בהמשך [מרכז הניהול](view-policies-and-devices.md) [ובפורטל Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - אשף ההתקנה גם תגדיר הגנה בסיסית על איומים והגדרות מניעת אובדן נתונים.
  
  בנוסף להגדרות האבטחה באשף ההתקנה, באפשרותך להגביר את האבטחה על-ידי הוספת ההגדרות הבאות:

- **הגנה מפני תוכנות זדוניות דוא ל**
- **ATP נגד דיוג**
- **אחסון בארכיון של Exchange Online**
- **תכלת הגנת מידע (Plan1**)

כדי להתחיל, ראה [הגברת הגנת האיום](increase-threat-protection.md) [והגדרת תכונות תאימות](set-up-compliance.md).

ראה גם [top 10 דרכים לאבטח את הפרמיה העסקית של Microsoft 365](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) למפת דרכים של נוהלי אבטחה מיטביים.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>שלב 3: הגדרת וניהול של התקני Windows 10

לאחר שתפעיל את אשף ההגדרה, תרצה להתקין את כל מחשבי Windwos 10 בארגון שלך.
  
- Windows 10 Pro הוא [תנאי מוקדם](pre-requisites-for-data-protection.md) עבור מיקרוסופט 365 עסקים Premium, אבל אם יש לך Windows 7 Pro, Windows 8 pro, או Windows 8.1 pro, המנוי שלך מזכה אותך [לשדרוג ל-Windows 10 pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- בצע את השלבים [במחשבים מאובטחים של windows 10](secure-win-10-pcs.md) כדי להגדיר מדיניות עבור התקני windows 10.

כאשר אתה מצטרף להתקן של Windows 10 לתכלת, מדיניות המדיניות שקבעת עבור מחשבי Windows 10 מוחלת עליו. לקבלת מידע נוסף, ראה [הגדרת התקני Windows עבור משתמשי Microsoft 365](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>שלב 4: התקנת Microsoft 365 Apps לעסקים
- באפשרותך להתקין את Office באופן אוטומטי בהתקני Windows באמצעות [אשף ההתקנה](set-up.md#deploy-office-365-client-apps).
- אפשר למשתמשים [להתקין יישומי Office](https://docs.microsoft.com/office365/admin/setup/install-applications) עבור Windows והתקנים.
     
## <a name="advanced"></a>מתקדם
- **השתמש בטייס אוטומטי כדי להגדיר התקנים חדשים**
            
     באפשרותך להשתמש [בטייס אוטומטי של windows](add-autopilot-devices-and-profile.md) כדי לקבוע מראש את התצורה של התקנים **חדשים** של windows 10 עבור משתמש, אך ייתכן שיהיה קל יותר לקבל [שותף](https://www.microsoft.com/solution-providers/search) שיוכל לעשות זאת עבורך. באפשרותך גם לעבור אל [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)ולבקש ממומחה טכנולוגיית ענן להגדיר התקנים חדשים שתרכוש.

- **גישה למשאבים מקומיים**

     - אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business Premium כדי להגן על התקני Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים המחייבים אימות מקומי. בצע את השלבים [בהפעלת התקנים של Windows 10 המצורפים לתחום כדי שינוהל על-ידי Microsoft 365 Business Premium](manage-windows-devices.md) כדי להגדיר זאת. זוהי השיטה המועדפת, והתקנים במצב זה נקראים "היברידית תכלת" התקנים המצורפים.

    - אם לעסק שלך יש Active Directory מקומי המכיל משאבים מסוימים מקומיים (כגון שיתופי קבצים ומדפסות), באפשרותך להעניק להתקנים המצורפים למשאבים אלה גישה אל משאבים אלה על-ידי ביצוע השלבים כאן: [גישה למשאבים מקומיים מהתקן תכלת-הצטרף ב-Microsoft 365 Business Premium](access-resources.md).

## <a name="see-also"></a>למידע נוסף

[מיקרוסופט 365 עבור סרטוני הדרכה עסקית](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
