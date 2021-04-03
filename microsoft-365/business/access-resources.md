---
title: Access משאבים מקומיים ממכשיר מצורף ל- Azure AD ב- Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: למד כיצד לקבל גישה למשאבים מקומיים, כמו שורה של אפליקציות עסקיות, שיתופי קבצים ומדפסות ממכשיר Azure Active Directory המצורף למכשיר Windows 10.
ms.openlocfilehash: 27549d6c3b03413f2f05c69845caad155333ca97
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580313"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Access משאבים מקומיים ממכשיר מצורף ל- Azure AD ב- Microsoft 365 Business Premium

מאמר זה חל על Microsoft 365 Business Premium.

לכל מכשיר Windows 10 המצורף ל- Azure Active Directory יש גישה לכל המשאבים המבוססים על ענן, כגון יישומי Microsoft 365 שלך, ו- Microsoft 365 Business Premium יכול להגן עליו. באפשרותך גם לאפשר גישה למשאבים מקומיים, כמו יישומי קו עסקים (LOB), שיתופי קבצים ומדפסות. כדי לאפשר גישה, השתמש [ב- Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) כדי לסנכרן את Active Directory המקומי שלך עם Azure Active Directory. 

כדי ללמוד עוד, ראה [מבוא לניהול מכשירים ב- Azure Active Directory](/azure/active-directory/device-management-introduction).
השלבים מסוכמים גם בסעיפים הבאים.
 
## <a name="run-azure-ad-connect"></a>הפעל את Azure AD Connect

בצע את השלבים הבאים כדי לאפשר למכשירים המצורפים ל- Azure AD של הארגון שלך לגשת למשאבים מקומיים.
  
1. כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מ- Active Directory המקומי לתוך Azure Active Directory, הפעל את אשף סינכרון מדריכי הכתובות ואת Azure AD Connect כמתואר בהגדיר סינכרון [מדריכי כתובות עבור Office 365.](../enterprise/set-up-directory-synchronization.md)
    
2. לאחר השלמת סינכרון מדריכי הכתובות, ודא שהתקני Windows 10 של הארגון שלך מצורפים ל- Azure AD. שלב זה נעשה בנפרד בכל מכשיר Windows 10. לקבלת [פרטים, ראה הגדרת מכשירי Windows עבור משתמשי Microsoft 365 Business Premium.](set-up-windows-devices.md) 
    
3. לאחר שמכשירי Windows 10 מצורפים ל- Azure AD, כל משתמש חייב לאתחל את המכשירים שלו ולהירשם באמצעות אישורי Microsoft 365 Business Premium שלו. לכל המכשירים יש כעת גישה למשאבים מקומיים גם כן.
    
אין צורך בשלבים נוספים כדי לקבל גישה למשאבים מקומיים עבור מכשירים מצורפים של Azure AD. פונקציונליות זו מוכללת ב- Windows 10. 

אם יש לך תוכניות להתחבר למכשיר AADJ, מלבד שיטת סיסמה כמו PIN/Bio-metric באמצעות כניסת אישור WHFB ולאחר מכן לגשת למשאבים מקומיים (שיתופים, מדפסות.) וכו'), פעל בהתאם https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
אם הארגון שלך אינו מוכן לפרוס בתצורת המכשיר המצורף של Azure AD המתוארת לעיל, שקול להגדיר תצורת [התקן היברידי של Azure AD Joined](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>שיקולים בעת הצטרפות להתקני Windows ל- Azure AD

אם התקן Windows שהצטרף ל- Azure-AD היה בעבר לתחום או בקבוצת עבודה, שקול את המגבלות הבאות:
  
- כאשר התקן Azure AD מצטרף, הוא יוצר משתמש חדש מבלי להפנות לפרופיל קיים. יש להעביר פרופילים באופן ידני. פרופיל משתמש מכיל מידע כמו מועדפים, קבצים מקומיים, הגדרות דפדפן והגדרות תפריט התחלה. הגישה הטובה ביותר היא למצוא כלי של ספקים אחרים כדי למפות קבצים והגדרות קיימים לפרופיל החדש.

- אם המכשיר משתמש באובייקטי מדיניות קבוצתית (GPO), ייתכן של- [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) GPO מסוימים אין ספק שירותי תצורה (CSP) דומה ב- Intune. הפעל את [הכלי MMAT כדי](https://www.microsoft.com/download/details.aspx?id=45520) למצוא CSPs ניתנים להשוואה עבור אובייקטי GPO קיימים.

- ייתכן שמשתמשים לא יוכלו לבצע אימות עבור יישומים התלויים באימות של Active Directory. הערכת היישום מדור קודם ושקול לעדכן ליישום המשתמש באות מודרנית, אם הדבר אפשרי.

- גילוי מדפסת של Active Directory לא יתפקד. באפשרותך לספק נתיבי מדפסת ישירים עבור כל המשתמשים או להשתמש [בהדפסה אוניברסלית.](/universal-print/)

### <a name="related-articles"></a>מאמרים קשורים

[דרישות מוקדמות עבור Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
