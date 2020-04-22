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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: למד כיצד לוודא ש-Microsoft 365 עבור הגדרות של הגנת יישומים עסקיים השפיעה על התקני Windows 10 של המשתמשים שלך.
ms.openlocfilehash: b63681f040b0fe49127693e9cb7aac7ba6c41af6
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43635703"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>אימות הגדרות הגנת התקן במחשבי Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>ודא שמדיניות ההתקנים של Windows 10 מוגדרת

לאחר [הגדרת פריטי מדיניות של התקנים](protection-settings-for-windows-10-pcs.md), המדיניות עשויה להימשך שעות ספורות כדי שהמדיניות ייכנסו לתוקף בהתקני המשתמשים. באפשרותך לאשר שהמדיניות השפיעה על-ידי התבוננות במסכים שונים של הגדרות Windows בהתקני המשתמשים. מאחר שהמשתמשים לא יוכלו לשנות את הגדרות windows Update ו-Windows Defender Antivirus בהתקני Windows 10 שלהם, אפשרויות רבות יופיעו באפור.
  
1. עבור אל **' הגדרות** \> ** &amp; עדכון אבטחה** \> **של Windows עדכון** \> **אפשרויות הפעלה מחדש** ולוודא שכל ההגדרות אפורות. 
    
    ![כל האפשרויות הפעלה מחדש מאפורות.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. עבור אל **הגדרות** \> ** &amp; עדכון אבטחה** \> **Windows עדכן** \> **אפשרויות מתקדמות** וודא כי כל ההגדרות אפורות. 
    
    ![אפשרויות העדכונים המתקדמים של Windows מאפורות כולן.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. עבור אל **הגדרות** \> ** &amp; עדכון אבטחה** \> **של Windows update** \> **אפשרויות** \> **מתקדמות בחר את אופן המשלוח של עדכונים**.
    
    ודא כי באפשרותך לראות את ההודעה (באדום) שההגדרות מסוימות מוסתרות או מנוהלות על-ידי הארגון שלך וכל האפשרויות מאפורות.
    
    ![בחר כיצד עדכונים מועברים לדף מציין שההגדרות מוסתרות או מנוהלות על-ידי הארגון שלך.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. כדי לפתוח את מרכז האבטחה של Windows defender, עבור אל **הגדרות** \> ** &amp; עדכון אבטחה** \> **windows defender** \> לחץ על **פתח windows Defender אבטחה מרכז** \> **וירוס &amp; הגנת הליך** \> הגנה **איום וירוס &amp; **. 
    
5. ודא שכל האפשרויות מעומעמת. 
    
    ![הגדרות הגנת הווירוס והאיום מאפורות.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>נושאים קרובים

[מיקרוסופט 365 עבור תיעוד עסקי ומשאבים](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[התחל לעבוד עם Microsoft 365 לעסקים](microsoft-365-business-overview.md)
  
[ניהול מיקרוסופט 365 לעסקים](manage.md)
  
[קביעת תצורות של מכשירים עבור מחשבי Windows 10](protection-settings-for-windows-10-pcs.md)
  

