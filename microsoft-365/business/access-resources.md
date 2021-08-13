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
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: למד כיצד לקבל גישה למשאבים מקומיים, כמו שורה של אפליקציות עסקיות, שיתופי קבצים ומדפסות ממכשיר Azure Active Directory המצורף Windows 10 שלך.
ms.openlocfilehash: 49d7150adb8bcb0dd611e7dce10ee92d3de1755dbe8662e454c9afcca2055e69
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809469"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Access משאבים מקומיים ממכשיר מצורף ל- Azure AD ב- Microsoft 365 Business Premium

מאמר זה חל על Microsoft 365 Business Premium.

לכל Windows 10 המצורף ל- Azure Active Directory יש גישה לכל המשאבים המבוססים על ענן, כגון יישומי Microsoft 365 שלך, ומוגנות על-ידי Microsoft 365 Business Premium. באפשרותך גם לאפשר גישה למשאבים מקומיים, כמו יישומי קו עסקים (LOB), שיתופי קבצים ומדפסות. כדי לאפשר גישה, השתמש [ב- Azure AD התחברות כדי](/azure/active-directory/connect/active-directory-aadconnect) לסנכרן את Active Directory המקומי שלך עם Azure Active Directory.

כדי ללמוד עוד, ראה [מבוא לניהול מכשירים ב- Azure Active Directory](/azure/active-directory/device-management-introduction).
השלבים מסוכמים גם בסעיפים הבאים.

## <a name="run-azure-ad-connect"></a>הפעל את Azure AD התחברות

בצע את השלבים הבאים כדי לאפשר למכשירים המצורפים ל- Azure AD של הארגון שלך לגשת למשאבים מקומיים.

1. כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מ- Active Directory המקומי לתוך Azure Active Directory, הפעל את אשף סינכרון מדריכי הכתובות ואת Azure AD התחברות כמתואר במאמר הגדרת [סינכרון מדריכי כתובות עבור Office 365.](../enterprise/set-up-directory-synchronization.md)

2. לאחר השלמת סינכרון מדריכי הכתובות, ודא שהמכשירים Windows 10 של Azure AD מצורפים. שלב זה נעשה בנפרד בכל Windows 10 שלך. ראה [הגדרת Windows עבור משתמשים Microsoft 365 Business Premium לקבלת](set-up-windows-devices.md) פרטים.

3. לאחר שהמכשירים Windows 10 Azure AD מצורפים, כל משתמש חייב לאתחל את המכשירים שלו ולהירשם באמצעות אישורי Microsoft 365 Business Premium שלהם. לכל המכשירים יש כעת גישה למשאבים מקומיים גם כן.

אין צורך בשלבים נוספים כדי לקבל גישה למשאבים מקומיים עבור מכשירים מצורפים של Azure AD. פונקציונליות זו מוכללת Windows 10.

אם יש לך תוכניות להתחבר למכשיר AADJ, מלבד שיטת הסיסמה כמו PIN/Bio-metric באמצעות כניסת אישור WHFB ולאחר מכן לגשת למשאבים מקומיים (שיתופים, מדפסות וכדומה), בצע [מאמר זה.](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

אם הארגון שלך אינו מוכן לפרוס בתצורת המכשיר המצורף של Azure AD המתוארת לעיל, שקול להגדיר תצורת [התקן היברידי של Azure AD Joined](manage-windows-devices.md).

### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>שיקולים בעת הצטרפות Windows ל- Azure AD

אם המכשיר Windows שמצורף ל- Azure-AD היה בעבר לתחום או בקבוצת עבודה, שקול את המגבלות הבאות:

- כאשר התקן Azure AD מצטרף, הוא יוצר משתמש חדש מבלי להפנות לפרופיל קיים. יש להעביר פרופילים באופן ידני. פרופיל משתמש מכיל מידע כמו מועדפים, קבצים מקומיים, הגדרות דפדפן תפריט התחלה שונות. הגישה הטובה ביותר היא למצוא כלי של ספקים אחרים כדי למפות קבצים והגדרות קיימים לפרופיל החדש.

- אם המכשיר משתמש באובייקטי מדיניות קבוצתית (GPO), ייתכן של- [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) GPO מסוימים אין ספק שירותי תצורה (CSP) דומה ב- Intune. הפעל את [הכלי MMAT כדי](https://www.microsoft.com/download/details.aspx?id=45520) למצוא CSPs ניתנים להשוואה עבור אובייקטי GPO קיימים.

- ייתכן שמשתמשים לא יוכלו לבצע אימות עבור יישומים התלויים באימות של Active Directory. הערכת היישום מדור קודם ושקול לעדכן ליישום המשתמש באות מודרנית, אם הדבר אפשרי.

- גילוי מדפסת של Active Directory לא יתפקד. באפשרותך לספק נתיבי מדפסת ישירים עבור כל המשתמשים או להשתמש [בהדפסה אוניברסלית.](/universal-print/)

### <a name="related-articles"></a>מאמרים קשורים

[דרישות מוקדמות עבור Azure AD התחברות](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
