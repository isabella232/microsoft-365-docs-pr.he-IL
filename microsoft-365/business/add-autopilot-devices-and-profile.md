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
ms.openlocfilehash: 8c4a14b4b9dcbf7a30c1e6e0bdd53418a1ab8a03
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660670"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="7a3a8-103">שימוש במדריך שלב אחר שלב להוספת מכשירים ופרופיל של Autopilot</span><span class="sxs-lookup"><span data-stu-id="7a3a8-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="7a3a8-104">באפשרותך להשתמש AutoPilot של Windows כדי להגדיר התקנים 10 חלונות **חדשים** עבור העסק שלך, כך הם מוכנים לשימוש יעיל ברגע שתיתן לו את העובדים שלך.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they are ready for productive use as soon as you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="7a3a8-105">דרישות המכשירים</span><span class="sxs-lookup"><span data-stu-id="7a3a8-105">Device requirements</span></span>

<span data-ttu-id="7a3a8-106">המכשירים צריכים לעמוד בדרישות אלה:</span><span class="sxs-lookup"><span data-stu-id="7a3a8-106">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="7a3a8-107">Windows ,10 גירסה 1703 ואילך.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-107">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="7a3a8-108">מכשירים חדשים שאינם נחשבים כמוצר Windows מוכן לשימוש.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-108">New devices that have not been through Windows out-of-box experience.</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="7a3a8-109">שימוש במדריך ההתקנה ליצירת מכשירים ופרופילים</span><span class="sxs-lookup"><span data-stu-id="7a3a8-109">Use the setup guide to create devices and profiles</span></span>

![כרזה המצביעים על https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="7a3a8-111">אם עדיין לא יצרת קבוצות מכשירים או פרופילים, הדרך הטובה ביותר להתחיל היא באמצעות מדריך צעד-אחר-צעד, אך תוכל גם [להוסיף מכשירים](create-and-edit-autopilot-devices.md) ו [להקצות להם פרופילים](create-and-edit-autopilot-profiles.md) מבלי להשתמש במדריך.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-111">If you have no device groups or profiles created yet, the best way to get started is by using the step-by-step guide, but you can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="7a3a8-112">עבור אל מרכז admin ב <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="7a3a8-113">בסרגל ניווט השמאלי לבחור **התקנים** \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-113">On the left nav choose **Devices** \> **AutoPilot**.</span></span>

    ![במרכז admin לבחור התקנים ולאחר מכן AutoPilot.](media/AutoPilot.png)
  
2. <span data-ttu-id="7a3a8-115">בדף **AutoPilot** , לחץ או הקש על **מדריך התחלה**.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-115">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="7a3a8-p101">בדף **העלאת קובץ ‎.csv עם רשימת מכשירים**, אתר את המיקומים שבהם נמצא קובץ ה- ‎.CSV המוכן, ולאחר מכן לחץ על **פתח** \> **הבא**. הקובץ אמור להכיל שלוש כותרות:</span><span class="sxs-lookup"><span data-stu-id="7a3a8-p101">On the **Upload .csv file with list of devices** page, browse to a locations where you have the prepared .CSV file, then **Open** \> **Next**. The file should have three headers:</span></span>
    
  - <span data-ttu-id="7a3a8-119">עמודה א: מספר סידורי של המכשיר</span><span class="sxs-lookup"><span data-stu-id="7a3a8-119">Column A: Device Serial Number</span></span>
    
  - <span data-ttu-id="7a3a8-120">עמודה ב: מזהה המוצר של Windows</span><span class="sxs-lookup"><span data-stu-id="7a3a8-120">Column B: Windows Product ID</span></span>
    
  - <span data-ttu-id="7a3a8-121">עמודה ג: קוד Hash של החומרה</span><span class="sxs-lookup"><span data-stu-id="7a3a8-121">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="7a3a8-122">ניתן לקבל מידע זה מספק החומרה, או להשתמש ב[קובץ Script של PowerShell, ‏Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) שייצור קובץ csv.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-122">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a CSV file.</span></span> 
    
    <span data-ttu-id="7a3a8-p102">למידע נוסף, ראה [קובץ CSV עם רשימת מכשירים](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). באפשרותך גם להוריד קובץ לדוגמה בדף **העלאת קובץ ‎.csv עם רשימת מכשירים**.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-p102">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="7a3a8-p103">בדף **הקצאת פרופיל**, תוכל לבחור פרופיל קיים או ליצור פרופיל חדש. אם עדיין אין לך חשבון, תתבקש ליצור חשבון חדש.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-p103">On the **Assign a profile** page, you can either pick an existing profile, or create a new one. If you don't have one yet, you will be prompted to create a new one.</span></span> 
    
    <span data-ttu-id="7a3a8-127">פרופיל הוא אוסף הגדרות שניתן להחיל על מכשיר בודד או על קבוצה של מכשירים.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-127">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="7a3a8-p104">תכונות ברירת המחדל נדרשות ויוגדרו באופן אוטומטי. תכונות ברירת המחדל הן:</span><span class="sxs-lookup"><span data-stu-id="7a3a8-p104">The default features are required and will be set automatically. The default features are:</span></span>
    
  - <span data-ttu-id="7a3a8-130">דילוג על רישום Cortana‏, OneDrive ו- OEM.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-130">Cortana, OneDrive and OEM registration is skipped.</span></span>
    
  - <span data-ttu-id="7a3a8-131">יצירת חוויית כניסה עם מותג החברה.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-131">Create sign-in experience with your company brand.</span></span>
    
  - <span data-ttu-id="7a3a8-132">המכשירים שלך עומדים להתחבר לחשבונות Azure Active Directory ולהירשם באופן אוטומטי לניהול על-ידי Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-132">Your devices are going to be connected to Azure Active Directory accounts and automatically enrolled to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="7a3a8-133">לקבלת מידע נוסף, ראה</span><span class="sxs-lookup"><span data-stu-id="7a3a8-133">For more information, see</span></span>
    
    <span data-ttu-id="7a3a8-134">[אודות ההגדרות של פרופיל AutoPilot](autopilot-profile-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="7a3a8-134">[About AutoPilot Profile settings](autopilot-profile-settings.md) .</span></span> 
    
5. <span data-ttu-id="7a3a8-135">שאר ההגדרות הן **דלג על הגדרות פרטיות** ו **אל תאפשר למשתמש להפוך למנהל המערכת המקומי**. שתי הגדרות אלה מוגדרות למצב **כבוי** כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="7a3a8-136">בחר **הבא**.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="7a3a8-p105">הדף **סיום** מציין שהפרופיל שיצרת (או בחרת) יוחל על קבוצת המכשירים שיצרת על-ידי העלאת רשימת המכשירים. הגדרות אלה ייכנסו לתוקף בפעם הבאה שמשתמשי המכשיר ייכנסו אליו. בחר **סגור**.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-p105">**You're done** page indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices. These settings will be in effect when the device users sign in next. Choose **Close**.</span></span>
    