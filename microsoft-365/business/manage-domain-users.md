---
title: סנכרן משתמשי תחום ל-Microsoft 365
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Adm_O365
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
description: סנכרן משתמשים מבוקרים בתחום עם Microsoft 365 לעסקים.
ms.openlocfilehash: af9cb7c9b2b639edc2375679a73ab41c4cf6de71
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081847"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>סנכרן משתמשי תחום ל-Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. היכונו לסנכרון ספריות 

לפני שתסנכרן את המשתמשים והמחשבים שלך מקבוצת המחשבים המקומית של Active Directory, סקור את [ההכנה לסנכרון ספריות ל-Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). בפרט:

   - ודא שאין כפילויות בספריה שלך עבור התכונות הבאות: **דואר**, **כתובות Proxyaddresses שמות** **משתמשים**. על ערכים אלה להיות ייחודיים ויש להסיר את כל הכפילויות.
   
   - מומלץ לקבוע את התצורה של התכונה **Userהפריפרישם** (UPN) עבור כל חשבון משתמש מקומי שיתאים לכתובת הדואר האלקטרוני הראשית המתאימה למשתמש Microsoft 365 המורשה. לדוגמה: *mary.shelley@contoso.com* ולא *mary@contoso. מקומיים*
   
   - אם קבוצת המחשבים של Active Directory מסתיימת בסיומת שאינה ניתנת לניתוב כגון. *local* או *. lan*, במקום סיומת אינטרנט הניתנת לניתוב כגון *. com* או *. org*, התאם תחילה את סיומת ה-UPN של חשבונות המשתמשים המקומיים כמתואר [בהכנת תחום שאינו ניתן לניתוב עבור סינכרון ספריות](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

**הפעל IdFix** בשלב ארבע (4) להלן, גם יוודא שהמחשב המקומי שלך active Directory מוכן לסינכרון dir.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. התקנה והגדרה של התחברות תכלת

כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מ-Active Directory המקומי לתוך מדריך כחול פעיל, התקן את האפשרות התחבר לספריית המשימות הפעילה והגדר סינכרון ספריות. 

 1. במרכז הניהול של <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> בחירת **ההתקנה** בניווט השמאלי.

 2. תחת **כניסה ואבטחה**, בחר באפשרות **תצוגה** תחת **משתמשי סינכרון מהספריה של הארגון**.

 3. בתיקיה **משתמשי סינכרון מתוך הספריה של הארגון** , בחר באפשרות ' **התחל**'.

 4. בשלב הראשון הכלי IdFix כדי להתכונן לסנכרון ספריות.

 5. בצע את צעדי האשף כדי להוריד את החיבור התכלת ולהשתמש בו כדי לסנכרן את המשתמשים שבשליטת התחום שלך ל-Microsoft 365.


ראה [הגדרת סינכרון ספריות עבור Microsoft 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) כדי ללמוד עוד.

כאשר אתה מגדיר את האפשרויות שלך עבור תכלת AD התחבר, אנו ממליצים לאפשר **סנכרון סיסמה**, **כניסה יחידה בודדת**, ואת **הסיסמה כתבה בחזרה** , אשר נתמך גם ב-Microsoft 365 לעסקים.

> [!NOTE]
> יש כמה שלבים נוספים עבור הסיסמה כתיבה מעבר לתיבת הסימון התחבר תכלת AD. לקבלת מידע נוסף, ראה [כיצד-to: הגדרת התצורה של הסיסמה ככתוב](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

אם ברצונך לנהל גם התקנים המצורפים לתחום של Windows 10, ראה [הפעלת התקנים של windows 10 המצורפים לתחום כדי שתנוהל על-ידי Microsoft 365 Business Premium](manage-windows-devices.md) כדי להגדיר את הצירוף היברידי לתכלת. 