---
title: אימות הגדרות הגנה של אפליקציות במחשבי Windows 10
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: למד כיצד לאמת את הגדרות ההגנה על אפליקציות של Microsoft 365 for business שהופעלו במכשירי Windows 10 של המשתמשים שלך.
ms.openlocfilehash: ff99b3a4fce49aebdb5c72f51e46678a7821e186
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912413"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>אימות הגדרות הגנה על מכשירים במחשבי Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>אימות ש-Windows 10 מדיניות התקן מוגדרים

לאחר [הגדרת מדיניות מכשירים](protection-settings-for-windows-10-pcs.md), ייתכן שיחלפו כמה שעות עד שהמדיניות תיכנס לתוקף של מכשירי משתמשים. באפשרותך לוודא שהמדיניות השפיעה על-ידי התבוננות במסכים שונים של הגדרות Windows במכשירים של המשתמשים. מכיוון שהמשתמשים לא יוכלו לשנות את הגדרות windows Update ו-Windows Defender Antivirus במכשירי Windows 10 שלהם, אפשרויות רבות ייראו באפור.
  
1. עבור אל  \> **&amp;** \>  \> **אפשרויות הפעלה מחדש** של עדכון אבטחה עבור הגדרות Windows update ואשר שכל ההגדרות מעומעמות. 
    
    ![כל אפשרויות ההפעלה מחדש מעומעמות.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. עבור אל  \> האפשרויות המתקדמות של **עדכון &amp; אבטחה** עבור \> **Windows update** \>  ואשר שכל ההגדרות מעומעמות. 
    
    ![האפשרויות ' עדכונים מתקדמים ' של Windows מעומעמות.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. עבור אל  \> **&amp;** \> ' אפשרויות מתקדמות ' של עדכוני אבטחה **של Windows update Windows** \>  \> , **בחר כיצד יישלחו עדכונים**.
    
    ודא שניתן לראות את ההודעה (באדום) שהגדרות מסוימות מוסתרות או מנוהלות על-ידי הארגון שלך, וכל האפשרויות מעומעמות.
    
    ![בחר כיצד עדכונים מועברים בדף מציין שההגדרות מוסתרות או מנוהלות על-ידי הארגון שלך.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. כדי לפתוח את מרכז האבטחה של windows defender, עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **של windows** defender \> לחץ על **פתח את windows defender מרכז** \> **האבטחה וירוסים וירוסים &amp; הגנה** על \> **&amp; הגדרות הגנה** מפני הגנה 
    
5. ודא שכל האפשרויות מעומעמות. 
    
    ![הגדרות הגנה מפני וירוסים ואיומים מעומעמות.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>נושאים קשורים

[תיעוד ומשאבים של Microsoft 365 for business](./index.yml)
  
[תחילת העבודה עם Microsoft 365 for business](microsoft-365-business-overview.md)
  
[ניהול Microsoft 365 for business](manage.md)
  
[קביעת תצורות של מכשירים עבור מחשבי Windows 10](protection-settings-for-windows-10-pcs.md)
