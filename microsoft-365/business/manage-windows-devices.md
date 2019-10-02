---
title: מתן אפשרות לניהול מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: למד כיצד לאפשר ל-Microsoft 365 להגן על התקנים המקומיים המצורפים ל-Windows 10.
ms.openlocfilehash: 452e884f952a4b2c2e87148bb7203ed48a48d944
ms.sourcegitcommit: 3a632d8ec009abf1aac57363eaf78aeeda5db136
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376094"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>מתן אפשרות לניהול מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business

אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business כדי להגן על התקני Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים המחייבים אימות מקומי.
כדי להגדיר את זה, אתה יכול ליישם **היברידית תכלת התקנים המצורפים**. אלה הם התקנים המצורפים הן ל-Active Directory המקומי ולספריה הפעילה שלך.

הווידאו הבא מפרט את השלבים עבור אופן ההגדרה עבור התרחיש הנפוץ ביותר המפורט גם בשלבים הבאים.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. היכונו לסנכרון ספריות 

לפני שתסנכרן את המשתמשים והמחשבים שלך מקבוצת המחשבים המקומית של Active Directory, סקור את [ההכנה לסנכרון ספריות ל-Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). בפרט:

   - ודא שאין כפילויות בספריה שלך עבור התכונות הבאות: **דואר**, **כתובות Proxyaddresses שמות** **משתמשים**. על ערכים אלה להיות ייחודיים ולהסיר את כל הכפילויות.
   
   - מומלץ לציין כי התכונה **Userהפריפלשם** (UPN) עבור כל חשבון משתמש מקומי מוגדרת להתאים לכתובת הדואר האלקטרוני הראשית המתאימה למשתמש המורשה של Microsoft 365. לדוגמה *mary.shelley@contoso.com* במקום *מרי @ contoso. מקומי*
   
   - אם קבוצת המחשבים של Active Directory מסתיימת בסיומת שאינה ניתנת לניתוב כגון *. local* או *. lan*, במקום סיומת אינטרנט הניתנת לניתוב כגון *. com* או *. org*, יהיה עליך לכוונן תחילה את סיומת ה-UPN של חשבונות המשתמשים המקומיים כמתואר ב [הכן תחום שאינו ניתן לניתוב עבור סינכרון ספריות](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. התקנה והגדרה של התחברות תכלת

כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מ-Active Directory המקומי לתוך מדריך כחול פעיל, התקן את האפשרות התחבר לספריית המשימות הפעילה והגדר סינכרון ספריות. ראה [הגדרת סינכרון ספריות עבור Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) כדי ללמוד עוד.

> [!NOTE]
> השלבים זהים בדיוק עבור Microsoft 365 Business. 

כאשר אתה מגדיר את האפשרויות שלך עבור תכלת AD התחבר, אנו ממליצים לאפשר **סנכרון סיסמה** **חלקה כניסה יחידה**, כמו גם את התכונה **הסיסמה ככתוב** , אשר נתמך גם ב-Microsoft 365 Business.

> [!NOTE]
> יש כמה שלבים נוספים עבור הסיסמה כתיבה מעבר לתיבת הסימון התחבר תכלת AD. לקבלת מידע נוסף, ראה [כיצד-to: הגדרת התצורה של הסיסמה ככתוב](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. להגדיר היברידית תכלת הצטרפות

לפני שתאפשר ל-Windows 10 להיות מצורף להתקן התכלת ההיברידית לספירה, עליך לוודא שאתה עומד בדרישות המוקדמות הבאות:

   - אתה מפעיל את הגירסה העדכנית ביותר של התחברות התכלת AD.

   - החיבור התכלת לספירה מסנכרן את כל אובייקטי המחשב של המכשירים שברצונך להיות היברידית תכלת לספירה הצטרפו. אם אובייקטי המחשב שייכים ליחידות ארגוניות מסוימות (OU), ודא שאלה אלה מוגדרות לסנכרון בתכלת הספירה גם כן.

כדי לרשום התקן קיים המצורפים ל-Windows 10 התקנים כמו תכלת היברידית לספירה הצטרף, בצע את השלבים [במדריך: קביעת תצורה של היברידית תכלת היברידי להצטרף לתחומים מנוהלים](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). פעולה זו תהפוך היברידית לזמינה הקיימת ב-Active Directory המקומי שלך הצטרף למחשבי Windows 10 ולגרום להם להיות מוכנים לענן.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. אפשר הרשמה אוטומטית ל-Windows 10

 כדי לרשום באופן אוטומטי התקני Windows 10 עבור ניהול התקנים ניידים ב-Intune, ראה [רישום התקן windows 10 באופן אוטומטי באמצעות מדיניות קבוצתית](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). באפשרותך להגדיר את המדיניות הקבוצתית ברמת מחשב מקומית, או עבור פעולות בצובר, באפשרותך ליצור הגדרת מדיניות קבוצתית זו בבקר התחום שלך באמצעות מסוף ניהול המדיניות הקבוצתית ותבניות ADMX.

## <a name="5-configure-seamless-single-sign-on"></a>5. קביעת תצורה של כניסה יחידה חלקה

  ערכת SSO חלקה תחתום באופן אוטומטי על משתמשים במשאבי הענן של Microsoft 365 שלהם בעת השימוש במחשבים ארגוניים. פשוט לפרוס אחת משתי אפשרויות המדיניות הקבוצתית המתוארות [כניסה יחידה של Active Directory בודדת: התחלה מהירה](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). האפשרות **מדיניות קבוצתית** אינה מאפשרת למשתמשים לשנות את הגדרותיו, בעוד שהאפשרות **העדפת מדיניות קבוצתית** מגדירה את הערכים, אך גם משאירה אותם להגדרה של המשתמש.

## <a name="6-set-up-windows-hello-for-business"></a>6. הגדרת Windows שלום עבור עסקים

 Windows שלום לעסק מחליף סיסמאות עם אימות שני גורמים חזק (2FA) לצורך כניסה למחשב מקומי. גורם אחד הוא זוג מפתחות אסימטרי, והשני הוא PIN או מחווה מקומית אחרת, כגון טביעת אצבע או זיהוי פנים אם המכשיר תומך בו. מומלץ להחליף סיסמאות באמצעות 2FA ו-Windows שלום לעסקים במידת האפשר.

כדי להגדיר היברידית Windows שלום עבור עסקים, לסקור את [מפתח היברידית אמון Windows שלום עבור דרישות מוקדמות בעסקים](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). לאחר מכן בצע את ההוראות ב- [קביעת תצורה של Windows Hybrid שלום עבור הגדרות אמון מפתח עסקי](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
