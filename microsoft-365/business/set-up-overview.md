---
title: מבט כולל על הכיוונון
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: מבט כולל על שלבי ההתקנה של Microsoft 365 Business.
ms.openlocfilehash: 3447f06d031462a7bebc6f129238de9f0c5dee41
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721558"
---
# <a name="overview-of-setup"></a>מבט כולל על הכיוונון

ניתן לבצע את רוב שלבי ההתקנה באשף ההתקנה, אך גם האפשרויות האחרות מפורטות.

## <a name="step-1-add-your-domain-and-users"></a>שלב 1: הוספת התחום שלך והמשתמשים

   - **[הוסף את התחום שלך](set-up.md#add-your-domain-to-personalize-sign-in)** (אם רכשת את התחום שלך במהלך [ההרשמה](sign-up.md), שלב זה כבר נעשה.)

    - **הוסיף משתמשים**. באפשרותך להוסיף משתמשים בכל אחת משלוש הדרכים:
        - באשף [](set-up.md#add-users-in-the-wizard).
        - השתמש בסינכרון ספריות כדי [להוסיף משתמשים על-ידי שימוש בתכלת AD להתקשרות](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) אם ברשותך ספריה פעילה מקומית.
        - באפשרותך גם [להוסיף משתמשים בהמשך](add-users-m365b.md) מרכז הניהול.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>שלב 2: הגדרת מדיניות אבטחה וקביעת תצורה של התקנים 

  - השתמש [באשף ההתקנה](set-up.md#protect-data-and-devices) כדי לקבוע את תצורת מדיניות ההתקן והאבטחה. 
  - באפשרותך גם להוסיף או לערוך אותם בהמשך [מרכז הניהול](view-policies-and-devices.md) [ובפורטל Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - בנוסף להגדרות האבטחה באשף ההתקנה, באפשרותך להגביר את האבטחה על-ידי הוספת ההגדרות הבאות:

      - **הגנה מפני תוכנות זדוניות דוא ל**
      - **קישורים מתקדמים להגנת האיומים (ATP)**
      - **מסמכים מצורפים בטוחים ב-ATP**
      - **ATP נגד דיוג**
      - **אחסון בארכיון של Exchange Online**
      - **מניעת אובדן נתונים (DLP)**
      - **תכלת הגנת מידע (Plan1**)

          כדי להתחיל לראות, [הגדר מדיניות אבטחה מתקדמת](set-up-advanced-security.md).

        ראה גם [top 10 דרכים לאבטח את Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) עבור מפת הדרכים של נוהלי האבטחה הטובה ביותר.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>שלב 3: הגדרת וניהול של התקני Windows 10

   כאשר אתה מצטרף להתקן של Windows 10 לתכלת, המדיניות שהגדרת [בשלב 2](#step-2-set-up-security-policies-and-configure-devices) מוחלת עליו.

   - Windows 10 Pro הוא [תנאי מוקדם](pre-requisites-for-data-protection.md) עבור Microsoft 365 Business, אבל אם יש לך Windows 7 Pro, Windows 8 pro, או Windows 8.1 pro, המנוי שלך מזכה אותך [לשדרוג ל-Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
    - השתמש [באשף ההתקנה](set-up.md#protect-data-and-devices) כדי לקבוע את תצורת פריטי המדיניות עבור התקני Windows 10.

## <a name="step-4-install-office-365-business"></a>שלב 4: התקנת Office 365 עסקים
- באפשרותך להתקין את Office באופן אוטומטי בהתקני Windows באמצעות [אשף ההתקנה](set-up.md#deploy-office-365-client-apps).
- אפשר למשתמשים [להתקין יישומי Office](https://docs.microsoft.com/office365/admin/setup/install-applications) עבור Windows והתקנים.
     
## <a name="advanced"></a>מתקדם
- **השתמש בטייס אוטומטי כדי להגדיר התקנים חדשים**
            
     באפשרותך להשתמש [בטייס אוטומטי של windows](add-autopilot-devices-and-profile.md) כדי לקבוע מראש את התצורה של התקנים **חדשים** של windows 10 עבור משתמש, אך ייתכן שיהיה קל יותר לקבל [שותף](https://www.microsoft.com/solution-providers/search) שיוכל לעשות זאת עבורך. באפשרותך גם לעבור אל [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)ולבקש ממומחה טכנולוגיית ענן להגדיר התקנים חדשים שתרכוש.

- **גישה למשאבים מקומיים**

     - אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business כדי להגן על התקני Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים המחייבים אימות מקומי. בצע את השלבים [בהפעלת התקני Windows 10 המצורפים לתחום כדי שיוכלו להיות מנוהלים על-ידי Microsoft 365 Business](manage-windows-devices.md) כדי להגדיר זאת. זוהי השיטה המועדפת, והתקנים במצב זה נקראים "היברידית תכלת" התקנים המצורפים.

    - אם לעסק שלך יש Active Directory מקומי המכיל משאבים מסוימים מקומיים (כגון שיתופי קבצים ומדפסות), באפשרותך להעניק להתקנים המצורפים למשאבים אלה גישה אל משאבים אלה על-ידי ביצוע השלבים כאן: [גישה למשאבים מקומיים מהתקן תכלת-הצטרף ב-Microsoft 365 business](access-resources.md).

  