---
title: הגדרת Microsoft 365 Business Premium
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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: גלה את שלבי ההגדרה Microsoft 365 Business Premium, כולל הוספת תחום ומשתמשים, הגדרת מדיניות אבטחה ועוד.
ms.openlocfilehash: 8158e911a8520c07cf5f85fea8b64d65820d603d7f9f49938849ff2df6fc45ed
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53881953"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>הגדרת Microsoft 365 Business Premium באשף ההגדרה

## <a name="watch-overview-of-microsoft-365-setup"></a>צפה: מבט כולל על Microsoft 365 ההתקנה

צפה בסרטון וידאו זה לקבלת מבט כולל על Microsoft 365 Business Premium ההגדרה.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>הוספת התחום, המשתמשים והגדירו פריטי מדיניות

בעת רכישת Microsoft 365 Business Premium, יש לך אפשרות להשתמש בתחום בבעלותך או לקנות תחום במהלך [הכניסה.](sign-up.md)

- אם רכשת תחום חדש כאשר נרשמת, התחום שלך מוגדר ו באפשרותך לעבור אל הוסף [משתמשים ולהקצות רשיונות](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>הוספת התחום שלך כדי להתאים אישית את הכניסה

1. היכנס ל- [מרכז הניהול של Microsoft 365 באמצעות](https://admin.microsoft.com) אישורי מנהל המערכת הכלליים שלך. 

2. בחר **עבור להגדרה כדי** להפעיל את האשף.

    ![בחר עבור להגדרה.](../media/gotosetupinadmincenter.png)

3. בדף **התקן את Office שלך,** באפשרותך להתקין את האפליקציות במחשב שלך.
    
4. בשלב הוספת **תחום,** הזן את שם התחום שברצונך להשתמש בו (כמו contoso.com).

    > [!IMPORTANT]
    > אם רכשת תחום במהלך הכניסה, לא תראה את השלב **הוסף תחום** כאן. עבור אל [הוסף משתמשים במקום](#add-users-and-assign-licenses) זאת.

    ![צילום מסך של דף הכניסה שלך להתאמה אישית.](../media/adddomain.png)

    
4. בצע את השלבים באשף כדי [ליצור רשומות DNS בכל ספק אירוח DNS עבור Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) המ מוודא שהתחום נמצא בבעלותך. אם אתה מכיר את מארח התחום שלך, ראה [גם הוספת תחום Microsoft 365.](/microsoft-365/admin/setup/add-domain)

    אם ספק האירוח שלך הוא GoDaddy או מארח אחר זמין עם חיבור תחום [,](/office365/admin/get-help-with-domains/domain-connect)התהליך קל, ואתה תתבקש להיכנס באופן אוטומטי ולאפשר ל- Microsoft לבצע אימות בשמך.

    ![בדף אישור GoDaddy Access, בחר אשר.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>הוספת משתמשים והקצאת רשיונות

באפשרותך להוסיף משתמשים באשף, אך באפשרותך גם [להוסיף משתמשים מאוחר](../admin/add-users/add-users.md) יותר במרכז הניהול. בנוסף, אם יש לך בקר תחום מקומי, באפשרותך להוסיף משתמשים עם [Azure AD התחברות](/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>הוספת משתמשים באשף

כל המשתמשים שאתה מוסיף באשף מקבלים באופן אוטומטי Microsoft 365 Business Premium רשיון.

![צילום מסך של הדף 'הוספת משתמשים חדשים' באשף](../media/addnewuserspage.png)

1. אם למנוי Microsoft 365 Business Premium שלך יש משתמשים קיימים (לדוגמה, אם השתמשת ב- Azure AD התחברות), אתה מקבל אפשרות להקצות להם רשיונות כעת. קדימה, הוסף רשיונות גם להם.

2. לאחר הוספת המשתמשים, תוכל גם לקבל אפשרות לשתף אישורים עם המשתמשים החדשים שהוספת. באפשרותך להדפיס אותם, לשלוח אותם בדואר אלקטרוני או להוריד אותם.

### <a name="connect-your-domain"></a>חיבור התחום שלך

> [!NOTE]
> אם בחרת להשתמש בתחום .onmicrosoft, או השתמשת ב- Azure AD התחברות כדי להגדיר משתמשים, לא תראה שלב זה.
  
להגדרת שירותים, עליך לעדכן כמה רשומות אצל מארח ה- DNS שלך או אצל רשם התחומים.
  
1. אשף ההגדרה מזהה בדרך כלל את הרשם שלך, ומספק לך קישור להוראות מפורטות לעדכון רשומות ה- NS באתר האינטרנט של הרשם. אם לא, שנה את משרתי השמות כדי להגדיר Microsoft 365 עם [רשם תחומים](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md). 

    - אם יש לך רשומות DNS קיימות, לדוגמה, אתר אינטרנט קיים, אך מארח ה- DNS שלך זמין עבור חיבור [תחום](/office365/admin/get-help-with-domains/domain-connect), בחר **הוסף רשומות עבורי**. בדף בחר **את השירותים המקוונים** שלך, קבל את כל  ברירות המחדל ובחר הבא **ובחר** אשר בדף מארח ה- DNS שלך.
    - אם יש לך רשומות DNS קיימות עם מארחי DNS אחרים (לא זמין עבור חיבור תחום), תרצה לנהל רשומות DNS משלך כדי לוודא שהשירותים הקיימים יישארו מחוברים. לקבלת [מידע נוסף, ראה יסודות](/office365/admin/get-help-with-domains/dns-basics) תחום.

        ![הפעלת עמוד רשומות.](../media/activaterecords.png)

2. בצע את השלבים באשף, והודעת הדואר האלקטרוני והשירותים האחרים יוגדרו בשבילך.

### <a name="protect-your-organization"></a>הגנה על הארגון שלך 

פריטי המדיניות שאתה מגדיר באשף מוחלים באופן אוטומטי על קבוצת אבטחה [בשם](/office365/admin/create-groups/compare-groups#security-groups) כל *המשתמשים.* באפשרותך גם ליצור קבוצות נוספות להקצאת פריטי מדיניות במרכז הניהול.

1. ב- שפר את ההגנה מפני איומי **סייבר** מתקדמים, מומלץ לקבל את ברירות המחדל [כדי Office 365 מראש הגנה](../security/office-365-security/defender-for-office-365.md) מפני איומים לסרוק קבצים וקישורים Office יישומים.

    ![צילום מסך של דף הגדל הגנה.](../media/increasetreatprotection.png)


2. בדף **מנע דליפות של** נתונים רגישים, קבל את ברירות המחדל כדי להפעיל את Office 365 מניעת אובדן נתונים (DLP) כדי לעקוב אחר נתונים רגישים באפליקציות Office ולמנוע שיתוף מקרי של נתונים אלה מחוץ לארגון שלך.

3. בדף הגן **על נתונים ב- Office למכשירים** ניידים, השאר את ניהול האפליקציות למכשירים ניידים זמינים, הרחב את ההגדרות וסמן אותם ולאחר מכן בחר צור מדיניות **ניהול אפליקציות למכשירים ניידים.**

    ![צילום מסך של הגן על נתונים Office עבור דף למכשירים ניידים.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>אבטחת Windows 10 PC

בסרגל הניווט הימני, בחר **הגדרה** ולאחר מכן, תחת **כניסה ואבטחה,** בחר **אבטח את Windows 10 שלך.** בחר **תצוגה** כדי להתחיל בעבודה. ראה [אבטחת Windows 10 שלך לקבלת](secure-win-10-pcs.md) הוראות מלאות.

## <a name="deploy-office-365-client-apps"></a>פריסת Office 365 לקוח

אם בחרת להתקין באופן אוטומטי Office יישומים במהלך ההתקנה, האפליקציות יותקנו במכשירי Windows 10 לאחר שהמשתמשים התחברו ל- Azure AD מהמכשירים Windows שלהם, תוך שימוש באישורי העבודה שלהם.

כדי להתקין Office במכשירי iOS או Android ניידים, [ראה הגדרת מכשירים ניידים עבור Microsoft 365 Business Premium המשתמשים.](set-up-mobile-devices.md)

באפשרותך גם להתקין Office בנפרד. ראה [Office במחשב PC או Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) לקבלת הוראות.

## <a name="related-content"></a>תוכן קשור

[Microsoft 365 הדרכה לעסקים](../business-video/index.yml) (דף קישור)
