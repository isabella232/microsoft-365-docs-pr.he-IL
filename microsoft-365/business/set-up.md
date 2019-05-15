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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: למד כיצד להגדיר את Microsoft 365 עסקיים.
ms.openlocfilehash: 42a35810531b6abd5b22e5fdbce2c0cfea57b8d7
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074589"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>הגדרת Microsoft 365 עסקיים באשף ההתקנה

## <a name="add-your-domain-users-and-set-up-policies"></a>הוסף את התחום שלך, משתמשים, ולהגדיר מדיניות

![כרזה המצביעים על https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

בעת רכישת עסקי 365 של Microsoft, יש לך את האפשרות של משתמש תחום בבעלותך, או לקנות אחד במהלך [ההרשמה](sign-up.md).

- אם רכשת תחום חדש בעת שנרשמת, התחום שלך הוא קבוצת כל למעלה ובאפשרותך להעביר [הוסף משתמשים והקצה רשיונות](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>הוסף את התחום כדי להתאים אישית את הכניסה

1. להיכנס אל [מרכז admin Microsoft 365](https://admin.microsoft.com) באמצעות אישורי ניהול הכללית שלך. 

2. בחרו ' **הוסף תחום** או **הוסף משתמשים** כדי להפעיל את האשף.
    > [!IMPORTANT]
    > אם רכשת תחום במהלך ההרשמה, יהיה באפשרותך לא ראה **להוסיף תחום** שלב כאן. עבור לדף [הוספת משתמשים](#add-users-and-assign-licenses) במקום זאת.

    ![בחר באפשרות ' הוסף תחום.](media/addadomainadmincenter.png)
    
3. באשף, הזן את שם התחום שבו ברצונך להשתמש (כמו contoso.com).


    ![צילום מסך של התאמה אישית של דף הכניסה שלך.](media/personalizesignin.png)

    
4. בצע את השלבים באשף [רשומות DNS ליצור אצל כל ספק אירוח DNS עבור Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) מוודא שאתה הבעלים של התחום. אם ידוע לך מארח התחום שלך, ראה גם [הוראות ספציפיות של המחשב המארח](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    אם ספק אירוח GoDaddy, התהליך קל, באופן אוטומטי, תתבקש להיכנס ותן Microsoft לאמת בשמך:

    ![בדף ' GoDaddy אשר Access, בחר למועדים.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>הוספת משתמשים והקצאת רשיונות

באפשרותך להוסיף משתמשים באשף, אך באפשרותך גם [להוסיף משתמשים מאוחר יותר](add-users-m365b.md) במרכז admin. בנוסף, אם יש לך בבקר קבוצת מחשבים מקומי, באפשרותך להוסיף משתמשים עם [חיבור AD תכלת הרקיע](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>הוסף משתמשים באשף

כל המשתמשים שאתה מוסיף באשף לקבל להקצות רשיון העסק 365 Microsoft באופן אוטומטי.

![צילום מסך של הוספת משתמשים הדף החדש באשף](media/addnewuserspage.png)

1. אם המנוי Microsoft 365 העסק שלך כולל משתמשים קיימים (לדוגמה, אם השתמשת תכלת הרקיע התחבר AD), תקבל אפשרות להקצות רשיונות אותם כעת. קדימה, הוסף רשיונות גם להם.

3. לאחר שהוספת את המשתמשים, תקבל גם אפשרות לשתף את האישורים עם המשתמשים החדשים שהוספת. באפשרותך להדפיס אותם, לשלוח אותם בדואר אלקטרוני או להוריד אותם.

4. דלג על העברת הודעות דואר אלקטרוני ובחר **הבא** בדף **העברת הודעות דואר אלקטרוני**. 

    אם אתה מעביר מספק דואר אלקטרוני אחר וברצונך להעתיק את הנתונים שלך מאוחר יותר, באפשרותך לבצע [העברת דואר אלקטרוני ואנשי קשר Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).


### <a name="connect-your-domain"></a>חיבור התחום שלך

> [!NOTE]
> אם בחרת להשתמש בתחום .onmicrosoft, או אם השתמשת תכלת הרקיע AD התחבר כדי להגדיר משתמשים, לא תראה שלב זה.
  
להגדרת שירותים, עליך לעדכן כמה רשומות אצל מארח ה- DNS שלך או אצל רשם התחומים.
  
1. אשף ההגדרה מזהה בדרך כלל את הרשם שלך, ומספק לך קישור להוראות מפורטות לעדכון רשומות ה- NS באתר האינטרנט של הרשם. אם לא, [שינוי nameservers כדי להגדיר את Office 365 עם כל רשם התחום](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - אם יש לך רשומות DNS קיימות, לדוגמה אתר אינטרנט קיים, ברצונך לנהל רשומות DNS משלך כדי לוודא שהשירותים הקיימים להישאר מחובר. ראה [יסודות התחום](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) לקבלת מידע נוסף.

        ![לחבר את המחשבים שלך דף עם ניתן לנהל רשומות DNS בעצמי.](media/connectyourdomainpage.png)

2. בצע את השלבים באשף ו דואר אלקטרוני ושירותים אחרים יוגדר עבורך.

### <a name="set-up-security-policies-and-device-configurations"></a>הגדרת מדיניות אבטחה ותצורות התקן 

פריטי המדיניות שהגדרת באשף מוחלים באופן אוטומטי [קבוצת אבטחה](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) בשם *כל המשתמשים*. באפשרותך גם ליצור קבוצות נוספות כדי להקצות פריטי מדיניות כדי במרכז admin.

1. על **להגן על הקבצים שלך עבודה במכשירים ניידים** האפשרות **הגן על קבצי עבודה כאשר התקנים שאבדו או נגנבו** נבחרת כברירת מחדל. יש לך אפשרות להפעיל **לנהל את האופן שבו משתמשים ניגשים קבצי Office במכשירים ניידים**, ומומלץ זה.

    ![קבצי עבודה צילום מסך של הגנה על דף מכשירים ניידים.](media/protectworkfilesondevices.png)

     - הרחב את **הגנת קבצי עבודה כאשר התקנים שאבדו או נגנבו** כדי להציג את [ערכי ברירת המחדל](protect-work-files-on-lost-or-stolen-device.md):

        ![צילום מסך של ערכי ברירת מחדל עבור הגנה על קבצים במכשירים אבד.](media/protectworkfilesondevicesdefault.png)

    - בחר **לנהל את האופן שבו משתמשים ניגשים קבצי Office במכשירים ניידים** והרחב אותו כדי להציג את [ערכי ברירת המחדל](manage-user-access-on-mobile-devices.md). אנו ממליצים כי אתה מקבל את ערכי ברירת המחדל במהלך ההתקנה כדי ליצור פריטי מדיניות יישומים עבור Android, iOS ו- Windows 10 החלות על כל המשתמשים. ניתן ליצור פריטי מדיניות נוספים לאחר השלמת ההתקנה.

        ![צילום מסך של הגדרות הגנה עבור קבצי Office על נייד.](media/useraccessonmobile.png)

2. השלב האחרון על להגן על הנתונים ואת התקנים מאפשרת לך להגדיר פריטי מדיניות כדי לאבטח התקני Windows 10. הגדרות אלה מוחלים באופן אוטומטי כאשר Windows 10 משתמש מתחבר לארגון שלך. באפשרותך להרחיב **התקנים לאבטח Windows 10** כדי לראות ולשנות את [ערכי ברירת המחדל](secure-windows-10-devices.md).
3. באפשרותך גם [להתקין את Office באופן אוטומטי](install-office-on-windows-10-during-setup.md) במכשירים Windows 10.

    ![צילום מסך של הגדרת עמוד תצורת התקן של Windows 10.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a>לפרוס יישומי לקוח של Office 365

אם בחרת להתקין באופן אוטומטי יישומי Office ב במהלך ערכת למעלה, apps יתקין בהתקני Windows 10 לאחר שהמשתמשים נרשמו לשירות AD תכלת הרקיע מהתקנים Windows שלהם עם אישורי העבודה שלהם.
כדי להתקין את Office iOS נייד או התקנים Android, ראה [הגדרת מכשירים ניידים עבור משתמשים עסקיים 365 של Microsoft](set-up-mobile-devices.md).

באפשרותך גם להתקין את Office בנפרד. ראה [התקנת Office במחשב האישי או Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) לקבלת הוראות.
