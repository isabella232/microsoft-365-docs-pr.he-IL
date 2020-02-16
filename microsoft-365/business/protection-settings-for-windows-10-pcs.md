---
title: קביעת הגדרות הגנה על מכשירים עבור מחשבי PC של Windows 10
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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: למד אודות ברירת המחדל והגדרות אחרות הזמינות ב-Microsoft 365 Business כדי לאבטח התקני Windows 10.
ms.openlocfilehash: 1b424fe6a85ad23b2914ea29f47d1dc16b333c94
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42064962"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a>קביעת הגדרות הגנה על מכשירים עבור מחשבי PC של Windows 10

## <a name="secure-windows-10-devices"></a>אבטחת מכשירים של Windows 10

צפה בסרטון וידאו המסביר כיצד לאבטח מכשירי Windows 10 עם Microsoft 365 Business:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. לך למרכז המנהלה 
    
2. בניווט השמאלי, בחר באפשרות **מדיניות** \> **** **התקנים** \> .
  
3. בחלונית **הוסף מדיניות**, הזן שם ייחודי עבור מדיניות זו. 
    
4. תחת **סוג מדיניות**, בחר **תצורת מכשיר Windows 10**.
    
5. הרחב את **אבטחת מכשירי 10 Windows** \> קבע את תצורת ההגדרות כפי שאתה רוצה. לקבלת מידע נוסף, ראה [הגדרות זמינות](#available-settings). 
    
    ניתן להשתמש תמיד בקישור **איפוס הגדרות ברירת מחדל** כדי לחזור להגדרת ברירת המחדל. 
    
    ![Add policy pane with Windows 10 Device configuration selected](../media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. לאחר מכן החלט **מי יקבל הגדרות אלה?** אם אינך מעוניין להשתמש בקבוצת האבטחה המוגדרת כברירת מחדל **כל המשתמשים**, בחר **שינוי**, חפש את קבוצת האבטחה שתקבל הגדרות אלה \> **בחר**.
    
7. לבסוף, בחר **סיום** כדי לשמור את המדיניות והקצה אותה למכשירים. 
    
## <a name="available-settings"></a>הגדרות זמינות

כברירת מחדל כל ההגדרות מוגדרות ל **פעיל**. ההגדרות הבאות זמינות.
  
לקבלת מידע נוסף, ראה [כיצד תכונות ההגנה של Microsoft 365 Business ממפות להגדרות Intune](map-protection-features-to-intune-settings.md). 
  
|||
|:-----|:-----|
|הגדרה  <br/> |תיאור  <br/> |
|עזור בהגנה על מחשבים מפני וירוסים ואיומים אחרים באמצעות האנטי-וירוס של Windows Defender  <br/> |דרושה הפעלה של האנטי-וירוס של Windows Defender כדי להגן על מחשבים מהסכנות הכרוכות בחיבור לאינטרנט.  <br/> |
|עזור בהגנה על מחשבים מפני איומים מבוססי-אינטרנט ב- Microsoft Edge  <br/> |הפעלת הגדרות ב- Microsoft Edge שעוזרות בהגנה על המשתמשים מפני אתרים זדוניים והורדות.  <br/> |
|שימוש בכללים המקטינים את שטח התקיפה של מכשירים  <br/> |כאשר צמצום שטח התקיפה מופעל, הוא עוזר בחסימת פעולות ויישומים המשמשים בדרך כלל תוכניות זדוניות כדי לזהם מכשירים. הגדרה זו זמינה רק אם אנטי-וירוס של Windows Defender מופעל. ראה [צמצום שטחי תקיפה](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/exploit-protection) כדי לקבל מידע נוסף.  <br/> |
|הגנה על תיקיות מפני איומים כגון תוכנת כופר  <br/> |הגדרה זו משתמשת בגישה מבוקרת לתיקיות כדי להגן על נתוני החברה מפני שינויים על-ידי יישומים חשודים או זדוניים, כגון תוכנות כופר. סוגי יישומים אלה אינם יכולים לבצע שינויים בתיקיות מוגנות. הגדרה זו זמינה רק אם אנטי-וירוס של Windows Defender מופעל. ראה [הגנה על תיקיות עם גישת תיקיות מבוקרת](https://docs.microsoft.com/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA) לקבלת מידע נוסף.  <br/> |
|מניעת גישה לרשת של תוכן באינטרנט שעשוי להיות זדוני  <br/> |השתמש בהגדרה זו כדי לחסום חיבורי משתמש יוצאים למיקומי אינטרנט בעלי מוניטין נמוך, העשויים לארח הונאות דיוג, מימוש לניצול או תוכן זדוני אחר. הגדרה זו זמינה רק אם Windows Defender Antivirus מוגדר **כפעיל**. לקבלת מידע נוסף, ראה [הגנה על הרשת שלך](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus).  <br/> |
|עזור להגן על קבצים ותיקיות במחשבים מפני גישה לא מורשית באמצעות BitLocker  <br/> |Bitlocker מגן על נתונים על-ידי הצפנת הכוננים הקשיחים של המחשב ומגן מפני חשיפת נתונים אם מחבר אבד או נגנב. לקבלת מידע נוסף, ראה [שאלות נפוצות](https://go.microsoft.com/fwlink/?linkid=871000)בדבר Bitlocker.  <br/> |
|אפשר למשתמשים להוריד אפליקציות מ- Microsoft Store  <br/> |הגדרה זו מאפשרת למשתמשים להוריד ולהתקין אפליקציות מ- Microsoft Store. אפליקציות כוללות את כל סוגי התוכן, החל ממשחקים וכלה בכלי פרודוקטיביות, לכן אנו משאירים הגדרה זו במצב **מופעל**, אך ניתן לבטל אותה להשגת אבטחה נוספת.  <br/> |
|אפשר למשתמשים לגשת ל- Cortana  <br/> |Cortana יכולה להיות שימושית מאוד! Cortana יכול להפעיל או לבטל הגדרות עבורך, לתת הוראות, ולוודא שאתה בזמן לפגישות, אז אנחנו שומרים על הגדרה זו על כברירת **מחדל** .  <br/> |
|אפשר למשתמשים לקבל עצות ופרסומות בנושא Windows מ- Microsoft  <br/> |העצות של Windows יכולות להיות שימושיות ולעזור למשתמשים להתמצא בעת הפצת התכונות החדשות.  <br/> |
|עדכן מכשירים של Windows 10 באופן אוטומטי  <br/> |הגדרה זו מוודאת שמכשירי Windows 10 מקבלים באופן אוטומטי את העדכונים האחרונים.  <br/> |
|כבה את מסך המכשיר כשהוא לא פעיל במשך  <br/> |הגדרה זו מוודאת שנתוני החברה מוגנים אם המשתמש אינו פעיל. ייתכן מצב שבו משתמש מסוים עובד במקום ציבורי, למשל בית קפה, שבו הוא מתרחק או שדעתו מוסחת לרגע קט ומשאיר את המכשיר שלו חשוף להצצות אקראיות. הגדרה זו מאפשרת לך לקבוע כמה זמן המשתמש יכול להיות לא פעיל לפני כיבוי המסך.  <br/> |
