---
title: התקנת Microsoft 365 Business
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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: גלה את שלבי ההתקנה של Microsoft 365 Business, כולל הוספת תחום ומשתמשים, הגדרת מדיניות אבטחה ועוד.
ms.openlocfilehash: 99994b6f1e9e817b4858aeafe4ce3ceaaf4c3c37
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561182"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>הגדרת העסק של Microsoft 365 באשף ההתקנה

צפה בסרטון וידאו זה למבט כולל על ההתקנה העסקית של Microsoft 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

אם סרטון וידאו זה היה שימושי עבורך, עיין ב[סדרת ההדרכה המלאה עבור עסקים קטנים ומשתמשים חדשים ב- Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>הוספת התחום, המשתמשים והגדרת המדיניות

[![תווית המיידעת אותך שמרכז הניהול משתנה ושניתן למצוא פרטים נוספים ב- aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

בעת רכישת Microsoft 365 Business, יש לך את האפשרות להשתמש בתחום שבבעלותך, או לקנות אחד במהלך [ההרשמה](sign-up.md).

- אם רכשת תחום חדש בעת החתימה, התחום שלך מוגדר ובאפשרותך לעבור [להוספת משתמשים ולהקצות רשיונות](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>הוסף את התחום שלך להתאמה אישית של הכניסה

1. היכנס ל- [Microsoft 365 admin center](https://admin.microsoft.com) באמצעות אישורי המנהל הגלובלי שלך. 

2. בחר באפשרות **עבור אל ההתקנה** כדי להפעיל את האשף.

    ![בחר באפשרות עבור לכיוונון.](../media/gotosetupinadmincenter.png)

3. בדף **התקנת היישומים שלך** ב-Office, באפשרותך להתקין את היישומים במחשב שלך באופן אופציונלי.
    
4. בשלב **הוספת תחום** , הזן את שם התחום בו ברצונך להשתמש (כגון contoso.com).

    > [!IMPORTANT]
    > אם רכשת תחום במהלך ההרשמה, לא תראה **הוספת שלב בתחום** כאן. עבור כדי [להוסיף משתמשים](#add-users-and-assign-licenses) במקום זאת.

    ![צילום מסך של התאמה אישית של דף הכניסה שלך.](../media/adddomain.png)

    
4. בצע את השלבים באשף כדי [ליצור רשומות dns בכל ספק dns המארח עבור Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) המאמת את התחום שלך. אם אתה מכיר את מארח התחום שלך, ראה גם את [ההנחיות הספציפיות למחשב המארח](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    אם ספק האירוח שלך הוא GoDaddy או מארח אחר הזמין עם [התחברות לקבוצת מחשבים](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), התהליך יהיה פשוט ותתבקש באופן אוטומטי להיכנס ולאפשר ל-Microsoft לבצע אימות בשמך.

    ![בעמוד הרשאה לאישור, בחר באפשרות הרשאת.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>הוספת משתמשים והקצאת רשיונות

באפשרותך להוסיף משתמשים באשף, אך באפשרותך גם [להוסיף משתמשים בהמשך](add-users-m365b.md) מרכז הניהול. בנוסף, אם ברשותך בקר תחום מקומי, באפשרותך להוסיף משתמשים בעלי [התקשרות תכלת](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>הוספת משתמשים באשף

כל משתמש שתוסיף באשף יוקצה באופן אוטומטי לרשיון עסקי של Microsoft 365.

![צילום מסך של הדף ' הוספת משתמשים חדשים ' באשף](../media/addnewuserspage.png)

1. אם למנוי העסקי שלך ב-Microsoft 365 יש משתמשים קיימים (לדוגמה, אם השתמשת בתכלת AD Connect), תקבל אפשרות להקצות להם רשיונות כעת. קדימה, הוסף רשיונות גם להם.

2. לאחר שהוספת את המשתמשים, תקבל גם אפשרות לשתף אישורים עם המשתמשים החדשים שהוספת. באפשרותך להדפיס אותם, לשלוח אותם בדואר אלקטרוני או להוריד אותם.

### <a name="connect-your-domain"></a>חיבור התחום שלך

> [!NOTE]
> אם בחרת להשתמש בקבוצת המחשבים onmicrosoft, או בשימוש בתכלת-AD כדי להגדיר משתמשים, לא תראה שלב זה.
  
להגדרת שירותים, עליך לעדכן כמה רשומות אצל מארח ה- DNS שלך או אצל רשם התחומים.
  
1. אשף ההגדרה מזהה בדרך כלל את הרשם שלך, ומספק לך קישור להוראות מפורטות לעדכון רשומות ה- NS באתר האינטרנט של הרשם. אם לא, [שנה את שרתי הnamםכדי להגדיר את Office 365 עם כל רשם תחום](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - אם יש לך רשומות DNS קיימות, לדוגמה אתר אינטרנט קיים, אך מארח ה-DNS שלך זמין עבור [התחברות לתחום](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), בחר **באפשרות ' הוסף רשומות**עבורי '. בדף **' בחירת שירותים מקוונים** ', קבל את כל ברירות המחדל ובחר באפשרות ' **הבא**' ובחר ' **אישור** ' בדף המארח של DNS.
    - אם יש לך רשומות DNS קיימות עם מארחי DNS אחרים (שאינם זמינים עבור התחברות לתחום), תרצה לנהל את רשומות ה-DNS שלך כדי לוודא שהשירותים הקיימים יישארו מחוברים. לקבלת מידע נוסף, ראה [יסודות קבוצת מחשבים](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .

        ![הפעלת דף רשומות.](../media/activaterecords.png)

2. בצע את השלבים באשף ובדואר אלקטרוני ובשירותים אחרים שהוגדרו עבורך.

### <a name="protect-your-organization"></a>הגן על הארגון שלך 

פריטי המדיניות שאתה מגדיר באשף מוחלים באופן אוטומטי על [קבוצת אבטחה](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) הנקראת ' *כל המשתמשים*'. באפשרותך גם ליצור קבוצות נוספות להקצאת פריטי מדיניות במרכז הניהול.

1. על **הגנה מפני הגדלת מאיומי סייבר מתקדמים**, מומלץ לקבל את ברירות המחדל כדי לאפשר ל- [Office 365 מראש הגנה על איומים](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) לסרוק קבצים וקישורים ב-office apps.

    ![צילום מסך של עמוד הגנה מפני הגדלת.](../media/increasetreatprotection.png)


2. על מנת **למנוע דליפות של דף נתונים רגישים** , קבל את ברירות המחדל כדי להפעיל את מניעת אובדן נתונים של Office 365 (DLP) כדי לעקוב אחר נתונים רגישים ביישומי office ולמנוע את השיתוף המקרי של אלה מחוץ לארגון שלך.

3. בעמוד **הגנה על הנתונים ב-Office for mobile** , השאר את ניהול האפליקציות הניידות, הרחב את ההגדרות וסקור אותן ולאחר מכן בחר באפשרות **צור מדיניות ניהול אפליקציות ניידות**.

    ![צילום מסך של הגנה על נתונים ב-Office עבור דף נייד.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>אבטחת Windows 10 מחשבים אישיים

בניווט השמאלי, בחר **בהגדרה** ולאחר מכן, תחת **שירה ואבטחה**, בחר **באבטחת מחשבי Windows 10 שלך**. בחר **' תצוגה '** כדי להתחיל. לקבלת הוראות מלאות, ראה [אבטחת מחשבי Windows 10](secure-win-10-pcs.md) .

## <a name="deploy-office-365-client-apps"></a>פריסת Office 365 יישומי לקוח

אם בחרת להתקין באופן אוטומטי יישומי Office במהלך ההתקנה, היישומים יותקנו בהתקני Windows 10 לאחר שהמשתמשים יחתמו לתכלת לספירה מהתקני Windows שלהם, תוך שימוש באישורי העבודה שלהם.

כדי להתקין את Office ב-iOS נייד או בהתקני Android, ראה [הגדרת מכשירים ניידים עבור משתמשים עסקיים של Microsoft 365](set-up-mobile-devices.md).

באפשרותך גם להתקין את Office בנפרד. ראה [התקנת Office במחשב או במקינטוש](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) לקבלת הוראות.

## <a name="see-also"></a>למידע נוסף

[סרטוני הדרכה בנושא Microsoft 365 Business](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
