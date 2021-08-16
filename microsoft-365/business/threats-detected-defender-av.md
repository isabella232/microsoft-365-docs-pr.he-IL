---
title: איומים שזוהו על-ידי אנטי-וירוס של Microsoft Defender
f1.keywords: CSH
ms.author: sharik
author: SKjerland
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- Adm_O365
- Adm_TOC
ms.custom: AdminSurgePortfolio
search.appverid: MET150
description: למד כיצד אנטי-וירוס של Microsoft Defender על מכשירי Windows שלך מפני איומי תוכנה, כגון וירוסים, תוכנות זדוניות ותוכנות ריגול.
ms.openlocfilehash: 79ec44a44c3939a4a868b98d75ab4f24eaf949fcd9bbafb7c0a3173e267f4680
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53896302"
---
# <a name="threats-detected-by-microsoft-defender-antivirus"></a>איומים שזוהו על-ידי אנטי-וירוס של Microsoft Defender

אנטי-וירוס של Microsoft Defender להגן על מכשירי Windows מפני איומי תוכנה, כגון וירוסים, תוכנות זדוניות ותוכנות ריגול.

- וירוסים מתפשטים בדרך כלל על-ידי צירוף הקוד שלהם לקבצים אחרים במכשיר או ברשת שלך ועלולה לגרום לתוכניות נגועות לפעול באופן שגוי.
- תוכנות זדוניות כוללות קבצים זדוניים, יישומים וקוד ה יכולים לגרום נזק ולשבש את השימוש הרגיל במכשירים. כמו כן, תוכנות זדוניות יכולות לאפשר גישה בלתי מורשית, להשתמש במשאבי מערכת, לגנוב סיסמאות ומידע חשבון, לנעול אותך מחוץ למחשב ולדרוש כופר ועוד.
- תוכנות ריגול אוספת נתונים, כגון פעילות גלישה באינטרנט, ושולחת את הנתונים לשרתים מרוחקים.
 
כדי לספק הגנה מפני איומים, אנטי-וירוס של Microsoft Defender בכמה שיטות. שיטות אלה כוללות הגנה מועברת בענן, הגנה בזמן אמת ועדכונים ייעודיים להגנה.

- הגנה מועברת בענן עוזרת לספק זיהוי וחסימה של איומים חדשים ומתעוררים.
- סריקה תמידית משתמשת בניטור קבצים ותהליכים-התנהגות ובטכניקות אחרות (המכונה גם *הגנה בזמן אמת).*
- עדכוני הגנה ייעודיים מבוססים על למידת מכונה, ניתוח נתונים גדולים אנושיים ואוטומטיים ומחקר מעמיק של התנגדות לאיום. 

לקבלת מידע נוסף על תוכנות זדוניות אנטי-וירוס של Microsoft Defender, עיין במאמרים הבאים: 

- [הבנת תוכנות זדוניות & איומים אחרים](/windows/security/threat-protection/intelligence/understanding-malware)
- [כיצד Microsoft מזהה תוכנות זדוניות ויישומים שעשויים להיות לא רצויים](/windows/security/threat-protection/intelligence/criteria)
- [הגנה מהדור הבא ב- Windows 10](/windows/security/threat-protection/microsoft-defender-antivirus/microsoft-defender-antivirus-in-windows-10)

## <a name="what-happens-when-a-non-microsoft-antivirus-solution-is-used"></a>מה קורה כאשר נעשה שימוש בפתרון אנטי-וירוס שאינו של Microsoft? 

אנטי-וירוס של Microsoft Defender היא חלק ממערכת ההפעלה והיא זמינה במכשירים פועלים Windows 10. עם זאת, אם אתה משתמש בפתרון אנטי-וירוס שאינו של Microsoft ואתה לא משתמש ב- [Microsoft Defender עבור נקודת](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-advanced-threat-protection)קצה , אנטי-וירוס של Microsoft Defender עובר באופן אוטומטי למצב לא זמין.  

במצב לא זמין, משתמשים ולקוחות יכולים עדיין להשתמש אנטי-וירוס של Microsoft Defender לסריקות מתוזמנות או לפי דרישה כדי לזהות איומים; עם זאת, אנטי-וירוס של Microsoft Defender לא תהיה עוד:

- יש להשתמש בו כיישום האנטי-וירוס המהווה ברירת מחדל.
- סרוק קבצים באופן פעיל כדי לסרוק איומים.
- תיקון, או פתרון, איומים.

אם תסיר את התקנת פתרון האנטי-וירוס שאינו Microsoft, אנטי-וירוס של Microsoft Defender באופן אוטומטי למצב פעיל כדי להגן על Windows שלך מפני איומים.

> [!TIP]
> - אם אתה משתמש ב- Microsoft 365, שקול להשתמש אנטי-וירוס של Microsoft Defender כפתרון האנטי-וירוס הראשי שלך. שילוב יכול לספק הגנה טובה יותר. ראה [טוב יותר יחד: אנטי-וירוס של Microsoft Defender ו- Office 365.](/windows/security/threat-protection/microsoft-defender-antivirus/office-365-microsoft-defender-antivirus)
> - הקפד לתכנת אנטי-וירוס של Microsoft Defender, גם אם אתה משתמש בפתרון אנטי-וירוס שאינו של Microsoft.

## <a name="what-to-expect-when-threats-are-detected"></a>למה לצפות כאשר איומים מזוהים

כאשר איומים מזוהים על-ידי אנטי-וירוס של Microsoft Defender, הדברים הבאים מתרחשים:

- משתמשים מקבלים [הודעות ב- Windows.](https://support.microsoft.com/windows/8942c744-6198-fe56-4639-34320cf9444e) 
- זיהויים מפורטים באפליקציית [אבטחת Windows בדף](/windows/security/threat-protection/windows-defender-security-center/windows-defender-security-center) **'היסטוריית הגנה'.**  
- אם אבטחת את מכשירי [Windows 10](secure-win-10-pcs.md) שלך ונרשמת אותם ב- [Intune](/mem/intune/enrollment/windows-enrollment-methods), והארגון שלך כולל 800 מכשירים או פחות, תראה זיהויי איומים ותובנות ב- <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">מרכז הניהול של Microsoft 365 בדף</a> איומים  ואנטי-וירוס, שאותן תוכל **לגשת מכרטיס אנטי-וירוס של Microsoft Defender בדף** הבית (או מתוך חלונית הניווט על-ידי בחירת איומים תקינות &    >  **אנטי-וירוס).**

    אם הארגון שלך כולל יותר מ- 800 מכשירים שנרשמו ל- Intune, תתבקש להציג זיהויי איומים [ותובנות מ- Microsoft Endpoint Manager](/mem/endpoint-manager-overview) במקום מהדף **'איומים' ו'אנטי-וירוס'.**
 
    > [!NOTE]
    > הכרטיס **אנטי-וירוס של Microsoft Defender** והדף **'איומים'** ו'אנטי-וירוס' מגולגלים בשלבים, ולכן ייתכן שלא תוכל לגשת אליהם באופן מיידי.

ברוב המקרים, משתמשים אינם צריכים לבצע פעולות נוספות. ברגע שקובץ או תוכנית זדוניים מזוהים במכשיר, אנטי-וירוס של Microsoft Defender אותו ומונע ממנו לפעול. בנוסף, איומים שזוהו לאחרונה מתווספים למנוע האנטי-וירוס והאנטי-תוכנות זדוניות כך שהתקנים ומשתמשים אחרים מוגנים גם הם.  

אם יש פעולה שמשתמש צריך לבצע, כגון אישור הסרה של קובץ זדוני, הוא יראה זאת בהודעה שהוא מקבל. כדי ללמוד עוד אודות פעולות אנטי-וירוס של Microsoft Defender משתמש, או פעולות שמשתמשים עשויים לבצע, ראה [היסטוריית הגנה](https://support.microsoft.com/office/f1e5fd95-09b4-46d1-b8c7-1059a1e09708). כדי ללמוד כיצד לנהל זיהויי איומים בתור מומחי IT/מנהל מערכת, ראה [סקירת איומים שזוהו ופעולה.](review-threats-take-action.md)

כדי ללמוד עוד אודות איומים שונים, <a href="https://www.microsoft.com/wdsi/threats" target="_blank">בקר באתר בינת אבטחה של Microsoft איומים</a>, שבו תוכל לבצע את הפעולות הבאות: 

- הצג מידע נוכחי אודות איומים מובילים.
- הצג את האיומים האחרונים עבור אזור ספציפי.
- חפש באנציקלופדיה של האיום פרטים אודות איום ספציפי.

## <a name="related-content"></a>תוכן קשור

[אבטחת Windows 10](secure-windows-10-devices.md) (מאמר)\
[הערכת אנטי-וירוס של Microsoft Defender](/windows/security/threat-protection/microsoft-defender-antivirus/evaluate-microsoft-defender-antivirus) (מאמר)\
[כיצד להפעיל הגנה מפני אנטי-וירוס בזמן אמת ובענן](/mem/intune/user-help/turn-on-defender-windows#turn-on-real-time-and-cloud-delivered-protection) (מאמר)\
[כיצד להפעיל ולהשתמש ב- אנטי-וירוס של Microsoft Defender מתוך אבטחת Windows](/windows/security/threat-protection/microsoft-defender-antivirus/microsoft-defender-security-center-antivirus) (מאמר)\
[כיצד להפעיל את אנטי-וירוס של Microsoft Defender באמצעות מדיניות קבוצתית](/mem/intune/user-help/turn-on-defender-windows#turn-on-windows-defender) (מאמר)\
[כיצד לעדכן את הגדרות האנטי-וירוס](/mem/intune/user-help/turn-on-defender-windows#update-your-antivirus-definitions) (מאמר)\
[כיצד לשלוח תוכנות זדוניות ולא תוכנות זדוניות ל- Microsoft לניתוח](/microsoft-365/security/office-365-security/submitting-malware-and-non-malware-to-microsoft-for-analysis) (מאמר)
