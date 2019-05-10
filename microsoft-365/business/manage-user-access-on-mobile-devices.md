---
title: נהל את האופן שבו המשתמשים ניגשים למסמכי Office במכשירים ניידים
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4OfficeMobile
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
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: למד אודות מדיניות הגנה שיכולה לסייע גישה מאובטחת יישומי Office ממכשירים ניידים.
ms.openlocfilehash: b49ec33f4899a25f92ffd9d7a25d3e435016749e
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660330"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="0637c-103">נהל את האופן שבו המשתמשים ניגשים למסמכי Office במכשירים ניידים</span><span class="sxs-lookup"><span data-stu-id="0637c-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="0637c-p101">הגדרות מדיניות שקובעות כיצד משתמשים ניגשים לקבצי Office מתוך המכשירים הניידים שלהם מוגדרות למצב **כבוי** כברירת מחדל. אנו ממליצים לקבל את ערכי ברירת המחדל במהלך ההתקנה כדי ליצור פריטי מדיניות של אפליקציות עבור Android,‏ iOS ו- Windows 10 שחלים על כל המשתמשים. ניתן ליצור פריטי מדיניות נוספים לאחר השלמת ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="0637c-p101">Policy settings that control how users access Office files from their mobile devices are **Off** by default. We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users. You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="0637c-107">הגדרות שקובעות כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים</span><span class="sxs-lookup"><span data-stu-id="0637c-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="0637c-108">ההגדרות הבאות זמינות לניהול אופן הגישה של משתמשים לקבצי עבודה של Office:</span><span class="sxs-lookup"><span data-stu-id="0637c-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="0637c-109">הגדרה</span><span class="sxs-lookup"><span data-stu-id="0637c-109">Setting</span></span>  <br/> |<span data-ttu-id="0637c-110">תיאור</span><span class="sxs-lookup"><span data-stu-id="0637c-110">Description</span></span>  <br/> |
|<span data-ttu-id="0637c-111">דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office</span><span class="sxs-lookup"><span data-stu-id="0637c-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="0637c-112">אם הגדרה זו נקבעה למצב **מופעל**, על המשתמשים לספק צורה אחרת של אימות, בנוסף לשם המשתמש והסיסמה שלהם, כדי שיוכלו להשתמש ביישומי Office במכשיר הנייד שלהם.</span><span class="sxs-lookup"><span data-stu-id="0637c-112">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="0637c-113">אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה</span><span class="sxs-lookup"><span data-stu-id="0637c-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="0637c-114">כדי למנוע ממשתמש לא מורשה לנחש באופן אקראי קוד PIN, הקוד יאופס לאחר מספר כניסות שגויות שאתה תציין.</span><span class="sxs-lookup"><span data-stu-id="0637c-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="0637c-115">דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך</span><span class="sxs-lookup"><span data-stu-id="0637c-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="0637c-116">הגדרה זו קובעת את משך הזמן שבו משתמש יכול להיות לא פעיל לפני שהוא מתבקש להיכנס שוב.</span><span class="sxs-lookup"><span data-stu-id="0637c-116">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="0637c-117">מנע גישה לקבצי עבודה במכשירים שנפרצו או שבוצעה בהם פעולת ROOT</span><span class="sxs-lookup"><span data-stu-id="0637c-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="0637c-p102">ייתכן מצב שבו משתמשים מתוחכמים יחזיקו במכשיר שנפרץ או שבוצעה בו פעולת ROOT. כלומר, המשתמש יכול לשנות את מערכת ההפעלה, עובדה שחושפת את המכשיר לתוכנות זדוניות. מכשירים אלה נחסמים כאשר ההגדרה מוגדרת למצב **פעיל**.  </span><span class="sxs-lookup"><span data-stu-id="0637c-p102">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="0637c-121">אל תאפשר למשתמשים להעתיק תוכן מ- Office apps לתוך יישומים אישי</span><span class="sxs-lookup"><span data-stu-id="0637c-121">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="0637c-122">כאשר **ההגדרה מופעלת,** למשתמש אין אפשרות להעתיק מידע בקובץ העבודה קובץ אישי.</span><span class="sxs-lookup"><span data-stu-id="0637c-122">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="0637c-123">אם ההגדרה אינה **פעילה**, המשתמש יכול להעתיק מידע מתוך קובץ עבודה app אישי או חשבון אישי.</span><span class="sxs-lookup"><span data-stu-id="0637c-123">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

