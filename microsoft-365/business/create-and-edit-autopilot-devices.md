---
title: יצירה ועריכה של מכשירי AutoPilot
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: למד כיצד להעלות מכשירים באמצעות טייס אוטומטי ב-Microsoft 365 Business Premium. באפשרותך להקצות פרופיל למכשיר או לקבוצת מכשירים.
ms.openlocfilehash: 910abb98b94b749177b04cd12c766f82d348e379
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913397"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="6033c-104">יצירה ועריכה של מכשירי AutoPilot</span><span class="sxs-lookup"><span data-stu-id="6033c-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="6033c-105">העלאת רשימה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="6033c-105">Upload a list of devices</span></span>

<span data-ttu-id="6033c-106">באפשרותך להשתמש [במדריך שלב אחר שלב](add-autopilot-devices-and-profile.md) להעלאת מכשירים, אך ניתן גם להעלות מכשירים בכרטיסיה ' **מכשירים** '.</span><span class="sxs-lookup"><span data-stu-id="6033c-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="6033c-107">המכשירים חייבים לעמוד בדרישות אלה:</span><span class="sxs-lookup"><span data-stu-id="6033c-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="6033c-108">Windows 10, גירסה 1703 ואילך</span><span class="sxs-lookup"><span data-stu-id="6033c-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="6033c-109">מכשירים חדשים שאינם מותקנים בחוויית Windows out-of-box</span><span class="sxs-lookup"><span data-stu-id="6033c-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="6033c-110">במרכז הניהול של Microsoft 365, בחר **מכשירים** \> **טייס אוטומטי**.</span><span class="sxs-lookup"><span data-stu-id="6033c-110">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="6033c-111">בדף **הטייס האוטומטי** , בחר את הכרטיסיה **מכשירים** \> **הוסף מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="6033c-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="6033c-113">בלוח **הוספת מכשירים** , אתר את [קובץ ה-CSV של רשימת](../admin/misc/device-list.md) המכשירים שהכנת \> **שמור** \> **בסגירה**.</span><span class="sxs-lookup"><span data-stu-id="6033c-113">On the **Add devices** panel, browse to a [Device list CSV file](../admin/misc/device-list.md) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="6033c-114">באפשרותך לקבל מידע זה מספק החומרה, או להשתמש [בסקריפט get-Windowsautopilotinfohttps PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) כדי ליצור קובץ CSV.</span><span class="sxs-lookup"><span data-stu-id="6033c-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="6033c-115">הקצאת פרופיל למכשיר או לקבוצה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="6033c-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="6033c-116">בדף **הכנת Windows** , בחר את הכרטיסיה **התקנים** ובחר את תיבת הסימון לצד התקן אחד או יותר.</span><span class="sxs-lookup"><span data-stu-id="6033c-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="6033c-117">בלוח **מכשיר**, בחר פרופיל מהתפריט הנפתח **פרופיל שהוקצה**.</span><span class="sxs-lookup"><span data-stu-id="6033c-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="6033c-118">אם עדיין אין לך פרופילים, ראה [יצירה ועריכה של פרופילי AutoPilot](create-and-edit-autopilot-profiles.md) לקבלת הוראות.</span><span class="sxs-lookup"><span data-stu-id="6033c-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
