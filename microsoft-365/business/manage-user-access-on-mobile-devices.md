---
title: נהל את האופן שבו המשתמשים ניגשים למסמכי Office במכשירים ניידים
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: למד אודות מדיניות הגנה שיכולה לסייע באבטחת גישה ליישומי Office ממכשירים ניידים.
ms.openlocfilehash: 39d28a3a78fb06d0020c484b1782b544f6a8c656
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593820"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="db5fb-103">נהל את האופן שבו המשתמשים ניגשים למסמכי Office במכשירים ניידים</span><span class="sxs-lookup"><span data-stu-id="db5fb-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="db5fb-104">הגדרות מדיניות שקובעות כיצד משתמשים ניגשים לקבצי Office מתוך המכשירים הניידים שלהם מוגדרות למצב **כבוי** כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="db5fb-104">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="db5fb-105">מומלץ לקבל את ערכי ברירת המחדל במהלך ההתקנה כדי ליצור מדיניות יישומים עבור אנדרואיד, iOS ו-Windows 10 החלים על כל המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="db5fb-105">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="db5fb-106">ניתן ליצור פריטי מדיניות נוספים לאחר השלמת ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="db5fb-106">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="db5fb-107">הגדרות שקובעות כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים</span><span class="sxs-lookup"><span data-stu-id="db5fb-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="db5fb-108">ההגדרות הבאות זמינות לניהול אופן הגישה של משתמשים לקבצי עבודה של Office:</span><span class="sxs-lookup"><span data-stu-id="db5fb-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="db5fb-109">הגדרה</span><span class="sxs-lookup"><span data-stu-id="db5fb-109">Setting</span></span>  <br/> |<span data-ttu-id="db5fb-110">תיאור</span><span class="sxs-lookup"><span data-stu-id="db5fb-110">Description</span></span>  <br/> |
|<span data-ttu-id="db5fb-111">דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office</span><span class="sxs-lookup"><span data-stu-id="db5fb-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="db5fb-112">אם הגדרה זו **מופעלת, על**המשתמשים לספק צורה אחרת של אימות, בנוסף לשם המשתמש והסיסמה שלהם, לפני שהם יוכלו להשתמש ביישומי Office במכשיר הנייד שלהם.</span><span class="sxs-lookup"><span data-stu-id="db5fb-112">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="db5fb-113">אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה</span><span class="sxs-lookup"><span data-stu-id="db5fb-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="db5fb-114">כדי למנוע ממשתמש לא מורשה לנחש באופן אקראי קוד PIN, הקוד יאופס לאחר מספר כניסות שגויות שאתה תציין.</span><span class="sxs-lookup"><span data-stu-id="db5fb-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="db5fb-115">דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך</span><span class="sxs-lookup"><span data-stu-id="db5fb-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="db5fb-116">הגדרה זו קובעת כמה זמן יכול המשתמש להיות לא פעיל לפני שתתבקש להיכנס שוב.</span><span class="sxs-lookup"><span data-stu-id="db5fb-116">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="db5fb-117">מנע גישה לקבצי עבודה במכשירים שנפרצו או שבוצעה בהם פעולת ROOT</span><span class="sxs-lookup"><span data-stu-id="db5fb-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="db5fb-118">ייתכן מצב שבו משתמשים מתוחכמים יחזיקו במכשיר שנפרץ או שבוצעה בו פעולת ROOT.</span><span class="sxs-lookup"><span data-stu-id="db5fb-118">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="db5fb-119">משמעות הדבר היא כי המשתמש יכול לשנות את מערכת ההפעלה, אשר יכול להפוך את המכשיר פגיע יותר לתוכנות זדוניות.</span><span class="sxs-lookup"><span data-stu-id="db5fb-119">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="db5fb-120">מכשירים אלה נחסמים כאשר ההגדרה מוגדרת למצב **פעיל**.</span><span class="sxs-lookup"><span data-stu-id="db5fb-120">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="db5fb-121">אל תאפשר למשתמשים להעתיק תוכן מיישומי Office ליישומים אישיים</span><span class="sxs-lookup"><span data-stu-id="db5fb-121">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="db5fb-122">כאשר ההגדרה **מופעלת**, המשתמש אינו יכול להעתיק מידע בקובץ עבודה לקובץ אישי.</span><span class="sxs-lookup"><span data-stu-id="db5fb-122">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="db5fb-123">אם ההגדרה **כבויה**, המשתמש יכול להעתיק מידע מקובץ עבודה לאפליקציה אישית או לחשבון אישי.</span><span class="sxs-lookup"><span data-stu-id="db5fb-123">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

