---
title: מתן אפשרות לניהול מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: למד כיצד לאפשר ל-Microsoft 365 להגן על התקנים המקומיים המצורפים ל-Windows 10.
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992228"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>מתן אפשרות לניהול מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business

אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business כדי להגן על התקני Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים המחייבים אימות מקומי. אתה יכול להגדיר את זה על ידי הראשון סינכרון הספרייה הפעילה שלך עם כחול Active Directory, ואחריו רישום התקנים של Windows 10 עם תכלת AD ולרשום אותם לניהול המכשיר הנייד על ידי Microsoft 365 Business.
הסרטון הבא מפרט את השלבים עבור אופן ההגדרה של התרחיש השכיח ביותר.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>הגדרת התקנים המצורפים לתחום לניהול על-ידי Microsoft 365 Business

כדי להגדיר את ההתקנים המצורפים לתחום של הארגון שלך כדי להפיק תועלת מהיכולות שסופקו על-ידי התכונה ' פעיל בספריה ' בנוסף ל-Active Directory המקומי, באפשרותך ליישם **התקנים מצורפים של ' תכלת היברידית**'. אלה הם התקנים המצורפים הן ל-Active Directory המקומי ולספריה הפעילה שלך. היברידית תכלת AD התקנים המצורפים יכול להיות מוגן ומנוהל על ידי מיקרוסופט 365 עסקים. 
  
להשלים את השלבים הבאים כדי להפוך את Windows 10 התקנים היברידית תכלת AD הצטרף והמנוהל על ידי Microsoft 365 Business.
  
1. כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מתוך Active Directory המקומי לתוך מדריך כחול פעיל, הפעל את אשף סינכרון הספריות והתחבר באמצעות התיקיה ' פעיל בספריה ' כמתואר [בהגדרת סינכרון ספריות עבור Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
    > [!NOTE]
    > השלבים זהים בדיוק עבור Microsoft 365 Business. 
  
2. לפני שתשלים את שלב 3 כדי לאפשר להתקני Windows 10 להיות מצורפים להתקן התכלת ההיברידית, עליך לוודא שאתה עומד בדרישות המוקדמות הבאות:

   - אתה מפעיל את הגירסה העדכנית ביותר של התחברות התכלת AD.

   - החיבור התכלת לספירה מסנכרן את כל אובייקטי המחשב של המכשירים שברצונך להיות היברידית תכלת לספירה הצטרפו. אם אובייקטי המחשב שייכים ליחידות ארגוניות מסוימות (OU), ודא שאלה אלה מוגדרות לסנכרון בתכלת הספירה גם כן.
    
3. רישום התקנים קיימים המצורפים ל-Windows 10 להיות היברידית תכלת AD הצטרפו ולרשום אותם לניהול המכשיר הנייד על ידי Intune (Microsoft 365 Business):
    
4. בצע את ההוראות צעד אחר צעד [כיצד להגדיר היברידי היברידית התקנים של התכלת המצורפים למכשירים](https://go.microsoft.com/fwlink/p/?linkid=872870). פעולה זו תאפשר את הסינכרון של מחשבי Active Directory המקומיים המצורפים ל-Windows 10 ויגרום להם להיות מוכנים לעננים.
    
5. כדי לרשום מכשיר Windows 10 עבור ניהול התקנים ניידים, ראה [רישום התקן של windows 10 באמצעות Intune באמצעות מדיניות קבוצתית](https://go.microsoft.com/fwlink/p/?linkid=872871) לקבלת הוראות. באפשרותך להגדיר את המדיניות הקבוצתית ברמת מחשב מקומית או עבור פעולות בצובר, באפשרותך ליצור הגדרת מדיניות קבוצתית זו בשרת בקר התחום שלך.