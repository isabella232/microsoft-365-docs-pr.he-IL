---
title: הפעל התקנים של Windows 10 המצורפים לתחום לניהול באמצעות Microsoft 365 עבור עסקים
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
description: למד כיצד לאפשר ל-Microsoft 365 להגן על התקנים מקומיים המצורפים ל-Windows 10 באמצעות ספריות בתוך מספר צעדים בלבד.
ms.openlocfilehash: 2eaf5aa76cae1680b93af008af615ae872e4fb20
ms.sourcegitcommit: fab425ea4580d1924fb421e6db233d135f5b7d19
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/31/2020
ms.locfileid: "46533784"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>אפשר להפעיל התקנים של Windows 10 המצורפים לתחום כדי שינוהל על-ידי Microsoft 365 Business Premium

אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business Premium כדי להגן על התקני Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים המחייבים אימות מקומי.
כדי להגדיר הגנה זו, באפשרותך ליישם **התקנים היברידית כחול לספירה המצורפים**. התקנים אלה מצורפים הן ל-Active Directory המקומי והן לספריה הפעילה שלך.

סרטון וידאו זה מתאר את השלבים עבור אופן ההגדרה של התרחיש הנפוץ ביותר, המפורט גם בשלבים הבאים.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>לפני שתתחיל, הקפד להשלים את השלבים הבאים:
- סנכרן משתמשים לתכלת והתחבר כתכלת.
- השלם תכלת AD חיבור יחידה ארגונית (OU) סינכרון.
- ודא שכל משתמשי התחום שתסנכרן כוללים רשיונות ל-Microsoft 365 Business Premium.

ראה [סינכרון משתמשי קבוצת מחשבים ל-Microsoft](manage-domain-users.md) עבור השלבים.

## <a name="1-verify-mdm-authority-in-intune"></a>1. ודא שרשות MDM בIntune

עבור אל portal.azure.com ובחלק העליון של חיפוש הדף עבור Intune.
בדף Microsoft Intune, בחר **הרשמת התקן** ובעמוד **מבט כולל** ודא **שהסמכות של MDM** היא **Intune**.

- אם **רשות mdm** אינה **קיימת**, לחץ על **הרשות mdm** כדי להגדיר אותה ל- **Intune**.
- אם **רשות mdm** היא **Microsoft Office 365**, עבור אל **התקנים**  >  **לרישום התקנים** והשתמש בתיבת הדו **הוספת הרשות של mdm** מימין כדי להוסיף את הרשות **Intune MDM** (תיבת הדו **הוספת הרשות של mdm** זמינה רק אם **הרשות MDM** מוגדרת ל-Microsoft Office 365).

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. ודא תכלת לספירה מופעל לצורך הצטרפות למחשבים

- עבור אל מרכז הניהול ב- <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ובחר באפשרות ' **active directory** ' (בחר הצג הכל אם הספריה הפעילה אינה גלויה) ברשימת **מרכזי הניהול** . 
- במרכז **הניהול של הספריה הפעילה**, עבור אל הכלי **הפעיל של active directory** , בחר באפשרות **התקנים** ולאחר מכן **הגדרות התקן**.
- ודא**כי משתמשים יכולים לצרף התקנים ל-"תכלת לספירה** " מופעלת 
    1. כדי להפוך את כל המשתמשים **לזמינים**, הגדר לכל.
    2. כדי להפוך משתמשים מסוימים לזמינים, הגדר **כנבחרת** כדי לאפשר קבוצה מסוימת של משתמשים.
        - הוסף את משתמשי התחום הרצויים המסונכרנת בתכלת לספירה [לקבוצת אבטחה](../admin/create-groups/create-groups.md).
        - בחר **קבוצות בחירה** כדי להפוך את טווח המשתמשים של MDM לזמין עבור קבוצת אבטחה זו.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. ודא תכלת לספירה מופעל עבור MDM

- עבור אל מרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> ובחר בחירת אנשי **מופע** של נקודות **הקצה**(בחר הצג הכל אם **מנהל נקודות הקצה** אינו גלוי)
- במרכז **הניהול של מנהל נקודות הקצה של Microsoft**, עבור אל **Devices**  >  **Windows**  >  **Windows Enrollment**  >  **הרישום האוטומטי**של התקנים של windows windows הרשמה.
- ודא שטווח המשתמש של MDM מופעל.

    1. כדי לרשום את כל המחשבים, הגדר **כולם** כדי לרשום באופן אוטומטי את כל מחשבי המשתמש המצורפים לתכלת AD ולמחשבים חדשים כאשר המשתמשים מוסיפים חשבון עבודה ל-Windows.
    2. מוגדר **כחלק** כדי לרשום את המחשבים של קבוצת משתמשים מסוימת.
        -  הוסף את משתמשי התחום הרצויים המסונכרנת בתכלת לספירה [לקבוצת אבטחה](../admin/create-groups/create-groups.md).
        -  בחר **קבוצות בחירה** כדי להפוך את טווח המשתמשים של MDM לזמין עבור קבוצת אבטחה זו.

## <a name="4-create-the-required-resources"></a>4. צור את המשאבים הדרושים 

ביצוע המשימות הנדרשות כדי [לקבוע את התצורה של היברידית התכלת להצטרף](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) היתה פשוטה באמצעות שימוש של [ההרשמה לאתחל-Secmgmthyהרשמה](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Cmdlet נמצא במודול [secmgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell. בעת הפעלת יישומון cmdlet זה, הוא ייצור ויקבע את התצורה של נקודת חיבור השירות הנדרשת והמדיניות הקבוצתית.

באפשרותך להתקין מודול זה על-ידי הפעלת הפעולה הבאה ממופע של PowerShell:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> מומלץ להתקין מודול זה ב-Windows Server שבו פועל התקשרות תכלת AD.

כדי ליצור את נקודת החיבור הדרושה של השירות והמדיניות הקבוצתית, עליך להפעיל את ה-cmdlet של [הרשמת ההתקן של התקנת האבטחה](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) . תזדקק לאישורי המנהל הגלובלי של Microsoft Business Premium 365 במהלך ביצוע משימה זו. כאשר תהיה מוכן ליצור את המשאבים, הפעל את הפעולות הבאות:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

הפקודה הראשונה תיצור חיבור עם ענן של Microsoft, וכאשר תתבקש, ציין את אישורי המנהל הכללי של מנהל העסקים של Microsoft 365.

## <a name="5-link-the-group-policy"></a>5. קשר את המדיניות הקבוצתית

1. במסוף ניהול המדיניות הקבוצתית (GPMC), לחץ באמצעות לחצן העכבר הימני על המיקום שבו ברצונך לקשר את המדיניות ובחר *קישור של GPO קיים.* ...
2. בחר את המדיניות שנוצרה בשלב הנ ל ולאחר מכן לחץ על **אישור**.

## <a name="get-the-latest-administrative-templates"></a>קבל את התבניות המנהליות העדכניות ביותר

אם אינך רואה שהמדיניות **מאפשרת הרשמה אוטומטית של MDM המשתמשת באישורי תכלת לספירה**, ייתכן שהסיבה לכך היא שאין ברשותך את ה-admx המותקנת עבור Windows 10, גירסה 1803, גירסה 1809 או גירסה 1903. כדי לפתור את הבעיה, בצע את הפעולות הבאות (הערה: MDM. admx האחרון תואם לאחור):

1.  [להוריד: תבניות מנהליות (. admx) עבור Windows 10 מאי 2019 עדכון (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).
2.  התקן את החבילה בבקר התחום הראשי (PDC).
3.  ניווט, בהתאם לגירסה לתיקיה: **C:\templletccome\n מיקרוסופט/Windows 10 May 2019 עדכון (1903) v3**.
4.  שנה את שם התיקיה **הגדרות מדיניות** בנתיב שלעיל **להגדרות**המדיניות.
5.  העתק את התיקיה ' **הגדרות** מדיניות ' ל- **C:\windows\so\t\uspe\n**. 
    -   אם בכוונתך להשתמש במאגר מדיניות מרכזי עבור כל התחום שלך, הוסף את תוכן המדיניות המבוטח.
6.  הפעל מחדש את בקר קבוצת המחשבים הראשי כדי שהמדיניות תהיה זמינה. הליך זה יפעל גם עבור כל גירסה עתידית.

בשלב זה אתה אמור להיות מסוגל לראות את המדיניות **לאפשר הרשמה אוטומטית MDM באמצעות ברירת המחדל של הודעות תכלת לספירה** זמין.
