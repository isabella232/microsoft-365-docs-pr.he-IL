---
title: גישה למשאבים מקומיים ממכשיר תכלת המצורף לאתר ב-Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: למד כיצד לקבל גישה למשאבים מקומיים כגון יישומים עסקיים, שיתופי קבצים ומדפסות מתוך מכשיר המצורף ל-Windows 10.
ms.openlocfilehash: 26ba0ffb64ddce32369002120657456e47ac0c7f
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287354"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>גישה למשאבים מקומיים ממכשיר תכלת המצורף לאתר ב-Microsoft 365 Business

כל מכשיר של Windows 10 שהוא הצטרף למשרד התכלת הפעילה יקבל גישה לכל המשאבים המבוססים על ענן צמתים כגון יישומי Office 365 וניתן להגן עליהם על-ידי Microsoft 365 Business. כדי לאפשר גם גישה למשאבים מקומיים כגון יישומים של שורה של עסקים (בלוב), מיקומים משותפים של קבצים ומדפסות, עליך לסנכרן את ה-Active Directory המקומי שלך עם מדריך הפעלה תכלת באמצעות [התחברות לספירה](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). 

ראה [מבוא לניהול התקנים ב-תכלת Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) כדי ללמוד עוד.
השלבים מסוכמים גם בסעיפים הבאים.

## <a name="run-azure-ad-connect"></a>הפעל תכלת והתחבר

השלם את השלבים הבאים כדי לאפשר להתקנים המצורפים של הארגון לבצע גישה למשאבים מקומיים.
  
1. כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מתוך Active Directory המקומי לתוך הספריה הפעילה של המשרד, הפעל את אשף סינכרון הספריות ואת ' כחול לספירה ' כמתואר [בהגדרת סינכרון ספריות עבור Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. לאחר השלמת סינכרון הספריות, ודא שהתקני Windows 10 של הארגון שלך הם המצורפים לתכלת. שלב זה נעשה בנפרד בכל התקן של Windows 10. ראה [הגדרת התקני Windows עבור משתמשים עסקיים של Microsoft 365](set-up-windows-devices.md) לפרטים. 
    
3. לאחר התקני Windows 10 הם תכלת לספירה הצטרפו, כל משתמש צריך לאתחל את המכשירים שלהם להתחבר עם האישורים העסקיים שלהם Microsoft 365. לכל ההתקנים תהיה כעת גישה גם למשאבים מקומיים.
    
אין צורך בצעדים נוספים כדי לקבל גישה למשאבים מקומיים עבור התקנים המצורפים ל-תכלת AD. זוהי פונקציונליות מוכללת הזמינה ב-Windows 10. 
  
אם הארגון שלך אינו מוכן לפרוס בתצורת ההתקן המצורף למטה לספירה המתוארת לעיל, שקול להגדיר את [תצורת ההתקן היברידית של התכלת ההיברידית](manage-windows-devices.md).
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>שיקולים בעת הצטרפות להתקני Windows לתכלת

אם אתה מצטרף להתקן של מערכת Windows שכבר הצטרף לתחום או בקבוצת עבודה, עליך לשקול את המגבלות הבאות:
  
- כאשר התקן "תכלת לספירה" מצטרף, הוא יוצר משתמש חדש מבלי ליצור הפניה לפרופיל קיים. כדי לתקן זאת, יש להעביר את הפרופילים באופן ידני. פרופיל משתמש מכיל מידע כגון מועדפים, קבצים מקומיים, הגדרות דפדפן, הגדרות תפריט התחלה וכו '. הגישה הטובה ביותר היא למצוא כלי של ספק חיצוני כדי למפות קבצים והגדרות קיימים לפרופיל החדש

- אם ההתקן משתמש באובייקטי מדיניות קבוצתית (GPO), ייתכן שלאובייקטי Gpo מסוימים אין [ספק שירותי תצורה](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) דומה (CSP) ב-Intune. הפעל את [הכלי Mmat](https://www.microsoft.com/download/details.aspx?id=45520) כדי לחפש מדיניות קבוצתית דומה עבור אובייקטי gpo קיימים.

- למשתמשים לא תהיה אפשרות לבצע אימות ליישומים התלויים באימות של Active Directory. כדי להתמודד עם זה להעריך באמצעות יישום מדור קודם ולשקול עדכון לאפליקציה המשתמשת באימות מודרני אם אפשרי.

- גילוי מדפסות של active Directory לא יפעל. כדי לתקן זאת, ספק נתיבי מדפסת ישירים עבור כל המשתמשים או לחץ על [הדפסת ענן היברידית](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
