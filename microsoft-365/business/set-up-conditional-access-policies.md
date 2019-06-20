---
title: להגדיר פריטי מדיניות של גישה מותנית עבור קמפיינים Microsoft 365
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
search.appverid:
- BCS160
- MET150
- MOE150
description: למד כיצד להגדיר פריטי מדיניות של גישה מותנית עבור קמפיינים 365 של Microsoft.
ms.openlocfilehash: 7d8e1f16019d151478aae57b1593b0e0758e5b19
ms.sourcegitcommit: 7e46db0b35c188ee6a7b40ab3eb2d76ff6c101c5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/19/2019
ms.locfileid: "35086335"
---
# <a name="set-up-conditional-access-policies"></a>להגדיר פריטי מדיניות של גישה מותנית

פריטי מדיניות של [גישה מותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) להוסיף אבטחה נוספת substancial. Microsoft מספקת קבוצה של פריטי מדיניות של גישה מותנית בסיסית המומלצים עבור כל הלקוחות. מדיניות בסיסית היא ערכה של מדיניות מוגדרת מראש המסייעות בהגנה על ארגונים מפני התקפות נפוצות רבות. התקפות נפוצים אלה יכולים לכלול התזה סיסמה, replay ודיוג.

פריטי מדיניות אלה דורשים מנהלים ומשתמשים להזנת טופס שני של אימות (נקרא אימות רב-גורמי או MFA) כאשר תנאים מסוימים מתקיימים. לדוגמה, אם משתמש הכניסה ממדינה אחרת, הכניסה עשויות להיחשב מסוכן ולחץ על המשתמש לספק טופס נוסף של אימות. 

כעת, מדיניות בסיסית כוללות:
- **דרוש MFA עבור מנהלים** — דורש אימות מגורמים רבים עבור תפקידי מנהל מורשה ביותר, כולל מנהל כללי.
- **הגנה על משתמש הקצה** — מחייב אימות מגורמים רבים עבור משתמשים רק בעת-הכניסה היא מסוכנת. 
- **אימות דור קודם של בלוק** -יישומים ישנים יותר של הלקוח ואת מספר יישומים חדשים אל תשתמש פרוטוקולי אימות חדשה יותר, בטוחה יותר. יישומים ישנים אלה יכולים לעקוף פריטי מדיניות של גישה מותנית ולהשיג גישה לא מורשית לסביבה שלך. זו מדיניות חוסם את הגישה מלקוחות שאינם תומכים גישה מותנית. 
- **דרוש MFA עבור ניהול שירות** -דורש אימות מגורמים רבים עבור גישה לכלי ניהול, כולל פורטל תכלת הרקיע (בהם לקבוע תצורה של פריטי מדיניות בסיסית). 

Microsoft ממליצה שתפעיל את כל פריטי מדיניות אלה בסיסית. לאחר פריטי מדיניות אלה מופעלות, מנהלים ומשתמשים תתבקש לרשום עבור אימות תכלת הרקיע Multii-פקטור.

לקבלת מידע נוסף אודות מדיניות אלה, ראה [מהן מדיניות בסיסית](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>הגדרת מדיניות בסיסית

1. מעבר לפורטל [תכלת הרקיע](https://portal.azure.com)ולאחר מכן נווט אל **הספריה הפעילה תכלת הרקיע** \> **Access מותנה**.
    
    מדיניות בסיסית מפורטים בדף. <br/> <br/>
    ![דף המפרט את מדיניות בסיסית עבור גישה מותנית.](media/baslinepolicies.png)
1. עיין בהוראות הספציפיות הבאות עבור כל מדיניות:

  - [דרוש MFA עבור מנהלים](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [MFA Reequire עבור משתמשים](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [אימות דור קודם של בלוק](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [דרוש MFA עבור ניהול שירות](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

באפשרותך להגדיר מדיניות נוספים רבים, כגון דרישת לקוח מאושרת apps. עיין [בתיעוד Access מותנה](https://docs.microsoft.com/azure/active-directory/conditional-access/) לקבלת מידע נוסף.