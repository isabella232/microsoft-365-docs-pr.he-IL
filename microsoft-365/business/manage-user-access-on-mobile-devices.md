---
title: נהל את האופן שבו המשתמשים ניגשים למסמכי Office במכשירים ניידים
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: למד אודות מדיניות הגנה המאפשרת לך לנהל את האופן בו משתמשים ניגשים לאפליקציות Office וקבצי עבודה ממכשירים ניידים.
ms.openlocfilehash: 7602b712f2dfc3ba369fd76979baaaa8d5da5c5c
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925278"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="83ae2-103">נהל את האופן שבו המשתמשים ניגשים למסמכי Office במכשירים ניידים</span><span class="sxs-lookup"><span data-stu-id="83ae2-103">Manage how users access Office documents on mobile devices</span></span>

<span data-ttu-id="83ae2-104">מאמר זה חל על Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="83ae2-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="83ae2-105">הגדרות מדיניות שקובעות כיצד משתמשים ניגשים לקבצי Office מתוך המכשירים הניידים שלהם מוגדרות למצב **כבוי** כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="83ae2-105">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="83ae2-106">מומלץ לקבל את ערכי ברירת המחדל במהלך ההגדרה כדי ליצור מדיניות יישומים עבור Android , iOS ו- Windows 10 החלים על כל המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="83ae2-106">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="83ae2-107">ניתן ליצור פריטי מדיניות נוספים לאחר השלמת ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="83ae2-107">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="83ae2-108">הגדרות שקובעות כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים</span><span class="sxs-lookup"><span data-stu-id="83ae2-108">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="83ae2-109">ההגדרות הבאות זמינות לניהול אופן הגישה של משתמשים לקבצי עבודה של Office:</span><span class="sxs-lookup"><span data-stu-id="83ae2-109">The following settings are available to manage how users access Office work files:</span></span>

|<span data-ttu-id="83ae2-110">הגדרה</span><span class="sxs-lookup"><span data-stu-id="83ae2-110">Setting</span></span>  <br/> |<span data-ttu-id="83ae2-111">תיאור</span><span class="sxs-lookup"><span data-stu-id="83ae2-111">Description</span></span>  <br/> |
|:-----|:-----|
|<span data-ttu-id="83ae2-112">דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office</span><span class="sxs-lookup"><span data-stu-id="83ae2-112">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="83ae2-113">אם הגדרה זו היא **On**, המשתמשים חייבים לספק צורה אחרת של אימות, בנוסף לשם המשתמש והסיסמה שלהם, כדי שהם יוכלו להשתמש באפליקציות Office במכשיר הנייד שלהם.</span><span class="sxs-lookup"><span data-stu-id="83ae2-113">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="83ae2-114">אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה</span><span class="sxs-lookup"><span data-stu-id="83ae2-114">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="83ae2-115">כדי למנוע ממשתמש לא מורשה לנחש באופן אקראי קוד PIN, הקוד יאופס לאחר מספר כניסות שגויות שאתה תציין.</span><span class="sxs-lookup"><span data-stu-id="83ae2-115">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="83ae2-116">דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך</span><span class="sxs-lookup"><span data-stu-id="83ae2-116">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="83ae2-117">הגדרה זו קובעת כמה זמן המשתמש יכול להיות לא פעיל לפני שהוא מתבקש להיכנס שוב.</span><span class="sxs-lookup"><span data-stu-id="83ae2-117">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="83ae2-118">מנע גישה לקבצי עבודה במכשירים שנפרצו או שבוצעה בהם פעולת ROOT</span><span class="sxs-lookup"><span data-stu-id="83ae2-118">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="83ae2-119">ייתכן מצב שבו משתמשים מתוחכמים יחזיקו במכשיר שנפרץ או שבוצעה בו פעולת ROOT.</span><span class="sxs-lookup"><span data-stu-id="83ae2-119">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="83ae2-120">משמעות הדבר היא שהמשתמש יכול לשנות את מערכת ההפעלה, אשר יכולה להפוך את המכשיר ל רגיש יותר לתוכנות זדוניות.</span><span class="sxs-lookup"><span data-stu-id="83ae2-120">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="83ae2-121">מכשירים אלה נחסמים כאשר ההגדרה מוגדרת למצב **פעיל**.</span><span class="sxs-lookup"><span data-stu-id="83ae2-121">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="83ae2-122">אל תאפשר למשתמשים להעתיק תוכן מאפליקציות Office לאפליקציות אישיות</span><span class="sxs-lookup"><span data-stu-id="83ae2-122">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="83ae2-123">כאשר ההגדרה **היא פועל,** למשתמש אין אפשרות להעתיק מידע בקובץ עבודה לקובץ אישי.</span><span class="sxs-lookup"><span data-stu-id="83ae2-123">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="83ae2-124">אם ההגדרה **כבויה,** המשתמש יכול להעתיק מידע מקובץ עבודה לאפליקציה אישית או לחשבון אישי.</span><span class="sxs-lookup"><span data-stu-id="83ae2-124">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

