---
title: מבט כולל על ההגדרה
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
description: למד את שלבי ההגדרה עבור Microsoft 365 Business Premium, החל מהוספת מנוי, הוספת תחום ומשתמשים, הגדרת מדיניות אבטחה ועוד.
ms.openlocfilehash: 749acbfdbde92ad97b09dc720c85dd850b76c9cf
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579933"
---
# <a name="overview-of-setup"></a>מבט כולל על ההגדרה

צפה בסרטון וידאו קצר אודות הגדרת Microsoft 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

אם סרטון וידאו זה היה שימושי עבורך, עיין ב[סדרת ההדרכה המלאה עבור עסקים קטנים ומשתמשים חדשים ב- Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

ניתן לבצע את רוב שלבי ההגדרה בהגדרה המודרך, אך האפשרויות האחרות מפורטות גם הן.

## <a name="step-1-add-your-domain-and-users"></a>שלב 1: הוספת התחום והמשתמשים שלך

   - **[הוסף את התחום](set-up.md#add-your-domain-to-personalize-sign-in)** שלך (אם קנית את התחום [שלך במהלך הלהירשם,](sign-up.md)שלב זה כבר בוצע.)

   - **הוספת משתמשים**. באפשרותך להוסיף משתמשים בכל אחת משלוש הדרכים הבאות:
        - בהגדרה [המודרך](set-up.md#add-users-in-the-wizard).
        - השתמש בסינכרון [מדריכי כתובות כדי להוסיף](../enterprise/set-up-directory-synchronization.md) משתמשים באמצעות Azure AD Connect אם יש לך Active directory מקומי.
        - באפשרותך גם [להוסיף משתמשים מאוחר](../admin/add-users/add-users.md) יותר במרכז הניהול.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>שלב 2: הגדרת מדיניות אבטחה והגדרת תצורה של מכשירים 

  - השתמש [בהגדרה המודרך כדי](set-up.md#protect-your-organization) לקבוע את תצורת מדיניות המכשיר. 
  - באפשרותך גם להוסיף עוד או לערוך אותם מאוחר יותר במרכז [הניהול](view-policies-and-devices.md) ובפורטל [Intune](/intune/tutorial-walkthrough-intune-portal).
  - אשף ההגדרה יגדיר גם הגדרות בסיסיות של הגנה מפני איומים ומניעת אובדן נתונים.
  
  בנוסף להגדרות האבטחה באשף ההגדרה, באפשרותך להגדיל את האבטחה על-ידי הוספת ההגדרות הבאות:

- **הגנה מפני תוכנות זדוניות בדואר אלקטרוני**
- **מניעת דיוג ב- Defender עבור Office 365**
- **אחסון בארכיון של Exchange Online**
- **Azure Information Protection (Plan1**)

כדי להתחיל, ראה [הגדלת ההגנה מפני איומים](increase-threat-protection.md) [והגדיר תכונות תאימות](set-up-compliance.md).

ראה גם [את 10 הדרכים המובילות לאבטחת Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) לקבלת מפת דרכים של שיטות עבודה מומלצות לאבטחה.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>שלב 3: הגדרה וניהול של מכשירי Windows 10

לאחר השלמת ההגדרה המודרך, תרצה להגן על כל מחשבי Windows 10 בארגון שלך.
  
- Windows 10 Pro [](pre-requisites-for-data-protection.md) הוא תנאי מוקדם עבור Microsoft 365 Business Premium, אך אם יש לך Windows 7 Pro , Windows 8 Pro או Windows 8.1 Pro, המנוי שלך מזכה אותך בשדרוג [ל- Windows 10 Pro](./upgrade-to-windows-pro-creators-update.md).
- בצע את השלבים [במחשבי Windows 10 המאובטחים](secure-win-10-pcs.md) כדי להגדיר פריטי מדיניות עבור מכשירי Windows 10.

בעת הצטרפות למכשיר Windows 10 ל- Azure AD, פריטי המדיניות שאתה מגדיר עבור מחשבי Windows 10 מוחלים עליו. לקבלת מידע נוסף, ראה [הגדרת מכשירי Windows עבור משתמשי Microsoft 365.](set-up-windows-devices.md)

## <a name="step-4-install-microsoft-365-apps-for-business"></a>שלב 4: התקנת יישומי Microsoft 365 לעסקים
- באפשרותך להתקין באופן אוטומטי את Office במכשירי Windows באמצעות [אשף ההגדרה.](set-up.md#deploy-office-365-client-apps)
- תן למשתמשים [להתקין אפליקציות Office](/office365/admin/setup/install-applications) עבור Windows ומכשירים.
     
## <a name="advanced"></a>מתקדם
- **שימוש ב- Autopilot כדי להגדיר מכשירים חדשים**
            
     באפשרותך להשתמש ב- [Windows Autopilot](add-autopilot-devices-and-profile.md) כדי לקבוע מראש באופן אוטומטי מכשירים חדשים של **Windows** 10 עבור משתמש, אך ייתכן שיהיה קל יותר להשיג שותף [שיכול](https://www.microsoft.com/solution-providers/search) לעשות זאת בשבילך. באפשרותך גם לעבור אל [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), ולשאול מומחה לטכנולוגיית ענן להגדיר מכשירים חדשים שאתה רוכש.

- **Access משאבים מקומיים**

     - אם הארגון שלך משתמש ב- Windows Server Active Directory באופן מקומי, באפשרותך להגדיר את Microsoft 365 Business Premium כדי להגן על מכשירי Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים הדורשים אימות מקומי. בצע את השלבים [המפורטים ב-Windows 10](manage-windows-devices.md) המצורף לתחום כדי לנהל אותם על-ידי Microsoft 365 Business Premium כדי להגדיר זאת. זוהי השיטה המועדפת, והמכשירים במצב זה נקראים מכשירים מצורפים היברידיים של Azure AD.

    - אם העסק שלך כולל Active Directory מקומי המכיל משאבים מקומיים (כגון מיקומים משותפים ומדפסות של קבצים), באפשרותך להעניק למכשירים המצורפים ל- Azure AD גישה למשאבים אלה על-ידי ביצוע השלבים כאן: Access משאבים מקומיים ממכשיר [מצורף ל- Azure AD ב- Microsoft 365 Business Premium.](access-resources.md)

## <a name="see-also"></a>למידע נוסף

[סרטוני הדרכה של Microsoft 365 לעסקים](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)