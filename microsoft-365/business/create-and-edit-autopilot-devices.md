---
title: יצירה ועריכה של מכשירי AutoPilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: למד כיצד להעלות מכשירים באמצעות AutoPilot ב- Microsoft 365 Business Premium. באפשרותך להקצות פרופיל למכשיר או לקבוצת מכשירים.
ms.openlocfilehash: 506ff44e3cb6656b19174e82688b5af141ea2b79
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578486"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="66cfb-104">יצירה ועריכה של מכשירי AutoPilot</span><span class="sxs-lookup"><span data-stu-id="66cfb-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="66cfb-105">העלאת רשימה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="66cfb-105">Upload a list of devices</span></span>

<span data-ttu-id="66cfb-106">באפשרותך להשתמש במדריך [שלב אחר שלב להעלאת](add-autopilot-devices-and-profile.md) מכשירים, אך באפשרותך גם להעלות מכשירים **בכרטיסיה מכשירים.**</span><span class="sxs-lookup"><span data-stu-id="66cfb-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="66cfb-107">מכשירים חייבים לעמוד בדרישות הבאות:</span><span class="sxs-lookup"><span data-stu-id="66cfb-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="66cfb-108">Windows 10, גירסה 1703 ואילך</span><span class="sxs-lookup"><span data-stu-id="66cfb-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="66cfb-109">מכשירים חדשים שלא עברו את החוויה 'מחוץ ל- Windows'</span><span class="sxs-lookup"><span data-stu-id="66cfb-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="66cfb-110">במרכז הניהול של Microsoft 365, בחר  \> **מכשירים AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="66cfb-110">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="66cfb-111">בדף **AutoPilot,** בחר בכרטיסיה **מכשירים** \> **הוסף מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="66cfb-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="66cfb-113">בלוח הוספת **מכשירים,** עבור אל קובץ [CSV של רשימת ההתקנים](../admin/misc/device-list.md) שהכנת \> **שמור** \> **סגור**.</span><span class="sxs-lookup"><span data-stu-id="66cfb-113">On the **Add devices** panel, browse to a [Device list CSV file](../admin/misc/device-list.md) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="66cfb-114">באפשרותך לקבל מידע זה מספק החומרה שלך, או להשתמש בקובץ [ה- Script Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) כדי ליצור קובץ CSV.</span><span class="sxs-lookup"><span data-stu-id="66cfb-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="66cfb-115">הקצאת פרופיל למכשיר או לקבוצה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="66cfb-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="66cfb-116">בדף **הכנת Windows,** בחר בכרטיסיה **מכשירים** ובחר את תיבת הסימון לצד מכשיר אחד או יותר.</span><span class="sxs-lookup"><span data-stu-id="66cfb-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="66cfb-117">בלוח **מכשיר**, בחר פרופיל מהתפריט הנפתח **פרופיל שהוקצה**.</span><span class="sxs-lookup"><span data-stu-id="66cfb-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="66cfb-118">אם עדיין אין לך פרופילים, ראה [יצירה ועריכה של פרופילי AutoPilot](create-and-edit-autopilot-profiles.md) לקבלת הוראות.</span><span class="sxs-lookup"><span data-stu-id="66cfb-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
