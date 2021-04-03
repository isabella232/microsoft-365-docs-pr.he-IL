---
title: אימות הגדרות הגנה של אפליקציות במחשבי Windows 10
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: למד כיצד לוודא שהגדרות ההגנה על אפליקציה של Microsoft 365 לעסקים השפיעו על מכשירי Windows 10 של המשתמשים שלך.
ms.openlocfilehash: fcb463fd98f692f7d4802689e0c03fe4e3e648a1
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579841"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>אימות הגדרות הגנה על מכשיר במחשבי Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>ודא שמדיניות המכשיר של Windows 10 מוגדרת

לאחר הגדרת [מדיניות מכשירים,](protection-settings-for-windows-10-pcs.md)ייתכן שיקח עד כמה שעות עד שהמדיניות תיתוקף במכשירים של המשתמשים. באפשרותך לאשר שמדיניות זו השפיעה על-ידי התסתכלות על מסכי הגדרות Windows השונים במכשירים של המשתמשים. מאחר שהמשתמשים לא יוכלו לשנות את הגדרות האנטי-וירוס של Windows Update ו- Windows Defender במכשירי Windows 10 שלהם, אפשרויות רבות יהיו באפור.
  
1. עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **אפשרויות הפעלה מחדש** של Windows Update \>  ואשר שכל ההגדרות מופיעות באפור. 
    
    ![כל אפשרויות ההפעלה מחדש מופיעות באפור.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **אפשרויות Windows Update** \> **Advanced** ואשר שכל ההגדרות מופיעות באפור. 
    
    ![אפשרויות העדכונים המתקדמות של Windows מופיעות באפור.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **אפשרויות מתקדמות של Windows Update** \>  \> **בחר כיצד ישלחו עדכונים.**
    
    אשר כי באפשרותך לראות את ההודעה (באדום) שהגדרות מסוימות מוסתרות או מנוהלות על-ידי הארגון שלך, וכל האפשרויות מופיעות באפור.
    
    ![בחר כיצד הדף מועבר מציין שההגדרות מוסתרות או מנוהלות על-ידי הארגון שלך.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. כדי לפתוח את מרכז האבטחה של Windows Defender, עבור **אל** הגדרות עדכון אבטחה \> **&amp;** Windows \> **Defender, לחץ** על פתח את הגדרות ההגנה מפני איומים מפני וירוסים של מרכז האבטחה של Windows \>  \> **&amp;** \> **&amp;** Defender. 
    
5. ודא שכל האפשרויות מופיעות באפור. 
    
    ![הגדרות ההגנה מפני וירוסים ואיומים מופיעות באפור.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>נושאים קשורים

[תיעוד ומשאבים של Microsoft 365 לעסקים](./index.yml)
  
[תחילת העבודה עם Microsoft 365 לעסקים](microsoft-365-business-overview.md)
  
[ניהול Microsoft 365 לעסקים](manage.md)
  
[קביעת תצורות של מכשירים עבור מחשבי Windows 10](protection-settings-for-windows-10-pcs.md)
