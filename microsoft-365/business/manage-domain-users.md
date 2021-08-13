---
title: סינכרון משתמשי תחום עם Microsoft 365
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: סנכרן משתמשים מבוקרי תחום עם Microsoft 365 לעסקים.
ms.openlocfilehash: 468fa943df55b12573f0a4f595294e39a146b1850f3c430ac2088a30991c0e60
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809311"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>סינכרון משתמשי תחום עם Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. התכונן לסינכרון מדריכי כתובות 

לפני סינכרון המשתמשים והמחשבים שלך מתחום Active Directory המקומי, עיין [בהכנה לסינכרון מדריכי כתובות Microsoft 365.](../enterprise/prepare-for-directory-synchronization.md) בפרט:

   - ודא שלא קיימים כפילויות במדריך הכתובות שלך עבור התכונות הבאות: **דואר**, **proxyAddresses** **ו- userPrincipalName**. ערכים אלה חייבים להיות ייחודיים ויש להסיר את כל הכפילויות.
   
   - מומלץ להגדיר את התכונה **userPrincipalName** (UPN) עבור כל חשבון משתמש מקומי כך שתהתאים לכתובת הדואר האלקטרוני הראשית התואמת למשתמש Microsoft 365 רשיון. לדוגמה: *mary.shelley@contoso.com* במקום *mary@contoso.local*
   
   - אם התחום של Active Directory מסתיים בסיומת לא ניתנת לניתוב, כגון *.local* או *.lan,* במקום סיומת הניתנת לניתוב באינטרנט, כגון *.com* או *.org,* התאם את סיומת UPN של חשבונות המשתמשים המקומיים תחילה כמתואר בנושא הכנת תחום שאינו ניתן לניתוב [עבור סינכרון מדריכי כתובות.](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md) 

ה- **Run IdFix** בשלב ארבע (4) להלן, יוודא גם ש- Active Directory המקומי מוכן לסינכרון מדריכי כתובות.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. התקן וקבע את תצורת Azure AD התחברות

כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מ- Active Directory המקומי לתוך Azure Active Directory, התקן את Azure Active Directory התחברות והגדיר סינכרון מדריכי כתובות. 

 1. במרכז [](https://go.microsoft.com/fwlink/p/?linkid=2024339)הניהול, בחר **הגדרה** בסרגל הניווט הימני.

 2. תחת **כניסה ואבטחה, בחר** הצג תחת **סינכרון** **משתמשים מהמדריך הכתובות של האתרים שלך.**

 3. בדף **סינכרון משתמשים ממדריך הכתובות של האתרים** שלך, בחר **תחילת העבודה**.

 4. בשלב הראשון הפעל את הכלי IdFix כדי להתכונן לסינכרון מדריך כתובות.

 5. בצע את שלבי האשף כדי להוריד את Azure AD התחברות להשתמש בו כדי לסנכרן את המשתמשים הנשלטים על-ידי התחום כדי Microsoft 365.


ראה [הגדרת סינכרון מדריכי כתובות Microsoft 365](../enterprise/set-up-directory-synchronization.md) לקבלת מידע נוסף.

כאשר תקבע את תצורת האפשרויות עבור Azure AD התחברות, מומלץ להפוך סינכרון סיסמאות **,** כניסה יחידה חלקה לזמינה ואת התכונה **writeback** של הסיסמה, הנתמכת גם היא ב- Microsoft 365 לעסקים.

> [!NOTE]
> ישנם כמה שלבים נוספים עבור writeback סיסמה מעבר לתיבת הסימון ב- Azure AD התחברות. לקבלת מידע נוסף, ראה [כיצד לעשות: קביעת תצורה של writeback של סיסמה](/azure/active-directory/authentication/howto-sspr-writeback). 

אם ברצונך גם לנהל התקני Windows 10, ראה הפיכת התקני Windows 10 לתחום לזמינים [לניהול על-ידי Microsoft 365 Business Premium](manage-windows-devices.md) כדי להגדיר צירוף Azure AD היברידי.