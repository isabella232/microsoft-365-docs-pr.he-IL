---
title: נהל את האופן שבו המשתמשים ניגשים למסמכי Office במכשירים ניידים
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
f1_keywords:
- 'O365E_BCSSetup4OfficeMobile '
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
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: למד אודות מדיניות הגנה שיכולה לסייע גישה מאובטחת יישומי Office ממכשירים ניידים.
ms.openlocfilehash: 75dbe79acccabd851c43259a165e79bfe3c509c0
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983184"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="166e7-103">נהל את האופן שבו המשתמשים ניגשים למסמכי Office במכשירים ניידים</span><span class="sxs-lookup"><span data-stu-id="166e7-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="166e7-p101">הגדרות מדיניות שקובעות כיצד משתמשים ניגשים לקבצי Office מתוך המכשירים הניידים שלהם מוגדרות למצב **כבוי** כברירת מחדל. אנו ממליצים לקבל את ערכי ברירת המחדל במהלך ההתקנה כדי ליצור פריטי מדיניות של אפליקציות עבור Android,‏ iOS ו- Windows 10 שחלים על כל המשתמשים. ניתן ליצור פריטי מדיניות נוספים לאחר השלמת ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="166e7-p101">Policy settings that control how users access Office files from their mobile devices are **Off** by default. We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users. You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="166e7-107">הגדרות שקובעות כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים</span><span class="sxs-lookup"><span data-stu-id="166e7-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="166e7-108">ההגדרות הבאות זמינות לניהול אופן הגישה של משתמשים לקבצי עבודה של Office:</span><span class="sxs-lookup"><span data-stu-id="166e7-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="166e7-109">הגדרה</span><span class="sxs-lookup"><span data-stu-id="166e7-109">Setting</span></span>  <br/> |<span data-ttu-id="166e7-110">תיאור</span><span class="sxs-lookup"><span data-stu-id="166e7-110">Description</span></span>  <br/> |
|<span data-ttu-id="166e7-111">דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office</span><span class="sxs-lookup"><span data-stu-id="166e7-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="166e7-112">אם הגדרה זו נקבעה למצב **מופעל**, על המשתמשים לספק צורה אחרת של אימות, בנוסף לשם המשתמש והסיסמה שלהם, כדי שיוכלו להשתמש ביישומי Office במכשיר הנייד שלהם.</span><span class="sxs-lookup"><span data-stu-id="166e7-112">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="166e7-113">אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה</span><span class="sxs-lookup"><span data-stu-id="166e7-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="166e7-114">כדי למנוע ממשתמש לא מורשה לנחש באופן אקראי קוד PIN, הקוד יאופס לאחר מספר כניסות שגויות שאתה תציין.</span><span class="sxs-lookup"><span data-stu-id="166e7-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="166e7-115">דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך</span><span class="sxs-lookup"><span data-stu-id="166e7-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="166e7-116">הגדרה זו קובעת את משך הזמן שבו משתמש יכול להיות לא פעיל לפני שהוא מתבקש להיכנס שוב.</span><span class="sxs-lookup"><span data-stu-id="166e7-116">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="166e7-117">מנע גישה לקבצי עבודה במכשירים שנפרצו או שבוצעה בהם פעולת ROOT</span><span class="sxs-lookup"><span data-stu-id="166e7-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="166e7-p102">ייתכן מצב שבו משתמשים מתוחכמים יחזיקו במכשיר שנפרץ או שבוצעה בו פעולת ROOT. כלומר, המשתמש יכול לשנות את מערכת ההפעלה, עובדה שחושפת את המכשיר לתוכנות זדוניות. מכשירים אלה נחסמים כאשר ההגדרה מוגדרת למצב **פעיל**.  </span><span class="sxs-lookup"><span data-stu-id="166e7-p102">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="166e7-121">אפשר למשתמשים להעתיק תוכן מאפליקציות Office לאפליקציות אישיות</span><span class="sxs-lookup"><span data-stu-id="166e7-121">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="166e7-p103">אנו מאפשרים זאת כברירת מחדל, אולם כאשר ההגדרה מוגדרת למצב **פעיל**, המשתמש יכול להעתיק מידע בקובץ עבודה לקובץ אישי. אם ההגדרה מוגדרת למצב **ביטול**, למשתמש אין אפשרות להעתיק מידע מקובץ עבודה לאפליקציה אישית או לחשבון אישי.  </span><span class="sxs-lookup"><span data-stu-id="166e7-p103">We allow this by default, but when the setting is **On**, the user can copy information in a work file to a personal file. If the setting is **Off**, the user can't copy information from a work file to a personal app or personal account.  </span></span><br/> |
   

