---
title: הגדרת מדיניות גישה מותנית עבור קמפיינים של Microsoft 365
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: למד כיצד להגדיר מדיניות גישה מותנית עבור קמפיינים של Microsoft 365 כדי להוסיף אבטחה משמעותית.
ms.openlocfilehash: d7c9cfee2ef00e4ebe231a28ccca185c10f53c6b
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403017"
---
# <a name="set-up-conditional-access-policies"></a>הגדרת מדיניות גישה מותנית

פריטי מדיניות [גישה מותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) מוסיפים אבטחה משמעותית. Microsoft מספקת מערכת של פריטי מדיניות גישה מותנית בסיסית המומלצת עבור כל הלקוחות. מדיניות בסיסית היא קבוצה של פריטי מדיניות מוגדרים מראש המסייעים להגן על ארגונים מפני התקפות נפוצות רבות. התקפות נפוצות אלה יכולות לכלול תרסיס סיסמה, הפעלה חוזרת ודיוג.

מדיניות זו דורשת ממנהלים ומשתמשים להזין סוג שני של אימות (הנקרא אימות מרובה גורמים או משרד המשנה) כאשר מתקיימים תנאים מסוימים. לדוגמה, אם משתמש נכנס ממדינה אחרת, ייתכן שהכניסה תיחשב כמסוכנת והמשתמש חייב לספק סוג נוסף של אימות. 

כעת, מדיניות בסיסית כוללת את הפעולות הבאות:
- **דרוש את משרד התואר למנהלים** &ndash; מחייב אימות רב-גורמי עבור תפקידי מנהל המערכת המיוחסים ביותר, כולל מנהל כללי.
- הגנת משתמש **קצה** &ndash; מחייב אימות רב-גורמי עבור משתמשים רק כאשר כניסה מסוכנת. 
- **חסום אימות** &ndash; מדור קודם יישומי לקוח ישנים ויישומים חדשים מסוימים אינם משתמשים בפרוטוקולי אימות חדשים ומאובטחים יותר. יישומים ישנים אלה יכולים לעקוף מדיניות גישה מותנית ולהשיג גישה בלתי מורשית לסביבה שלך. מדיניות זו חוסמת את הגישה מלקוחות שאינם תומכים בגישה מותנית. 
- **דרוש משרד לניהול** &ndash; שירות מחייב אימות רב-גורמי לקבלת גישה לכלי ניהול, כולל פורטל תכלת (שם תקבע את תצורת מדיניות בסיסית). 

Microsoft ממליצה להפוך את כל פריטי המדיניות הבסיסיים לזמינים. לאחר שפריטי מדיניות אלה מופעלים, מנהלים ומשתמשים יתבקשו להירשם לאימות מרובה הגורמים התכלת.

לקבלת מידע נוסף אודות פריטי מדיניות אלה, ראה [מהן מדיניות בסיסית](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>הגדרת מדיניות בסיסית

1. עבור [לפורטל התכלת](https://portal.azure.com)ונווט אל **Azure Active Directory** \> **הגישה המותנית**של active Directory.
    
    פריטי המדיניות הבסיסיים מפורטים בדף. <br/> <br/>
    ![דף המפרט מדיניות בסיסית עבור גישה מותנית.](../media/baslinepolicies.png)
1. עיין בהנחיות הספציפיות הבאות עבור כל מדיניות:

  - [דרוש את משרד התואר למנהלים](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [דרוש משרד למשתמש](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [חסום אימות מדור קודם](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [דרוש תואר שירות למען ניהול השירות](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

באפשרותך להגדיר פריטי מדיניות נוספים רבים, כגון דרישת יישומי לקוח מאושרים. לקבלת מידע נוסף, עיין [בתיעוד של גישה מותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/).
