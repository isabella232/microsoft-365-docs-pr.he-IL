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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: למד כיצד לאפשר ל-Microsoft 365 להגן על התקנים המקומיים המצורפים ל-Windows 10.
ms.openlocfilehash: 9bfd540c0ff113762485f62707f1975ff53accc4
ms.sourcegitcommit: 1162d676b036449ea4220de8a6642165190e3398
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068104"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>מתן אפשרות לניהול מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business

אם הארגון שלך משתמש ב-Windows Server Active Directory מקומי, באפשרותך להגדיר את Microsoft 365 Business כדי להגן על התקני Windows 10 שלך, תוך שמירה על גישה למשאבים מקומיים המחייבים אימות מקומי. אתה יכול להגדיר את זה על ידי הראשון סינכרון הספרייה הפעילה שלך עם כחול Active Directory, ואחריו רישום התקנים של Windows 10 עם תכלת AD ולרשום אותם לניהול המכשיר הנייד על ידי Microsoft 365 Business.
הסרטון הבא מפרט את השלבים עבור אופן ההגדרה של התרחיש השכיח ביותר.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>הגדרת התקנים המצורפים לתחום לניהול על-ידי Microsoft 365 Business

כדי להגדיר את ההתקנים המצורפים לתחום של הארגון שלך כדי להפיק תועלת מהיכולות שסופקו על-ידי התכונה ' פעיל בספריה ' בנוסף ל-Active Directory המקומי, באפשרותך ליישם **התקנים מצורפים של ' תכלת היברידית**'. אלה הם התקנים המצורפים הן ל-Active Directory המקומי ולספריה הפעילה שלך. היברידית תכלת AD התקנים המצורפים יכול להיות מוגן ומנוהל על ידי מיקרוסופט 365 עסקים. 
  
להשלים את השלבים הבאים כדי להפוך את Windows 10 התקנים היברידית תכלת AD הצטרף והמנוהל על ידי Microsoft 365 Business.
  
1. **התכונן לסנכרון ספריות**: לפני שתסנכרן את המשתמשים והמחשבים שלך מקבוצת המחשבים המקומית של active Directory, סקור את [ההכנה לסנכרון ספריות ל-Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). בפרט:

   - ודא שאין כפילויות בספריה שלך עבור התכונות הבאות: **דואר**, **כתובות Proxyaddresses שמות** **משתמשים**. על ערכים אלה להיות ייחודיים ולהסיר את כל הכפילויות.
   
   - **המלצתי** למשתמש להתאים את כתובת הדואר האלקטרוני הראשית התואמת ל-Microsoft 365 המורשה של משתמש מקומי. לדוגמה **mary.shelley@contoso.com** במקום **מרי @ contoso. מקומי**
   
   - אם קבוצת המחשבים של Active Directory מסתיימת בסיומת שאינה ניתנת לניתוב כגון **. local** או **. lan**, במקום סיומת אינטרנט הניתנת לניתוב כגון **. com** או **. org**, יהיה עליך לכוונן תחילה את סיומת ה-UPN של חשבונות המשתמשים המקומיים כמתואר ב [הכן תחום שאינו ניתן לניתוב עבור סינכרון ספריות](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

2. **להתקין ולקבוע את התצורה של תכלת החיבור**: כדי לסנכרן את המשתמשים, הקבוצות ואנשי הקשר שלך מ-active directory המקומי לתוך מדריך הפעילות של תכלת פעילה, הפעל את אשף סינכרון הספריות מתוך התחברות מדריך הכתובות של ראה [הגדרת סינכרון ספריות עבור Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) כדי ללמוד עוד.
    
    > [!NOTE]
    > השלבים זהים בדיוק עבור Microsoft 365 Business. 
    
כאשר אתה מגדיר את האפשרויות שלך עבור תכלת AD התחבר, אנו ממליצים לאפשר **סנכרון סיסמה** **חלקה כניסה יחידה**, כמו גם את התכונה **הסיסמה ככתוב** , אשר נתמך גם ב-Microsoft 365 Business.

> [!NOTE]
> יש כמה שלבים נוספים עבור הסיסמה כתיבה מעבר לתיבת הסימון התחבר תכלת AD. התייחס [לאופן ההגדרה: הגדר את הסיסמה ככתוב בחזרה](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 
     
3. **הגדרת תכלת היברידית להצטרף**: לפני שאתה מאפשר ל-Windows 10 התקנים להיות היברידית תכלת לספירה הצטרף, עליך לוודא שאתה עומד בדרישות המוקדמות הבאות:

   - אתה מפעיל את הגירסה העדכנית ביותר של התחברות התכלת AD.

   - החיבור התכלת לספירה מסנכרן את כל אובייקטי המחשב של המכשירים שברצונך להיות היברידית תכלת לספירה הצטרפו. אם אובייקטי המחשב שייכים ליחידות ארגוניות מסוימות (OU), ודא שאלה אלה מוגדרות לסנכרון בתכלת הספירה גם כן.

כדי לרשום התקן קיים המצורפים ל-Windows 10 התקנים כמו תכלת היברידית לספירה הצטרף, בצע את השלבים [במדריך: קביעת תצורה של היברידית תכלת היברידי להצטרף לתחומים מנוהלים](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). פעולה זו תהפוך היברידית לזמינה הקיימת ב-Active Directory המקומי שלך הצטרף למחשבי Windows 10 ולגרום להם להיות מוכנים לענן.
    
4. **אפשר הרשמה אוטומטית עבור windows 10**: כדי לרשום באופן אוטומטי התקני windows 10 עבור ניהול התקנים ניידים ב-Intune, ראה [רישום התקן windows 10 באופן אוטומטי באמצעות מדיניות קבוצתית](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). באפשרותך להגדיר את המדיניות הקבוצתית ברמת מחשב מקומית, או עבור פעולות בצובר, באפשרותך ליצור הגדרת מדיניות קבוצתית זו בבקר התחום שלך באמצעות מסוף ניהול המדיניות הקבוצתית ותבניות ADMX.

5. **קביעת תצורה של כניסה יחידה חלקה: מערכת**SSO חלקה תחתום באופן אוטומטי על משתמשים במשאבי ענן של Microsoft 365 שלהם כשהם משתמשים במחשבים ארגוניים. פשוט לפרוס אחת משתי אפשרויות המדיניות הקבוצתית המתוארות [כניסה יחידה של Active Directory בודדת: התחלה מהירה](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). האפשרות **מדיניות קבוצתית** אינה מאפשרת למשתמשים לשנות את הגדרותיו, בעוד שהאפשרות **העדפת מדיניות קבוצתית** מגדירה את הערכים, אך גם משאירה אותם להגדרה של המשתמש.

6. **הגדרת Windows שלום לעסקים**: Windows שלום לעסק מחליף סיסמאות עם אימות שני גורמים חזק (2fa) לצורך כניסה למחשב מקומי. גורם אחד הוא זוג מפתחות אסימטרי, והשני הוא PIN או מחווה מקומית אחרת, כגון טביעת אצבע או זיהוי פנים אם המכשיר תומך בו. אנו ממליצים לך להחליף סיסמאות עם 2FA ו-Windows שלום לעסקים במידת האפשר.

כדי להגדיר היברידית Windows שלום עבור עסקים, לסקור את [מפתח היברידית אמון Windows שלום עבור דרישות מוקדמות בעסקים](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). לאחר מכן בצע את ההוראות כדי [להגדיר היברידית Windows שלום עבור הגדרות אמון מפתח עסקי](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
