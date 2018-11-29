---
title: מתן אפשרות לניהול מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: למד כיצד להפעיל 365 Microsoft להגן על AD המקומי מצורף התקני Windows 10.
ms.openlocfilehash: 6e66a2c5417c9037232c1ada654d4cac3c520607
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982654"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>מתן אפשרות לניהול מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business

אם הארגון שלך משתמש Windows Server Active Directory המקומית, באפשרותך להגדיר עסקיים 365 של Microsoft להגנה על התקני Windows 10 שלך, תוך שמירה עדיין גישה למשאבים המקומית המחייבים אימות מקומי. באפשרותך להגדיר זאת על-ידי סינכרון Active Directory שלך עם תכלת הרקיע Active Directory, ואחריו רישום התקני Windows 10 עם AD תכלת הרקיע לבין רושם אותם עבור ניהול התקנים ניידים על-ידי Microsoft 365 עסקיים.
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>הגדרת התקני לתחום כדי להיות מנוהל על-ידי Microsoft 365 עסקי

כדי להגדיר את התקנים לתחום של הארגון שלך יועיל להם היכולות שמספק תכלת הרקיע Active Directory בנוסף המקומית Active Directory, באפשרותך ליישם **היברידית AD תכלת הרקיע לחבר התקנים**. אלו הם התקנים המצורפים הן מקומיות של Active Directory ולאחר תכלת הרקיע של Active Directory. היברידית AD תכלת הרקיע מצורף יכול להיות מוגן והתקנים מנוהל על-ידי ביקור 365 Microsoft... 
  
השלם את השלבים הבאים כדי להפוך את ההתקנים שלך Windows 10 היברידית AD תכלת הרקיע המצורפים ואת מנוהל על-ידי Microsoft 365 עסקיים.
  
1. כדי לסנכרן שלך משתמשים, קבוצות ואנשי קשר מ- Active Directory המקומי לתוך תכלת הרקיע Active Directory, הפעל את אשף סינכרון הספריות וחבר תכלת הרקיע Active Directory כפי שמתואר [להגדיר סינכרון ספריות עבור Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
    > [!NOTE]
    > השלבים זהים לחלוטין לעסקים 365 של Microsoft. 
  
2. לפני ביצוע שלב 3 כדי לאפשר להתקנים Windows 10 להיות היברידית מצורף AD תכלת הרקיע, עליך לוודא כי אתה עומד בתנאים המוקדמים הבאים:
    
   - אתה מפעיל את הגירסה העדכנית ביותר של AD תכלת הרקיע להתחבר.
    
   - תכלת הרקיע AD לחבר יש לסנכרן את כל האובייקטים המחשב של ההתקנים שברצונך להיות היברידית AD תכלת הרקיע מצורף. אם האובייקטים המחשב שייך ספציפיים יחידות ארגוניות (OU) ולאחר מכן ודא שיחידות ארגוניות אלה מוגדרות עבור סינכרון ב- AD תכלת הרקיע להתחבר גם.
    
3. רישום קיים לתחום Windows 10 התקנים היברידית Joined AD תכלת הרקיע או להירשם אותם עבור ניהול התקנים ניידים על-ידי Intune (Microsoft 365 עסקי):
    
4. בצע את הוראות שלב אחר שלב [כיצד לקבוע תצורה של התקני תכלת הרקיע Active Directory מצורף היברידית](https://go.microsoft.com/fwlink/p/?linkid=872870). פעולה זו תפעיל את הסינכרון של המקומית Active Directory שלך לקבוצת המחשבים של Windows 10 והפוך אותם ענן מוכן.
    
5. כדי להירשם התקן Windows 10 עבור ניהול התקנים ניידים, ראה [הרשמה התקן Windows 10 עם Intune על-ידי שימוש במדיניות קבוצתית](https://go.microsoft.com/fwlink/p/?linkid=872871) לקבלת הוראות. באפשרותך להגדיר את המדיניות הקבוצתית בכל מחשב מקומי ברמה או עבור פעולות בצובר, באפשרותך ליצור הגדרת מדיניות קבוצתית זו בשרת בקר קבוצת המחשבים שלך. 
    

