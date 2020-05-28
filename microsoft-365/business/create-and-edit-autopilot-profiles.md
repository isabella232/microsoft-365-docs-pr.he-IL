---
title: יצירה ועריכה של פרופילי AutoPilot
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: למד ליצור פרופיל טייס אוטומטי ולהחיל אותו על התקן, כמו גם לערוך או למחוק פרופיל או להסיר פרופיל מהתקן.
ms.openlocfilehash: e58418813ed0b4d23a5fa7e1d23aae33d8850e7f
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400973"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="8a7a1-103">יצירה ועריכה של פרופילי AutoPilot</span><span class="sxs-lookup"><span data-stu-id="8a7a1-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="8a7a1-104">יצירת פרופיל</span><span class="sxs-lookup"><span data-stu-id="8a7a1-104">Create a profile</span></span>

<span data-ttu-id="8a7a1-105">פרופיל חל על מכשיר או על קבוצה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="8a7a1-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="8a7a1-106">במרכז הניהול של Microsoft 365, בחר **התקנים** \> **טייס אוטומטי**.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-106">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="8a7a1-107">בעמוד **הטייס האוטומטי** , בחרו בכרטיסייה ' **פרופילים** ' כדי \> **ליצור פרופיל**.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="8a7a1-108">בדף **יצירת פרופיל** , הזן שם עבור הפרופיל שמסייע לך לזהות אותו, לדוגמה שיווק.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing.</span></span> <span data-ttu-id="8a7a1-109">הפעל את ההגדרה הרצויה ולאחר מכן בחר **בשמור**.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-109">Turn on the setting you want, and then choose **Save**.</span></span> <span data-ttu-id="8a7a1-110">לקבלת מידע נוסף אודות הגדרות פרופיל טייס אוטומטי, ראה [אודות הגדרות פרופיל טייס אוטומטי](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="8a7a1-110">For more information about AutoPilot profile settings, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="8a7a1-112">החלת פרופיל על מכשיר</span><span class="sxs-lookup"><span data-stu-id="8a7a1-112">Apply profile to a device</span></span>

<span data-ttu-id="8a7a1-113">לאחר יצירת פרופיל, באפשרותך להחילו על התקן או על קבוצת התקנים.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-113">After you create a profile, you can apply it to a device or a group of devices.</span></span> <span data-ttu-id="8a7a1-114">באפשרותך לבחור פרופיל קיים [במדריך שלב-אחר-שלב](add-autopilot-devices-and-profile.md) ולהחילו על התקנים חדשים, או להחליף פרופיל קיים עבור התקן או קבוצת התקנים.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-114">You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md) and apply it to new devices, or replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="8a7a1-115">בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-115">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="8a7a1-116">בחר בתיבת הסימון שליד שם התקן, ובחלונית **ההתקן** , בחר פרופיל מהרשימה הנפתחת **פרופיל שהוקצה** \> **שמור**.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-116">Select the check box next to a device name, and in the **Device** panel, choose a profile from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="8a7a1-118">עריכה, מחיקה או הסרה של פרופיל</span><span class="sxs-lookup"><span data-stu-id="8a7a1-118">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="8a7a1-p103">לאחר שהקצית פרופיל למכשיר, תוכל לעדכן אותו גם אם כבר נתת את המכשיר למשתמש. כאשר המכשיר יתחבר לאינטרנט, הוא יוריד את הגירסה העדכנית ביותר של הפרופיל שלך במהלך תהליך ההתקנה. אם המשתמש משחזר את המכשיר שלו את להגדרות ברירת המחדל של היצרן, המכשיר יוריד שוב את העדכונים האחרונים לפרופיל שלך.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-p103">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="8a7a1-122">עריכת פרופיל</span><span class="sxs-lookup"><span data-stu-id="8a7a1-122">Edit a profile</span></span>

1. <span data-ttu-id="8a7a1-123">בדף **הכנת Windows**, בחר בכרטיסיה **פרופילים**.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-123">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="8a7a1-124">בחר בתיבת הסימון לצד שם התקן, ובחלונית **הפרופיל** , עדכן כל אחת מההגדרות הזמינות \> **שמור**.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-124">Select the check box next to a device name, and in the **Profile** panel, update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="8a7a1-125">אם תבצע פעולות אלה לפני שהמשתמש יחבר את המכשיר לאינטרנט, הפרופיל יוחל על תהליך ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-125">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="8a7a1-126">מחיקת פרופיל</span><span class="sxs-lookup"><span data-stu-id="8a7a1-126">Delete a profile</span></span>

1. <span data-ttu-id="8a7a1-127">בדף **הכנת Windows**, בחר בכרטיסיה **פרופילים**.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-127">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="8a7a1-128">בחרו בתיבת הסימון שליד שם התקן, ובחלונית ' **פרופיל** ', בחרו ' **מחק פרופיל** \> **שמור**'.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-128">Select the check box next to a device name, and in the **Profile** panel, select **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="8a7a1-129">כאשר תמחק פרופיל, הוא יוסר מהכשיר או מקבוצת המכשירים שלהם הוא הוקצה.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-129">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="8a7a1-130">הסרת פרופיל</span><span class="sxs-lookup"><span data-stu-id="8a7a1-130">Remove a profile</span></span>

1. <span data-ttu-id="8a7a1-131">בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-131">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="8a7a1-132">בחר בתיבת הסימון שליד שם התקן, ובחלונית **ההתקן** , בחר **בללא** מתוך הרשימה הנפתחת **פרופיל שהוקצתה** \> **Save**.</span><span class="sxs-lookup"><span data-stu-id="8a7a1-132">Select the check box next to a device name, and in the **Device** panel, choose **None** from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
