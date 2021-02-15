---
title: גישה למשאבים מקומיים באמצעות מכשיר מצורף לכיוון תכלת ב-Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: למד כיצד לקבל גישה למשאבים מקומיים כגון שורה של אפליקציות עסקיות, מניות קבצים ומדפסות ממכשיר של תכלת Active Directory המצורף ל-Windows 10.
ms.openlocfilehash: fc02fd30f41f25f52e653e750a6bdfd1bd7f800e
ms.sourcegitcommit: a62ac3c01ba700a51b78a647e2301f27ac437c5a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/12/2021
ms.locfileid: "50233839"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>גישה למשאבים מקומיים באמצעות מכשיר תכלת מצורף ב-Microsoft 365 Business Premium

מאמר זה חל על Microsoft 365 Business Premium.

כל מכשיר Windows 10 שהוא תכלת Active Directory הצטרף אליו כולל גישה לכל המשאבים המבוססים על ענן, כגון יישומי Microsoft 365, וניתן להתגונן על-ידי Microsoft 365 Business Premium. באפשרותך גם לאפשר גישה למשאבים מקומיים כגון יישומי line-business (LOB), מניות קבצים ומדפסות. כדי לאפשר גישה, השתמש ב- [תכלת AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) כדי לסנכרן את active directory המקומי עם תכלת active directory. 

לקבלת מידע נוסף, ראה [מבוא לניהול מכשירים ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
השלבים מסוכמים גם בסעיפים הבאים.
 
## <a name="run-azure-ad-connect"></a>הרצת התחברות של תכלת לספירה

בצע את השלבים הבאים כדי להפוך את המכשירים המצורפים של הארגון שלך ל-תכלת לזמינים כדי לגשת למשאבים מקומיים.
  
1. כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מ-Active Directory המקומי ל-תכלת Active Directory, הפעל את אשף סינכרון מדריכי הכתובות והקישור תכלת AD כמתואר [בהגדרת סינכרון מדריכי כתובות עבור Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization).
    
2. לאחר השלמת סינכרון מדריכי הכתובות, ודא שמכשירי Windows 10 של הארגון שלך מצורפים ל-תכלת לספירה. שלב זה מתבצע בנפרד בכל מכשיר Windows 10. ראה [הגדרת מכשירי Windows עבור משתמשי Microsoft 365 Business Premium](set-up-windows-devices.md) לקבלת פרטים. 
    
3. לאחר הצטרפות המכשירים של Windows 10, כל משתמש צריך להפעיל מחדש את המכשירים ולהיכנס באמצעות האישורים שלהם ב-Microsoft 365 Business Premium. לכל המכשירים יש כעת גישה גם למשאבים מקומיים.
    
אין צורך לבצע שלבים נוספים כדי לקבל גישה למשאבים מקומיים עבור מכשירים המצורפים של תכלת לספירה. פונקציונליות זו מוכללת ב-Windows 10. 

אם יש לך תוכניות להיכנס למכשיר AADJ מלבד שיטת סיסמה כגון PIN/Bio-מדד באמצעות כניסת האישורים של WHFB ולאחר מכן גישה למשאבים מקומיים (מיקומים משותפים, מדפסות. וכדומה), פעל בהתאם https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
אם הארגון שלך אינו מוכן לפריסה בתצורת ההתקן של תכלת לספירה שתוארה לעיל, שקול להגדיר את הגדרת [התצורה ההיברידית של תכלת לספירה הצטרפת למכשיר](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>שיקולים בעת הצטרפות למכשירי Windows לתכלת לספירה

אם התקן Windows שאתה מחובר אליו באמצעות הודעות מיידיות, הצטרף בעבר לתחום או לקבוצת עבודה, שקול את המגבלות הבאות:
  
- כאשר התקן תכלת מצטרף להודעה, הוא יוצר משתמש חדש ללא הפניה לפרופיל קיים. יש להעביר את הפרופילים באופן ידני. פרופיל משתמש מכיל מידע כגון מועדפים, קבצים מקומיים, הגדרות דפדפן והגדרות תפריט התחלה. הגישה הטובה ביותר היא למצוא כלי של ספק חיצוני כדי למפות קבצים והגדרות קיימים לפרופיל החדש.

- אם ההתקן משתמש באובייקטי מדיניות קבוצתית (GPO), ייתכן שאובייקטי Gpo מסוימים לא יהיו בעלי [ספק שירותי תצורה](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) מקביל (CSP) בתוך המנגינה. הפעילו את [הכלי MMAT](https://www.microsoft.com/download/details.aspx?id=45520) כדי למצוא את מחשב ה-csp הדומה לאובייקטי gpo קיימים.

- ייתכן שמשתמשים לא יוכלו לבצע אימות ליישומים התלויים באימות של Active Directory. הערך את האפליקציה legacy ושקול לעדכן את היישום המשתמש באימות מודרני, אם ניתן.

- גילוי מדפסת של Active Directory לא יפעל. באפשרותך לספק נתיבי מדפסת ישירים עבור כל המשתמשים או להשתמש [בהדפס אוניברסלי](https://aka.ms/UPDocs).
