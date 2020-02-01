---
title: גישה למשאבים מקומיים ממכשיר תכלת המצורף לאתר ב-Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: למד כיצד לקבל גישה למשאבים מקומיים כגון שורה של יישומים עסקיים, שיתופי קבצים ומדפסות מתוך מכשיר המצורף ל-Windows 10.
ms.openlocfilehash: 653b53d29e84bbdc91273cb78b9b8407c0f6a209
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593232"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>גישה למשאבים מקומיים ממכשיר תכלת המצורף לאתר ב-Microsoft 365 Business

לכל מכשיר של Windows 10 המצורף ל'תכלת הספריות ' יש גישה לכל המשאבים המבוססים על ענן צמתים, כגון יישומי Office 365, וניתן להגן עליהם על-ידי Microsoft 365 Business. כמו כן, באפשרותך לאפשר גישה למשאבים מקומיים כגון יישומים של שורה עסקית, שיתופי קבצים ומדפסות. כדי לאפשר גישה, השתמש [בתכלת והתחבר](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) כדי לסנכרן את הספריה המקומית שלך באמצעות הספריה הפעילה. 

לקבלת מידע נוסף, ראה [מבוא לניהול התקנים בתוך הספריה הפעילה](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
השלבים מסוכמים גם בסעיפים הבאים.

> [!IMPORTANT]
> הליך זה ישים רק ל-OAuth ו-NTLM. אין תמיכה ב-Kerberos.
 
## <a name="run-azure-ad-connect"></a>הפעל תכלת והתחבר

השלם את השלבים הבאים כדי לאפשר להתקנים המצורפים של הארגון לבצע גישה למשאבים מקומיים.
  
1. כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מתוך Active Directory המקומי לתוך מדריך כחול פעיל, הפעל את אשף סינכרון הספריות והשתמש בתכלת AD כמתואר [בהגדרת סינכרון ספריות עבור Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. לאחר השלמת סינכרון הספריות, ודא שהתקני Windows 10 של הארגון שלך מצורפים לתכלת. שלב זה נעשה בנפרד בכל התקן של Windows 10. ראה [הגדרת התקני Windows עבור משתמשים עסקיים של Microsoft 365](set-up-windows-devices.md) לפרטים. 
    
3. לאחר שהתקני Windows 10 הם המצורפים לתכלת, כל משתמש חייב לאתחל את המכשירים שלהם ולהיכנס עם האישורים העסקיים של Microsoft 365 שלהם. לכל ההתקנים יש כעת גישה גם למשאבים מקומיים.
    
אין צורך בצעדים נוספים כדי לקבל גישה למשאבים מקומיים עבור התקנים המצורפים ל-תכלת AD. פונקציונליות זו מוכללת ב-Windows 10. 

אם יש לך תוכניות להתחבר למכשיר AADJ אחר מאשר שיטת סיסמה כמו PIN/Bio-מטרי באמצעות התחברות האישור WHFB ולאחר מכן לגשת למשאבים המקומי (מיקומים משותפים, מדפסות... וכו '), אנא עקוב אחרhttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
אם הארגון שלך אינו מוכן לפרוס בתצורת ההתקן המצורף של התכלת שתוארה לעיל, שקול להגדיר [תצורת התקן היברידית של התכלת ההיברידית](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>שיקולים כאשר אתה מצטרף להתקני Windows לתכלת

אם התקן Windows שאליו הצטרפת התכלת-לספירה הצטרף לתחום בעבר או בקבוצת עבודה, שקול את המגבלות הבאות:
  
- כאשר התקן "תכלת לספירה" מצטרף, הוא יוצר משתמש חדש מבלי ליצור הפניה לפרופיל קיים. יש להעביר באופן ידני פרופילים. פרופיל משתמש מכיל מידע כגון מועדפים, קבצים מקומיים, הגדרות דפדפן והגדרות תפריט התחלה. הגישה הטובה ביותר היא למצוא כלי של ספק חיצוני כדי למפות קבצים והגדרות קיימים לפרופיל החדש.

- אם ההתקן משתמש באובייקטי מדיניות קבוצתית (GPO), ייתכן שלאובייקטי Gpo מסוימים אין [ספק שירותי תצורה](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) דומה (CSP) ב-Intune. הפעל את [הכלי Mmat](https://www.microsoft.com/download/details.aspx?id=45520) כדי לחפש מדיניות קבוצתית דומה עבור אובייקטי gpo קיימים.

- משתמשים לא יוכלו לבצע אימות ליישומים התלויים באימות של Active Directory. הערכת יישום מדור קודם ושקול לעדכן לאפליקציה המשתמשת ב-אימות מודרני, במידת האפשר.

- גילוי מדפסות של active Directory לא יפעל. באפשרותך לספק נתיבי מדפסת ישירים עבור כל המשתמשים או להשתמש [בהדפס ענן היברידי](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
