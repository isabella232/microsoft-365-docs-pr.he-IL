---
title: עריכה או הגדרה של הגדרות הגנה של יישומים עבור מכשירי Windows 10
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: למד כיצד ליצור או לערוך מדיניות של ניהול יישומים ולהגן על קבצי עבודה במכשירי Windows 10 אישיים של משתמשים.
ms.openlocfilehash: 64c6aa620171a373cd7564c7de3abbf4a4546c4e
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912821"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="ffe7c-103">הגדרה או עריכה של הגדרות הגנה של יישומים עבור מכשירי Windows 10</span><span class="sxs-lookup"><span data-stu-id="ffe7c-103">Set or edit application protection settings for Windows 10 devices</span></span>

<span data-ttu-id="ffe7c-104">מאמר זה חל על Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="edit-an-app-management-policy-for-windows-10"></a><span data-ttu-id="ffe7c-105">עריכת מדיניות ניהול יישומים עבור Windows 10</span><span class="sxs-lookup"><span data-stu-id="ffe7c-105">Edit an app management policy for Windows 10</span></span>

1. <span data-ttu-id="ffe7c-106">עבור אל מרכז הניהול ב <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> -.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>     
2. <span data-ttu-id="ffe7c-107">בסרגל הניווט הימני  , בחר \> **מדיניות** מכשירים.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-107">On the left nav, choose **Devices** \> **Policies** .</span></span>
1. <span data-ttu-id="ffe7c-108">בחר מדיניות קיימת של Windows app ולאחר מכן **ערוך**.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-108">Choose an existing Windows app policy and then **Edit**.</span></span>
1. <span data-ttu-id="ffe7c-109">בחר **ערוך** לצד הגדרה שברצונך לשנות ולאחר מכן **שמור**.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-109">Choose **Edit** next to a setting you want to change and then **Save**.</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="ffe7c-110">יצירת מדיניות לניהול יישומים עבור Windows 10</span><span class="sxs-lookup"><span data-stu-id="ffe7c-110">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="ffe7c-111">אם למשתמשים שלך יש מכשירים אישיים של Windows 10 שהם מבצעים דרכם משימות עבודה, באפשרותך להגן על הנתונים שלך גם במכשירים אלה.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-111">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="ffe7c-112">עבור אל מרכז הניהול ב <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> -.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
2. <span data-ttu-id="ffe7c-113">בסרגל הניווט הימני  , בחר באפשרות \> הוסף **מדיניות** מכשירים \> .</span><span class="sxs-lookup"><span data-stu-id="ffe7c-113">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
3. <span data-ttu-id="ffe7c-114">בחלונית **הוסף מדיניות**, הזן שם ייחודי עבור מדיניות זו.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-114">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
4. <span data-ttu-id="ffe7c-115">תחת **סוג מדיניות**, בחר **ניהול יישומים עבור Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-115">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
5. <span data-ttu-id="ffe7c-116">תחת **סוג מכשיר**, בחר **אישית** או **חברה בבעלות**.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-116">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
6. <span data-ttu-id="ffe7c-117">האפשרות **הצפן קבצי עבודה** מופעלת באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-117">The **Encrypt work files** is turned on automatically.</span></span> 
7. <span data-ttu-id="ffe7c-118">קבע את ההגדרה **מנע ממשתמשים להעתיק נתוני חברה לקבצים אישיים וכפה עליהם לשמור קבצי עבודה ב- OneDrive for Business** למצב **מופעל** אם אינך מעוניין שהמשתמשים ישמרו קבצי עבודה במחשב שלהם.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-118">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
9. <span data-ttu-id="ffe7c-119">הרחב את **שחזור הנתונים במכשירי Windows**.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-119">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="ffe7c-120">**מומלץ להפעיל** אותה.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-120">We recommend that you turn it **On**.</span></span>
    <span data-ttu-id="ffe7c-121">לפני שתוכל לנווט אל מיקום האישור של סוכן שחזור הנתונים, עליך תחילה ליצור את האישור.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-121">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="ffe7c-122">לקבלת הוראות, ראה [יצירה ואימות של אישור סוכן שחזור נתונים (EFS) של מערכת קבצים מצפינה (EFS](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)).</span><span class="sxs-lookup"><span data-stu-id="ffe7c-122">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate).</span></span>
    
    <span data-ttu-id="ffe7c-123">כברירת מחדל, קבצי עבודה מוצפנים באמצעות מפתח סודי שמאוחסן במכשיר ומשויך לפרופיל של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-123">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="ffe7c-124">רק המשתמש יכול לפתוח ולפענח את הקובץ.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-124">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="ffe7c-125">עם זאת, במקרה של אובדן המכשיר או הסרת משתמש, הקובץ יכול להיתקע במצב מוצפן.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-125">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="ffe7c-126">מנהל מערכת יכול להשתמש באישור סוכן שחזור נתונים (DRA) כדי לפענח את הקובץ.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-126">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="ffe7c-128">הרחב את **ההגנה על מיקומים נוספים ברשת ובענן** אם ברצונך להוסיף תחומים נוספים או מיקומים של SharePoint Online כדי לוודא שהקבצים בכל היישומים הרשומים מוגנים.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-128">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="ffe7c-129">אם עליך להזין יותר מפריט אחד עבור שדה כלשהו, השתמש בנקודה-פסיק (;) בין הפריטים.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-129">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="ffe7c-p104">לאחר מכן החלט **מי יקבל הגדרות אלה?** אם אינך מעוניין להשתמש בקבוצת האבטחה המוגדרת כברירת מחדל **כל המשתמשים**, בחר **שינוי**, בחר את קבוצות האבטחה שיקבלו הגדרות אלה \> **בחר**.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
12. <span data-ttu-id="ffe7c-133">לבסוף, בחר **הוסף** כדי לשמור את המדיניות והקצה אותה למכשירים.</span><span class="sxs-lookup"><span data-stu-id="ffe7c-133">Finally, choose **Add** to save the policy, and assign it to devices.</span></span>