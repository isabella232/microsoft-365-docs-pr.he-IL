---
title: אבטחת מכשירים של Windows 10
f1.keywords:
- CSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4WindowsConfig
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: למד אודות קביעת התצורה של ההגדרות של מדיניות ההתקן המוגדרת כברירת מחדל שכל מכשיר Windows 10 יקבל בעת כניסה לחשבון בעבודה או בבית הספר.
ms.openlocfilehash: b586e687d6b61873b77fac8586396ab51fd90b9b
ms.sourcegitcommit: 90efec455336b4cecc06a8cbf0ce287740433523
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/26/2020
ms.locfileid: "46898067"
---
# <a name="secure-windows-10-devices"></a>אבטחת מכשירים של Windows 10

מאמר זה חל על Microsoft 365 Business Premium.

ההגדרות שאתה קובע כאן הן חלק ממדיניות ברירת המחדל של המכשיר עבור Windows 10. כל המשתמשים שמחברים מכשיר Windows 10, כולל מכשירים ניידים ומחשבים, על-ידי כניסה באמצעות חשבון העבודה שלהם, יקבלו באופן אוטומטי הגדרות אלה. אנו ממליצים לקבל את מדיניות ברירת המחדל במהלך ההתקנה ולהוסיף פריטי מדיניות המתמקדים בקבוצות משתמשים ספציפיות במועד מאוחר יותר.
  
## <a name="settings-to-secure-windows-10-devices"></a>הגדרות לאבטחת מכשירים של Windows 10

כברירת מחדל כל ההגדרות מוגדרות ל **פעיל**. ההגדרות הבאות זמינות:
  
|||
|:-----|:-----|
|הגדרה  <br/> |תיאור  <br/> |
|עזור בהגנה על מחשבים מפני וירוסים ואיומים אחרים באמצעות האנטי-וירוס של Windows Defender  <br/> |דרושה הפעלה של האנטי-וירוס של Windows Defender כדי להגן על מחשבים מהסכנות הכרוכות בחיבור לאינטרנט.  <br/> |
|עזור בהגנה על מחשבים מפני איומים מבוססי-אינטרנט ב- Microsoft Edge  <br/> |הפעלת הגדרות ב- Microsoft Edge שעוזרות בהגנה על המשתמשים מפני אתרים זדוניים והורדות.  <br/> |
|כבה את מסך המכשיר כאשר הוא לא פעיל למשך פרק זמן זה  <br/> |הגדרה זו מוודאת שנתוני החברה מוגנים אם המשתמש אינו פעיל. ייתכן מצב שבו משתמש מסוים עובד במקום ציבורי, למשל בית קפה, שבו הוא מתרחק או שדעתו מוסחת לרגע קט ומשאיר את המכשיר שלו חשוף להצצות אקראיות. הגדרה זו מאפשרת לך לקבוע כמה זמן המשתמש יכול להיות לא פעיל לפני כיבוי המסך.  <br/> |
|אפשר למשתמשים להוריד אפליקציות מ- Microsoft Store  <br/> |הגדרה זו מאפשרת למשתמשים להוריד ולהתקין אפליקציות מ- Microsoft Store. אפליקציות כוללות את כל סוגי התוכן, החל ממשחקים וכלה בכלי פרודוקטיביות, לכן אנו משאירים הגדרה זו במצב **מופעל**, אך ניתן לבטל אותה להשגת אבטחה נוספת.  <br/> |
|