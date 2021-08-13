---
title: עריכה או יצירה של הגדרות הגנה על מכשיר עבור Windows 10 אישיים
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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: למד אודות הגדרות הזמינות ב- Microsoft 365 לעסקים לאבטחת Windows 10 אחרים.
ms.openlocfilehash: b246a0caeb34bac8b9ccbecc9e1008992a700f9e16083a78c98e780605c5af01
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809275"
---
# <a name="edit-or-create-device-protection-settings-for-windows-10-pcs"></a>עריכה או יצירה של הגדרות הגנה על מכשיר עבור Windows 10 אישיים

מאמר זה חל על Microsoft 365 Business Premium.

לאחר הגדרת הגדרות ברירת המחדל Windows הגנה בדף הגדרה, באפשרותך להוסיף הגדרות חדשות החלות על כל המשתמשים או על קבוצת משתמשים. באפשרותך גם לערוך כל אחד מהעורכים שיצרת.

## <a name="create-protection-settings-for-windows-10-devices"></a>יצירת הגדרות הגנה עבור Windows 10 שונים

הצג סרטון וידאו על אבטחת Windows 10 עם Microsoft 365 Business Premium:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. עבור אל מרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> ב- . 
2. בסרגל הניווט הימני, בחר **מדיניות** \> **מכשירים** \> **הוסף**.
3. בחלונית **הוסף מדיניות**, הזן שם ייחודי עבור מדיניות זו. 
4. תחת **סוג מדיניות**, בחר **תצורת מכשיר Windows 10**.
5. הרחב את **אבטחת מכשירי 10 Windows** \> קבע את תצורת ההגדרות כפי שאתה רוצה. לקבלת מידע נוסף, ראה [הגדרות זמינות](#available-settings). 
    
    ניתן להשתמש תמיד בקישור **איפוס הגדרות ברירת מחדל** כדי לחזור להגדרת ברירת המחדל. 
    
    ![Add policy pane with Windows 10 Device configuration selected](../media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. לאחר מכן החלט **מי יקבל הגדרות אלה?** אם אינך מעוניין להשתמש בקבוצת האבטחה המוגדרת כברירת מחדל **כל המשתמשים**, בחר **שינוי**, חפש את קבוצת האבטחה שתקבל הגדרות אלה \> **בחר**.
7. לבסוף, בחר **סיום** כדי לשמור את המדיניות והקצה אותה למכשירים. 

## <a name="edit-windows-10-protection-settings"></a>עריכת Windows 10 הגדרות הגנה
 
1. עבור אל מרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> ב- .     
2. בסרגל הניווט הימני, בחר **מדיניות** \> **מכשירים** .
1. בחר מדיניות Windows קיימת ולאחר מכן **ערוך**.
1. בחר **ערוך** לצד הגדרה שברצונך לשנות ולאחר מכן **שמור**.

## <a name="available-settings"></a>הגדרות זמינות

כברירת מחדל כל ההגדרות מוגדרות ל **פעיל**. ההגדרות הבאות זמינות.
  
לקבלת מידע נוסף, ראה [כיצד ניתן להגן על תכונות Microsoft 365 Premium מפה להגדרות Intune](map-protection-features-to-intune-settings.md). 


|הגדרה  <br/> |תיאור  <br/> |
|:-----|:-----|
|עזור בהגנה על מחשבים מפני וירוסים ואיומים אחרים באמצעות האנטי-וירוס של Windows Defender  <br/> |דרושה הפעלה של האנטי-וירוס של Windows Defender כדי להגן על מחשבים מהסכנות הכרוכות בחיבור לאינטרנט.  <br/> |
|עזור בהגנה על מחשבים מפני איומים מבוססי-אינטרנט ב- Microsoft Edge  <br/> |הפעלת הגדרות ב- Microsoft Edge שעוזרות בהגנה על המשתמשים מפני אתרים זדוניים והורדות.  <br/> |
|שימוש בכללים המקטינים את שטח התקיפה של מכשירים  <br/> |כאשר צמצום שטח התקיפה מופעל, הוא עוזר בחסימת פעולות ויישומים המשמשים בדרך כלל תוכניות זדוניות כדי לזהם מכשירים. הגדרה זו זמינה רק אם אנטי-וירוס של Windows Defender מופעל. ראה [צמצום שטחי תקיפה](/windows/security/threat-protection/microsoft-defender-atp/exploit-protection) כדי לקבל מידע נוסף.  <br/> |
|הגנה על תיקיות מפני איומים כגון תוכנת כופר  <br/> |הגדרה זו משתמשת בגישה מבוקרת לתיקיות כדי להגן על נתוני החברה מפני שינויים על-ידי יישומים חשודים או זדוניים, כגון תוכנות כופר. סוגי יישומים אלה אינם יכולים לבצע שינויים בתיקיות מוגנות. הגדרה זו זמינה רק אם אנטי-וירוס של Windows Defender מופעל. ראה [הגנה על תיקיות עם גישה מבוקרת לתיקיות](/mem/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA) כדי לקבל מידע נוסף.  <br/> |
|מניעת גישה לרשת של תוכן באינטרנט שעשוי להיות זדוני  <br/> |השתמש בהגדרה זו כדי לחסום חיבורי משתמשים יוצאים למיקום אינטרנט בעל מוניטין נמוך, העשויים לארח הונאות דיוג, ניצול לרעה או תוכן זדוני אחר. הגדרה זו זמינה רק אם אנטי-וירוס של Windows Defender מוגדרת **ל- On**. לקבלת מידע נוסף, ראה [הגנה על הרשת שלך.](/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus)  <br/> |
|עזור להגן על קבצים ותיקיות במחשבים מפני גישה לא מורשית באמצעות BitLocker  <br/> |Bitlocker מגן על נתונים על-ידי הצפנת הכוננים הקשיחים של המחשב ומגן מפני חשיפת נתונים אם מחבר אבד או נגנב. לקבלת מידע נוסף, ראה [שאלות נפוצות אודות Bitlocker](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions).  <br/> |
|אפשר למשתמשים להוריד אפליקציות מ- Microsoft Store  <br/> |הגדרה זו מאפשרת למשתמשים להוריד ולהתקין אפליקציות מ- Microsoft Store. אפליקציות כוללות את כל סוגי התוכן, החל ממשחקים וכלה בכלי פרודוקטיביות, לכן אנו משאירים הגדרה זו במצב **מופעל**, אך ניתן לבטל אותה להשגת אבטחה נוספת.  <br/> |
|אפשר למשתמשים לגשת ל- Cortana  <br/> |Cortana יכולה להיות שימושית מאוד! Cortana להפעיל או לבטל הגדרות כברירת מחדל, לתת הוראות הגעה, לוודא שאתה נמצא בזמן לפעילויות, לכן אנו שומרים על הגדרה זו כברירת מחדל.   <br/> |
|אפשר למשתמשים לקבל עצות ופרסומות בנושא Windows מ- Microsoft  <br/> |העצות של Windows יכולות להיות שימושיות ולעזור למשתמשים להתמצא בעת הפצת התכונות החדשות.  <br/> |
|עדכן מכשירים של Windows 10 באופן אוטומטי  <br/> |הגדרה זו מוודאת שמכשירי Windows 10 מקבלים באופן אוטומטי את העדכונים האחרונים.  <br/> |
|כבה את מסך המכשיר כשהוא לא פעיל במשך  <br/> |הגדרה זו מוודאת שנתוני החברה מוגנים אם המשתמש אינו פעיל. ייתכן מצב שבו משתמש מסוים עובד במקום ציבורי, למשל בית קפה, שבו הוא מתרחק או שדעתו מוסחת לרגע קט ומשאיר את המכשיר שלו חשוף להצצות אקראיות. הגדרה זו מאפשרת לך לקבוע כמה זמן המשתמש יכול להיות לא פעיל לפני כיבוי המסך.  <br/> |