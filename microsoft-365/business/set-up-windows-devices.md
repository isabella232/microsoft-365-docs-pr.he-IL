---
title: הגדרת מכשירי Windows עבור משתמשי Microsoft 365 Business Premium
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
description: למד כיצד להגדיר מכשירי Windows שבהם פועל Windows 10 Pro עבור משתמשי Microsoft 365 Business Premium, המאפשרים ניהול מרכזי ופקדי אבטחה.
ms.openlocfilehash: c95b9e51c7ec3c440509fe34084d2a030c7f2eec
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841258"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>הגדרת מכשירי Windows עבור משתמשי Microsoft 365 Business Premium

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a>דרישות מוקדמות להגדרת מכשירי Windows עבור משתמשי Microsoft 365 Business Premium

לפני שתוכל להגדיר מכשירי Windows עבור משתמשי Microsoft 365 Business Premium, ודא שכל מכשירי Windows פועלים באמצעות Windows 10 Pro, גירסה 1703 (עדכון יוצרים). Windows 10 Pro הוא תנאי מימוש מיותר לפריסה של Windows 10 Business, שהוא ערכה של יכולות ניהול ושירותי ענן וניהול מכשירים המשלימים את Windows 10 Pro ומאפשרים את פקדי הניהול והאבטחה המרוכזים של Microsoft 365 Business Premium.
  
אם יש לך מכשירי Windows שבהם פועל Windows 7 pro, Windows 8 Pro או Windows 8.1 Pro, מנוי Microsoft 365 Business Premium שברשותך זכאי לשדרוג של Windows 10.
  
לקבלת מידע נוסף על שדרוג מכשירי Windows לעדכון Windows 10 ליוצרים, פעל לפי השלבים בנושא זה: [שדרוג מכשירי Windows לעדכון Windows Pro ליוצרים](upgrade-to-windows-pro-creators-update.md).
  
ראה [אימות שההתקן מחובר ל-תכלת AD](#verify-the-device-is-connected-to-azure-ad) כדי לאמת את השדרוג, או כדי לוודא שהשדרוג עבד.

צפה בסרטון וידאו קצר אודות חיבור Windows ל-Microsoft 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

אם סרטון וידאו זה היה שימושי עבורך, עיין ב[סדרת ההדרכה המלאה עבור עסקים קטנים ומשתמשים חדשים ב- Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>צירוף מכשירי Windows 10 ל- Azure AD של הארגון שלך

כאשר כל מכשירי Windows בארגון שלך שודרגו ל-Windows 10 Pro Creators Update או שכבר מופעלים עדכון Windows 10 של יוצרי Pro, באפשרותך להצטרף למכשירים אלה אל מדריך הכתובות הפעיל של הארגון שלך ב-תכלת. לאחר הצטרפות המכשירים, הם ישודרגו באופן אוטומטי ל-Windows 10 Business, שהוא חלק ממנוי Microsoft 365 Business Premium.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>עבור מכשיר Windows 10 Pro חדש לגמרי או ששודרג לאחרונה

עבור מכשיר חדש לגמרי שעדכון Windows 10 Pro ליוצרים פועל בו, או עבור מכשיר ששודרג לעדכון Windows 10 Pro ליוצרים אך לא הוגדר ל- Windows 10, בצע את השלבים הבאים.
  
1. עבור על פרטי ההגדרה של מכשיר Windows 10 עד שתגיע לעמוד **כיצד ברצונך להגדיר?**. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. כאן, בחר **הגדר עבור ארגון** ולאחר מכן הזן את שם המשתמש והסיסמה שלך עבור Microsoft 365 Business Premium. 
    
3. סיים את הגדרת מכשיר Windows 10.
    
   כשתסיים, המשתמש יהיה מחובר ל- Azure AD של הארגון שלך. ראה [אימות שהמכשיר מחובר ל- Azure AD](#verify-the-device-is-connected-to-azure-ad) כדי לוודא. 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>עבור מכשיר שכבר מוגדר וש- Windows 10 Pro פועל בו

 **חיבור משתמשים ל- Azure AD:**
  
1. במחשב ה- Windows של המשתמש שלך, שפועל בו Windows 10 Pro, גירסה 1703 (עדכון ליוצרים) (ראה [דרישות מוקדמות](pre-requisites-for-data-protection.md)), לחץ על סמל Windows ולאחר מכן על סמל 'הגדרות'.
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. ב **הגדרות** , עבור אל **חשבונות**.
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. בדף **המידע שלך** , לחץ על **גישה לחשבון עבודה או בית ספר** \> **התחבר**.
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. בתיבת הדו-שיח **הגדר חשבון בעבודה או בבית ספר** , תחת **פעולות חלופיות** , בחר **צרף מכשיר זה ל- Azure Active Directory**.
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. בדף **בוא נבצע את תהליך הכניסה** , הזן את החשבון שלך בעבודה או בבית הספר \> **הבא**.
  
   בדף **הזנת סיסמה** , הזן את הסיסמה שלך \> **כניסה**.
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. בדף **ודא שזה הארגון שלך** , ודא שהמידע נכון ובחר **הצטרף**.
  
   בכרטיסיה **הכל מוכן!** דף, chosse **בוצעה**.
  
   ![במסך ודא שזהו המסך של הארגון שלך, בחר הצטרף](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
אם העלית קבצים אל OneDrive for Business, סנכרן אותם בחזרה. אם השתמשת בכלי של ספק חיצוני כדי להעביר פרופילים וקבצים, סנכרן אותם גם לפרופיל החדש.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>אימות שהמכשיר מחובר ל- Azure AD

כדי לאמת את מצב הסינכרון, בדף ' **הגדרות** **בעבודה או בבית הספר של Access** ' בהגדרות, בחר את האזור ' **מחובר עד** _ \<organization name\> _ ' כדי לחשוף את **פרטי** הלחצנים ולהתנתק. **Disconnect** בחר **מידע** כדי לקבל את מצב הסינכרון. 
  
בדף ' **מצב סינכרון** ', בחר באפשרות **סנכרן** כדי לקבל את מדיניות ניהול המכשירים הניידים העדכניים ביותר במחשב.
  
כדי להתחיל להשתמש בחשבון Microsoft 365 Business Premium, עבור אל לחצן ' **התחל** ' של Windows, לחץ באמצעות לחצן העכבר הימני על תמונת החשבון הנוכחית שלך ולאחר מכן **החלף חשבון**. היכנס באמצעות הדואר האלקטרוני והסיסמה של הארגון שלך.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a>אימות שהמחשב משודרג ל-Windows 10 Business

ודא שמכשירי windows 10 שהצטרפו למודעת ה-תכלת שודרגו ל-Windows 10 Business כחלק ממנוי Microsoft 365 Business Premium.
  
1. עבור אל **הגדרות** \> **מערכת** \> **אודות**.
    
2. ודא שתחת **מהדורה** מופיע **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>השלבים הבאים

כדי להגדיר את המכשירים הניידים שלך, ראה [הגדרת מכשירים ניידים עבור משתמשי Microsoft 365 Business Premium](set-up-mobile-devices.md), כדי להגדיר מדיניות הגנה על מכשירים או מדיניות הגנה של יישומים, ראה [ניהול microsoft 365 for Business](manage.md).
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a>לקבלת מידע נוסף אודות הגדרה ושימוש ב-Microsoft 365 Business Premium

[סרטוני וידאו של הדרכה של Microsoft 365 for business](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
