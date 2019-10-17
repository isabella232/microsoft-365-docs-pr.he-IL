---
title: קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: למד כיצד ליצור מדיניות ניהול יישומים ולהגן על קבצי עבודה בהתקני Windows 10.
ms.openlocfilehash: 0e1221e533418166b80afd94431414016774f247
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575777"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="ef4b6-103">קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10</span><span class="sxs-lookup"><span data-stu-id="ef4b6-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="ef4b6-104">יצירת מדיניות לניהול יישומים עבור Windows 10</span><span class="sxs-lookup"><span data-stu-id="ef4b6-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="ef4b6-105">אם למשתמשים שלך יש מכשירים אישיים של Windows 10 שהם מבצעים דרכם משימות עבודה, באפשרותך להגן על הנתונים שלך גם במכשירים אלה.</span><span class="sxs-lookup"><span data-stu-id="ef4b6-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="ef4b6-106"><a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. לך למרכז המנהלה</span><span class="sxs-lookup"><span data-stu-id="ef4b6-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="ef4b6-107">בניווט השמאלי, בחר באפשרות **מדיניות** \> \*\*\*\* **התקנים** \> .</span><span class="sxs-lookup"><span data-stu-id="ef4b6-107">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>

3. <span data-ttu-id="ef4b6-108">בחלונית **הוסף מדיניות**, הזן שם ייחודי עבור מדיניות זו.</span><span class="sxs-lookup"><span data-stu-id="ef4b6-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="ef4b6-109">תחת **סוג מדיניות**, בחר **ניהול יישומים עבור Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="ef4b6-109">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="ef4b6-110">תחת **סוג התקן**, בחר בבעלות **אישית** או **בחברה**.</span><span class="sxs-lookup"><span data-stu-id="ef4b6-110">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="ef4b6-111">האפשרות **הצפן קבצי עבודה** מופעלת באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="ef4b6-111">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="ef4b6-112">קבע את ההגדרה **מנע ממשתמשים להעתיק נתוני חברה לקבצים אישיים וכפה עליהם לשמור קבצי עבודה ב- OneDrive for Business** למצב **מופעל** אם אינך מעוניין שהמשתמשים ישמרו קבצי עבודה במחשב שלהם.</span><span class="sxs-lookup"><span data-stu-id="ef4b6-112">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
9. <span data-ttu-id="ef4b6-113">הרחב את **שחזר נתונים במכשירי Windows** ומומלץ להגדיר את האפשרות למצב **מופעל**.</span><span class="sxs-lookup"><span data-stu-id="ef4b6-113">Expand **Recover data on Windows devices** and it is recommended that you turn it **On**.</span></span>
    
    <span data-ttu-id="ef4b6-p101">לפני שתוכל לנווט אל מיקום האישור של סוכן שחזור הנתונים, עליך תחילה ליצור את האישור. לקבלת הוראות עיין בנושא [יצירה ואימות של אישור מסוג מערכת קבצים מצפינה (EFS) סוכן שחזור נתונים (DRA)](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="ef4b6-p101">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one. For instructions see, [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="ef4b6-p102">כברירת מחדל, קבצי עבודה מוצפנים באמצעות מפתח סודי שמאוחסן במכשיר ומשויך לפרופיל של המשתמש. רק המשתמש יכול לפתוח ולפענח את הקובץ. עם זאת, במקרה של אובדן המכשיר או הסרת משתמש, הקובץ יכול להיתקע במצב מוצפן. מנהל מערכת יכול להשתמש באישור של סוכן שחזור נתונים (DRA) כדי לפענח את הקובץ.</span><span class="sxs-lookup"><span data-stu-id="ef4b6-p102">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile. Only the user can open and decrypt the file. However, if a device is lost or a user is removed, a file can be stuck in an encrypted state. The Data Recovery Agent (DRA) certificate can be used by an admin to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="ef4b6-p103">הרחב את **הגן על מיקומים נוספים ברשת ובענן** אם ברצונך להוסיף תחומים נוספים או מיקומים נוספים של SharePoint Online כדי לוודא שהקבצים בכל היישומים המפורטים יהיו מוגנים. אם עליך להזין יותר מפריט אחד עבור שדה כלשהו, השתמש בנקודה-פסיק (;) בין הפריטים.</span><span class="sxs-lookup"><span data-stu-id="ef4b6-p103">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps will be protected. If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="ef4b6-p104">לאחר מכן החלט **מי יקבל הגדרות אלה?** אם אינך מעוניין להשתמש בקבוצת האבטחה המוגדרת כברירת מחדל **כל המשתמשים**, בחר **שינוי**, בחר את קבוצות האבטחה שיקבלו הגדרות אלה \> **בחר**.</span><span class="sxs-lookup"><span data-stu-id="ef4b6-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="ef4b6-126">לבסוף, בחר **הוסף** כדי לשמור את המדיניות והקצה אותה למכשירים.</span><span class="sxs-lookup"><span data-stu-id="ef4b6-126">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 