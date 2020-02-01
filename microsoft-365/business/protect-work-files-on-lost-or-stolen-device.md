---
title: הגנה על קבצי עבודה במקרה של אובדן או גניבה של מכשיר נייד
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4StolenDevice
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c12164c7-6190-4294-b88a-590580c9869a
description: למד אודות ההגדרות הזמינות להגנה על קבצי העבודה אם התקן המשתמש אובד או נגנב.
ms.openlocfilehash: 5f137354b51a0151e57e5e109b1ebbb043c68f60
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593555"
---
# <a name="protect-work-files-when-a-mobile-device-is-lost-or-stolen"></a><span data-ttu-id="eec6a-103">הגנה על קבצי עבודה במקרה של אובדן או גניבה של מכשיר נייד</span><span class="sxs-lookup"><span data-stu-id="eec6a-103">Protect work files when a mobile device is lost or stolen</span></span>

<span data-ttu-id="eec6a-104">הגדרות המדיניות קובעות מה קורה באופן אוטומטי כדי להגן על מכשיר במקרה של אובדן או גניבה.</span><span class="sxs-lookup"><span data-stu-id="eec6a-104">The policy settings determine what happens automatically to protect a device that is lost or stolen.</span></span> <span data-ttu-id="eec6a-105">מומלץ לקבל את ערכי ברירת המחדל במהלך ההתקנה כדי ליצור מדיניות יישומים עבור אנדרואיד, iOS ו-Windows 10 החלים על כל המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="eec6a-105">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="eec6a-106">ניתן ליצור פריטי מדיניות נוספים לאחר השלמת ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="eec6a-106">You can create more policies after setup completes.</span></span>
  
## <a name="settings-that-protect-work-files"></a><span data-ttu-id="eec6a-107">הגדרות להגנה על קבצי עבודה</span><span class="sxs-lookup"><span data-stu-id="eec6a-107">Settings that protect work files</span></span>

<span data-ttu-id="eec6a-108">ההגדרות הבאות זמינות כדי להגן על קבצי עבודה במקרה אובדן או גניבה של מכשיר משתמש:</span><span class="sxs-lookup"><span data-stu-id="eec6a-108">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="eec6a-109">הגדרה</span><span class="sxs-lookup"><span data-stu-id="eec6a-109">Setting</span></span>  <br/> |<span data-ttu-id="eec6a-110">תיאור</span><span class="sxs-lookup"><span data-stu-id="eec6a-110">Description</span></span>  <br/> |
|<span data-ttu-id="eec6a-111">מחק קבצי עבודה ממכשיר לא פעיל לאחר מספר הימים הבא</span><span class="sxs-lookup"><span data-stu-id="eec6a-111">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="eec6a-112">אם התקן אינו משמש למספר הימים שתציין כאן, כל קבצי העבודה המאוחסנים בהתקן יימחקו באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="eec6a-112">If a device isn't used for the number of days that you specify here, any work files stored on the device are automatically deleted.</span></span>  <br/> |
|<span data-ttu-id="eec6a-113">אלץ משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="eec6a-113">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="eec6a-114">אם הגדרה זו **מופעלת**, מיקום השמירה היחיד הזמין עבור קבצי עבודה הוא Onedrive עבור Business.</span><span class="sxs-lookup"><span data-stu-id="eec6a-114">If this setting is **On**, the only available save location for work files is OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="eec6a-115">הצפן קבצי עבודה</span><span class="sxs-lookup"><span data-stu-id="eec6a-115">Encrypt work files</span></span>  <br/> |<span data-ttu-id="eec6a-116">השאר הגדרה זו במצב **פעיל** כך שקבצי העבודה יהיו מוגנים על-ידי הצפנה.</span><span class="sxs-lookup"><span data-stu-id="eec6a-116">Keep this setting **On** so that work files are protected by encryption.</span></span> <span data-ttu-id="eec6a-117">גם אם ההתקן אובד או נגנב, אף אחד לא יכול לקרוא את נתוני החברה שלך.</span><span class="sxs-lookup"><span data-stu-id="eec6a-117">Even if the device is lost or stolen, no one can read your company data.</span></span>  <br/> |
   

