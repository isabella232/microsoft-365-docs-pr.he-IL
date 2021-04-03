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
description: גלה את שלבי ההגדרה עבור Microsoft 365 Business Premium, כולל הוספת תחום ומשתמשים, הגדרת מדיניות אבטחה ועוד.
ms.openlocfilehash: c8e2ca94f4947d4f9c69915d2fef410a6075bfed
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579913"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>הגדרת Microsoft 365 Business Premium באשף ההגדרה

צפה בסרטון וידאו זה לקבלת מבט כולל על הגדרת Microsoft 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>הוספת התחום, המשתמשים והגדירו פריטי מדיניות

בעת רכישת Microsoft 365 Business Premium, יש לך אפשרות להשתמש בתחום בבעלותך או לקנות תחום במהלך [הלהירשם.](sign-up.md)

- אם רכשת תחום חדש כאשר נרשמת, התחום שלך מוגדר ו באפשרותך לעבור אל הוסף [משתמשים ולהקצות רשיונות](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>הוספת התחום שלך כדי להתאים אישית את הכניסה

1. היכנס למרכז הניהול [של Microsoft 365 באמצעות](https://admin.microsoft.com) אישורי הניהול הכלליים שלך. 

2. בחר **עבור להגדרה כדי** להפעיל את האשף.

    ![בחר עבור להגדרה.](../media/gotosetupinadmincenter.png)

3. בדף **התקנת יישומי Office,** באפשרותך להתקין את האפליקציות במחשב שלך.
    
4. בשלב הוספת **תחום,** הזן את שם התחום שברצונך להשתמש בו (כמו contoso.com).

    > [!IMPORTANT]
    > אם רכשת תחום במהלך הכניסה, לא תראה את השלב **הוסף תחום** כאן. עבור אל [הוסף משתמשים במקום](#add-users-and-assign-licenses) זאת.

    ![צילום מסך של דף הכניסה שלך להתאמה אישית.](../media/adddomain.png)

    
4. בצע את השלבים באשף כדי [ליצור רשומות DNS בכל ספק אירוח DNS עבור Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) המ מאמת את בעלותך על התחום. אם אתה מכיר את מארח התחום שלך, עיין גם [בהוראות הספציפיות של המארח.](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)

    אם ספק האירוח שלך הוא GoDaddy או מארח אחר זמין עם חיבור תחום [,](/office365/admin/get-help-with-domains/domain-connect)התהליך קל, ואתה תתבקש להיכנס באופן אוטומטי ולאפשר ל- Microsoft לבצע אימות בשמך.

    ![בדף אישור GoDaddy Access, בחר אשר.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>הוספת משתמשים והקצאת רשיונות

באפשרותך להוסיף משתמשים באשף, אך באפשרותך גם [להוסיף משתמשים מאוחר](../admin/add-users/add-users.md) יותר במרכז הניהול. בנוסף, אם יש לך בקר תחום מקומי, באפשרותך להוסיף משתמשים באמצעות [Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>הוספת משתמשים באשף

כל המשתמשים שאתה מוסיף באשף מקבלים באופן אוטומטי רשיון Microsoft 365 Business Premium.

![צילום מסך של הדף 'הוספת משתמשים חדשים' באשף](../media/addnewuserspage.png)

1. אם מנוי Microsoft 365 Business Premium שלך כולל משתמשים קיימים (לדוגמה, אם השתמשת ב- Azure AD Connect), תוכל להקצות להם רשיונות כעת. קדימה, הוסף רשיונות גם להם.

2. לאחר הוספת המשתמשים, תוכל גם לקבל אפשרות לשתף אישורים עם המשתמשים החדשים שהוספת. באפשרותך להדפיס אותם, לשלוח אותם בדואר אלקטרוני או להוריד אותם.

### <a name="connect-your-domain"></a>חיבור התחום שלך

> [!NOTE]
> אם בחרת להשתמש בתחום .onmicrosoft או השתמשת ב- Azure AD Connect כדי להגדיר משתמשים, לא תראה שלב זה.
  
להגדרת שירותים, עליך לעדכן כמה רשומות אצל מארח ה- DNS שלך או אצל רשם התחומים.
  
1. אשף ההגדרה מזהה בדרך כלל את הרשם שלך, ומספק לך קישור להוראות מפורטות לעדכון רשומות ה- NS באתר האינטרנט של הרשם. אם לא, שנה [את שרת השמות כדי להגדיר את Microsoft 365 עם רשם תחומים כלשהו.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md) 

    - אם יש לך רשומות DNS קיימות, לדוגמה, אתר אינטרנט קיים, אך מארח ה- DNS שלך זמין עבור חיבור [תחום](/office365/admin/get-help-with-domains/domain-connect), בחר **הוסף רשומות עבורי**. בדף בחר **את השירותים המקוונים** שלך, קבל את כל  ברירות המחדל ובחר הבא **ובחר** אשר בדף מארח ה- DNS שלך.
    - אם יש לך רשומות DNS קיימות עם מארחי DNS אחרים (לא זמין עבור חיבור תחום), תרצה לנהל רשומות DNS משלך כדי לוודא שהשירותים הקיימים יישארו מחוברים. לקבלת [מידע נוסף, ראה יסודות](/office365/admin/get-help-with-domains/dns-basics) תחום.

        ![הפעלת עמוד רשומות.](../media/activaterecords.png)

2. בצע את השלבים באשף, והודעת הדואר האלקטרוני והשירותים האחרים יוגדרו בשבילך.

### <a name="protect-your-organization"></a>הגנה על הארגון שלך 

פריטי המדיניות שאתה מגדיר באשף מוחלים באופן אוטומטי על קבוצת אבטחה [בשם](/office365/admin/create-groups/compare-groups#security-groups) כל *המשתמשים.* באפשרותך גם ליצור קבוצות נוספות להקצאת פריטי מדיניות במרכז הניהול.

1. ב- שפר את ההגנה מפני איומי **סייבר** מתקדמים, מומלץ לקבל את ברירות המחדל כדי לתת [ל- Office 365 Advance Threat Protection](../security/office-365-security/defender-for-office-365.md) לסרוק קבצים וקישורים באפליקציות Office.

    ![צילום מסך של דף הגדל הגנה.](../media/increasetreatprotection.png)


2. בדף **מנע דליפות של** נתונים רגישים, קבל את ברירות המחדל כדי להפעיל את Office 365 Data Loss Prevent (DLP) כדי לעקוב אחר נתונים רגישים באפליקציות Office ולמנוע שיתוף מקרי של נתונים אלה מחוץ לארגון שלך.

3. בדף **הגנה על נתונים ב- Office למכשירים** ניידים, השאר את ניהול האפליקציות למכשירים ניידים זמינים, הרחב את ההגדרות ו לסקור אותם ולאחר מכן בחר צור מדיניות **ניהול אפליקציות למכשירים ניידים**.

    ![צילום מסך של דף הגן על נתונים ב- Office למכשירים ניידים.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>אבטחת מחשבי Windows 10

בסרגל הניווט הימני, בחר **הגדרה ולאחר** מכן, תחת **כניסה ואבטחה, בחר** **אבטח את מחשבי Windows 10**. בחר **תצוגה** כדי להתחיל בעבודה. ראה [אבטחת מחשבי Windows 10 לקבלת](secure-win-10-pcs.md) הוראות מלאות.

## <a name="deploy-office-365-client-apps"></a>פריסת יישומי לקוח של Office 365

אם בחרת להתקין באופן אוטומטי יישומי Office במהלך ההתקנה, האפליקציות יותקנו במכשירי Windows 10 לאחר שהמשתמשים התחברו ל- Azure AD מהתקני Windows שלהם, תוך שימוש באישורי העבודה שלהם.

כדי להתקין את Office במכשירי iOS או Android ניידים, ראה [הגדרת מכשירים ניידים עבור משתמשי Microsoft 365 Business Premium](set-up-mobile-devices.md).

באפשרותך גם להתקין את Office בנפרד. לקבלת [הוראות, ראה התקנת Office](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) במחשב PC או Mac.

## <a name="see-also"></a>למידע נוסף

[סרטוני הדרכה של Microsoft 365 לעסקים](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
