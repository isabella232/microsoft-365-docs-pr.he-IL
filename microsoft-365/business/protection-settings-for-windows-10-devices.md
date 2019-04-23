---
title: קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: למד כיצד ליצור מדיניות ניהול app ולהגן על קבצי עבודה בהתקני Windows 10.
ms.openlocfilehash: 289c6a74f6ccb53f6a833612a7b4a5bcddd3ea56
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32278173"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="4b349-103">קביעת הגדרות הגנה של יישומים עבור מכשירי Windows 10</span><span class="sxs-lookup"><span data-stu-id="4b349-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="4b349-104">יצירת מדיניות לניהול יישומים עבור Windows 10</span><span class="sxs-lookup"><span data-stu-id="4b349-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="4b349-105">אם למשתמשים שלך יש מכשירים אישיים של Windows 10 שהם מבצעים דרכם משימות עבודה, באפשרותך להגן על הנתונים שלך גם במכשירים אלה.</span><span class="sxs-lookup"><span data-stu-id="4b349-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="4b349-106">היכנס אל [מרכז ניהול](https://go.microsoft.com/fwlink/p/?linkid=837890) עם אישורי מנהל כללי.</span><span class="sxs-lookup"><span data-stu-id="4b349-106">Sign in to [admin center](https://go.microsoft.com/fwlink/p/?linkid=837890) with global admin credentials.</span></span> <span data-ttu-id="4b349-107">בחר את האריח **ניהול** כדי לעבור אל מרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="4b349-107">Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="4b349-108">נווט השמאלי, בחר **התקנים** \> **מדיניות** \> **הוספה**.</span><span class="sxs-lookup"><span data-stu-id="4b349-108">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>

3. <span data-ttu-id="4b349-109">בחלונית **הוסף מדיניות**, הזן שם ייחודי עבור מדיניות זו.</span><span class="sxs-lookup"><span data-stu-id="4b349-109">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="4b349-110">תחת **סוג מדיניות**, בחר **ניהול יישומים עבור Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="4b349-110">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="4b349-111">תחת \*\* סוג מכשיר \*\*, בחר **אישי** או **בבעלות של חברה**.</span><span class="sxs-lookup"><span data-stu-id="4b349-111">Under \*\* Device type \*\*, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="4b349-112">האפשרות **הצפן קבצי עבודה** מופעלת באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="4b349-112">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="4b349-113">קבע את ההגדרה **מנע ממשתמשים להעתיק נתוני חברה לקבצים אישיים וכפה עליהם לשמור קבצי עבודה ב- OneDrive for Business** למצב **מופעל** אם אינך מעוניין שהמשתמשים ישמרו קבצי עבודה במחשב שלהם.</span><span class="sxs-lookup"><span data-stu-id="4b349-113">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
8. <span data-ttu-id="4b349-114">הרחב את **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים** \> קבע את תצורת ההגדרות כפי שאתה רוצה.</span><span class="sxs-lookup"><span data-stu-id="4b349-114">Expand **Manage how users access Office files on devices** \> configure the settings how you would like.</span></span> <span data-ttu-id="4b349-115">האפשרות **קבע כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים** מוגדרת ל **מבוטל** כברירת מחדל, אך מומלץ להגדיר אותה למצב **מופעל** ולקבל את ערכי ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="4b349-115">The **Manage how users access Office devices on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="4b349-116">לקבלת מידע נוסף, ראה [הגדרות זמינות](#available-settings).</span><span class="sxs-lookup"><span data-stu-id="4b349-116">See [Available settings](#available-settings)for more information.</span></span> 
    
    <span data-ttu-id="4b349-117">ניתן להשתמש תמיד בקישור **איפוס הגדרות ברירת מחדל** כדי לחזור להגדרת ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="4b349-117">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
9. <span data-ttu-id="4b349-118">הרחב את **שחזר נתונים במכשירי Windows** ומומלץ להגדיר את האפשרות למצב **מופעל**.</span><span class="sxs-lookup"><span data-stu-id="4b349-118">Expand **Recover data on Windows devices** and it is recommended that you turn it **On**.</span></span>
    
    <span data-ttu-id="4b349-p103">לפני שתוכל לנווט אל מיקום האישור של סוכן שחזור הנתונים, עליך תחילה ליצור את האישור. לקבלת הוראות עיין בנושא [יצירה ואימות של אישור מסוג מערכת קבצים מצפינה (EFS) סוכן שחזור נתונים (DRA)](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="4b349-p103">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one. For instructions see, [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="4b349-p104">כברירת מחדל, קבצי עבודה מוצפנים באמצעות מפתח סודי שמאוחסן במכשיר ומשויך לפרופיל של המשתמש. רק המשתמש יכול לפתוח ולפענח את הקובץ. עם זאת, במקרה של אובדן המכשיר או הסרת משתמש, הקובץ יכול להיתקע במצב מוצפן. מנהל מערכת יכול להשתמש באישור של סוכן שחזור נתונים (DRA) כדי לפענח את הקובץ.</span><span class="sxs-lookup"><span data-stu-id="4b349-p104">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile. Only the user can open and decrypt the file. However, if a device is lost or a user is removed, a file can be stuck in an encrypted state. The Data Recovery Agent (DRA) certificate can be used by an admin to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="4b349-p105">הרחב את **הגן על מיקומים נוספים ברשת ובענן** אם ברצונך להוסיף תחומים נוספים או מיקומים נוספים של SharePoint Online כדי לוודא שהקבצים בכל היישומים המפורטים יהיו מוגנים. אם עליך להזין יותר מפריט אחד עבור שדה כלשהו, השתמש בנקודה-פסיק (;) בין הפריטים.</span><span class="sxs-lookup"><span data-stu-id="4b349-p105">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps will be protected. If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span> 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="4b349-p106">לאחר מכן החלט **מי יקבל הגדרות אלה?** אם אינך מעוניין להשתמש בקבוצת האבטחה המוגדרת כברירת מחדל **כל המשתמשים**, בחר **שינוי**, בחר את קבוצות האבטחה שיקבלו הגדרות אלה \> **בחר**.</span><span class="sxs-lookup"><span data-stu-id="4b349-p106">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="4b349-131">לבסוף, בחר **הוסף** כדי לשמור את המדיניות והקצה אותה למכשירים.</span><span class="sxs-lookup"><span data-stu-id="4b349-131">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="4b349-132">הגדרות זמינות</span><span class="sxs-lookup"><span data-stu-id="4b349-132">Available settings</span></span>

<span data-ttu-id="4b349-133">ההגדרות הבאות זמינות לניהול אופן הגישה של משתמשים לקבצי עבודה של Office.</span><span class="sxs-lookup"><span data-stu-id="4b349-133">The following settings are available to manage how users access Office work files.</span></span>
  
<span data-ttu-id="4b349-134">לקבלת מידע נוסף, ראה [כיצד תכונות ההגנה של Microsoft 365 Business ממפות להגדרות Intune](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="4b349-134">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span>
  
|<span data-ttu-id="4b349-135">**הגדרה**</span><span class="sxs-lookup"><span data-stu-id="4b349-135">**Setting**</span></span>|<span data-ttu-id="4b349-136">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="4b349-136">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4b349-137">דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office</span><span class="sxs-lookup"><span data-stu-id="4b349-137">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="4b349-138">אם הגדרה זו נקבעה למצב **מופעל**, על המשתמשים לספק צורה אחרת של אימות, בנוסף לשם המשתמש והסיסמה שלהם, כדי שיוכלו להשתמש ביישומי Office במכשיר הנייד שלהם.</span><span class="sxs-lookup"><span data-stu-id="4b349-138">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="4b349-139">אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה</span><span class="sxs-lookup"><span data-stu-id="4b349-139">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="4b349-140">כדי למנוע ממשתמש לא מורשה לנחש באופן אקראי קוד PIN, הקוד יאופס לאחר מספר כניסות שגויות שאתה תציין.</span><span class="sxs-lookup"><span data-stu-id="4b349-140">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="4b349-141">דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך</span><span class="sxs-lookup"><span data-stu-id="4b349-141">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="4b349-142">הגדרה זו קובעת את משך הזמן שבו משתמש יכול להיות לא פעיל לפני שהוא מתבקש להיכנס שוב.</span><span class="sxs-lookup"><span data-stu-id="4b349-142">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
   

