---
title: מבט כולל על הגדר
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: מבט כולל על הגדר השלבים עבור העסק 365 של Microsoft.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086326"
---
# <a name="overview-of-setup"></a>מבט כולל על כיוונון

ניתן לעשות זאת רוב להגדיר השלבים באשף ההתקנה, אך רשומים גם אפשרויות אחרות.


## <a name="step-1-add-your-domain-and-users"></a>שלב 1: הוספת קבוצת המחשבים והמשתמשים שלך

   - **[הוסף קבוצת המחשבים שלך](set-up.md#add-your-domain-to-personalize-sign-in)** (אם רכשת את התחום שלך במהלך [להירשם](sign-up.md), שלב זה כבר בוצע.)

    - **הוסף משתמשים**. ניתן לעשות זאת באחת משלוש דרכים:
        - [אשף](set-up.md#add-users-in-the-wizard).
        - השתמש סינכרון ספריות כדי [להוסיף משתמשים באמצעות חיבור AD תכלת הרקיע](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) אם ברשותך המקומית של Active directory.
        - באפשרותך גם [להוסיף משתמשים מאוחר יותר](add-users-m365b.md) במרכז admin.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>שלב 2: הגדרת מדיניות אבטחה וקביעת תצורה של התקנים 

  - השתמש [באשף ההתקנה](set-up.md#set-up-security-policies-and-device-configurations) כדי להגדיר פריטי מדיניות התקן ואבטחה. 
  - באפשרותך גם להוסיף יותר או לערוך אותם מאוחר יותר ב- [מרכז admin](view-policies-and-devices.md) [פורטל Intune](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - בנוסף להגדרות אבטחה באשף ההתקנה, באפשרותך להגביר את האבטחה על-ידי הוספת את ההגדרות הבאות:

      - **הגנה מפני תוכנות זדוניות דוא**
      - **קישורים בטוח מתקדם של הגנה מפני איום (ATP)**
      - **קבצים מצורפים מתאימים ATP**
      - **ATP למניעת דיוג**
      - **אחסון בארכיון של Exchange Online**
      - **מניעת אובדן נתונים (DLP)**
      - **הגנה על מידע תכלת הרקיע (Plan1**)

          כדי לקבל מופעל, ראה [הגדרת מדיניות אבטחה מתקדמות](set-up-advanced-security.md).

        ראה גם [העליון 10 דרכים לאבטחת העסק 365 Microsoft](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) עבור מפת דרכים של שיטות עבודה מומלצות של אבטחה.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>שלב 3: להגדיר ולנהל התקני Windows 10

   בעת הצטרפות התקן Windows 10 כדי AD תכלת הרקיע, פריטי המדיניות שהגדרת [בשלב](#step-2-set-up-security-policies-and-configure-devices) 2 לקבל שהוחלה עליו.

   - Windows 10 Pro [קדם הדרושים](pre-requisites-for-data-protection.md) לעסקים 365 של Microsoft, אך אם יש לך Windows 7 Pro, Windows 8 Pro או Windows 8.1 Pro, המנוי שלך מקנה לך [שדרוג ל- Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
    - השתמש [באשף הגדרת](set-up.md#set-up-security-policies-and-device-configurations) כדי להגדיר פריטי מדיניות עבור התקני Windows 10.

## <a name="stes-4-install-office-365-business"></a>Stes 4: התקנת Office 365 עסקי
- באפשרותך להתקין את Office באופן אוטומטי בהתקני Windows באמצעות [אשף ההתקנה](set-up.md#deploy-office-365-client-apps).
- באופן אוטומטי [להתקין את Office](auto-install-or-uninstall-office.md) ממרכז admin.
- לאפשר למשתמשים [להתקין את יישומי Office](https://docs.microsoft.com/office365/admin/setup/install-applications) עבור Windows והתקנים.
     
## <a name="advanced"></a>מתקדם
- **השתמש Autopilot כדי להגדיר התקנים חדשים**
            
     באפשרותך להשתמש ב- [Windows Autopilot](add-autopilot-devices-and-profile.md) כדי לקבוע מראש של התקנים 10 חלונות **חדשים** עבור משתמש באופן אוטומטי, אך ייתכן שיהיה קל יותר לקבל [שותף](https://www.microsoft.com/solution-providers/search) מי יכול לבצע זאת עבורך. באפשרותך גם לעבור לחנות [Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) ובקש טכנולוגיה ענן מומחה להגדיר התקנים חדשים שאתה רוכש עבורך.

- **Access המקומית משאבים**

     - אם הארגון שלך משתמש Windows Server Active Directory המקומית, באפשרותך להגדיר עסקיים 365 של Microsoft להגנה על התקני Windows 10 שלך, תוך שמירה עדיין גישה למשאבים המקומית המחייבים אימות מקומי. בצע את השלבים [אפשר לתחום התקני Windows 10 להיות מנוהל על-ידי Microsoft 365 עסקיים](manage-windows-devices.md) כדי להגדיר זאת. זוהי השיטה המועדפת ואת התקנים במצב זה נקראות תכלת הרקיע היברידית AD לחבר התקנים.

    - אם בעסק שלך יש מקומי Active Directory המכילה כמה המקומית משאבים (כגון שיתופי קבצים ומדפסות), באפשרותך להעניק גישה ההתקנים המצורפים AD תכלת הרקיע שלך למשאבים אלה על-ידי ביצוע השלבים כאן: [Access המקומית משאבים מ תכלת הרקיע מצורף AD ההתקן ב- Microsoft 365 Business](access-resources.md).

  