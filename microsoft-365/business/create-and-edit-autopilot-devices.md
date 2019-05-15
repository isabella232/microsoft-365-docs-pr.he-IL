---
title: יצירה ועריכה של מכשירי AutoPilot
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: למד כיצד להעלות התקנים באמצעות AutoPilot בעסק 365 של Microsoft. באפשרותך להקצות פרופיל התקן או קבוצה של התקנים.
ms.openlocfilehash: dee77a014ef519f3487a082edc3cf81058ec1c00
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34071639"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="abcfa-104">יצירה ועריכה של מכשירי AutoPilot</span><span class="sxs-lookup"><span data-stu-id="abcfa-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="abcfa-105">העלאת רשימה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="abcfa-105">Upload a list of devices</span></span>

<span data-ttu-id="abcfa-106">באפשרותך להשתמש ב[מדריך צעד-אחר-צעד](add-autopilot-devices-and-profile.md) כדי להעלות מכשירים, אך ניתן גם להעלות בכרטיסיה **מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="abcfa-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="abcfa-107">המכשירים צריכים לעמוד בדרישות אלה:</span><span class="sxs-lookup"><span data-stu-id="abcfa-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="abcfa-108">Windows ,10 גירסה 1703 ואילך.</span><span class="sxs-lookup"><span data-stu-id="abcfa-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="abcfa-109">מכשירים חדשים שאינם נחשבים כמוצר Windows מוכן לשימוש.</span><span class="sxs-lookup"><span data-stu-id="abcfa-109">New devices that have not been through Windows out-of-box experience.</span></span>

1. <span data-ttu-id="abcfa-110">במרכז הניהול העסקי של Microsoft 365, בחר **התקנים** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="abcfa-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="abcfa-111">בדף ' **AutoPilot** ', בחר את הכרטיסיה **התקנים** \> **הוסף התקנים**.</span><span class="sxs-lookup"><span data-stu-id="abcfa-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="abcfa-113">בלוח **התקנים הוסף** , דפדף אל [רשימת התקנים קובץ CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) שהכנת \> **שמור** \> **סגור**.</span><span class="sxs-lookup"><span data-stu-id="abcfa-113">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="abcfa-114">ניתן לקבל מידע זה מספק החומרה, או להשתמש ב[קובץ Script של PowerShell, ‏Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) שייצור קובץ csv.</span><span class="sxs-lookup"><span data-stu-id="abcfa-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="abcfa-115">הקצאת פרופיל למכשיר או לקבוצה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="abcfa-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="abcfa-116">בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים** וסמן את תיבת הסימון לצד מכשיר אחד או יותר.</span><span class="sxs-lookup"><span data-stu-id="abcfa-116">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="abcfa-117">בלוח **מכשיר**, בחר פרופיל מהתפריט הנפתח **פרופיל שהוקצה**.</span><span class="sxs-lookup"><span data-stu-id="abcfa-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="abcfa-118">אם עדיין אין לך פרופילים, ראה [יצירה ועריכה של פרופילי AutoPilot](create-and-edit-autopilot-profiles.md) לקבלת הוראות.</span><span class="sxs-lookup"><span data-stu-id="abcfa-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
