---
title: התקנת Microsoft 365 Business
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: למד כיצד להגדיר את Microsoft 365 Business.
ms.openlocfilehash: 4f31af3fa63416d3b1bd7281f7712313252ad437
ms.sourcegitcommit: cbf117a4cd92a907115c9f10752f3c557361e586
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/10/2019
ms.locfileid: "37440595"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>הגדרת העסק של Microsoft 365 באשף ההתקנה

## <a name="add-your-domain-users-and-set-up-policies"></a>הוספת התחום, המשתמשים והגדרת המדיניות

[![תווית כדי ליידע אותך שמרכז הניהול משתנה ובאפשרותך למצוא פרטים נוספים ב-aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

בעת רכישת Microsoft 365 Business, יש לך את האפשרות להשתמש בתחום שבבעלותך, או לקנות אחד במהלך [ההרשמה](sign-up.md).

- אם רכשת תחום חדש בעת החתימה, התחום שלך מוגדר ובאפשרותך לעבור [להוספת משתמשים ולהקצות רשיונות](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>הוסף את התחום שלך להתאמה אישית של הכניסה

1. היכנס ל- [Microsoft 365 admin center](https://admin.microsoft.com) באמצעות אישורי המנהל הגלובלי שלך. 

2. בחר **בהוסף תחום** או **הוסף משתמשים** כדי להפעיל את האשף.
    > [!IMPORTANT]
    > אם רכשת תחום במהלך ההרשמה, לא תראה **הוספת שלב בתחום** כאן. עבור כדי [להוסיף משתמשים](#add-users-and-assign-licenses) במקום זאת.

    ![בחר באפשרות עבור לכיוונון.](media/gotosetupinadmincenter.png)
    
3. באשף, הזן את שם התחום בו ברצונך להשתמש (כגון contoso.com).


    ![צילום מסך של התאמה אישית של דף הכניסה שלך.](media/personalizesignin.png)

    
4. בצע את השלבים באשף כדי [ליצור רשומות dns בכל ספק dns המארח עבור Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) המאמת את התחום שלך. אם אתה מכיר את מארח התחום שלך, ראה גם את [ההנחיות הספציפיות למחשב המארח](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    אם ספק האירוח שלך הוא GoDaddy, או מארח אחר הזמין עם [התחברות לקבוצת מחשבים](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), התהליך יהיה פשוט ותתבקש באופן אוטומטי להיכנס ולאפשר למיקרוסופט לבצע אימות בשמך:

    ![בעמוד הרשאה לאישור, בחר באפשרות הרשאת.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>הוספת משתמשים והקצאת רשיונות

באפשרותך להוסיף משתמשים באשף, אך באפשרותך גם [להוסיף משתמשים בהמשך](add-users-m365b.md) מרכז הניהול. בנוסף, אם ברשותך בקר תחום מקומי, באפשרותך להוסיף משתמשים בעלי [התקשרות תכלת](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>הוספת משתמשים באשף

כל משתמש שתוסיף באשף יוקצה באופן אוטומטי לרשיון עסקי של Microsoft 365.

![צילום מסך של הדף ' הוספת משתמשים חדשים ' באשף](media/addnewuserspage.png)

1. אם למנוי העסקי שלך ב-Microsoft 365 יש משתמשים קיימים (לדוגמה, אם השתמשת בתכלת AD Connect), תקבל אפשרות להקצות להם רשיונות כעת. קדימה, הוסף רשיונות גם להם.

2. לאחר שהוספת את המשתמשים, תהיה לך גם אפשרות לשתף אישורים עם המשתמשים החדשים שהוספת. באפשרותך להדפיס אותם, לשלוח אותם בדואר אלקטרוני או להוריד אותם.

3. באפשרות צור צוותים עבור הארגון שלך, באפשרותך לבחור להוסיף צוותים ולהוסיף להם משתמשים. אתה יכול גם לעשות את זה מאוחר יותר. לקבלת מידע נוסף, ראה [יצירת צוות ברחבי החברה](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3).

4. דלג על העברת הודעות דואר אלקטרוני ובחר **הבא** בדף **העברת הודעות דואר אלקטרוני**. 

    אם אתה עובר מספק דואר אלקטרוני אחר וברצונך להעתיק את הנתונים שלך מאוחר יותר, באפשרותך [להעביר דואר אלקטרוני ואנשי קשר ל-Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).


### <a name="connect-your-domain"></a>חיבור התחום שלך

> [!NOTE]
> אם בחרת להשתמש בקבוצת המחשבים onmicrosoft, או בשימוש בתכלת-AD כדי להגדיר משתמשים, לא תראה שלב זה.
  
להגדרת שירותים, עליך לעדכן כמה רשומות אצל מארח ה- DNS שלך או אצל רשם התחומים.
  
1. אשף ההגדרה מזהה בדרך כלל את הרשם שלך, ומספק לך קישור להוראות מפורטות לעדכון רשומות ה- NS באתר האינטרנט של הרשם. אם לא, [שנה את שרתי הnamםכדי להגדיר את Office 365 עם כל רשם תחום](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - אם יש לך רשומות DNS קיימות, לדוגמה אתר אינטרנט קיים, אך מארח ה-DNS שלך זמין עבור [התחברות לתחום](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), בחר **באפשרות ' הוסף רשומות**עבורי '. בדף **' בחירת שירותים מקוונים** ', קבל את כל ברירות המחדל ובחר באפשרות ' **הבא**' ובחר ' **אישור** ' בדף המארח של DNS.
    - אם יש לך רשומות DNS קיימות עם מארחי DNS אחרים (שאינם זמינים עבור התחברות לתחום), תרצה לנהל את רשומות ה-DNS שלך כדי לוודא שהשירותים הקיימים יישארו מחוברים. לקבלת מידע נוסף, ראה [יסודות קבוצת מחשבים](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .

        ![חבר את דף התחום שלך עם אני ינהל את רשומות ה-DNS שלי.](media/connectyourdomainpage.png)

2. בצע את השלבים באשף ובדואר אלקטרוני ובשירותים אחרים שהוגדרו עבורך.

### <a name="protect-data-and-devices"></a>הגנה על נתונים והתקנים 

פריטי המדיניות שאתה מגדיר באשף מוחלים באופן אוטומטי על [קבוצת אבטחה](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) הנקראת ' *כל המשתמשים*'. באפשרותך גם ליצור קבוצות נוספות להקצאת פריטי מדיניות במרכז הניהול.

1. בהגנה על **קבצי העבודה שלך במכשירים ניידים** האפשרות **להגן על קבצי עבודה כאשר התקנים אובדים או גנובים מסומנים כברירת** מחדל. יש לך אפשרות להפעיל את **ניהול האופן שבו משתמשים ניגשים לקבצי Office במכשירים ניידים**, ומומלץ לעשות זאת.

    ![צילום מסך של הגנה על קבצי עבודה בדף התקנים ניידים.](media/protectworkfilesondevices.png)

     - הרחב **הגן על קבצי עבודה כאשר התקנים אובדים או גנובים** כדי להציג את [ערכי ברירת המחדל](protect-work-files-on-lost-or-stolen-device.md):

        ![צילום מסך של ערכי ברירת מחדל להגנה על קבצים בהתקנים אבודים.](media/protectworkfilesondevicesdefault.png)

    - בחר באפשרות **נהל את אופן הגישה של משתמשים לקבצי Office בהתקנים ניידים** והרחב אותו כדי להציג את [ערכי ברירת המחדל](manage-user-access-on-mobile-devices.md). מומלץ לקבל את ערכי ברירת המחדל במהלך ההתקנה כדי ליצור מדיניות יישומים עבור אנדרואיד, iOS ו-Windows 10 החלים על כל המשתמשים. ניתן ליצור פריטי מדיניות נוספים לאחר השלמת ההתקנה.

        ![צילום מסך של הגדרות הגנה עבור קבצי Office בנייד.](media/useraccessonmobile.png)

2. השלב האחרון בהגנה על נתונים והתקנים מאפשר לך להגדיר מדיניות לאבטחת התקני Windows 10. הגדרות אלה מוחלות באופן אוטומטי בעת התחברות Windows 10 של משתמש לארגון. באפשרותך להרחיב **התקנים מאובטחים של Windows 10** כדי לראות ולשנות את [ערכי ברירת המחדל](secure-windows-10-devices.md).
3. באפשרותך גם לבחור [להתקין באופן אוטומטי את Office](install-office-on-windows-10-during-setup.md) בהתקני Windows 10.

    ![צילום מסך של הגדרת Windows 10 תצורת התקן הדף.](media/setwin10config.png)


## <a name="deploy-office-365-client-apps"></a>פריסת Office 365 יישומי לקוח

אם בחרת להתקין באופן אוטומטי יישומי Office במהלך ההתקנה, היישומים יותקנו בהתקני Windows 10 לאחר שהמשתמשים יחתמו לתכלת המחשב מהתקני Windows שלהם עם אישורי העבודה שלהם.
כדי להתקין את Office ב-iOS נייד או בהתקני Android, ראה [הגדרת מכשירים ניידים עבור משתמשים עסקיים של Microsoft 365](set-up-mobile-devices.md).

באפשרותך גם להתקין את Office בנפרד. ראה [התקנת Office במחשב או במקינטוש](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) לקבלת הוראות.
