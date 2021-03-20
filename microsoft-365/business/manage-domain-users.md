---
title: סינכרון משתמשי תחום ל-Microsoft 365
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
description: סנכרן משתמשים הנשלטים על-ידי התחום באמצעות Microsoft 365 for business.
ms.openlocfilehash: 1c939dec7229f02991b15f08c48f184efecaddb0
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913253"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>סינכרון משתמשי תחום ל-Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. הכנה לסינכרון מדריכי כתובות 

לפני שתסנכרן את המשתמשים והמחשבים שלך מהתחום המקומי של Active Directory, סקור את האפשרות [התכונן לסינכרון מדריכי כתובות ב-Microsoft 365](../enterprise/prepare-for-directory-synchronization.md). בפרט:

   - ודא שהאפשרות ללא כפילויות קיימת במדריך הכתובות של התכונות הבאות: **mail**, **ProxyAddresses** ו- **userPrincipalName**. ערכים אלה חייבים להיות ייחודיים ולהסיר כל כפילויות.
   
   - מומלץ לקבוע את תצורת התכונה **userPrincipalName** (UPN) עבור כל חשבון משתמש מקומי כדי להתאים לכתובת הדואר האלקטרוני הראשית התואמת למשתמש Microsoft 365 המורשה. לדוגמה: *mary.shelley@contoso.com* ולא *mary@contoso. local*
   
   - אם התחום של Active Directory מסתיים בסיומת שאינה ניתנת לניתוב *, כגון.* lan או. lan, במקום סיומת לאינטרנט הניתנת לניתוב כגון *. com* או *.* *lan*, התאם את סיומת ה-UPN של חשבונות המשתמשים המקומיים תחילה כמתואר [בהכנת תחום שאינו ניתן לניתוב עבור סינכרון מדריכי כתובות](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md). 

הפעל את **IdFix** בשלב 4 (4) להלן, וודא ש-Active directory המקומי שלך מוכן לסינכרון מדריכי כתובות.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. התקנה וקביעת תצורה של התחברות למודעת תכלת

כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מ-Active Directory המקומי לתכלת Active Directory, התקן את תכלת Active Directory התחבר והגדר סינכרון מדריכי כתובות. 

 1. במרכז [הניהול](https://go.microsoft.com/fwlink/p/?linkid=2024339), בחר **הגדרה** בניווט הימני.

 2. תחת **כניסה ואבטחה**, בחר **הצג**  תחת **סנכרן משתמשים ממדריך הארגון שלך**.

 3. בדף **סינכרון משתמשים מתוך מדריך הכתובות של הארגון שלך** , בחר **תחילת** העבודה.

 4. בכלי השלב הראשון של ההפעלה IdFix כדי להתכונן לסינכרון מדריכי כתובות.

 5. בצע את שלבי האשף כדי להוריד את תכלת AD Connect והשתמש בו כדי לסנכרן את המשתמשים שנשלטים על-ידי התחום שלך ב-Microsoft 365.


ראה [הגדרת סינכרון מדריכי כתובות עבור Microsoft 365](../enterprise/set-up-directory-synchronization.md) לקבלת מידע נוסף.

בעת קביעת התצורה של האפשרויות עבור התחברות של תכלת לספירה, אנו ממליצים להפוך **סינכרון סיסמה** לזמין, **כניסה יחידה חלקה** והתכונה **Password writeback** , הנתמכת גם ב-Microsoft 365 for business.

> [!NOTE]
> קיימים כמה שלבים נוספים עבור סיסמה writeback מעבר לתיבת הסימון בקישור תכלת AD. לקבלת מידע נוסף, ראה [כיצד לעשות זאת: קביעת תצורה של writeback password](/azure/active-directory/authentication/howto-sspr-writeback). 

אם ברצונך גם לנהל מכשירי Windows 10 המצורפים לתחום, ראה [הפיכת מכשירי windows 10 המצורפים לתחום למנוהל על-ידי Microsoft 365 Business Premium](manage-windows-devices.md) כדי להגדיר הצטרפות להודעה משולבת של תכלת.