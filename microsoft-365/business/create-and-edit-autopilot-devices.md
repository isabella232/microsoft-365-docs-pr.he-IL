---
title: יצירה ועריכה של מכשירי AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
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
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: למד כיצד להעלות התקנים באמצעות AutoPilot בעסק 365 של Microsoft. באפשרותך להקצות פרופיל התקן או קבוצה של התקנים.
ms.openlocfilehash: 6492f1469a1ac9ea67750e9ffa071d19c88c743f
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660401"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="5515c-104">יצירה ועריכה של מכשירי AutoPilot</span><span class="sxs-lookup"><span data-stu-id="5515c-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="5515c-105">העלאת רשימה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="5515c-105">Upload a list of devices</span></span>

<span data-ttu-id="5515c-106">באפשרותך להשתמש ב[מדריך צעד-אחר-צעד](add-autopilot-devices-and-profile.md) כדי להעלות מכשירים, אך ניתן גם להעלות בכרטיסיה **מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="5515c-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="5515c-107">המכשירים צריכים לעמוד בדרישות אלה:</span><span class="sxs-lookup"><span data-stu-id="5515c-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="5515c-108">Windows ,10 גירסה 1703 ואילך.</span><span class="sxs-lookup"><span data-stu-id="5515c-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="5515c-109">מכשירים חדשים שאינם נחשבים כמוצר Windows מוכן לשימוש.</span><span class="sxs-lookup"><span data-stu-id="5515c-109">New devices that have not been through Windows out-of-box experience.</span></span>

1. <span data-ttu-id="5515c-110">במרכז הניהול העסקי של Microsoft 365, בחר **התקנים** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="5515c-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="5515c-111">בדף ' **AutoPilot** ', בחר את הכרטיסיה **התקנים** \> **הוסף התקנים**.</span><span class="sxs-lookup"><span data-stu-id="5515c-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="5515c-113">בלוח **התקנים הוסף** , דפדף אל [רשימת התקנים קובץ CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) שהכנת \> **שמור** \> **סגור**.</span><span class="sxs-lookup"><span data-stu-id="5515c-113">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="5515c-114">ניתן לקבל מידע זה מספק החומרה, או להשתמש ב[קובץ Script של PowerShell, ‏Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) שייצור קובץ csv.</span><span class="sxs-lookup"><span data-stu-id="5515c-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="5515c-115">הקצאת פרופיל למכשיר או לקבוצה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="5515c-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="5515c-116">בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים** וסמן את תיבת הסימון לצד מכשיר אחד או יותר.</span><span class="sxs-lookup"><span data-stu-id="5515c-116">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="5515c-117">בלוח **מכשיר**, בחר פרופיל מהתפריט הנפתח **פרופיל שהוקצה**.</span><span class="sxs-lookup"><span data-stu-id="5515c-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="5515c-118">אם עדיין אין לך פרופילים, ראה [יצירה ועריכה של פרופילי AutoPilot](create-and-edit-autopilot-profiles.md) לקבלת הוראות.</span><span class="sxs-lookup"><span data-stu-id="5515c-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
