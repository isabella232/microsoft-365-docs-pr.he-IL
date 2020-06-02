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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: למד אודות מדיניות הגנה המאפשרת לך לנהל את אופן הגישה של משתמשים ליישומי Office ולקבצי עבודה ממכשירים ניידים.
ms.openlocfilehash: b2b828cf2e201360f12b8fadcb395e72958230f6
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471066"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="6a98c-103">נהל את האופן שבו המשתמשים ניגשים למסמכי Office במכשירים ניידים</span><span class="sxs-lookup"><span data-stu-id="6a98c-103">Manage how users access Office documents on mobile devices</span></span>

<span data-ttu-id="6a98c-104">מאמר זה חל על 365 עסקים Premium של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6a98c-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="6a98c-105">הגדרות מדיניות שקובעות כיצד משתמשים ניגשים לקבצי Office מתוך המכשירים הניידים שלהם מוגדרות למצב **כבוי** כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="6a98c-105">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="6a98c-106">מומלץ לקבל את ערכי ברירת המחדל במהלך ההתקנה כדי ליצור מדיניות יישומים עבור אנדרואיד, iOS ו-Windows 10 החלים על כל המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="6a98c-106">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="6a98c-107">ניתן ליצור פריטי מדיניות נוספים לאחר השלמת ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="6a98c-107">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="6a98c-108">הגדרות שקובעות כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים</span><span class="sxs-lookup"><span data-stu-id="6a98c-108">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="6a98c-109">ההגדרות הבאות זמינות לניהול אופן הגישה של משתמשים לקבצי עבודה של Office:</span><span class="sxs-lookup"><span data-stu-id="6a98c-109">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="6a98c-110">הגדרה</span><span class="sxs-lookup"><span data-stu-id="6a98c-110">Setting</span></span>  <br/> |<span data-ttu-id="6a98c-111">תיאור</span><span class="sxs-lookup"><span data-stu-id="6a98c-111">Description</span></span>  <br/> |
|<span data-ttu-id="6a98c-112">דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office</span><span class="sxs-lookup"><span data-stu-id="6a98c-112">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="6a98c-113">אם הגדרה זו **מופעלת, על**המשתמשים לספק צורה אחרת של אימות, בנוסף לשם המשתמש והסיסמה שלהם, לפני שהם יוכלו להשתמש ביישומי Office במכשיר הנייד שלהם.</span><span class="sxs-lookup"><span data-stu-id="6a98c-113">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="6a98c-114">אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה</span><span class="sxs-lookup"><span data-stu-id="6a98c-114">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="6a98c-115">כדי למנוע ממשתמש לא מורשה לנחש באופן אקראי קוד PIN, הקוד יאופס לאחר מספר כניסות שגויות שאתה תציין.</span><span class="sxs-lookup"><span data-stu-id="6a98c-115">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="6a98c-116">דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך</span><span class="sxs-lookup"><span data-stu-id="6a98c-116">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="6a98c-117">הגדרה זו קובעת כמה זמן יכול המשתמש להיות לא פעיל לפני שתתבקש להיכנס שוב.</span><span class="sxs-lookup"><span data-stu-id="6a98c-117">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="6a98c-118">מנע גישה לקבצי עבודה במכשירים שנפרצו או שבוצעה בהם פעולת ROOT</span><span class="sxs-lookup"><span data-stu-id="6a98c-118">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="6a98c-119">ייתכן מצב שבו משתמשים מתוחכמים יחזיקו במכשיר שנפרץ או שבוצעה בו פעולת ROOT.</span><span class="sxs-lookup"><span data-stu-id="6a98c-119">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="6a98c-120">משמעות הדבר היא כי המשתמש יכול לשנות את מערכת ההפעלה, אשר יכול להפוך את המכשיר פגיע יותר לתוכנות זדוניות.</span><span class="sxs-lookup"><span data-stu-id="6a98c-120">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="6a98c-121">מכשירים אלה נחסמים כאשר ההגדרה מוגדרת למצב **פעיל**.</span><span class="sxs-lookup"><span data-stu-id="6a98c-121">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="6a98c-122">אל תאפשר למשתמשים להעתיק תוכן מיישומי Office ליישומים אישיים</span><span class="sxs-lookup"><span data-stu-id="6a98c-122">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="6a98c-123">כאשר ההגדרה **מופעלת**, המשתמש אינו יכול להעתיק מידע בקובץ עבודה לקובץ אישי.</span><span class="sxs-lookup"><span data-stu-id="6a98c-123">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="6a98c-124">אם ההגדרה **כבויה**, המשתמש יכול להעתיק מידע מקובץ עבודה לאפליקציה אישית או לחשבון אישי.</span><span class="sxs-lookup"><span data-stu-id="6a98c-124">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

