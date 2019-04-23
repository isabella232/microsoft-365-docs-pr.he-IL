---
title: שימוש במדריך שלב אחר שלב להוספת מכשירים ופרופיל של Autopilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: למד כיצד להשתמש AutoPilot של Windows כדי להתקין התקנים חדשים של Windows 10 עבור העסק שלך.
ms.openlocfilehash: e0802ddcc0964d0b8d102f7dbdb9116b33cdcf58
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277114"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="b4f52-103">שימוש במדריך שלב אחר שלב להוספת מכשירים ופרופיל של Autopilot</span><span class="sxs-lookup"><span data-stu-id="b4f52-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="b4f52-104">באפשרותך להשתמש ב- Windows Autopilot כדי להגדיר מכשירים חדשים של Windows 10 עבור העסק שלך, כך שהם יהיו מוכנים לשימוש פרודוקטיבי ברגע שתספק אותם לעובדים שלך.</span><span class="sxs-lookup"><span data-stu-id="b4f52-104">You can use Windows AutoPilot to set up new Windows 10 devices for your business so they are ready for productive use as soon as you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="b4f52-105">דרישות המכשירים</span><span class="sxs-lookup"><span data-stu-id="b4f52-105">Device requirements</span></span>

<span data-ttu-id="b4f52-106">המכשירים צריכים לעמוד בדרישות אלה:</span><span class="sxs-lookup"><span data-stu-id="b4f52-106">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="b4f52-107">Windows ,10 גירסה 1703 ואילך.</span><span class="sxs-lookup"><span data-stu-id="b4f52-107">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="b4f52-108">מכשירים חדשים שאינם נחשבים כמוצר Windows מוכן לשימוש.</span><span class="sxs-lookup"><span data-stu-id="b4f52-108">New devices that have not been through Windows out-of-box experience.</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="b4f52-109">שימוש במדריך ההתקנה ליצירת מכשירים ופרופילים</span><span class="sxs-lookup"><span data-stu-id="b4f52-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="b4f52-110">אם עדיין לא יצרת קבוצות מכשירים או פרופילים, הדרך הטובה ביותר להתחיל היא באמצעות מדריך צעד-אחר-צעד, אך תוכל גם [להוסיף מכשירים](create-and-edit-autopilot-devices.md) ו [להקצות להם פרופילים](create-and-edit-autopilot-profiles.md) מבלי להשתמש במדריך.</span><span class="sxs-lookup"><span data-stu-id="b4f52-110">If you have no device groups or profiles created yet, the best way to get started is by using the step-by-step guide, but you can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="b4f52-111">במרכז הניהול של Microsoft 365 Business, אתר כרטיס **פעולות מכשיר** ובחר **פרוס את Windows באמצעות AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="b4f52-111">In the Microsoft 365 Business admin center, locate the **Device actions** card, and choose **Deploy Windows with Autopilot**.</span></span>
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="b4f52-113">בכרטיסיה **הכנת Windows**, לחץ או הקש על **מדריך התחלה**.</span><span class="sxs-lookup"><span data-stu-id="b4f52-113">On the **Prepare Windows** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="b4f52-p101">בדף **העלאת קובץ ‎.csv עם רשימת מכשירים**, אתר את המיקומים שבהם נמצא קובץ ה- ‎.CSV המוכן, ולאחר מכן לחץ על **פתח** \> **הבא**. הקובץ אמור להכיל שלוש כותרות:</span><span class="sxs-lookup"><span data-stu-id="b4f52-p101">On the **Upload .csv file with list of devices** page, browse to a locations where you have the prepared .CSV file, then **Open** \> **Next**. The file should have three headers:</span></span>
    
  - <span data-ttu-id="b4f52-117">עמודה א: מספר סידורי של המכשיר</span><span class="sxs-lookup"><span data-stu-id="b4f52-117">Column A: Device Serial Number</span></span>
    
  - <span data-ttu-id="b4f52-118">עמודה ב: מזהה המוצר של Windows</span><span class="sxs-lookup"><span data-stu-id="b4f52-118">Column B: Windows Product ID</span></span>
    
  - <span data-ttu-id="b4f52-119">עמודה ג: קוד Hash של החומרה</span><span class="sxs-lookup"><span data-stu-id="b4f52-119">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="b4f52-120">ניתן לקבל מידע זה מספק החומרה, או להשתמש ב[קובץ Script של PowerShell, ‏Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) שייצור קובץ csv.</span><span class="sxs-lookup"><span data-stu-id="b4f52-120">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a CSV file.</span></span> 
    
    <span data-ttu-id="b4f52-p102">למידע נוסף, ראה [קובץ CSV עם רשימת מכשירים](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). באפשרותך גם להוריד קובץ לדוגמה בדף **העלאת קובץ ‎.csv עם רשימת מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="b4f52-p102">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="b4f52-p103">בדף **הקצאת פרופיל**, תוכל לבחור פרופיל קיים או ליצור פרופיל חדש. אם עדיין אין לך חשבון, תתבקש ליצור חשבון חדש.</span><span class="sxs-lookup"><span data-stu-id="b4f52-p103">On the **Assign a profile** page, you can either pick an existing profile, or create a new one. If you don't have one yet, you will be prompted to create a new one.</span></span> 
    
    <span data-ttu-id="b4f52-125">פרופיל הוא אוסף הגדרות שניתן להחיל על מכשיר בודד או על קבוצה של מכשירים.</span><span class="sxs-lookup"><span data-stu-id="b4f52-125">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="b4f52-p104">תכונות ברירת המחדל נדרשות ויוגדרו באופן אוטומטי. תכונות ברירת המחדל הן:</span><span class="sxs-lookup"><span data-stu-id="b4f52-p104">The default features are required and will be set automatically. The default features are:</span></span>
    
  - <span data-ttu-id="b4f52-128">דילוג על רישום Cortana‏, OneDrive ו- OEM.</span><span class="sxs-lookup"><span data-stu-id="b4f52-128">Cortana, OneDrive and OEM registration is skipped.</span></span>
    
  - <span data-ttu-id="b4f52-129">יצירת חוויית כניסה עם מותג החברה.</span><span class="sxs-lookup"><span data-stu-id="b4f52-129">Create sign-in experience with your company brand.</span></span>
    
  - <span data-ttu-id="b4f52-130">המכשירים שלך עומדים להתחבר לחשבונות Azure Active Directory ולהירשם באופן אוטומטי לניהול על-ידי Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="b4f52-130">Your devices are going to be connected to Azure Active Directory accounts and automatically enrolled to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="b4f52-131">לקבלת מידע נוסף, ראה</span><span class="sxs-lookup"><span data-stu-id="b4f52-131">For more information, see</span></span>
    
    <span data-ttu-id="b4f52-132">[אודות ההגדרות של פרופיל AutoPilot](autopilot-profile-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="b4f52-132">[About AutoPilot Profile settings](autopilot-profile-settings.md) .</span></span> 
    
5. <span data-ttu-id="b4f52-133">שאר ההגדרות הן **דלג על הגדרות פרטיות** ו **אל תאפשר למשתמש להפוך למנהל המערכת המקומי**. שתי הגדרות אלה מוגדרות למצב **כבוי** כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="b4f52-133">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="b4f52-134">בחר **הבא**.</span><span class="sxs-lookup"><span data-stu-id="b4f52-134">Choose **Next**.</span></span>
    
6. <span data-ttu-id="b4f52-p105">הדף **סיום** מציין שהפרופיל שיצרת (או בחרת) יוחל על קבוצת המכשירים שיצרת על-ידי העלאת רשימת המכשירים. הגדרות אלה ייכנסו לתוקף בפעם הבאה שמשתמשי המכשיר ייכנסו אליו. בחר **סגור**.</span><span class="sxs-lookup"><span data-stu-id="b4f52-p105">**You're done** page indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices. These settings will be in effect when the device users sign in next. Choose **Close**.</span></span>
    