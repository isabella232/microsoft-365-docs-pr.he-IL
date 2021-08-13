---
title: נהל את האופן שבו המשתמשים ניגשים למסמכי Office במכשירים ניידים
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4OfficeMobile
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: למד אודות מדיניות הגנה המאפשרת לך לנהל את האופן בו משתמשים ניגשים לאפליקציות Office וקבצי עבודה ממכשירים ניידים.
ms.openlocfilehash: 6e48ef857de8046854a94d470b28ba5db96b373bc8b190dc1062d4f408a9802c
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809251"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a>נהל את האופן שבו המשתמשים ניגשים למסמכי Office במכשירים ניידים

מאמר זה חל על Microsoft 365 Business Premium.

הגדרות מדיניות שקובעות כיצד משתמשים ניגשים לקבצי Office מתוך המכשירים הניידים שלהם מוגדרות למצב **כבוי** כברירת מחדל. מומלץ לקבל את ערכי ברירת המחדל במהלך ההגדרה כדי ליצור מדיניות יישומים עבור Android , iOS ו- Windows 10 החלים על כל המשתמשים. ניתן ליצור פריטי מדיניות נוספים לאחר השלמת ההתקנה. 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>הגדרות שקובעות כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים

ההגדרות הבאות זמינות לניהול אופן הגישה של משתמשים לקבצי עבודה של Office:

|הגדרה  <br/> |תיאור  <br/> |
|:-----|:-----|
|דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office  <br/> |אם הגדרה זו היא **On**, המשתמשים חייבים לספק צורה אחרת של אימות, בנוסף לשם המשתמש והסיסמה שלהם, כדי שהם יוכלו להשתמש באפליקציות Office במכשיר הנייד שלהם.  <br/> |
|אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה  <br/> |כדי למנוע ממשתמש לא מורשה לנחש באופן אקראי קוד PIN, הקוד יאופס לאחר מספר כניסות שגויות שאתה תציין.  <br/> |
|דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך  <br/> |הגדרה זו קובעת כמה זמן המשתמש יכול להיות לא פעיל לפני שהוא מתבקש להיכנס שוב.  <br/> |
|מנע גישה לקבצי עבודה במכשירים שנפרצו או שבוצעה בהם פעולת ROOT  <br/> |ייתכן מצב שבו משתמשים מתוחכמים יחזיקו במכשיר שנפרץ או שבוצעה בו פעולת ROOT. משמעות הדבר היא שהמשתמש יכול לשנות את מערכת ההפעלה, אשר יכולה להפוך את המכשיר ל רגיש יותר לתוכנות זדוניות. מכשירים אלה נחסמים כאשר ההגדרה מוגדרת למצב **פעיל**.  <br/> |
|אל תאפשר למשתמשים להעתיק תוכן מאפליקציות Office לאפליקציות אישיות  <br/> |כאשר ההגדרה **היא פועל,** למשתמש אין אפשרות להעתיק מידע בקובץ עבודה לקובץ אישי. אם ההגדרה **כבויה,** המשתמש יכול להעתיק מידע מקובץ עבודה לאפליקציה אישית או לחשבון אישי.  <br/> |
   

