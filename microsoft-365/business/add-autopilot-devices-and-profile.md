---
title: שימוש במדריך שלב אחר שלב להוספת מכשירים ופרופיל של Autopilot
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: למד כיצד להשתמש בטייס אוטומטי של Windows כדי להגדיר התקנים חדשים של Windows 10 עבור העסק שלך כך שהם מוכנים לשימוש בעובדים.
ms.openlocfilehash: de14012ebf9e7cdd22e41505f316ab665773c670
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165880"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="e8fab-103">שימוש במדריך שלב אחר שלב להוספת מכשירים ופרופיל של Autopilot</span><span class="sxs-lookup"><span data-stu-id="e8fab-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="e8fab-104">באפשרותך להשתמש בטייס אוטומטי של Windows כדי להגדיר windows **חדש** 10 התקנים עבור העסק שלך כך שהם מוכנים לשימוש כאשר אתה נותן אותם לעובדים שלך.</span><span class="sxs-lookup"><span data-stu-id="e8fab-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="e8fab-105">דרישות המכשירים</span><span class="sxs-lookup"><span data-stu-id="e8fab-105">Device requirements</span></span>

<span data-ttu-id="e8fab-106">על התקנים לעמוד בדרישות הבאות:</span><span class="sxs-lookup"><span data-stu-id="e8fab-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="e8fab-107">Windows 10, גירסה 1703 ואילך</span><span class="sxs-lookup"><span data-stu-id="e8fab-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="e8fab-108">מכשירים חדשים שלא עברו חוויה מחוץ לקופסא של Windows</span><span class="sxs-lookup"><span data-stu-id="e8fab-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="e8fab-109">שימוש במדריך ההתקנה ליצירת מכשירים ופרופילים</span><span class="sxs-lookup"><span data-stu-id="e8fab-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="e8fab-110">[![תווית המיידעת אותך שמרכז הניהול משתנה ושניתן למצוא פרטים נוספים ב- aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="e8fab-110">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="e8fab-111">אם עדיין לא יצרת קבוצות או פרופילים של התקנים, הדרך הטובה ביותר להתחיל היא באמצעות המדריך צעד-אחר-צעד.</span><span class="sxs-lookup"><span data-stu-id="e8fab-111">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="e8fab-112">באפשרותך גם [להוסיף התקנים](create-and-edit-autopilot-devices.md) [ולהקצות אליהם פרופילים](create-and-edit-autopilot-profiles.md) מבלי להשתמש במדריך.</span><span class="sxs-lookup"><span data-stu-id="e8fab-112">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="e8fab-113"><a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. לך למרכז המנהלה</span><span class="sxs-lookup"><span data-stu-id="e8fab-113">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="e8fab-114">בחלונית הניווט השמאלית, בחר באפשרות **התקנים** \> **טייס אוטומטי**.</span><span class="sxs-lookup"><span data-stu-id="e8fab-114">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![במרכז הניהול, בחר התקנים ולאחר מכן טייס אוטומטי.](../media/AutoPilot.png)
  
2. <span data-ttu-id="e8fab-116">בעמוד **הטייס האוטומטי** , לחץ או הקש על **התחל מדריך**.</span><span class="sxs-lookup"><span data-stu-id="e8fab-116">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="e8fab-118">בקובץ **העלאה. csv עם רשימת ההתקנים** , אתר את המיקום שבו הכנת את הרשימה. קובץ CSV ולאחר מכן **פתח את** \> **הבא**.</span><span class="sxs-lookup"><span data-stu-id="e8fab-118">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="e8fab-119">הקובץ חייב לכלול שלוש כותרות:</span><span class="sxs-lookup"><span data-stu-id="e8fab-119">The file must have three headers:</span></span>
    
    - <span data-ttu-id="e8fab-120">עמודה א: מספר סידורי של המכשיר</span><span class="sxs-lookup"><span data-stu-id="e8fab-120">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="e8fab-121">עמודה ב: מזהה המוצר של Windows</span><span class="sxs-lookup"><span data-stu-id="e8fab-121">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="e8fab-122">עמודה ג: קוד Hash של החומרה</span><span class="sxs-lookup"><span data-stu-id="e8fab-122">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="e8fab-123">אתה יכול לקבל את המידע הזה מספק החומרה שלך, או שאתה יכול להשתמש [בסקריפט לקבל-Windowsautopilinfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) כדי ליצור קובץ CSV.</span><span class="sxs-lookup"><span data-stu-id="e8fab-123">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="e8fab-p103">למידע נוסף, ראה [קובץ CSV עם רשימת מכשירים](https://docs.microsoft.com/microsoft-365/admin/misc/device-list). באפשרותך גם להוריד קובץ לדוגמה בדף **העלאת קובץ ‎.csv עם רשימת מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="e8fab-p103">For more information, see [Device list CSV-file](https://docs.microsoft.com/microsoft-365/admin/misc/device-list). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="e8fab-126">בדף **הקצאת פרופיל** , באפשרותך לבחור פרופיל קיים או ליצור דף חדש.</span><span class="sxs-lookup"><span data-stu-id="e8fab-126">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="e8fab-127">אם עדיין אין לך אחד, תתבקש ליצור אחד.</span><span class="sxs-lookup"><span data-stu-id="e8fab-127">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="e8fab-128">פרופיל הוא אוסף הגדרות שניתן להחיל על מכשיר בודד או על קבוצה של מכשירים.</span><span class="sxs-lookup"><span data-stu-id="e8fab-128">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="e8fab-129">תכונות ברירת המחדל נדרשות ומוגדרות באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="e8fab-129">The default features are required and are set automatically.</span></span> <span data-ttu-id="e8fab-130">תכונות ברירת המחדל הן:</span><span class="sxs-lookup"><span data-stu-id="e8fab-130">The default features are:</span></span>
    
    - <span data-ttu-id="e8fab-131">לדלג קורטנה, OneDrive, ו-OEM רישום.</span><span class="sxs-lookup"><span data-stu-id="e8fab-131">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="e8fab-132">יצירת חוויית כניסה עם מותג החברה.</span><span class="sxs-lookup"><span data-stu-id="e8fab-132">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="e8fab-133">חבר את המכשירים שלך לחשבונות מדריך הפעלה התכלת, ורשום אותם באופן אוטומטי כדי שינוהל על-ידי Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="e8fab-133">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business Premium.</span></span>
    
    <span data-ttu-id="e8fab-134">לקבלת מידע נוסף, ראה [אודות הגדרות פרופיל טייס אוטומטי](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="e8fab-134">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="e8fab-135">שאר ההגדרות הן **דלג על הגדרות פרטיות** ו **אל תאפשר למשתמש להפוך למנהל המערכת המקומי**. שתי הגדרות אלה מוגדרות למצב **כבוי** כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="e8fab-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="e8fab-136">בחר **הבא**.</span><span class="sxs-lookup"><span data-stu-id="e8fab-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="e8fab-137">**סיימת** מציין שהפרופיל שיצרת (או בחרת) יוחל על קבוצת ההתקנים שיצרת על-ידי טעינת רשימת ההתקנים.</span><span class="sxs-lookup"><span data-stu-id="e8fab-137">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="e8fab-138">ההגדרות ייכנסו לתוקף כאשר משתמשי ההתקן ייכנסו בשלב הבא.</span><span class="sxs-lookup"><span data-stu-id="e8fab-138">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="e8fab-139">בחר **סגור**.</span><span class="sxs-lookup"><span data-stu-id="e8fab-139">Choose **Close**.</span></span>
    
