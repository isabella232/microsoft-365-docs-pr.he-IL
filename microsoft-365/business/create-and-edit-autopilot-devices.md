---
title: יצירה ועריכה של מכשירי AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
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
ms.openlocfilehash: cc1f81e9efd9b16e27b8abfbb0927d241535077e
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982934"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="77fa9-104">יצירה ועריכה של מכשירי AutoPilot</span><span class="sxs-lookup"><span data-stu-id="77fa9-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="77fa9-105">העלאת רשימה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="77fa9-105">Upload a list of devices</span></span>

<span data-ttu-id="77fa9-106">באפשרותך להשתמש ב[מדריך צעד-אחר-צעד](add-autopilot-devices-and-profile.md) כדי להעלות מכשירים, אך ניתן גם להעלות בכרטיסיה **מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="77fa9-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="77fa9-107">המכשירים צריכים לעמוד בדרישות אלה:</span><span class="sxs-lookup"><span data-stu-id="77fa9-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="77fa9-108">Windows ,10 גירסה 1703 ואילך.</span><span class="sxs-lookup"><span data-stu-id="77fa9-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="77fa9-109">מכשירים חדשים שאינם נחשבים כמוצר Windows מוכן לשימוש.</span><span class="sxs-lookup"><span data-stu-id="77fa9-109">New devices that have not been through Windows out-of-box experience.</span></span>
    
1. <span data-ttu-id="77fa9-110">במרכז הניהול של Microsoft 365 Business, בחר **פרוס את Windows באמצעות AutoPilot** בכרטיס **פעולות מכשיר**.</span><span class="sxs-lookup"><span data-stu-id="77fa9-110">In the Microsoft 365 Business Admin center, choose **Deploy Windows with AutoPilot** on the **Device actions** card.</span></span> 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="77fa9-112">בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים** \> **הוסף מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="77fa9-112">On the **Prepare Windows** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="77fa9-114">בלוח **התקנים הוסף** , דפדף אל [רשימת התקנים קובץ CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) שהכנת \> **שמור** \> **סגור**.</span><span class="sxs-lookup"><span data-stu-id="77fa9-114">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="77fa9-115">ניתן לקבל מידע זה מספק החומרה, או להשתמש ב[קובץ Script של PowerShell, ‏Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) שייצור קובץ csv.</span><span class="sxs-lookup"><span data-stu-id="77fa9-115">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="77fa9-116">הקצאת פרופיל למכשיר או לקבוצה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="77fa9-116">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="77fa9-117">בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים** וסמן את תיבת הסימון לצד מכשיר אחד או יותר.</span><span class="sxs-lookup"><span data-stu-id="77fa9-117">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="77fa9-118">בלוח **מכשיר**, בחר פרופיל מהתפריט הנפתח **פרופיל שהוקצה**.</span><span class="sxs-lookup"><span data-stu-id="77fa9-118">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="77fa9-119">אם עדיין אין לך פרופילים, ראה [יצירה ועריכה של פרופילי AutoPilot](create-and-edit-autopilot-profiles.md) לקבלת הוראות.</span><span class="sxs-lookup"><span data-stu-id="77fa9-119">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
