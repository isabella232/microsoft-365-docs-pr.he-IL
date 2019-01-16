---
title: תחילת העבודה עם Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 9/20/2018
ms.audience: Admin
ms.topic: overview
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: למד כיצד להגדיר עסקיים 365 של Microsoft.
ms.openlocfilehash: ee15ffa98de032d7936d950124cdf772335949bd
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983284"
---
# <a name="get-started-with-microsoft-365-business"></a>תחילת העבודה עם Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>מהו Microsoft 365 Business

Microsoft 365 Business הוא ערכה מקיפה של כלי שיתוף פעולה ופרודוקטיביות עסקית, כגון Outlook,‏ Word,‏ Excel ומוצרי Office אחרים שמעודכנים תמיד. באפשרותך להגן על קבצי העבודה שלך בכל מכשירי iOS,‏ Android ו- Windows 10 שברשותך עם אבטחה פשוטה לניהול ברמת הארגון.
  
Microsoft 365 Business נועד עבור עד 300 רשיונות. אם אתה זקוק לרשיונות נוספים, עיין בתיעוד של [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) לקבלת מידע נוסף. 
  
## <a name="get-microsoft-365-business"></a>השגת Microsoft 365 Business

- אם יש לך שותף, הוא יקבל את Microsoft 365 Business: [השג את Microsoft 365 Business ממרכז השותפים של Microsoft](get-microsoft-365-business.md).
    
- אם אין לך שותף ואתה מעוניין להשיג את Microsoft 365 Business, באפשרותך [לקנות אותו כאן](https://www.microsoft.com/en-us/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>התקנת Microsoft 365 Business

 **מבט כולל על חבילת עסקית של 365 Microsoft להגדיר**
  
הדיאגרמה הבאה מתארת כיצד להגדיר מנהלים עסקיים 365 של Microsoft. הוא גם מתאר את השלבים כדי להכין מחשבים אישיים של Windows עבור העסק 365 של Microsoft. באפשרותך גם להוסיף התקנים חדשים כדי במרכז ניהול עסקי 365 Microsoft עם [Windows AutoPilot](add-autopilot-devices-and-profile.md). באפשרותך להשתמש AutoPilot כדי להגדיר ולהגדיר מראש התקנים חדשים, שכנוע מוכן לשימוש יעיל כמו משתמש יוסיף באמצעות אישורי Microsoft 365 העסק שלהם.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: הגדרת Microsoft 365 עסקי (מנהל)

היכנס ל[מרכז הניהול של Microsoft 365 Business](https://portal.office.com/adminportal/home) עם אישורי מנהל מערכת כללי, ובצע את השלבים הבאים כדי להתקין את Microsoft 365 Business. 
  
1. [דרישות מוקדמות להגנה על נתונים במכשירים עם Microsoft 365 Business](pre-requisites-for-data-protection.md)
    
    קרא את הדרישות המוקדמות תחילה כדי לוודא שהמכשירים שלך מוכנים לקראת Microsoft 365 Business.
    
2. [התקנה של Microsoft 365 Business באמצעות אשף ההתקנה](set-up.md)
    
    אם אתה **מעביר לצמיתות מ Active Directory המקומי אל הענן**, באפשרותך להוסיף משתמשים שלך באופן ידני במרכז ניהול עסקי 365 Microsoft באמצעות אשף ההתקנה, או באפשרותך לבצע סינכרון חד-פעמי עם חיבור AD תכלת הרקיע. קיימות שתי דרכים לעשות זאת: 
    
  - אם יש לך Exchange 2010, Exchange 2013 או שרת Exchange 2016, באפשרותך [שימוש מינימלי היברידית במהירות להעביר תיבות דואר של Exchange Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). השלבים היברידית מינימלית לכלול סינכרון חד-פעמית של משתמשים AD תכלת הרקיע וכן דואר אלקטרוני בהעברה מ מקומי אל הענן. לאחר השלמת ההעברה דוא ל, סינכרון ספריות מבוטלת באופן אוטומטי בעת שימוש בשיטה זו.
    
  - השתמש באשף סינכרון מדריכי הכתובות של Office 365 כדי לסנכרן את המשתמשים שלך עם הענן. בצע את השלבים המפורטים תחת [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) כדי להשלים את התהליך. לאחר שתסנכרן את המשתמשים שלך עם הענן, תצטרך [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    כמו כן יהיה עליך להעניק לכל משתמש שנוסף באופן זה רשיון לעסק 365 של Microsoft. באפשרותך לעשות זאת [אשף ההתקנה](set-up.md), או [להקצות רשיונות המשתמשים ב- Office 365 עבור העסק](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: הכנת מכשירים ניידים

פעל לפי[הגדרת מכשירים ניידים עבור משתמשים עסקיים 365 של Microsoft](set-up-mobile-devices.md) כדי להתקין את יישומי Office וודא שהם מוגנים על-ידי ביקור 365 Microsoft והתקנים. 
  
### <a name="3-prepare-pcs"></a>3: הכנת מחשבים אישיים

מנהלים ניתן לבחור מראש הגדרות עבור התקנים חדשים מחשבים אישיים של 10 Windows באמצעות [Windows AutoPilot](add-autopilot-devices-and-profile.md). משתמשים יכולים להגדיר שלהם התקנים 10 חלונות קיימים או חדשים על-ידי ביצוע השלבים בנושא זה: [הגדרת מחשבי Windows עבור משתמשים עסקיים 365 של Microsoft](set-up-windows-devices.md). עבור התקנים קיימים משתמשים יכולים גם **אם תרצה**[להעביר קבצים כדי OneDrive עבור העסק](move-files-to-onedrive.md). באפשרותם להשתמש גם כלים של ספקים חיצוניים כדי להעביר קבצים המשויכים לפרופיל Windows כדי OneDrive.
  
אם הארגון שלך משתמש Windows Server Active Directory המקומית, באפשרותך להגדיר עסקיים 365 של Microsoft להגנה על התקני Windows 10 שלך, תוך שמירה עדיין גישה למשאבים המקומית המחייבים אימות מקומי. בצע את השלבים [אפשר לתחום התקני Windows 10 להיות מנוהל על-ידי Microsoft 365 עסקיים](manage-windows-devices.md) כדי להגדיר זאת. זוהי השיטה המועדפת ואת התקנים במצב זה נקראות **היברידית AD תכלת הרקיע לחבר התקנים**. 
  
אם לשמור את מקומי Active Directory המכילה כמה המקומית משאבים (כגון שיתופי קבצים ומדפסות), באפשרותך להעניק גישה **ההתקנים המצורפים AD תכלת הרקיע** שלך למשאבים אלה על-ידי ביצוע השלבים כאן: [Access המקומית משאבים מ תכלת הרקיע מצורף AD ההתקן ב- Microsoft 365 Business](access-resources.md).
  
לאחר הגדרת Windows 10 מחשבים, באפשרותך [להתקין את Office באופן אוטומטי](auto-install-or-uninstall-office.md) להתקנים. 
  
## <a name="contact-support"></a>פנה לתמיכה

 **אם עליך ליצור קשר עם התמיכה:**
  
- פנה לשותף שלך.
    
- כמנהל עסקי 365 של Microsoft, יש לך גישה אל צוות התמיכה של הלקוח שלנו, ** [פנה למרכז התמיכה עבור מוצרים עסקיים - Admin עזרה](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
