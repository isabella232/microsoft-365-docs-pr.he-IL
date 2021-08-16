---
title: אודות ההגדרות של פרופיל AutoPilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: פרופילי AutoPilot עוזרים לך לקבוע Windows ההתקנה במכשירי משתמש. הפרופילים מכילים הגדרות ברירת מחדל והגדרות אופציונליות, כמו Cortana התקנה.
ms.openlocfilehash: 67ad6e92583d71207e2807657a7ad00261e1249291e2e6a7546f544ea924b394
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53896322"
---
# <a name="about-autopilot-profile-settings"></a>אודות ההגדרות של פרופיל AutoPilot

## <a name="autopilot-profile-settings"></a>הגדרות פרופיל AutoPilot

באפשרותך להשתמש בפרופילי AutoPilot כדי לשלוט באופן Windows מותקן במכשירי משתמש. הפרופילים מכילים את ההגדרות הבאות.
  
 **תכונות ברירת המחדל של AutoPilot (נדרש) המוגדרות באופן אוטומטי:**
  
|**הגדרה**|**תיאור**|
|:-----|:-----|
|דלג Cortana, OneDrive ורישום OEM  <br/> |מדלג על ההתקנה של יישומי צרכנים, Cortana ואפליקציות OneDrive. משתמש המכשיר יכול להתקין תקנות אלה מאוחר יותר כל עוד המשתמש הוא מנהל מערכת מקומי במכשיר. המערכת דילגה על רישום היצרן המקורי מאחר שהמכשיר ינוהל על-ידי Microsoft 365 Business Premium.  <br/> |
|חוויית כניסה באמצעות מותג החברה שלך  <br/> |אם לחברה שלך יש מיתוג הוסף את [החברה שלך Microsoft 365 כניסה,](../admin/setup/customize-sign-in-page.md)משתמש המכשיר מקבל חוויה זו בעת הכניסה.  <br/> |
|הרשמה אוטומטית של MDM עם חשבונות AAD שהוגדרו.  <br/> |זהות המשתמש תנוהל על-ידי Azure Active Directory, והמשתמשים יירשם ל- Windows ו- Microsoft 365 עם אישורי Microsoft 365 Business Premium שלהם.  <br/> |
   
 **הגדרות אופציונליות:**
  
|**הגדרה**|**תיאור**|
|:-----|:-----|
|דלג על הגדרות הפרטיות (כבוי כברירת מחדל)  <br/> |אם אפשרות זו מוגדרת **ל'הפעל',** משתמש המכשיר לא יראה את הסכם הרשיון עבור המכשיר Windows כאשר הוא נכנס לראשונה.  <br/> |
|אל תאפשר למשתמש להפוך למנהל המערכת המקומי  <br/> |אם אפשרות זו מוגדרת **ל'הפעל',** משתמש המכשיר לא יוכל להתקין אפליקציות אישיות כלשהן, כגון Cortana.<br/> |
