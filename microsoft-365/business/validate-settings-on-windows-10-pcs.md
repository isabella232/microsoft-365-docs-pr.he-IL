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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: למד כיצד לאמת את הגדרות הגנת היישום העסקי של Microsoft 365 בהתקני Windows 10.
ms.openlocfilehash: e3cd0a1927e0b81c9a97d26196603086b9ea2293
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594954"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>אימות הגדרות הגנת התקן במחשבי Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>ודא שמדיניות ההתקנים של Windows 10 מוגדרת

לאחר [הגדרת פריטי מדיניות של התקנים](protection-settings-for-windows-10-pcs.md), המדיניות עשויה להימשך שעות ספורות כדי שהמדיניות ייכנסו לתוקף בהתקני המשתמשים. באפשרותך לאשר שהמדיניות השפיעה על-ידי התבוננות במסכים שונים של הגדרות Windows בהתקני המשתמשים. מאחר שהמשתמשים לא יוכלו לשנות את הגדרות windows Update ו-Windows Defender Antivirus בהתקני Windows 10 שלהם, אפשרויות רבות יופיעו באפור.
  
1. עבור אל **' הגדרות** \> ** &amp; עדכון אבטחה** \> **של Windows עדכון** \> **אפשרויות הפעלה מחדש** ולוודא שכל ההגדרות אפורות. 
    
    ![כל האפשרויות הפעלה מחדש מאפורות.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. עבור אל **הגדרות** \> ** &amp; עדכון אבטחה** \> **Windows עדכן** \> **אפשרויות מתקדמות** וודא כי כל ההגדרות אפורות. 
    
    ![אפשרויות העדכונים המתקדמים של Windows מאפורות כולן.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. עבור אל **הגדרות** \> ** &amp; עדכון אבטחה** \> **של Windows update** \> **אפשרויות** \> **מתקדמות בחר את אופן המשלוח של עדכונים**.
    
    ודא כי באפשרותך לראות את ההודעה (באדום) שההגדרות מסוימות מוסתרות או מנוהלות על-ידי הארגון שלך וכל האפשרויות מאפורות.
    
    ![בחר כיצד עדכונים מועברים לדף מציין שההגדרות מוסתרות או מנוהלות על-ידי הארגון שלך.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. כדי לפתוח את מרכז האבטחה של Windows defender, עבור אל **הגדרות** \> ** &amp; עדכון אבטחה** \> **windows defender** \> לחץ על **פתח windows Defender אבטחה מרכז** \> **וירוס &amp; הגנת הליך** \> הגנה **איום וירוס &amp; **. 
    
5. ודא שכל האפשרויות מעומעמת. 
    
    ![הגדרות הגנת הווירוס והאיום מאפורות.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>נושאים קרובים

[תיעוד ומשאבים עבור Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[תחילת העבודה עם Microsoft 365 Business](microsoft-365-business-overview.md)
  
[ניהול של Microsoft 365 Business](manage.md)
  
[קביעת תצורות של מכשירים עבור מחשבי Windows 10](protection-settings-for-windows-10-pcs.md)
  

