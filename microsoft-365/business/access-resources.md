---
title: Access המקומית משאבים ממכשיר מצורף AD תכלת הרקיע ב- Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: למד כיצד לקבל גישה למשאבים המקומית כמו יישומים שורה של העסק, שיתופי קבצים ומדפסות מתכלת הרקיע של Active Directory המצורפים להתקן Windows 10.
ms.openlocfilehash: 212685bc229f519152e69b09d0a745bfac7a38cd
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32276880"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Access המקומית משאבים ממכשיר מצורף AD תכלת הרקיע ב- Microsoft 365 Business

כל התקן Windows 10 הוא תכלת הרקיע Active Directory מצורף תהיה גישה לכל המשאבים מבוססות ענן כגון יישומי Office 365 שלך ואת להיות מוגן על-ידי Microsoft 365 עסקיים. גם לאפשר גישה למשאבים המקומית כמו apps של קו עסקיים (LOB), שיתופי קבצים ומדפסות, עליך לסנכרן המקומית של Active Directory עם תכלת הרקיע Active Directory באמצעות [חיבור AD תכלת הרקיע](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). ראה [מבוא ניהול התקנים ב- Active Directory תכלת הרקיע](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) כדי ללמוד עוד. 
  
## <a name="run-azure-ad-connect"></a>הפעל AD תכלת הרקיע ההתקשרות

השלם את השלבים הבאים כדי לאפשר להתקנים AD תכלת הרקיע מצורף של הארגון שלך לקבל גישה למשאבים המקומית.
  
1. כדי לסנכרן שלך משתמשים, קבוצות ואנשי קשר מ- Active Directory המקומי לתוך תכלת הרקיע Active Directory, הפעל את אשף סינכרון הספריה ולאחר התחבר AD תכלת הרקיע כפי שמתואר [להגדיר סינכרון ספריות עבור Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. לאחר סינכרון ספריות הושלמה, ודא ש-AD תכלת הרקיע מצורף הם התקני Windows 10 של הארגון שלך. שלב זה מבוצע בנפרד בכל התקן Windows 10. לקבלת פרטים, ראה [הגדרת התקני Windows עבור משתמשים עסקיים 365 של Microsoft](set-up-windows-devices.md) . 
    
3. לאחר ההתקנים 10 חלונות הם AD תכלת הרקיע המצורפים, כל משתמש עליך לאתחל מחדש התקנים והכניסה שלהם עם אישורי Microsoft 365 העסק שלהם. כל ההתקנים כעת תהיה גישה למשאבים המקומית גם.
    
ללא שלבים נוספים נדרשים כדי לקבל גישה מקומית משאבים עבור הפרסומת תכלת הרקיע לחבר התקנים. זהו פונקציונליות מובנית זמינה ב- Windows 10. 
  
אם הארגון שלך אינו מוכן לפריסה בתכלת הרקיע AD מצורף תצורת ההתקן המתואר לעיל, שקול להגדיר את [תצורת ההתקן Joined AD תכלת הרקיע היברידית](manage-windows-devices.md).
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>שיקולים בעת הצטרפות התקני Windows שלך כדי AD תכלת הרקיע

אם אתה AD תכלת הרקיע הצטרפות התקן Windows שהיתה בעבר לתחום או לקבוצת עבודה, עליך לקחת בחשבון את המגבלות הבאות:
  
- כאשר התקן AD תכלת הרקיע מצטרף, הוא יוצר משתמש חדש ללא הפניה פרופיל קיים. כדי לפתור בעיה זו, פרופילי צורך להעביר באופן ידני. פרופיל המשתמש מכיל מידע, כגון מועדפים קבצים מקומיים, הגדרות הדפדפן, הגדרות תפריט התחלה, וכו '. הגישה הטובה ביותר היא למצוא כלי צד שלישי כדי למפות הגדרות וקבצים קיימים לפרופיל החדש
    
- אם ההתקן משתמש אובייקטי מדיניות קבוצתית (GPO), אובייקטי Gpo מסוימים ייתכן שאין דומים [התצורה של ספק שירות](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) ב- Intune. הפעל את [הכלי MMAT](https://www.microsoft.com/download/details.aspx?id=45520) כדי למצוא Csp דומים עבור אובייקטי Gpo קיים. 
    
- למשתמשים לא תהיה אפשרות לאמת ליישומים התלויים אימות של Active Directory. כדי להתמודד עם זה להעריך באמצעות app מדור קודם ושקול עדכון ליישום העושה אימות מודרניים במידת האפשר.
    
- גילוי מדפסת הספריה הפעילה לא יפעלו. כדי לפתור בעיה זו, מספקים נתיבי הדפסה ישירה עבור כל המשתמשים או למנף [הדפסה ענן היברידי](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
    

