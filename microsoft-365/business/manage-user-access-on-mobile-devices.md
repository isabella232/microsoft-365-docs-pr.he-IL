---
title: נהל את האופן שבו המשתמשים ניגשים למסמכי Office במכשירים ניידים
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
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
description: למד אודות מדיניות הגנה המאפשרת לך לנהל את אופן הגישה של משתמשים ליישומי Office ולקבצי עבודה ממכשירים ניידים.
ms.openlocfilehash: b2b828cf2e201360f12b8fadcb395e72958230f6
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471066"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a>נהל את האופן שבו המשתמשים ניגשים למסמכי Office במכשירים ניידים

מאמר זה חל על 365 עסקים Premium של Microsoft.

הגדרות מדיניות שקובעות כיצד משתמשים ניגשים לקבצי Office מתוך המכשירים הניידים שלהם מוגדרות למצב **כבוי** כברירת מחדל. מומלץ לקבל את ערכי ברירת המחדל במהלך ההתקנה כדי ליצור מדיניות יישומים עבור אנדרואיד, iOS ו-Windows 10 החלים על כל המשתמשים. ניתן ליצור פריטי מדיניות נוספים לאחר השלמת ההתקנה. 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>הגדרות שקובעות כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים

ההגדרות הבאות זמינות לניהול אופן הגישה של משתמשים לקבצי עבודה של Office:
  
|||
|:-----|:-----|
|הגדרה  <br/> |תיאור  <br/> |
|דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office  <br/> |אם הגדרה זו **מופעלת, על**המשתמשים לספק צורה אחרת של אימות, בנוסף לשם המשתמש והסיסמה שלהם, לפני שהם יוכלו להשתמש ביישומי Office במכשיר הנייד שלהם.  <br/> |
|אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה  <br/> |כדי למנוע ממשתמש לא מורשה לנחש באופן אקראי קוד PIN, הקוד יאופס לאחר מספר כניסות שגויות שאתה תציין.  <br/> |
|דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך  <br/> |הגדרה זו קובעת כמה זמן יכול המשתמש להיות לא פעיל לפני שתתבקש להיכנס שוב.  <br/> |
|מנע גישה לקבצי עבודה במכשירים שנפרצו או שבוצעה בהם פעולת ROOT  <br/> |ייתכן מצב שבו משתמשים מתוחכמים יחזיקו במכשיר שנפרץ או שבוצעה בו פעולת ROOT. משמעות הדבר היא כי המשתמש יכול לשנות את מערכת ההפעלה, אשר יכול להפוך את המכשיר פגיע יותר לתוכנות זדוניות. מכשירים אלה נחסמים כאשר ההגדרה מוגדרת למצב **פעיל**.  <br/> |
|אל תאפשר למשתמשים להעתיק תוכן מיישומי Office ליישומים אישיים  <br/> |כאשר ההגדרה **מופעלת**, המשתמש אינו יכול להעתיק מידע בקובץ עבודה לקובץ אישי. אם ההגדרה **כבויה**, המשתמש יכול להעתיק מידע מקובץ עבודה לאפליקציה אישית או לחשבון אישי.  <br/> |
   

