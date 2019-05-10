---
title: התקנת Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660798"
---
# <a name="set-up-microsoft-365-business"></a>התקנת Microsoft 365 Business

לפני שתתחיל לעבוד, [לקבל ביקור 365 של Microsoft](get-microsoft-365-business.md) לקבלת פרטים, עיין הרשמה.

צפה בסרטון [וידאו קצר כיצד להגדיר עסקיים 365 של Microsoft](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) על-ידי שימוש בערכת למעלה אשף, וכאשר אין לך המקומית של Active Directory
  

## <a name="overview"></a>מבט כולל

ניתן לעשות זאת רוב להגדיר השלבים באשף ההתקנה, אך רשומים גם אפשרויות אחרות.

1. [הוסף קבוצת המחשבים שלך](#add-your-domain-to-personalize-sign-in) (אם רכשת את התחום שלך במהלך [להירשם](sign-up.md), שלב זה כבר בוצע.)
2. הוספת משתמשים. ניתן לעשות זאת באחת משלוש דרכים:
    - [אשף ההתקנה](#add-users-in-the-wizard).
    - השתמש סינכרון ספריות כדי [להוסיף משתמשים באמצעות חיבור AD תכלת הרקיע](#add-users-by-using-azure-ad-connect) אם ברשותך המקומית של Active directory.
    - באפשרותך גם [להוסיף משתמשים מאוחר יותר](add-users-m365b.md) במרכז admin.
3. הגדרת מדיניות אבטחה וקביעת תצורה של התקנים. ניתן לעשות זאת באחת משלוש דרכים:
    - [אשף ההתקנה](#set-up-policies-in-the-wizard).  
    - [מרכז admin](#modify-or-add-policies-in-the-admin-center).
    - [מרכז הניהוליים Intune](https://docs.microsoft.com/intune/what-is-device-management).
4. להגדיר ולנהל התקני Windows 10.

    בעת הצטרפות התקן WIndows 10 כדי AD תכלת הרקיע, כל פריטי המדיניות לקבל שהוחלה עליו.
    - קבע תצורות התקן Windows 10 של [אשף ההתקנה](#set-up-policies-in-the-wizard).
    - לצרף [התקן חדש של Windows 10](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) AD תכלת הרקיע.
    - צירוף של [התקן Windows 10 קיים](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) כדי AD תכלת הרקיע.
1. התקנת Office 365 עסקיים.
    - באפשרותך להתקין את Office באופן אוטומטי בהתקני Windows באמצעות [אשף ההתקנה](#set-up-policies-in-the-wizard).
    - באופן אוטומטי [להתקין את Office](auto-install-or-uninstall-office.md) ממרכז admin.
    - לאפשר למשתמשים [להתקין את יישומי Office](https://docs.microsoft.com/office365/admin/setup/install-applications) עבור Windows והתקנים.
     
1. הגדרת אבטחה נוספים.
    - אשף ההתקנה מוסיפה מדיניות כדי לאבטח את ההתקנים שלך, אך באפשרותך גם להנות מהיתרון של יכולות [אבטחה נוספות](#additional-security-settings) כדי מסייע מאובטח נתונים, וחשבונות דוא. 

## <a name="add-your-domain-users-and-set-up-policies"></a>הוסף את התחום שלך, משתמשים ולהגדיר מדיניות

![כרזה המצביעים על https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

בעת רכישת עסקי 365 של Microsoft, יש לך את האפשרות של משתמש תחום בבעלותך, או לקנות אחד במהלך [ההרשמה](sign-up.md).

- אם רכשת תחום חדש בעת שנרשמת, התחום שלך הוא קבוצת כל למעלה ובאפשרותך להעביר [הוסף משתמשים והקצה רשיונות](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>הוסף את התחום כדי להתאים אישית את הכניסה

1. להיכנס אל [מרכז admin Microsoft 365](https://admin.microsoft.com) באמצעות אישורי ניהול הכללית שלך. 

2. בחר **הוסף מחשבים** כדי להפעיל את האשף.

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
אם בקר קבוצת מחשבים מקומיים, אתה משתמש ב- Active Directory, ראה [כיצד משתמשים ddd באמצעות חיבור AD תכלת הרקיע](#add-users-by-using-azure-ad-connect).

![צילום מסך של הוספת משתמשים הדף החדש באשף](media/addnewuserspage.png)

1. אם המנוי שלך ל- Microsoft 365 Business כולל משתמשים קיימים (לדוגמה, אם השתמשת ב- Azure AD Connect), תהיה לך אפשרות להקצות להם רשיונות כעת. קדימה, הוסף רשיונות גם להם.

3. לאחר שהוספת את המשתמשים, תקבל גם אפשרות לשתף את האישורים עם המשתמשים החדשים שהוספת. באפשרותך להדפיס אותם, לשלוח אותם בדואר אלקטרוני או להוריד אותם.

4. דלג על העברת הודעות דואר אלקטרוני ובחר **הבא** בדף **העברת הודעות דואר אלקטרוני**. 

    אם אתה מעביר מספק דואר אלקטרוני אחר וברצונך להעתיק את הנתונים שלך מאוחר יותר, באפשרותך לבצע [העברת דואר אלקטרוני ואנשי קשר Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).

#### <a name="add-users-by-using-azure-ad-connect"></a>הוסף משתמשים באמצעות חיבור AD תכלת הרקיע

 אם ברשותך בקר תחום מקומי עם Active Directory, סינכרון למשתמשים עסקיים 365 של Microsoft באמצעות [חיבור AD תכלת הרקיע](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express). השלם פעולה זו לפני שתפעיל את אשף ההתקנה. באפשרותך להוריד אותו במרכז admin:

- עבור אל **משתמשים** \> **משתמשים פעילים**, בחר את שלוש הנקודות בראש הדף ולאחר מכן בחר **סינכרון ספריות** להוריד התחבר AD תכלת הרקיע.

    ![בדף משתמשים פעילים בחר אליפסות > הספריה snchronization.](media/setupdirsync.png)

    > [!IMPORTANT]
    > אם אתה יוצר משתמשים בדרך זו, עדיין יהיה עליך להקצות רשיונות אותם במרכז admin.

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a>להמשיך לגשת לתחום יישומים והתקנים

אם ברצונך להמשיך לגשת לתחום יישומים והתקנים, קרא את המאמרים הבאים עבור שני בדרך אחרת של הפעלת אשר:
  
- [מתן אפשרות לניהול מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business](manage-windows-devices.md)
    - זוהי הדרך המומלצת.

- [Access המקומית משאבים ממכשיר מצורף AD תכלת הרקיע ב- Microsoft 365 Business](access-resources.md)

### <a name="connect-your-domain"></a>חיבור התחום שלך

> [!NOTE]
> אם בחרת להשתמש בתחום .onmicrosoft, או אם השתמשת תכלת הרקיע AD התחבר כדי להגדיר משתמשים, לא תראה שלב זה.
  
להגדרת שירותים, עליך לעדכן כמה רשומות אצל מארח ה- DNS שלך או אצל רשם התחומים.
  
1. אשף ההגדרה מזהה בדרך כלל את הרשם שלך, ומספק לך קישור להוראות מפורטות לעדכון רשומות ה- NS באתר האינטרנט של הרשם. אם לא, [שינוי nameservers כדי להגדיר את Office 365 עם כל רשם התחום](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - אם יש לך רשומות DNS קיימות, לדוגמה אתר אינטרנט קיים, ברצונך לנהל רשומות DNS משלך כדי לוודא שהשירותים הקיימים להישאר מחובר. ראה [יסודות התחום](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) לקבלת מידע נוסף.

        ![לחבר את המחשבים שלך דף עם ניתן לנהל רשומות DNS בעצמי.](media/connectyourdomainpage.png)

2. בצע את השלבים באשף ו דואר אלקטרוני ושירותים אחרים יוגדר עבורך.

### <a name="set-up-security-policies-and-device-configurations"></a>הגדרת מדיניות אבטחה ותצורות התקן 

פריטי מדיניות אלה חלות על כל משתמש להעניק רשיון, או קבוצת משתמשים אם תחליט להקצות פריטי מדיניות שונים קבוצת משתמשים.

#### <a name="set-up-policies-in-the-wizard"></a>הגדרת מדיניות באשף

פריטי המדיניות שהגדרת באשף מוחלים באופן אוטומטי [קבוצת אבטחה](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) בשם *כל המשתמשים*.

1. על **להגן על הקבצים שלך עבודה במכשירים ניידים** האפשרות **הגן על קבצי עבודה כאשר התקנים שאבדו או נגנבו** נבחרת כברירת מחדל. יש לך אפשרות להפעיל **לנהל את האופן שבו משתמשים ניגשים קבצי Office במכשירים ניידים**, ומומלץ זה.

    ![קבצי עבודה צילום מסך של הגנה על דף מכשירים ניידים.](media/protectworkfilesondevices.png)

     - אם תרחיב את **הגנת קבצי עבודה כאשר התקנים אבד או נגנב**, [ערכי ברירת המחדל](protect-work-files-on-lost-or-stolen-device.md) הם שנבחרו מראש:

        ![צילום מסך של ערכי ברירת מחדל עבור הגנה על קבצים במכשירים אבד.](media/protectworkfilesondevicesdefault.png)

    - אם אתה בוחר **לנהל את האופן שבו משתמשים ניגשים קבצי Office במכשירים ניידים** להרחיב אותה, מוצגים [ערכי ברירת מחדל](manage-user-access-on-mobile-devices.md) . אנו ממליצים לקבל את ערכי ברירת המחדל במהלך ההתקנה כדי ליצור פריטי מדיניות של אפליקציות עבור Android,‏ iOS ו- Windows 10 שחלים על כל המשתמשים. ניתן ליצור פריטי מדיניות נוספים לאחר השלמת ההתקנה.

        ![צילום מסך של הגדרות הגנה עבור קבצי Office על נייד.](media/useraccessonmobile.png)

2. השלב האחרון על להגן על הנתונים ואת התקנים מאפשרת לך להגדיר פריטי מדיניות כדי לאבטח התקני Windows 10. הגדרות אלה מוחלים באופן אוטומטי כאשר Windows 10 משתמש מתחבר לארגון שלך. באפשרותך להרחיב **התקנים לאבטח Windows 10** כדי לראות ולשנות את [ערכי ברירת המחדל](secure-windows-10-devices.md).
3. באפשרותך גם [להתקין את Office באופן אוטומטי](install-office-on-windows-10-during-setup.md) במכשירים Windows 10.

    ![צילום מסך של הגדרת עמוד תצורת התקן של Windows 10.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a>לשנות או להוסיף פריטי מדיניות במרכז admin

ראה [ניהול עסקי 365 Microsoft](manage.md) עבור קישורים לנושאים כיצד להציג ולשנות התקן והגנה על יישום מדיניות, וכיצד להסיר נתונים, או לאפס את התקני משתמש.

## <a name="deploy-and-manage-windows-10"></a>לפרוס ולנהל Windows 10
ראה [הגדרת התקני Windows עבור משתמשים עסקיים 365 Microsoft](set-up-windows-devices.md) כדי להתחבר ידנית AD תכלת הרקיע במהלך ההתקנה עבור מחשבים חדשים, או על-ידי שינוי פרופיל הכניסה עבור המחשבים הקיימים. 

### <a name="use-autopilot-to-set-up-new-devices"></a>השתמש Autopilot כדי להגדיר התקנים חדשים

באפשרותך להשתמש ב- [Windows Autopilot](add-autopilot-devices-and-profile.md) כדי לקבוע מראש של התקנים 10 חלונות **חדשים** עבור משתמש באופן אוטומטי, אך ייתכן שיהיה קל יותר לקבל [שותף](https://www.microsoft.com/solution-providers/search) מי יכול לבצע זאת עבורך. באפשרותך גם לעבור לחנות [Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) ובקש טכנולוגיה ענן מומחה להגדיר התקנים חדשים שאתה רוכש עבורך.

### <a name="access-on-premises-resources"></a>Access המקומית משאבים

אם הארגון שלך משתמש Windows Server Active Directory המקומית, באפשרותך להגדיר עסקיים 365 של Microsoft להגנה על התקני Windows 10 שלך, תוך שמירה עדיין גישה למשאבים המקומית המחייבים אימות מקומי. בצע את השלבים [אפשר לתחום התקני Windows 10 להיות מנוהל על-ידי Microsoft 365 עסקיים](manage-windows-devices.md) כדי להגדיר זאת. זוהי השיטה המועדפת ואת התקנים במצב זה נקראות תכלת הרקיע היברידית AD לחבר התקנים.

אם בעסק שלך יש מקומי Active Directory המכילה כמה המקומית משאבים (כגון שיתופי קבצים ומדפסות), באפשרותך להעניק גישה ההתקנים המצורפים AD תכלת הרקיע שלך למשאבים אלה על-ידי ביצוע השלבים כאן: [Access המקומית משאבים מ תכלת הרקיע מצורף AD ההתקן ב- Microsoft 365 Business](access-resources.md).

## <a name="deploy-office-365-client-apps"></a>לפרוס יישומי לקוח של Office 365

אם בחרת להתקין באופן אוטומטי יישומי Office ב במהלך ערכת למעלה, apps יתקין בהתקני Windows 10 לאחר שהמשתמשים נרשמו לשירות AD תכלת הרקיע מהתקנים Windows שלהם עם אישורי העבודה שלהם.
כדי להתקין את Office iOS נייד או התקנים Android, ראה [הגדרת מכשירים ניידים עבור משתמשים עסקיים 365 של Microsoft](set-up-mobile-devices.md).

באפשרותך גם להתקין את Office בנפרד. ראה [התקנת Office במחשב האישי או Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) לקבלת הוראות.

## <a name="additional-security-settings"></a>הגדרות אבטחה נוספת

בנוסף אבטחה הגדרת תאימות באשף ההתקנה, באפשרותך גם להגדיר את ההגדרות הנוספות הבאות:
  
- **הגנה מפני תוכנות זדוניות דוא**
- **מסמכים מצורפים בטוחים איום מתקדם הגנה (ATP)**
- **קישורים מתאימים ATP**
- **דירה למניעת דיוג**
- **אחסון בארכיון של Exchange Online**
- **מניעת אובדן נתונים (DLP)**
- **הגנה על מידע תכלת הרקיע** (תכנון 1)
- **זמינות הפורטל Intune**

כדי לקבל מופעל, ראה [הגדרת מדיניות אבטחה מתקדמות](set-up-advanced-security.md).

ראה גם [העליון 10 דרכים לאבטחת העסק 365 Microsoft](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) עבור מפת דרכים של שיטות עבודה מומלצות של אבטחה.