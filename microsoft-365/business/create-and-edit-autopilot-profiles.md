---
title: יצירה ועריכה של פרופילי AutoPilot
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
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'למד כיצד ליצור, לערוך, למחוק או להסיר פרופילי AutoPilot. '
ms.openlocfilehash: 4658a27e5f2c64a52f8a7d08b3fc13df5e239dc3
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983134"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="e96ca-103">יצירה ועריכה של פרופילי AutoPilot</span><span class="sxs-lookup"><span data-stu-id="e96ca-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="e96ca-104">יצירת פרופיל</span><span class="sxs-lookup"><span data-stu-id="e96ca-104">Create a profile</span></span>

<span data-ttu-id="e96ca-105">פרופיל חל על מכשיר או על קבוצה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="e96ca-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="e96ca-106">במרכז הניהול של Microsoft 365 Business, בחר **פרוס את Windows באמצעות AutoPilot** בכרטיס **פעולות מכשיר**.</span><span class="sxs-lookup"><span data-stu-id="e96ca-106">In the Microsoft 365 Business Admin center, choose **Deploy Windows with AutoPilot** on the **Device actions** card.</span></span> 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="e96ca-108">בדף **הכנת Windows**, בחר בכרטיסיה **פרופילים** \> **צור פרופיל**.</span><span class="sxs-lookup"><span data-stu-id="e96ca-108">On the **Prepare Windows** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="e96ca-109">בדף **יצירת פרופיל**, הזן שם עבור הפרופיל שיעזור לך לזהות אותו, לדוגמה, שיווק, הפעל את ההגדרה הרצויה (למידע נוסף, ראה [אודות ההגדרות של פרופיל AutoPilot](autopilot-profile-settings.md)), ובחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="e96ca-109">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing, turn on the setting you want (see [About AutoPilot Profile settings](autopilot-profile-settings.md) for more information), and choose **Save**.</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="e96ca-111">החלת פרופיל על מכשיר</span><span class="sxs-lookup"><span data-stu-id="e96ca-111">Apply profile to a device</span></span>

<span data-ttu-id="e96ca-p101">לאחר שתיצור פרופיל, תוכל להחיל אותו על מכשיר או על קבוצה של מכשירים. תוכל לבחור פרופיל קיים ב[מדריך צעד-אחד-צעד](add-autopilot-devices-and-profile.md), תוכל להחיל אותו על מכשירים חדשים או תוכל להחליף פרופיל קיים עבור מכשיר או קבוצת מכשירים.</span><span class="sxs-lookup"><span data-stu-id="e96ca-p101">After you create a profile you can apply it to a device or a group of devices. You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md), you can apply it to new devices, or you can replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="e96ca-114">בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="e96ca-114">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="e96ca-115">לחץ על תיבת הסימון לצד שם מכשיר בלוח **מכשיר**, בחר פרופיל בתפריט הנפתח **פרופיל שהוקצה** \> **שמור**.</span><span class="sxs-lookup"><span data-stu-id="e96ca-115">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="e96ca-117">עריכה, מחיקה או הסרה של פרופיל</span><span class="sxs-lookup"><span data-stu-id="e96ca-117">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="e96ca-p102">לאחר שהקצית פרופיל למכשיר, תוכל לעדכן אותו גם אם כבר נתת את המכשיר למשתמש. כאשר המכשיר יתחבר לאינטרנט, הוא יוריד את הגירסה העדכנית ביותר של הפרופיל שלך במהלך תהליך ההתקנה. אם המשתמש משחזר את המכשיר שלו את להגדרות ברירת המחדל של היצרן, המכשיר יוריד שוב את העדכונים האחרונים לפרופיל שלך.</span><span class="sxs-lookup"><span data-stu-id="e96ca-p102">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="e96ca-121">עריכת פרופיל</span><span class="sxs-lookup"><span data-stu-id="e96ca-121">Edit a profile</span></span>

1. <span data-ttu-id="e96ca-122">בדף **הכנת Windows**, בחר בכרטיסיה **פרופילים**.</span><span class="sxs-lookup"><span data-stu-id="e96ca-122">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="e96ca-123">לחץ על תיבת הסימון לצד שם מכשיר, ובלוח **פרופיל** עדכן אחת מההגדרות הזמינות \> **שמור**.</span><span class="sxs-lookup"><span data-stu-id="e96ca-123">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="e96ca-124">אם תבצע פעולות אלה לפני שהמשתמש יחבר את המכשיר לאינטרנט, הפרופיל יוחל על תהליך ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="e96ca-124">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="e96ca-125">מחיקת פרופיל</span><span class="sxs-lookup"><span data-stu-id="e96ca-125">Delete a profile</span></span>

1. <span data-ttu-id="e96ca-126">בדף **הכנת Windows**, בחר בכרטיסיה **פרופילים**.</span><span class="sxs-lookup"><span data-stu-id="e96ca-126">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="e96ca-127">לחץ על תיבת הסימון לצד שם מכשיר, ובלוח **פרופיל** לחץ על **מחק פרופיל** \> **שמור**.</span><span class="sxs-lookup"><span data-stu-id="e96ca-127">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="e96ca-128">כאשר תמחק פרופיל, הוא יוסר מהכשיר או מקבוצת המכשירים שלהם הוא הוקצה.</span><span class="sxs-lookup"><span data-stu-id="e96ca-128">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="e96ca-129">הסרת פרופיל</span><span class="sxs-lookup"><span data-stu-id="e96ca-129">Remove a profile</span></span>

1. <span data-ttu-id="e96ca-130">בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="e96ca-130">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="e96ca-131">לחץ על תיבת הסימון לצד שם מכשיר בלוח **מכשיר**, בחר **ללא** בתפריט הנפתח **פרופיל שהוקצה** \> **שמור**.</span><span class="sxs-lookup"><span data-stu-id="e96ca-131">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span></span>
    
