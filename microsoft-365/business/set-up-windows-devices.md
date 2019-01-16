---
title: הגדרת מכשירי Windows עבור משתמשים של Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: 'למד כיצד להגדיר התקני Windows פועל Windows 10 Pro עבור משתמשים עסקיים 365 של Microsoft. '
ms.openlocfilehash: 482199b175c568bfae420619aa02024303894789
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982854"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a>הגדרת מכשירי Windows עבור משתמשים של Microsoft 365 Business

## <a name="prerequisites"></a>דרישות מוקדמות

לפני שתוכל להגדיר מכשירי Windows עבור משתמשי Microsoft 365 Business, ודא שבכל מכשירי Windows פועלת מהדורה 1703 של Windows 10 Pro (העדכון ליוצרים). Windows 10 Pro מהווה דרישה מוקדמת לפריסת Windows 10 Business, שהוא קבוצה של שירותי ענן ויכולות ניהול מכשירים שמשלימות את Windows 10 Pro ומאפשרות את ההפעלה של הניהול המרכזי ובקרות האבטחה של Microsoft 365 Business.
  
אם יש לך מכשיר Windows עם Windows 7 Pro, ‏Windows 8 Pro או Windows 8.1 Pro, מנוי Microsoft 365 Business שלך מזכה אותך בשדרוג ל- Windows 10.
  
לקבלת מידע נוסף על שדרוג מכשירי Windows לעדכון Windows 10 ליוצרים, פעל לפי השלבים בנושא זה: [שדרוג מכשירי Windows לעדכון Windows Pro ליוצרים](upgrade-to-windows-pro-creators-update.md).
  
ראה [אימות שהמכשיר משודרג ל- Windows 10 Business](set-up-windows-devices.md#bkmk_verifywin10) כדי לאמת שביצעת את השדרוג, או כדי לוודא שהשדרוג עבד. 
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>צירוף מכשירי Windows 10 ל- Azure AD של הארגון שלך

לאחר השדרוג של כל מכשירי Windows בארגון לעדכון Windows 10 Pro ליוצרים, או אם המכשירים כבר פועלים עם עדכון Windows 10 Pro ליוצרים, ניתן לצרף מכשירים אלה ל- Azure Active Directory של הארגון. לאחר צירוף המכשירים, הם ישודרגו באופן אוטומטי ל- Windows 10 Business, המהווה חלק ממנוי Microsoft 365 Business.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>עבור מכשיר Windows 10 Pro חדש לגמרי או ששודרג לאחרונה

עבור מכשיר חדש לגמרי שעדכון Windows 10 Pro ליוצרים פועל בו, או עבור מכשיר ששודרג לעדכון Windows 10 Pro ליוצרים אך לא הוגדר ל- Windows 10, בצע את השלבים הבאים.
  
1. עבור על פרטי ההגדרה של מכשיר Windows 10 עד שתגיע לעמוד **כיצד ברצונך להגדיר?**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. כאן, בחר **הגדרה עבור ארגון** ולאחר מכן הזן את שם המשתמש והסיסמה שלך עבור Microsoft 365 Business. 
    
3. סיים את הגדרת מכשיר Windows 10.
    
   כשתסיים, המשתמש יהיה מחובר ל- Azure AD של הארגון שלך. ראה [אימות שהמכשיר מחובר ל- Azure AD](set-up-windows-devices.md#bkmk_verifyaad) כדי לוודא. 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>עבור מכשיר שכבר מוגדר וש- Windows 10 Pro פועל בו

 **חיבור משתמשים ל- Azure AD:**
  
1. במחשב ה- Windows של המשתמש שלך, שפועל בו Windows 10 Pro, גירסה 1703 (עדכון ליוצרים) (ראה [דרישות מוקדמות](pre-requisites-for-data-protection.md)), לחץ על סמל Windows ולאחר מכן על סמל 'הגדרות'.
  
   ![In the Start menu, click Windows Settings icon](media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. ב **הגדרות**, עבור אל **חשבונות**.
  
   ![In Windows Settings, go to Accounts](media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. בדף **המידע שלך**, לחץ על **גישה לחשבון עבודה או בית ספר** \> **התחבר**.
  
   ![Choose Connect under Access work or school](media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. בתיבת הדו-שיח **הגדר חשבון בעבודה או בבית ספר**, תחת **פעולות חלופיות**, בחר **צרף מכשיר זה ל- Azure Active Directory**.
  
   ![Click Join this device to Azure Active Directory](media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. בדף **בוא נבצע את תהליך הכניסה**, הזן את החשבון שלך בעבודה או בבית הספר \> **הבא**.
  
   בדף **הזנת סיסמה**, הזן את הסיסמה שלך \> **כניסה**.
  
   ![Enter your work or school email on the Let's get you signed in page](media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. על ה * * ודא כי זהו הארגון שלך * * עמוד, ודא שהמידע נכון ולאחר מכן לחץ על **הצטרף**.
  
   בדף **הכל מוכן!**, לחץ על **סיום**.
  
   ![On the Make sure this is your organization screen, click Join](media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
אם העלית קבצים אל OneDrive for Business, סנכרן אותם בחזרה. אם השתמשת בכלי של ספק חיצוני להעברת פרופיל וקבצים, סנכרן אותם עם הפרופיל החדש.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>אימות שהמכשיר מחובר ל- Azure AD

כדי לאמת את מצב הסינכרון שלך, בדף **גישה לחשבון עבודה או בית ספר** ב **הגדרות**, לחץ באזור **מחובר ל** _ \<organization name\> _ כדי לחשוף את הלחצנים **מידע** ו **התנתק**. לחץ על **מידע** כדי לקבל את מצב הסינכרון. 
  
בדף 'מצב סינכרון', לחץ על 'סינכרון' כדי לקבל את פריטי מדיניות הניהול העדכניים ביותר של המכשיר הנייד במחשב ה- PC.
  
כדי להתחיל להשתמש בחשבון Microsoft 365 Business, עבור אל לחצן **התחל** של Windows, לחץ באמצעות לחצן העכבר הימני על תמונת החשבון הנוכחי שלך ולאחר מכן **החלף חשבון**. היכנס באמצעות הדואר האלקטרוני והסיסמה של הארגון שלך.
  
![Click Info button to view synchronization status](media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a>אימות שהמכשיר משודרג ל- Windows 10 Business

ודא שמכשירי Windows 10 שהצטרפו ל- Azure AD שודרגו ל- Windows 10 Business כחלק מהמנוי ל- Microsoft 365 Business.
  
1. עבור אל **הגדרות** \> **מערכת** \> **אודות**.
    
2. ודא שתחת **מהדורה** מופיע **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>השלבים הבאים

כדי להגדיר את המכשירים הניידים שלך, ראה [הגדרת מכשירים ניידים עבור משתמשי Microsoft 365 Business](set-up-mobile-devices.md). כדי להגדיר כללי מדיניות הגנה למכשירים או ליישומים, ראה [ניהול Microsoft 365 Business](manage.md).
  