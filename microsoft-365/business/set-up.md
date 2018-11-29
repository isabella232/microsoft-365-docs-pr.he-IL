---
title: הגדרה של Microsoft 365 Business באמצעות אשף ההגדרה
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
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: למד כיצד להגדיר עסקיים 365 של Microsoft על-ידי השלמת ארבעה שלבים.
ms.openlocfilehash: f57239b884bd2e186c0bc01973130a10fa4cfe84
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982194"
---
# <a name="set-up-microsoft-365-business-by-using-the-setup-wizard"></a>הגדרה של Microsoft 365 Business באמצעות אשף ההגדרה

השלם את שלבים 1-4 להלן.
  
### <a name="set-up-microsoft-365-business"></a>התקנת Microsoft 365 Business

צפה בסרטון וידאו המסביר כיצד להגדיר עסקיים 365 Microsoft כשאין לך המקומית של Active Directory:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/0705c337-f3e8-4d28-bb6c-530cd28e99f2?autoplay=false]
  
השלבים הגדרת כוללים מידע עבור כיוונונים הכוללים Active Directory המקומי. אם ברצונך להמשיך לגשת לתחום התקנים, קרא את המאמרים הבאים עבור שני בדרך אחרת של הפעלת אשר, ולהשלים את השלבים לפני שתפעיל את אשף ההתקנה:
  
- [מתן אפשרות לניהול מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business](manage-windows-devices.md)
    
    -זוהי הדרך המומלצת.
    
- [Access המקומית משאבים ממכשיר מצורף AD תכלת הרקיע ב- Microsoft 365 Business](access-resources.md)
    
### <a name="step-1-personalize-sign-in"></a>שלב 1: התאמה אישית של כניסה

1. היכנס ל- [Microsoft 365 Business](https://portal.microsoft.com) באמצעות אישורים של מנהל מערכת כללי. בחר את האריח **ניהול** כדי לעבור אל מרכז הניהול. 
    
2. בחר **התחל בהגדרה** (בהתאם למצב שלך ייתכן שתראה **המשך בהגדרה** במקום זאת) במרכז הניהול כדי להפעיל את האשף. 
    
3. הזן את שם התחום שבו ברצונך להשתמש (כגון contoso.com).
    
    המשך והזן את התחום שלך אפילו אם וידאת אותה תוך שימוש התחבר AD תכלת הרקיע, לדוגמה. שני השלבים הבאים אינם חלים על לך אם השתמשת תכלת הרקיע AD התחבר כדי לאמת את התחום שלך.
    
4. בצע את השלבים באשף [רשומות DNS ליצור אצל כל ספק אירוח DNS עבור Office 365](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) מוודא שאתה הבעלים של התחום. 
    
    באפשרותך להציג וידאו דוגמה של [וידאו: תוכנית ההתקנה של Office 365 במרכז Admin חדשה](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8). שים לב וידאו זה אינו כולל את השלבים הגנת הנתונים של Microsoft 365 העסק.
    
    ![Screenshot of the Business Cloud Suite setup wizard.](media/3c4fd40c-2de1-4a87-8ee0-78d3928c7bb7.png)
  
### <a name="step-2-add-users-and-assign-licenses"></a>שלב 2: הוספת משתמשים והקצה רשיונות

1. ניתן להוסיף משתמשים כאן, או [להוסיף משתמשים בהמשך](add-users-m365b.md) במרכז הניהול. 
    
    לכל המשתמשים שאתה מוסיף מוקצה באופן אוטומטי רשיון Microsoft 365 Business.
    
2. אם המנוי שלך ל- Microsoft 365 Business כולל משתמשים קיימים (לדוגמה, אם השתמשת ב- Azure AD Connect), תהיה לך אפשרות להקצות להם רשיונות כעת. קדימה, הוסף רשיונות גם להם.
    
3. תהיה לך גם אפשרות לשתף אישורים עם המשתמשים החדשים שהוספת. באפשרותך להדפיס אותם, לשלוח אותם בדואר אלקטרוני או להוריד אותם.
    
4. דלג על העברת הודעות דואר אלקטרוני ובחר **הבא** בדף **העברת הודעות דואר אלקטרוני**. 
    
    אם אתה מעביר מספק דואר אלקטרוני אחר וברצונך להעתיק את הנתונים שלך מאוחר יותר, באפשרותך לבצע [העברת דואר אלקטרוני ואנשי קשר Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).
    
    ![Screenshot of two new users added in the setup wizard](media/8f729967-5c65-4ceb-b737-18119db40564.png)
  
### <a name="step-3-connect-your-domain"></a>שלב 3: חיבור המחשבים שלך

> [!NOTE]
> אם בחרת להשתמש בתחום .onmicrosoft, או אם השתמשת התחבר AD תכלת הרקיע, לא תראה שלב זה. 
  
להגדרת שירותים, עליך לעדכן כמה רשומות אצל מארח ה- DNS שלך או אצל רשם התחומים.
  
1. אשף ההתקנה בדרך כלל מזהה רשם שלך ומעניק לך קישור הוראות שלב אחר שלב עבור עדכון ברשומות NS שלך באתר רשם. אם לא, [שינוי nameservers כדי להגדיר את Office 365 עם כל רשם התחום](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).
    
2. דואר אלקטרוני ושירותים אחרים יוגדרו עבורך
    
### <a name="step-4-manage-devices-and-work-files"></a>שלב 4: ניהול התקנים ולעבוד קבצים

1. על **קבצי עבודה הגן במכשירים הניידים שלך** עמוד הגדר **הגנה על קבצים עבודה כאשר התקנים שאבדו או נגנבו** והגדרות **לנהל את האופן שבו משתמשים ניגשים קבצי Office במכשירים ניידים** **בסרגל**. באפשרותך גם לגשת לכל משנה הגדרת על-ידי לחיצה על הסוגריים הזוויתיים לצד כל הגדרה.
  
  כל הקבצים עבודת המשתמשים המורשים שלך כעת מוגנים ב- iOS והתקנים Android, מיד כאשר הם [להתקין יישומי Office](set-up-mobile-devices.md) (ולאמת עם אישורי Microsoft 365 העסק שלהם). 
  
  ![Screenshot of protect work files on your mobile devices page](media/3139a9aa-6228-4e74-8166-c6a886d7319f.PNG)
  
2. בדף ' **קביעת התצורה של התקן Windows 10** , להגדיר הגדרה **מאובטחת התקנים 10 של Windows** **ב-**.
  
   באפשרותך גם לגשת לכל משנה הגדרת על-ידי לחיצה על לחצן הסוגר הזוויתי לצידו.
  
3. לקבוע את ההגדרה **התקנת Office במכשירים 10 Windows** **כן** אם כל המשתמשים בעלי מחשבים Windows 10, ומתקינה או Office לא קיים, או לחץ על run על התקנת Office. אם זה אינו המקרה, הגדר אפשרות זו כ- **No**. באפשרותך [להתקין את Office באופן אוטומטי](auto-install-or-uninstall-office.md) במועד מאוחר יותר ממרכז admin לאחר שהכנת את מחשבי המשתמשים. לקבלת הוראות, ראה [הכנת עבור התקנת לקוח של Office](prepare-for-office-client-deployment.md).
  
    ניתן להקרין מיד כאשר הם קבצי עבודה של המשתמשים המורשים בהתקני Windows 10 [התקן Windows 10 שלהם להצטרף](set-up-windows-devices.md) לקבוצת מחשבים עסקיים Microsoft 365 AD תכלת הרקיע או [להתקין את Windows 10 במחשב חדש](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) בעת הצטרפות בו-זמנית Microsoft 365 תחום של AD תכלת הרקיע עסקיים. 
  
4. לחץ על **הבא** וסיימת עם ההתקנה. 
  
    אנא ספק לנו משוב בשלב זה, כדי לעזור לנו בשיפור החוויה.
  
    ![Screenshot of Prepare Windows 10 devices page](media/bff701c1-48a3-44f4-aa95-9d959d57c85b.PNG)
  
## <a name="additional-security-settings"></a>הגדרות אבטחה נוספת

בנוסף אבטחה הגדרת תאימות באשף ההתקנה, באפשרותך גם להגדיר את ההגדרות הנוספות הבאות:
  
- הגדר הגנה מפני קבצים מצורפים לא בטוחים. **הגנה מפני איום מתקדם** (ATP) מזהה תוכן זדוני ולאחר מכן תחסום את המסירה של קבצים מצורפים לא בטוחים, לסייע להגן עליך מפני מזימות דיוג ותוכנות הידבקויות ransomware. כדי להפעיל הגנה מצורף, ראה [הגדרת פריטי מדיניות של Office 365 ATP מסמכים מצורפים בטוחים](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).
    
- הגן על הסביבה שלך כאשר משתמשים לוחצים על קישורים זדוניים. ATP בוחן קישורים בדואר אלקטרוני בזמן שמשתמש לוחץ אותם. אם קישור אינו בטוח, המשתמש אזהרות לא כדי לבקר באתר או ליידע האתר זה נחסם. פעולה זו מסייעת בהגנה מפני הונאות דיוג. [הגדרת מדיניות קישורים בטוח של Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) או [להגדיר פריטי מדיניות של קישורי בטוח של Office 365 ATP](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).
    
- ניתן לשמר את כל התוכן של תיבת הדואר כולל פריטים שנמחקו על-ידי הצבת תיבת הדואר כולה של משתמש על **תביעה משפטית החזק**. לקבלת הוראות, ראה 
- [הגדרת דואר אלקטרוני שמירה עם Exchange Online בארכיון](security-features.md#set-up-email-retention-with-exchange-online-archiving).
    
- להגדיר **מדיניות שמירה**מותאם אישית, לדוגמה, כדי לשמר למשך פרק זמן מסוים או למחוק את התוכן לצמיתות, בסוף תקופת ההחזקה. באפשרותך להפעיל מדיניות שמירה מותאמת אישית ב ניירות ערך מרכז תאימות, עבור אל **התנהלות נתונים** \> **השמירה**, ולאחר מכן בצע את השלבים באשף. לקבלת מידע נוסף, ראה [מבט כולל על מדיניות שמירה](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).
    
## <a name="next-steps"></a>השלבים הבאים

עבור משתמשים בעלי רשיונות, השלב הבא הוא להגדיר את המכשירים.<br/> ראה [הגדרת מכשירי Windows עבור משתמשי Microsoft 365 Business](set-up-windows-devices.md) ו [התקנת מכשירים ניידים עבור משתמשי Microsoft 365 Business](set-up-mobile-devices.md). <br/>ראה [ניהול Microsoft 365 Business](manage.md) לקבלת קישורים לנושאים העוסקים בהגדרת כללי מדיניות להגנה על מכשירים ויישומים, ובהסרת נתונים ממכשירי המשתמשים. 
  


