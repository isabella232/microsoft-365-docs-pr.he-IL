---
title: הפיכת מכשירי Windows 10 לתחום למנוהלים על-ידי Microsoft 365 לעסקים
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
description: למד כיצד לאפשר Microsoft 365 להגן על מכשירי Active-Directory Windows 10 מקומיים בכמה שלבים בלבד.
ms.openlocfilehash: ec80159bdceffd8a13d09a297a2acc1b78c9b1b3
ms.sourcegitcommit: 17f0aada83627d9defa0acf4db03a2d58e46842f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/24/2021
ms.locfileid: "52636085"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>הפיכת מכשירי Windows 10 לתחום למנוהלים על-ידי Microsoft 365 Business Premium

אם הארגון שלך משתמש ב- Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business Premium כדי להגן על מכשירי Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים הדורשים אימות מקומי.
כדי להגדיר הגנה זו, באפשרותך ליישם מכשירים **מצורפים היברידיים של Azure AD**. מכשירים אלה מצורפים הן ל- Active Directory המקומי ול- Azure Active Directory שלך.

## <a name="watch-configure-hybrid-azure-active-directory-join"></a>צפה: קביעת תצורה של צירוף היברידי של Azure Active Directory

סרטון וידאו זה מתאר את השלבים לאיך להגדיר זאת עבור התרחיש הנפוץ ביותר, המפורט גם בשלבים המפורטים.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="before-you-begin"></a>לפני שתתחיל

- סינכרון משתמשים עם Azure AD עם Azure AD התחברות.
- השלם את סינכרון התחברות Azure AD (OU).
- ודא שלמשתמשי התחום שאתה מסנכרן יש רשיונות Microsoft 365 Business Premium.

ראה [סינכרון משתמשי תחום עם Microsoft](manage-domain-users.md) לקבלת השלבים.

## <a name="1-verify-mdm-authority-in-intune"></a>1. אימות רשות MDM ב- Intune

עבור אל [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) ובדף Microsoft Intune, **בחר** הרשמה למכשירים ולאחר מכן,  בדף מבט כולל, ודא כי **רשות MDM** היא **Intune**.

- אם **רשות MDM** היא **ללא**, לחץ על **רשות MDM** כדי להגדיר אותה ל- **Intune**.
- אם **רשות MDM** **Microsoft Office 365,עבור** אל מכשירים הרשמה מכשירים והשתמש בתיבת הדו-שיח הוספת רשות MDM בצד ימין כדי להוסיף רשות  >   **Intune MDM** (תיבת הדו-שיח הוספת **רשות MDM** זמינה רק אם רשות **MDM** מוגדרת Microsoft Office 365). 

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. ודא ש- Azure AD זמין להצטרפות למחשבים

- עבור אל מרכז הניהול ב ובחר Azure Active Directory (בחר הצג הכל אם Azure Active Directory אינו <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> גלוי) **ברשימה מרכזי הניהול.**  
- במרכז הניהול **של Azure Active Directory**, עבור אל Azure Active **Directory** , בחר **מכשירים ולאחר** מכן בחר **הגדרות מכשיר**.
- אימות **שמשתמשים עשויים להצטרף למכשירים ל- Azure AD** זמין 
    1. כדי להפוך את כל המשתמשים לזמינים, הגדר את **האפשרות הכל.**
    2. כדי להפוך משתמשים ספציפיים לזמינים, הגדר **את האפשרות נבחר** כדי להפוך קבוצת משתמשים ספציפית לזמינה.
        - הוסף את משתמשי התחום הרצויים מסונכרנים ב- Azure AD [לקבוצת אבטחה](../admin/create-groups/create-groups.md).
        - בחר **בחר קבוצות כדי** להפוך טווח משתמש MDM לזמין עבור קבוצת אבטחה זו.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. ודא ש- Azure AD זמין עבור MDM

- עבור אל מרכז הניהול ב ובחר באפשרות <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **Endpoint Managemen** t (בחר **הצג** **הכל אם Endpoint Manager** אינו גלוי)
- במרכז **הניהול Microsoft Endpoint Manager**, עבור אל **מכשירים**  >  **Windows**  >  **Windows הרשמה**  >  **אוטומטית**.
- ודא שטווח המשתמש של MDM זמין.

    1. כדי לרשום את כל המחשבים, **הגדר** הכל כדי לרשום באופן אוטומטי את כל מחשבי המשתמשים המצורפים ל- Azure AD ולמחשבים חדשים כאשר המשתמשים מוסיפים חשבון עבודה ל- Windows.
    2. הגדר לחלק **כדי** לרשום את המחשבים של קבוצת משתמשים ספציפית.
        -  הוסף את משתמשי התחום הרצויים מסונכרנים ב- Azure AD [לקבוצת אבטחה](../admin/create-groups/create-groups.md).
        -  בחר **בחר קבוצות כדי** להפוך טווח משתמש MDM לזמין עבור קבוצת אבטחה זו.

## <a name="4-create-the-required-resources"></a>4. יצירת המשאבים הדרושים 

ביצוע המשימות הדרושות לקביעת התצורה של [צירוף Azure AD](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) היברידי התפשט באמצעות השימוש [ב- cmdlet של Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) שנמצא במודול [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell. כאשר אתה להפעיל cmdlet זה, הוא ייצור ויגדיר את נקודת החיבור הנדרשת של השירות ואת המדיניות הקבוצתית.

באפשרותך להתקין מודול זה על-ידי הפעלה של הפריטים הבאים ממופע של PowerShell:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> מומלץ להתקין מודול זה בשרת Windows Azure AD התחברות.

כדי ליצור את נקודת החיבור הנדרשת של השירות ומדיניות קבוצתית, תוכל להפעיל את [cmdlet Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) תצטרך את אישורי Microsoft 365 Business Premium הכלליים שלך בעת ביצוע משימה זו. כאשר תהיה מוכן ליצור את המשאבים, להפעיל את הפעולות הבאות:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

הפקודה הראשונה תבסס חיבור עם הענן של Microsoft, וכאשר תתבקש, ציין את אישורי Microsoft 365 Business Premium הכלליים.

## <a name="5-link-the-group-policy"></a>5. קישור המדיניות הקבוצתית

1. במסוף ניהול המדיניות הקבוצתית (GPMC), לחץ באמצעות לחצן העכבר הימני על המיקום שבו ברצונך לקשר את המדיניות ובחר קשר *GPO קיים...* בתפריט תלוי ההקשר.
2. בחר את המדיניות שנוצרה בשלב לעיל ולאחר מכן לחץ על **אישור.**

## <a name="get-the-latest-administrative-templates"></a>קבל את תבניות הניהול העדכניות ביותר

אם אינך רואה את המדיניות הפוך הרשמה **אוטומטית של MDM** לזמינה באמצעות אישורי Azure AD המוגדרים כברירת מחדל, ייתכן שהאפשרות היא ש- ADMX אינו מותקן עבור Windows 10, גירסה 1803 ואילך. כדי לפתור את הבעיה, בצע את השלבים הבאים (הערה: MDM.admx העדכני ביותר תואם לאחור):

1.  הורד: [תבניות מנהליות ( .admx) עבור עדכון Windows 10 אוקטובר 2020 (20H2)](https://www.microsoft.com/download/102157).
2.  התקן את החבילה בבקר תחום.
3.  נווט, בהתאם לגירסת תבניות הניהול לתיקיה: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 עדכון אוקטובר 2020 (20H2)**.
4.  שנה את **שם התיקיה** הגדרות מדיניות בנתיב לעיל **למדיניותDefinitions**.
5.  העתק את **התיקיה PolicyDefinitions** לשיתוף SYSVOL שלך, הממוקמת כברירת מחדל **ב- C:\Windows\SYSVOL\domain\Policies**. 
    -   אם בכוונתך להשתמש בחנות מדיניות מרכזית עבור התחום כולו, הוסף את התוכן של PolicyDefinitions שם.
6.  במקרה שיש לך כמה בקרי תחום, המתן עד ש- SYSVOL ישכפל כדי שמדיניות תהיה זמינה. הליך זה יעבוד גם עבור כל גירסה עתידית של תבניות הניהול.

בשלב זה, תוכל לראות את המדיניות הפוך הרשמה אוטומטית של MDM לזמינה באמצעות אישורי **Azure AD המוגדרים כברירת** מחדל.

## <a name="related-content"></a>תוכן קשור

[סינכרון משתמשי תחום Microsoft 365](manage-domain-users.md) (מאמר)\
[יצירת קבוצה במרכז הניהול](../admin/create-groups/create-groups.md) (מאמר)\
[ערכת לימוד: קביעת תצורה של צירוף היברידי של Azure Active Directory עבור תחומים מנוהלים](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (מאמר)