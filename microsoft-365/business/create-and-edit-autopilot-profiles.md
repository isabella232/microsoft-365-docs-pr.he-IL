---
title: יצירה ועריכה של פרופילי AutoPilot
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
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'למד כיצד ליצור, לערוך, למחוק או להסיר פרופילי AutoPilot. '
ms.openlocfilehash: 7987cafb3ea234d81be72c79aee8e584a3770875
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34073489"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="451c0-103">יצירה ועריכה של פרופילי AutoPilot</span><span class="sxs-lookup"><span data-stu-id="451c0-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="451c0-104">יצירת פרופיל</span><span class="sxs-lookup"><span data-stu-id="451c0-104">Create a profile</span></span>

<span data-ttu-id="451c0-105">פרופיל חל על מכשיר או על קבוצה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="451c0-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="451c0-106">במרכז הניהול העסקי של Microsoft 365, בחר **התקנים** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="451c0-106">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="451c0-107">בדף **AutoPilot** , בחר את הכרטיסייה **פרופילי** \> **צור פרופיל**.</span><span class="sxs-lookup"><span data-stu-id="451c0-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="451c0-108">בדף **יצירת פרופיל**, הזן שם עבור הפרופיל שיעזור לך לזהות אותו, לדוגמה, שיווק, הפעל את ההגדרה הרצויה (למידע נוסף, ראה [אודות ההגדרות של פרופיל AutoPilot](autopilot-profile-settings.md)), ובחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="451c0-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing, turn on the setting you want (see [About AutoPilot Profile settings](autopilot-profile-settings.md) for more information), and choose **Save**.</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="451c0-110">החלת פרופיל על מכשיר</span><span class="sxs-lookup"><span data-stu-id="451c0-110">Apply profile to a device</span></span>

<span data-ttu-id="451c0-p101">לאחר שתיצור פרופיל, תוכל להחיל אותו על מכשיר או על קבוצה של מכשירים. תוכל לבחור פרופיל קיים ב[מדריך צעד-אחד-צעד](add-autopilot-devices-and-profile.md), תוכל להחיל אותו על מכשירים חדשים או תוכל להחליף פרופיל קיים עבור מכשיר או קבוצת מכשירים.</span><span class="sxs-lookup"><span data-stu-id="451c0-p101">After you create a profile you can apply it to a device or a group of devices. You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md), you can apply it to new devices, or you can replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="451c0-113">בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="451c0-113">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="451c0-114">לחץ על תיבת הסימון לצד שם מכשיר בלוח **מכשיר**, בחר פרופיל בתפריט הנפתח **פרופיל שהוקצה** \> **שמור**.</span><span class="sxs-lookup"><span data-stu-id="451c0-114">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="451c0-116">עריכה, מחיקה או הסרה של פרופיל</span><span class="sxs-lookup"><span data-stu-id="451c0-116">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="451c0-p102">לאחר שהקצית פרופיל למכשיר, תוכל לעדכן אותו גם אם כבר נתת את המכשיר למשתמש. כאשר המכשיר יתחבר לאינטרנט, הוא יוריד את הגירסה העדכנית ביותר של הפרופיל שלך במהלך תהליך ההתקנה. אם המשתמש משחזר את המכשיר שלו את להגדרות ברירת המחדל של היצרן, המכשיר יוריד שוב את העדכונים האחרונים לפרופיל שלך.</span><span class="sxs-lookup"><span data-stu-id="451c0-p102">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="451c0-120">עריכת פרופיל</span><span class="sxs-lookup"><span data-stu-id="451c0-120">Edit a profile</span></span>

1. <span data-ttu-id="451c0-121">בדף **הכנת Windows**, בחר בכרטיסיה **פרופילים**.</span><span class="sxs-lookup"><span data-stu-id="451c0-121">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="451c0-122">לחץ על תיבת הסימון לצד שם מכשיר, ובלוח **פרופיל** עדכן אחת מההגדרות הזמינות \> **שמור**.</span><span class="sxs-lookup"><span data-stu-id="451c0-122">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="451c0-123">אם תבצע פעולות אלה לפני שהמשתמש יחבר את המכשיר לאינטרנט, הפרופיל יוחל על תהליך ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="451c0-123">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="451c0-124">מחיקת פרופיל</span><span class="sxs-lookup"><span data-stu-id="451c0-124">Delete a profile</span></span>

1. <span data-ttu-id="451c0-125">בדף **הכנת Windows**, בחר בכרטיסיה **פרופילים**.</span><span class="sxs-lookup"><span data-stu-id="451c0-125">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="451c0-126">לחץ על תיבת הסימון לצד שם מכשיר, ובלוח **פרופיל** לחץ על **מחק פרופיל** \> **שמור**.</span><span class="sxs-lookup"><span data-stu-id="451c0-126">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="451c0-127">כאשר תמחק פרופיל, הוא יוסר מהכשיר או מקבוצת המכשירים שלהם הוא הוקצה.</span><span class="sxs-lookup"><span data-stu-id="451c0-127">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="451c0-128">הסרת פרופיל</span><span class="sxs-lookup"><span data-stu-id="451c0-128">Remove a profile</span></span>

1. <span data-ttu-id="451c0-129">בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="451c0-129">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="451c0-130">לחץ על תיבת הסימון לצד שם מכשיר בלוח **מכשיר**, בחר **ללא** בתפריט הנפתח **פרופיל שהוקצה** \> **שמור**.</span><span class="sxs-lookup"><span data-stu-id="451c0-130">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span></span>
    
