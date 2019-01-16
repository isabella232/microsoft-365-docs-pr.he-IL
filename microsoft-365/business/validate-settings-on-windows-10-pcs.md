---
title: אימות הגדרות הגנה של אפליקציות במחשבי Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: למד כיצד לאמת את הגדרות ההגנה app עסקיים 365 Microsoft ב- Windows 10 התקנים.
ms.openlocfilehash: db05c86bd75cc30e22e025034a3dab478d0f5365
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982704"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>אימות הגדרות הגנה התקן במחשבים 10 חלונות

## <a name="verify-that-windows-10-device-policies-are-set"></a>ודא כי מדיניות התקן Windows 10 מוגדרות

לאחר [הגדרת פריטי מדיניות של התקנים](protection-settings-for-windows-10-pcs.md), עשוי להימשך עד מספר שעות עבור המדיניות ייכנסו לתוקף במכשירים של המשתמשים. באפשרותך לאשר למדיניות ארך אפקט על-ידי התבוננות מסכי הגדרות Windows שונים במכשירים של המשתמשים. מאחר למשתמשים לא תהיה אפשרות לשנות את הגדרות Windows Update ו- Windows Defender וירוס בהתקנים שלהם Windows 10, מספר רב של אפשרויות אלה יעומעמו.
  
1. עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **עדכון Windows** \> **אפשרויות הפעלה מחדש** ואשר כל ההגדרות הם greyed החוצה. 
    
    ![כל האפשרויות מחדש הם greyed החוצה.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **עדכון Windows** \> **אפשרויות מתקדמות** ואשר כל ההגדרות הם greyed החוצה. 
    
    ![אפשרויות מתקדמות של Windows של עדכונים הם כל greyed החוצה.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **עדכון Windows** \> **אפשרויות מתקדמות** \> **בחר כיצד העדכונים יועברו**.
    
    ודא כי באפשרותך לראות את ההודעה (באדום) הגדרות מסוימות הן מוסתרות או מנוהל על-ידי הארגון שלך, ולא כל האפשרויות הם greyed החוצה.
    
    ![בחר כיצד מועברים עדכוני דף מציין הגדרות הן מוסתרות או מנוהל על-ידי הארגון שלך.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. כדי לפתוח את מרכז האבטחה של Windows Defender, עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **Windows Defender** \> לחץ על **פתח את Windows Defender מרכז האבטחה** \> **וירוס &amp; משנה (thread) הגנה** \> **וירוס &amp; איום הגדרות הגנה**. 
    
5. ודא כי כל האפשרויות הם greyed החוצה. 
    
    ![הגדרות ההגנה מפני וירוסים ותוכנות איום הם greyed החוצה.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>נושאים קשורים

[תיעוד ומשאבים עבור Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[תחילת העבודה עם Microsoft 365 Business](microsoft-365-business-overview.md)
  
[ניהול של Microsoft 365 Business](manage.md)
  
[קביעת תצורות של מכשירים עבור מחשבי Windows 10](protection-settings-for-windows-10-pcs.md)
  

