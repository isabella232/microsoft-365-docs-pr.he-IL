---
title: עריכה או הגדרה של הגדרות הגנה על יישומים עבור מכשירי Windows 10
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
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
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: למד כיצד ליצור או לערוך מדיניות ניהול אפליקציות ולהגן על קבצי עבודה במכשירי Windows 10 האישיים של המשתמשים שלך.
ms.openlocfilehash: aa270c563e6bdce6fd48f8713d7db3ce23921925
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580013"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="41ed4-103">הגדרה או עריכה של הגדרות הגנת יישומים עבור מכשירי Windows 10</span><span class="sxs-lookup"><span data-stu-id="41ed4-103">Set or edit application protection settings for Windows 10 devices</span></span>

<span data-ttu-id="41ed4-104">מאמר זה חל על Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="41ed4-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="edit-an-app-management-policy-for-windows-10"></a><span data-ttu-id="41ed4-105">עריכת מדיניות ניהול יישומים עבור Windows 10</span><span class="sxs-lookup"><span data-stu-id="41ed4-105">Edit an app management policy for Windows 10</span></span>

1. <span data-ttu-id="41ed4-106">עבור אל מרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> ב- .</span><span class="sxs-lookup"><span data-stu-id="41ed4-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>     
2. <span data-ttu-id="41ed4-107">בסרגל הניווט הימני, בחר **מדיניות** \> **מכשירים** .</span><span class="sxs-lookup"><span data-stu-id="41ed4-107">On the left nav, choose **Devices** \> **Policies** .</span></span>
1. <span data-ttu-id="41ed4-108">בחר מדיניות קיימת של אפליקציית Windows ולאחר מכן **ערוך**.</span><span class="sxs-lookup"><span data-stu-id="41ed4-108">Choose an existing Windows app policy and then **Edit**.</span></span>
1. <span data-ttu-id="41ed4-109">בחר **ערוך** לצד הגדרה שברצונך לשנות ולאחר מכן **שמור**.</span><span class="sxs-lookup"><span data-stu-id="41ed4-109">Choose **Edit** next to a setting you want to change and then **Save**.</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="41ed4-110">יצירת מדיניות לניהול יישומים עבור Windows 10</span><span class="sxs-lookup"><span data-stu-id="41ed4-110">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="41ed4-111">אם למשתמשים שלך יש מכשירים אישיים של Windows 10 שהם מבצעים דרכם משימות עבודה, באפשרותך להגן על הנתונים שלך גם במכשירים אלה.</span><span class="sxs-lookup"><span data-stu-id="41ed4-111">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="41ed4-112">עבור אל מרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> ב- .</span><span class="sxs-lookup"><span data-stu-id="41ed4-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
2. <span data-ttu-id="41ed4-113">בסרגל הניווט הימני, בחר **מדיניות** \> **מכשירים** \> **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="41ed4-113">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
3. <span data-ttu-id="41ed4-114">בחלונית **הוסף מדיניות**, הזן שם ייחודי עבור מדיניות זו.</span><span class="sxs-lookup"><span data-stu-id="41ed4-114">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
4. <span data-ttu-id="41ed4-115">תחת **סוג מדיניות**, בחר **ניהול יישומים עבור Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="41ed4-115">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
5. <span data-ttu-id="41ed4-116">תחת **סוג מכשיר**, בחר אישי **או** **בבעלות חברה.**</span><span class="sxs-lookup"><span data-stu-id="41ed4-116">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
6. <span data-ttu-id="41ed4-117">האפשרות **הצפן קבצי עבודה** מופעלת באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="41ed4-117">The **Encrypt work files** is turned on automatically.</span></span> 
7. <span data-ttu-id="41ed4-118">קבע את ההגדרה **מנע ממשתמשים להעתיק נתוני חברה לקבצים אישיים וכפה עליהם לשמור קבצי עבודה ב- OneDrive for Business** למצב **מופעל** אם אינך מעוניין שהמשתמשים ישמרו קבצי עבודה במחשב שלהם.</span><span class="sxs-lookup"><span data-stu-id="41ed4-118">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
9. <span data-ttu-id="41ed4-119">הרחב **את שחזור נתונים במכשירי Windows**.</span><span class="sxs-lookup"><span data-stu-id="41ed4-119">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="41ed4-120">מומלץ להפעיל **אותו.**</span><span class="sxs-lookup"><span data-stu-id="41ed4-120">We recommend that you turn it **On**.</span></span>
    <span data-ttu-id="41ed4-121">לפני שתוכל לנווט אל מיקום האישור של סוכן שחזור הנתונים, עליך תחילה ליצור את האישור.</span><span class="sxs-lookup"><span data-stu-id="41ed4-121">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="41ed4-122">לקבלת הוראות, ראה יצירה ואימות של אישור סוכן שחזור נתונים (DRA) של מערכת קבצים [מצפינה (EFS).](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)</span><span class="sxs-lookup"><span data-stu-id="41ed4-122">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate).</span></span>
    
    <span data-ttu-id="41ed4-123">כברירת מחדל, קבצי עבודה מוצפנים באמצעות מפתח סודי שמאוחסן במכשיר ומשויך לפרופיל של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="41ed4-123">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="41ed4-124">רק המשתמש יכול לפתוח ולפענח את הקובץ.</span><span class="sxs-lookup"><span data-stu-id="41ed4-124">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="41ed4-125">עם זאת, במקרה של אובדן המכשיר או הסרת משתמש, הקובץ יכול להיתקע במצב מוצפן.</span><span class="sxs-lookup"><span data-stu-id="41ed4-125">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="41ed4-126">מנהל מערכת יכול להשתמש באישור סוכן שחזור נתונים (DRA) כדי לפענח את הקובץ.</span><span class="sxs-lookup"><span data-stu-id="41ed4-126">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="41ed4-128">הרחב **את הגן על מיקומי רשת וענן** נוספים אם ברצונך להוסיף תחומים נוספים או מיקומי SharePoint Online כדי לוודא שהקבצים בכל האפליקציות המפורטות מוגנים.</span><span class="sxs-lookup"><span data-stu-id="41ed4-128">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="41ed4-129">אם עליך להזין יותר מפריט אחד עבור שדה כלשהו, השתמש בנקודה-פסיק (;) בין הפריטים.</span><span class="sxs-lookup"><span data-stu-id="41ed4-129">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="41ed4-p104">לאחר מכן החלט **מי יקבל הגדרות אלה?** אם אינך מעוניין להשתמש בקבוצת האבטחה המוגדרת כברירת מחדל **כל המשתמשים**, בחר **שינוי**, בחר את קבוצות האבטחה שיקבלו הגדרות אלה \> **בחר**.</span><span class="sxs-lookup"><span data-stu-id="41ed4-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
12. <span data-ttu-id="41ed4-133">לבסוף, בחר **הוסף** כדי לשמור את המדיניות והקצה אותה למכשירים.</span><span class="sxs-lookup"><span data-stu-id="41ed4-133">Finally, choose **Add** to save the policy, and assign it to devices.</span></span>