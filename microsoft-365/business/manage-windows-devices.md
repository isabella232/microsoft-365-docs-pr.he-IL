---
title: הפיכת מכשירי Windows 10 המצורפים לתחום למנוהל על-ידי Microsoft 365 for business
f1.keywords:
- CSH
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: למד כיצד להפוך את Microsoft 365 לזמין כדי להגן על מכשירים מקומיים של Active Directory המצורפים ל-Windows 10 בשלבים ספורים בלבד.
ms.openlocfilehash: 82d4ac3f1d6aba9489f9ea153de3a3d2083b47ec
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913193"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>הפיכת מכשירי Windows 10 המצורפים לתחום למנוהל על-ידי Microsoft 365 Business Premium

אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business Premium כדי להגן על מכשירי Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים הדורשים אימות מקומי.
כדי להגדיר הגנה זו, באפשרותך ליישם **מכשירים המצורפים להודעה משולבת של תכלת**. מכשירים אלה מצורפים הן ל-Active Directory המקומי והן ל-תכלת Active Directory שלך.

סרטון וידאו זה מתאר את השלבים להגדרת פעולה זו עבור התרחיש הנפוץ ביותר, המפורט גם בשלבים הבאים.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>לפני שתתחיל, הקפד להשלים שלבים אלה:
- סנכרן משתמשים לתכלת לספירה באמצעות התחברות של תכלת לספירה.
- השלם את הסינכרון של היחידה הארגונית של "תכלת" (OU).
- ודא שכל משתמשי התחום שאתה מסנכרן הם בעלי רשיונות ל-Microsoft 365 Business Premium.

ראה [סינכרון משתמשי תחום ל-Microsoft](manage-domain-users.md) לקבלת השלבים.

## <a name="1-verify-mdm-authority-in-intune"></a>1. אימות הרשות של MDM בתוך המנגינה

עבור אל [מנהל נקודות הקצה](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) ולאחר מכן, בעמוד ההתאמה של Microsoft, בחר באפשרות **הרשמת מכשיר** ולאחר מכן, בדף **מבט כולל** , ודא **שסמכות MDM** מתכוונת **.**

- אם **הרשות של mdm** היא **None**, לחץ על **הרשות mdm** כדי **להגדיר** אותה כתכונה.
- אם **הרשות של MDM** היא **microsoft office 365**, **עבור אל** מכשירי רישום של מכשירים  >   והשתמש בתיבת הדו **הוספת רשות mdm** בצד שמאל כדי להוסיף **כוונון רשות mdm** (תיבת הדו **הוספת רשות mdm** זמינה רק אם **הרשות mdm** מוגדרת ל-Microsoft office 365).

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. ודא שתכלת לספירה מופעל לצורך הצטרפות למחשבים

- עבור אל מרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  ובחר **תכלת active directory** (בחר הצג הכל אם תכלת active directory אינו גלוי) ברשימת **מרכזי הניהול** . 
- במרכז **הניהול של תכלת Active directory**, עבור **אל תכלת active directory** , בחר **התקנים** ולאחר מכן **הגדרות התקן**.
- אימות **משתמשים עשויים לצרף מכשירים לתכלת AD** מופעל 
    1. כדי להפוך את כל המשתמשים לזמינים, הגדר **הכל**.
    2. כדי להפוך משתמשים ספציפיים לזמינים, הגדר לאפשרות **נבחרה** כדי להפוך קבוצת משתמשים ספציפית לזמינה.
        - הוסף את משתמשי התחום הרצויים מסונכרנים בתכלת לספירה [לקבוצת אבטחה](../admin/create-groups/create-groups.md).
        - בחר **באפשרות בחר קבוצות** כדי להפוך את טווח המשתמש של MDM לזמין עבור קבוצת אבטחה זו.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. אימות תכלת לספירה מופעל עבור MDM

- עבור אל מרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  ובחר באפשרות בחר **נקודת קצה Managemen** t (בחר **הצג הכל** אם **מנהל נקודות הקצה** אינו גלוי)
- במרכז **הניהול של מנהל נקודות הקצה של Microsoft**, עבור אל מכשירים   >    >    >  **ההרשמה האוטומטית** של windows windows הרשמה.
- אימות טווח המשתמשים של MDM זמין.

    1. כדי לרשום את כל המחשבים, הגדר **הכל** כדי לרשום באופן אוטומטי את כל מחשבי המשתמש המצורפים לתכלת לספירה ולמחשבים חדשים כאשר המשתמשים מוסיפים חשבון עבודה ל-Windows.
    2. הגדר **כמה** כדי לרשום את המחשבים של קבוצת משתמשים ספציפית.
        -  הוסף את משתמשי התחום הרצויים מסונכרנים בתכלת לספירה [לקבוצת אבטחה](../admin/create-groups/create-groups.md).
        -  בחר **באפשרות בחר קבוצות** כדי להפוך את טווח המשתמש של MDM לזמין עבור קבוצת אבטחה זו.

## <a name="4-create-the-required-resources"></a>4. יצירת המשאבים הדרושים 

ביצוע המשימות הנדרשות כדי [לקבוע את התצורה של הצטרפות היברידית של ' תכלת לספירה](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) ' היה פשוט יותר באמצעות ה-Cmdlet ' [אתחול-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) ' שנמצא במודול [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell. כאשר אתה מפעיל את ה-cmdlet הזה, הוא ייצור ויקבע את התצורה של נקודת חיבור השירות הנדרשת והמדיניות הקבוצתית.

באפשרותך להתקין מודול זה על-ידי הפעלת הפרטים הבאים מתוך מופע של PowerShell:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> מומלץ להתקין מודול זה בשרת Windows שבו פועל הקישור תכלת לספירה.

כדי ליצור את נקודת חיבור השירות הדרושה ומדיניות קבוצתית, עליך להפעיל את ה  [-Cmdlet אתחול-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) . תזדקק לאישורי מנהל מערכת כללי של Microsoft 365 Business Premium בעת ביצוע משימה זו. כאשר תהיה מוכן ליצור את המשאבים, הפעל את הפרטים הבאים:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

הפקודה הראשונה תיצור חיבור עם הענן של Microsoft, וכאשר תתבקש, ציין את אישורי מנהל המערכת הכלליים של Microsoft 365 Business Premium.

## <a name="5-link-the-group-policy"></a>5. קישור מדיניות קבוצתית

1. במסוף ניהול מדיניות קבוצתית (GPMC), לחץ באמצעות לחצן העכבר הימני על המיקום שבו ברצונך לקשר את המדיניות ובחר קשר אובייקט מדיניות *קיים.* ... מהתפריט תלוי ההקשר.
2. בחר את המדיניות שנוצרה בשלב שלעיל ולאחר מכן לחץ על **אישור**.

## <a name="get-the-latest-administrative-templates"></a>קבל את תבניות הניהול האחרונות

אם אינך רואה את המדיניות **הפיכת הרשמה אוטומטית של MDM לזמינה באמצעות כברירת מחדל של הודעות מיידיות**, ייתכן שהסיבה לכך היא ש-ADMX אינו מותקן עבור Windows 10, גירסה 1803 ואילך. כדי לפתור את הבעיה, בצע שלבים אלה (הערה: הגירסה העדכנית ביותר של MDM. admx היא תואמת לאחור):

1.  [הורד: תבניות ניהול (. admx) עבור Windows 10 באוקטובר 2020 Update (20H2)](https://www.microsoft.com/download/102157).
2.  התקן את החבילה בבקר תחום.
3.  נווט, בהתאם לגירסת תבניות הניהול לתיקיה: **C:\Program Files (x86) \Microsoft Group Policy\Windows 10 באוקטובר 2020 Update (20H2)**.
4.  שנה את שם התיקיה ' **הגדרות מדיניות** ' בנתיב שלעיל אל **PolicyDefinitions**.
5.  העתק את התיקיה **PolicyDefinitions** למיקום המשותף של SYSVOL, כברירת מחדל, הממוקמת ב- **C:\Windows\SYSVOL\domain\Policies**. 
    -   אם בכוונתך להשתמש בחנות מדיניות מרכזית עבור התחום כולו, הוסף את התוכן של PolicyDefinitions שם.
6.  למקרה שיהיו לך כמה בקרי תחומים, המתן עד ש-SYSVOL ישכפל כדי שהמדיניות תהיה זמינה. הליך זה יפעל גם עבור כל גירסה עתידית של תבניות ניהול.

בשלב זה, תוכל לראות את המדיניות **הפיכת הרשמה אוטומטית של MDM לזמינה באמצעות כברירת מחדל של הודעות מיידיות** .