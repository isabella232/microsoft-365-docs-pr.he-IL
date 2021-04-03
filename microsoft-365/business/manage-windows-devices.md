---
title: אפשר ניהול של מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 לעסקים
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
description: למד כיצד לאפשר ל- Microsoft 365 להגן על מכשירי Windows 10 מקומיים המצורפים ל- Active-Directory בכמה שלבים בלבד.
ms.openlocfilehash: 8a45c6959bee368491c5c6424e3713300c443779
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580133"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>אפשר ניהול של מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business Premium

אם הארגון שלך משתמש ב- Windows Server Active Directory באופן מקומי, באפשרותך להגדיר את Microsoft 365 Business Premium כדי להגן על מכשירי Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים הדורשים אימות מקומי.
כדי להגדיר הגנה זו, באפשרותך ליישם מכשירים **מצורפים היברידיים של Azure AD**. מכשירים אלה מצורפים הן ל- Active Directory המקומי ול- Azure Active Directory שלך.

סרטון וידאו זה מתאר את השלבים לאיך להגדיר זאת עבור התרחיש הנפוץ ביותר, המפורט גם בשלבים המפורטים.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>לפני תחילת העבודה, הקפד להשלים שלבים אלה:
- סנכרן משתמשים עם Azure AD באמצעות Azure AD Connect.
- השלם את סינכרון היחידה הארגונית (OU) של Azure AD Connect.
- ודא שלמשתמשי התחום שאתה מסנכרן יש רשיונות ל- Microsoft 365 Business Premium.

ראה [סינכרון משתמשי תחום עם Microsoft](manage-domain-users.md) לקבלת השלבים.

## <a name="1-verify-mdm-authority-in-intune"></a>1. אימות רשות MDM ב- Intune

עבור אל מנהל [נקודות הקצה](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) ובדף Microsoft Intune, בחר  הרשמה למכשירים ולאחר מכן, בדף מבט כולל, ודא כי **רשות MDM** היא **Intune**. 

- אם **רשות MDM** היא **ללא**, לחץ על **רשות MDM** כדי להגדיר אותה ל- **Intune**.
- אם **רשות MDM** היא **Microsoft Office 365**,עבור אל מכשירים הרשמה מכשירים והשתמש בתיבת הדו-שיח הוספת רשות MDM בצד ימין כדי להוסיף רשות MDM של Intune (תיבת הדו-שיח הוספת רשות MDM זמינה רק אם רשות MDM מוגדרת ל- Microsoft Office  >   365).    

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. ודא ש- Azure AD זמין להצטרפות למחשבים

- עבור אל מרכז הניהול ב ובחר Azure Active Directory (בחר הצג הכל אם Azure Active Directory אינו <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> גלוי) **ברשימה מרכזי הניהול.**  
- במרכז הניהול **של Azure Active Directory**, עבור אל Azure Active **Directory** , בחר **מכשירים ולאחר** מכן בחר **הגדרות מכשיר**.
- אימות **שמשתמשים עשויים להצטרף למכשירים ל- Azure AD** זמין 
    1. כדי להפוך את כל המשתמשים לזמינים, הגדר את **האפשרות הכל.**
    2. כדי להפוך משתמשים ספציפיים לזמינים, הגדר **את האפשרות נבחר** כדי להפוך קבוצת משתמשים ספציפית לזמינה.
        - הוסף את משתמשי התחום הרצויים מסונכרנים ב- Azure AD [לקבוצת אבטחה](../admin/create-groups/create-groups.md).
        - בחר **בחר קבוצות כדי** להפוך טווח משתמש MDM לזמין עבור קבוצת אבטחה זו.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. ודא ש- Azure AD זמין עבור MDM

- עבור אל מרכז הניהול ב ובחר <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  באפשרות **Endpoint Managemen** t (בחר **הצג הכל אם** מנהל נקודות **הקצה** אינו גלוי)
- במרכז הניהול **של Microsoft Endpoint Manager**, עבור אל 'הרשמה **אוטומטית'** של  >  **מכשירים** של Windows  >  **הרשמה** אוטומטית של Windows  >  .
- ודא שטווח המשתמש של MDM זמין.

    1. כדי לרשום את כל המחשבים, הגדר הכל **כדי** לרשום באופן אוטומטי את כל מחשבי המשתמשים המצורפים ל- Azure AD ולמחשבים חדשים כאשר המשתמשים מוסיפים חשבון עבודה ל- Windows.
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
> מומלץ להתקין מודול זה בשרת Windows שבו פועל Azure AD Connect.

כדי ליצור את נקודת החיבור הנדרשת של השירות ומדיניות קבוצתית, תוכל להפעיל את [cmdlet Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) תצטרך את אישורי מנהל המערכת הכלליים של Microsoft 365 Business Premium בעת ביצוע משימה זו. כאשר תהיה מוכן ליצור את המשאבים, להפעיל את הפעולות הבאות:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

הפקודה הראשונה תבסס חיבור לענן Microsoft, וכאשר תתבקש לעשות זאת, ציין את אישורי הניהול הכלליים של Microsoft 365 Business Premium.

## <a name="5-link-the-group-policy"></a>5. קישור המדיניות הקבוצתית

1. במסוף ניהול המדיניות הקבוצתית (GPMC), לחץ באמצעות לחצן העכבר הימני על המיקום שבו ברצונך לקשר את המדיניות ובחר קשר *GPO קיים...* בתפריט תלוי ההקשר.
2. בחר את המדיניות שנוצרה בשלב לעיל ולאחר מכן לחץ על **אישור.**

## <a name="get-the-latest-administrative-templates"></a>קבל את תבניות הניהול העדכניות ביותר

אם אינך רואה את המדיניות הפוך הרשמה **אוטומטית של MDM** לזמינה באמצעות אישורי Azure AD המוגדרים כברירת מחדל, ייתכן שהאפשרות היא שה- ADMX אינו מותקן עבור Windows 10, גירסה 1803 ואילך. כדי לפתור את הבעיה, בצע את השלבים הבאים (הערה: MDM.admx העדכני ביותר תואם לאחור):

1.  הורד: [תבניות מנהליות (.admx) עבור Windows 10 אוקטובר 2020 Update (20H2)](https://www.microsoft.com/download/102157).
2.  התקן את החבילה בבקר תחום.
3.  נווט, בהתאם לגירסת תבניות הניהול לתיקיה: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.
4.  שנה את **שם התיקיה** הגדרות מדיניות בנתיב לעיל **למדיניותDefinitions**.
5.  העתק את **התיקיה PolicyDefinitions** לשיתוף SYSVOL שלך, הממוקמת כברירת מחדל **ב- C:\Windows\SYSVOL\domain\Policies**. 
    -   אם בכוונתך להשתמש בחנות מדיניות מרכזית עבור התחום כולו, הוסף את התוכן של PolicyDefinitions שם.
6.  במקרה שיש לך כמה בקרי תחום, המתן עד ש- SYSVOL ישכפל כדי שמדיניות תהיה זמינה. הליך זה יעבוד גם עבור כל גירסה עתידית של תבניות הניהול.

בשלב זה, תוכל לראות את המדיניות הפוך הרשמה אוטומטית של MDM לזמינה באמצעות אישורי **Azure AD המוגדרים כברירת** מחדל.