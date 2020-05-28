---
title: הגדרת התקני Windows עבור משתמשי Microsoft Business Premium 365
f1.keywords:
- CSH
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
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: למד כיצד להגדיר התקני Windows שבהם פועל Windows 10 Pro עבור משתמשי Microsoft Business Premium 365, המאפשרים ניהול מרוכז ובקרת אבטחה.
ms.openlocfilehash: ecd9f5aa348d29d34e77061657619c015b09c41a
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44402957"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>הגדרת התקני Windows עבור משתמשי Microsoft Business Premium 365

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a>דרישות מוקדמות להתקנת התקני Windows עבור משתמשי פרימיום של Microsoft 365

לפני שתוכל להגדיר התקני Windows עבור Microsoft 365 Business Premium משתמשים, ודא שכל ההתקנים של Windows פועלים ב-Windows 10 Pro, גירסה 1703 (יוצרי עדכונים). Windows 10 Pro הוא תנאי מוקדם לפריסת Windows 10 Business, שהיא קבוצה של שירותי ענן ויכולות ניהול התקנים המשלימים את Windows 10 Pro ולאפשר בקרת ניהול ואבטחה מרוכזת של Microsoft 365 Business Premium.
  
אם ברשותך התקני Windows הפועלים באמצעות Windows 7 Pro, Windows 8 Pro או Windows 8.1 Pro, מנוי הפרמיה של 365 Microsoft Business Premium מקנה לך את שדרוג Windows 10.
  
לקבלת מידע נוסף על שדרוג מכשירי Windows לעדכון Windows 10 ליוצרים, פעל לפי השלבים בנושא זה: [שדרוג מכשירי Windows לעדכון Windows Pro ליוצרים](upgrade-to-windows-pro-creators-update.md).
  
ראה [אימות ההתקן מחובר לתכלת AD](#verify-the-device-is-connected-to-azure-ad) כדי לוודא שיש לך את השדרוג, או כדי לוודא שהשדרוג עבד.

צפה בסרטון וידאו קצר אודות חיבור Windows ל-Microsoft 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

אם סרטון וידאו זה היה שימושי עבורך, עיין ב[סדרת ההדרכה המלאה עבור עסקים קטנים ומשתמשים חדשים ב- Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>צירוף מכשירי Windows 10 ל- Azure AD של הארגון שלך

כאשר כל התקני Windows בארגון שלך שודרגו ל-Windows 10 Pro יוצרי עדכון או שכבר פועל Windows 10 Pro יוצרי עדכון, אתה יכול להצטרף התקנים אלה לתוך הארגון שלך הפעיל הספריה. לאחר הצירוף של המכשירים, הם ישודרגו באופן אוטומטי ל-Windows 10 Business, המהווה חלק מהמנוי שלך ל-Microsoft Business Premium 365.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>עבור מכשיר Windows 10 Pro חדש לגמרי או ששודרג לאחרונה

עבור מכשיר חדש לגמרי שעדכון Windows 10 Pro ליוצרים פועל בו, או עבור מכשיר ששודרג לעדכון Windows 10 Pro ליוצרים אך לא הוגדר ל- Windows 10, בצע את השלבים הבאים.
  
1. עבור על פרטי ההגדרה של מכשיר Windows 10 עד שתגיע לעמוד **כיצד ברצונך להגדיר?**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. כאן, בחר **בהגדרה עבור ארגון** ולאחר מכן הזן את שם המשתמש והסיסמה שלך עבור Microsoft 365 Business Premium. 
    
3. סיים את הגדרת מכשיר Windows 10.
    
   כשתסיים, המשתמש יהיה מחובר ל- Azure AD של הארגון שלך. ראה [אימות שהמכשיר מחובר ל- Azure AD](#verify-the-device-is-connected-to-azure-ad) כדי לוודא. 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>עבור מכשיר שכבר מוגדר וש- Windows 10 Pro פועל בו

 **חיבור משתמשים ל- Azure AD:**
  
1. במחשב ה- Windows של המשתמש שלך, שפועל בו Windows 10 Pro, גירסה 1703 (עדכון ליוצרים) (ראה [דרישות מוקדמות](pre-requisites-for-data-protection.md)), לחץ על סמל Windows ולאחר מכן על סמל 'הגדרות'.
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. ב **הגדרות**, עבור אל **חשבונות**.
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. בדף **המידע שלך**, לחץ על **גישה לחשבון עבודה או בית ספר** \> **התחבר**.
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. בתיבת הדו-שיח **הגדר חשבון בעבודה או בבית ספר**, תחת **פעולות חלופיות**, בחר **צרף מכשיר זה ל- Azure Active Directory**.
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. בדף **בוא נבצע את תהליך הכניסה**, הזן את החשבון שלך בעבודה או בבית הספר \> **הבא**.
  
   בדף **הזנת סיסמה**, הזן את הסיסמה שלך \> **כניסה**.
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. ב-ודא שזהו דף **הארגון שלך** , ודא שהמידע נכון ולחץ על **הצטרף**.
  
   בדף **הכל מוכן!**, לחץ על **סיום**.
  
   ![On the Make sure this is your organization screen, click Join](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
אם העלית קבצים אל OneDrive for Business, סנכרן אותם בחזרה. אם השתמשת בכלי של ספק חיצוני כדי להעביר פרופיל וקבצים, סנכרן גם אותם לפרופיל החדש.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>אימות שהמכשיר מחובר ל- Azure AD

כדי לאמת את מצב הסינכרון, בדף **עבודה או בית ספר** **בהגדרות**של Access, לחץ באזור **המחובר אל** _ \<organization name\> _ כדי לחשוף את **פרטי** הלחצנים **והתנתק**. לחץ על **מידע** כדי לקבל את מצב הסינכרון. 
  
בדף 'מצב סינכרון', לחץ על 'סינכרון' כדי לקבל את פריטי מדיניות הניהול העדכניים ביותר של המכשיר הנייד במחשב ה- PC.
  
כדי להתחיל להשתמש בחשבון הפרמיה של Microsoft 365 Business, עבור אל לחצן **התחל** של Windows, לחץ לחיצה ימנית על תמונת החשבון הנוכחית שלך ולאחר מכן **החלף חשבון**. היכנס באמצעות הדואר האלקטרוני והסיסמה של הארגון שלך.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a>אימות שהמכשיר משודרג ל- Windows 10 Business

ודא שה "שלך הצטרף ל-Windows 10 התקנים שודרגו ל-Windows 10 Business כחלק מהמנוי שלך ל-Microsoft Business Premium 365.
  
1. עבור אל **הגדרות** \> **מערכת** \> **אודות**.
    
2. ודא שתחת **מהדורה** מופיע **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>השלבים הבאים

כדי להגדיר את המכשירים הניידים שלך, ראה [הגדרת התקנים ניידים עבור משתמשי Microsoft Business Premium 365](set-up-mobile-devices.md), כדי להגדיר מדיניות הגנת התקנים או הגנה על יישומים, ראה [ניהול Microsoft 365 לעסקים](manage.md).
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a>לקבלת פרטים נוספים על הגדרה ושימוש ב-Microsoft 365 Business Premium

[מיקרוסופט 365 עבור סרטוני הדרכה עסקית](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
