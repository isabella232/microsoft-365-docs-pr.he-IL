---
title: אימות הגדרות הגנה של אפליקציות במחשבי Windows 10
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: למד כיצד לאמת את הגדרות הגנת היישום העסקי של Microsoft 365 בהתקני Windows 10.
ms.openlocfilehash: 66e83df19e44419b37bcc1c5678ab13317162dbc
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288594"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>אימות הגדרות הגנת התקן במחשבי Windows 10

## <a name="verify-that-windows-10-device-policies-are-set"></a>ודא שמדיניות ההתקנים של Windows 10 מוגדרת

לאחר [הגדרת פריטי מדיניות של התקנים](protection-settings-for-windows-10-pcs.md), המדיניות עשויה להימשך שעות ספורות כדי שהמדיניות ייכנסו לתוקף בהתקני המשתמשים. באפשרותך לאשר שהמדיניות השפיעה על-ידי התבוננות במסכים שונים של הגדרות Windows בהתקני המשתמשים. מכיוון שהמשתמשים לא יוכלו לשנות את הגדרות windows Update ו-Windows Defender Antivirus בהתקני Windows 10 שלהם, הרבה אפשרויות אלה יהיה מאפיר.
  
1. עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **של Windows עדכון** \> **אפשרויות הפעלה** ולוודא כי כל ההגדרות מאפיר. 
    
    ![כל האפשרויות הפעלה מחדש מאפיר.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. עבור אל **הגדרות** \> ** &amp; עדכון אבטחה** \> **Windows עדכן** \> **אפשרויות מתקדמות** ולאשר כי כל ההגדרות מאפיר. 
    
    ![אפשרויות העדכונים המתקדמים של Windows כולן החוצה.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. עבור אל **הגדרות** \> ** &amp; עדכון אבטחה** \> **של Windows update** \> **אפשרויות** \> **מתקדמות בחר את אופן המשלוח של עדכונים**.
    
    ודא שאתה יכול לראות את ההודעה (באדום) שההגדרות מסוימות מוסתרות או מנוהלות על-ידי הארגון שלך, וכל האפשרויות מאפיר.
    
    ![בחר כיצד עדכונים מועברים לדף מציין שההגדרות מוסתרות או מנוהלות על-ידי הארגון שלך.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. כדי לפתוח את מרכז האבטחה של Windows defender, עבור אל **הגדרות** \> ** &amp; עדכון אבטחה** \> **windows defender** \> לחץ על **פתח windows Defender אבטחה מרכז** \> **וירוס &amp; הליך משנה הגנת** \> **וירוס &amp; איום הגדרות הגנה**. 
    
5. ודא שכל האפשרויות מאפיר. 
    
    ![הגדרות הגנת הוירוס והאיום מאפיר.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>נושאים קרובים

[תיעוד ומשאבים עבור Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[תחילת העבודה עם Microsoft 365 Business](microsoft-365-business-overview.md)
  
[ניהול של Microsoft 365 Business](manage.md)
  
[קביעת תצורות של מכשירים עבור מחשבי Windows 10](protection-settings-for-windows-10-pcs.md)
  

