---
title: תחילת העבודה עם Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: למד להגדיר את Microsoft 365 Business.
ms.openlocfilehash: 4c744d6a900dba3c11ee51e75602a430268e15bb
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/07/2019
ms.locfileid: "38029103"
---
# <a name="get-started-with-microsoft-365-business"></a>תחילת העבודה עם Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>מהו Microsoft 365 Business

Microsoft 365 Business הוא ערכה מקיפה של כלי שיתוף פעולה ופרודוקטיביות עסקית, כגון Outlook,‏ Word,‏ Excel ומוצרי Office אחרים שמעודכנים תמיד. באפשרותך להגן על קבצי העבודה שלך בכל מכשירי iOS,‏ Android ו- Windows 10 שברשותך עם אבטחה פשוטה לניהול ברמת הארגון.
  
Microsoft 365 Business נועד עבור עד 300 רשיונות. אם אתה זקוק לרשיונות נוספים, עיין בתיעוד של [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) לקבלת מידע נוסף. 
  
## <a name="get-microsoft-365-business"></a>השג את Microsoft 365 Business

- אם יש לך שותף, הוא יקבל את Microsoft 365 Business: [השג את Microsoft 365 Business ממרכז השותפים של Microsoft](get-microsoft-365-business.md).
    
- אם אין לך שותף ואתה מעוניין להשיג את Microsoft 365 Business, באפשרותך [לקנות אותו כאן](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>התקנת Microsoft 365 Business

 **מבט כולל על חבילת העסקים של Microsoft 365 מוגדר**
  
הדיאגרמה הבאה מתארת כיצד מנהלים מגדיר עסק של Microsoft 365 Business. היא גם מתארת את השלבים להכנת מחשבי Windows עבור Microsoft 365 Business. באפשרותך גם להוסיף מכשירים חדשים במרכז הניהול של Microsoft 365 Business עם [Windows AutoPilot](add-autopilot-devices-and-profile.md). באפשרותך להשתמש ב- AutoPilot כדי להגדיר ולקבוע מראש את התצורה של מכשירים חדשים, כדי להכין אותם לשימוש פרודוקטיבי ברגע שהמשתמש מתחבר עם אישורי Microsoft 365 Business שלו.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: הגדרת מיקרוסופט 365 עסקים (מנהל)

היכנס ל[מרכז הניהול של Microsoft 365 Business](https://portal.office.com/adminportal/home) עם אישורי מנהל מערכת כללי, ובצע את השלבים הבאים כדי להתקין את Microsoft 365 Business. 
  
1. [דרישות מוקדמות להגנה על נתונים במכשירים עם Microsoft 365 Business](pre-requisites-for-data-protection.md)
    
    קרא את הדרישות המוקדמות תחילה כדי לוודא שהמכשירים שלך מוכנים לקראת Microsoft 365 Business.
    
2. [התקנה של Microsoft 365 Business באמצעות אשף ההתקנה](set-up.md)
    
    אם אתה **עובר לצמיתות מתוך Active Directory מקומי אל ענן הצמתים**, באפשרותך להוסיף את המשתמשים שלך באופן ידני במרכז הניהול העסקי של Microsoft 365 באמצעות אשף ההתקנה, או לבצע סינכרון חד פעמי עם ' התחברות למטה-התכלת '. ניתן לעשות זאת בשתי דרכים: 
    
  - אם יש לך גם שרת Exchange 2010, Exchange 2013 או Exchange 2016, [באפשרותך להשתמש באפשרות ' היברידית מינימלית ' כדי להעביר במהירות תיבות דואר של exchange ל-Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). שלבי התצורה ההיברידית המינימלית כוללים סינכרון חד-פעמי של משתמשים עם Azure AD וכן העברת דואר אלקטרוני מסביבה מקומית לענן. לאחר השלמת העברת הדואר האלקטרוני, סינכרון מדריכי הכתובות מבוטל באופן אוטומטי בעת השימוש בשיטה זו.
    
  - השתמש באשף סינכרון מדריכי הכתובות של Office 365 כדי לסנכרן את המשתמשים שלך עם הענן. בצע את השלבים המפורטים תחת [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) כדי להשלים את התהליך. לאחר שתסנכרן את המשתמשים שלך עם הענן, תצטרך [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    בנוסף, תצטרך לתת לכל משתמש שנוסף בדרך זו רשיון ל- Microsoft 365 Business. באפשרותך לעשות זאת [באשף ההתקנה](set-up.md), או [להקצות רשיונות למשתמשים ב-Office 365 לצורך עסקים](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: הכנת מכשירים ניידים

בצע את השלבים[בהגדרת התקנים ניידים עבור microsoft 365 משתמשים עסקיים](set-up-mobile-devices.md) כדי להתקין יישומי Office בהתקנים ולוודא שהם מוגנים על-ידי Microsoft 365 Business. 
  
### <a name="3-prepare-pcs"></a>3: הכנת מחשבים אישיים

מנהלים יכולים לבחור הגדרות מראש עבור התקנים חדשים של Windows 10 PCs באמצעות [Windows טייס אוטומטי](add-autopilot-devices-and-profile.md). משתמשים יכולים להגדיר את ההתקנים הקיימים או החדשים של Windows 10 על-ידי ביצוע השלבים בנושא זה: [הגדרת מחשבי Windows עבור משתמשים עסקיים של Microsoft 365](set-up-windows-devices.md). עבור התקנים קיימים משתמשים יכולים גם באופן **אופציונלי**[להעביר קבצים לכונן אחד עבור עסקים](move-files-to-onedrive.md). הם יכולים גם להשתמש בכלים של צד שלישי כדי להעביר קבצים המשויכים לפרופיל של Windows ל-OneDrive.
  
אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business כדי להגן על התקני Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים המחייבים אימות מקומי. בצע את השלבים [בהפעלת התקני Windows 10 המצורפים לתחום כדי שיוכלו להיות מנוהלים על-ידי Microsoft 365 Business](manage-windows-devices.md) כדי להגדיר זאת. זוהי השיטה המועדפת והמכשירים במצב זה נקראים " **היברידית תכלת" התקנים המצורפים**. 
  
אם אתה שומר על active Directory מקומי המכיל משאבים מסוימים מקומיים (כגון שיתופי קבצים ומדפסות), באפשרותך להעניק **להתקנים המצורפים** למשאבים אלה גישה אל משאבים אלה על-ידי ביצוע השלבים כאן: [גישה למשאבים מקומיים מ המכשיר המצורף למודעה ב-Microsoft 365 Business](access-resources.md).
  
לאחר הגדרת מחשבי Windows 10, באפשרותך [להתקין את Office באופן אוטומטי](auto-install-or-uninstall-office.md) בהתקנים. 
  
## <a name="contact-support"></a>פנה לתמיכה

 **אם עליך ליצור קשר עם התמיכה:**
  
- פנה לשותף שלך.
    
- כמנהל עסקים של Microsoft 365, יש לך גישה לצוות התמיכה בלקוחות שלנו, ** [צור קשר עם תמיכה עבור מוצרים עסקיים-עזרה מנהל](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="related-topics"></a>נושאים קרובים
[תיעוד ומשאבים עבור Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[ניהול Microsoft 365 Business](manage.md)[מעבר אל Microsoft 365 Business](migrate-to-microsoft-365-business.md)
  

