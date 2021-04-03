---
title: קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: למד כיצד ליצור, לערוך או למחוק מדיניות ניהול יישומים ולהגן על קבצי עבודה במכשירי Android או iOS.
ms.openlocfilehash: 2e157737990c7aca6e87a676e90f62f0d40ad372
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580293"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="acf8d-103">קביעת הגדרות הגנה של אפליקציות עבור מכשירי Android או iOS</span><span class="sxs-lookup"><span data-stu-id="acf8d-103">Set app protection settings for Android or iOS devices</span></span>

<span data-ttu-id="acf8d-104">מאמר זה חל על Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="acf8d-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="create-an-app-management-policy"></a><span data-ttu-id="acf8d-105">יצירת מדיניות לניהול יישומים</span><span class="sxs-lookup"><span data-stu-id="acf8d-105">Create an app management policy</span></span>

1. <span data-ttu-id="acf8d-106">עבור אל מרכז הניהול <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> ב- .</span><span class="sxs-lookup"><span data-stu-id="acf8d-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="acf8d-107">בסרגל הניווט הימני, בחר **מדיניות** \> **מכשירים** \> **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="acf8d-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="acf8d-108">בחלונית **הוסף מדיניות**, הזן שם ייחודי עבור מדיניות זו.</span><span class="sxs-lookup"><span data-stu-id="acf8d-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="acf8d-109">תחת **סוג מדיניות**, בחר ניהול יישומים עבור **Android** או ניהול יישומים **עבור iOS**, בהתאם לערכה של פריטי המדיניות שברצונך ליצור.</span><span class="sxs-lookup"><span data-stu-id="acf8d-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS**, depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="acf8d-110">הרחב **את הגן על קבצי עבודה כאשר מכשירים אובדים או נגנבים** **ונהל את אופן הגישה של משתמשים לקבצי Office במכשירים ניידים**.</span><span class="sxs-lookup"><span data-stu-id="acf8d-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices**.</span></span> <span data-ttu-id="acf8d-111">קבע את תצורת ההגדרות באופן ותקבע את תצורתן.</span><span class="sxs-lookup"><span data-stu-id="acf8d-111">Configure the settings how you would like.</span></span> <span data-ttu-id="acf8d-112">**נהל את אופן הגישה של משתמשים לקבצי Office** במכשירים ניידים כברירת מחדל, אך מומלץ להפעיל אותו **ולקבל** את ערכי ברירת המחדל. </span><span class="sxs-lookup"><span data-stu-id="acf8d-112">**Manage how users access Office files on mobile devices** is **Off** by default, but we recommend that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="acf8d-113">לקבלת מידע נוסף, ראה [הגדרות זמינות](#available-settings).</span><span class="sxs-lookup"><span data-stu-id="acf8d-113">For more information, see [Available settings](#available-settings).</span></span> 
    
    <span data-ttu-id="acf8d-114">ניתן להשתמש תמיד בקישור **איפוס הגדרות ברירת מחדל** כדי לחזור להגדרת ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="acf8d-114">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="acf8d-116">לאחר מכן החלט **מי יקבל הגדרות אלה?**</span><span class="sxs-lookup"><span data-stu-id="acf8d-116">Next decide **Who will get these settings?**</span></span> <span data-ttu-id="acf8d-117">אם אינך מעוניין להשתמש בקבוצת האבטחה 'כל המשתמשים' **המהווה ברירת** מחדל, בחר **שנה**, בחר את קבוצות האבטחה המ מקבלות הגדרות \> **אלה בחר**.</span><span class="sxs-lookup"><span data-stu-id="acf8d-117">If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups that get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="acf8d-118">לבסוף, בחר **סיום** כדי לשמור את המדיניות והקצה אותה למכשירים.</span><span class="sxs-lookup"><span data-stu-id="acf8d-118">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="acf8d-119">עריכת מדיניות לניהול יישומים</span><span class="sxs-lookup"><span data-stu-id="acf8d-119">Edit an app management policy</span></span>

1. <span data-ttu-id="acf8d-120">בכרטיס **מדיניות,** בחר **ערוך מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="acf8d-120">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="acf8d-121">בחלונית **ערוך מדיניות**, בחר את המדיניות שברצונך לשנות</span><span class="sxs-lookup"><span data-stu-id="acf8d-121">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="acf8d-122">בחר **ערוך** לצד כל הגדרה כדי לשנות את הערכים במדיניות.</span><span class="sxs-lookup"><span data-stu-id="acf8d-122">Choose **Edit** next to each setting to change the values in the policy.</span></span> <span data-ttu-id="acf8d-123">בעת שינוי ערך, הוא נשמר באופן אוטומטי במדיניות.</span><span class="sxs-lookup"><span data-stu-id="acf8d-123">When you change a value, it's automatically saved in the policy.</span></span>
    
4. <span data-ttu-id="acf8d-124">כשתסיים, סגור את **חלונית עריכת מדיניות.**</span><span class="sxs-lookup"><span data-stu-id="acf8d-124">When you're finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="acf8d-125">מחיקת מדיניות לניהול יישומים</span><span class="sxs-lookup"><span data-stu-id="acf8d-125">Delete an app management policy</span></span>

1. <span data-ttu-id="acf8d-126">בדף **מדיניות,** בחר מדיניות ולאחר מכן **מחק**.</span><span class="sxs-lookup"><span data-stu-id="acf8d-126">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="acf8d-127">בחלונית **מחיקת מדיניות,** בחר **אשר** כדי למחוק את המדיניות או פריטי המדיניות שבחרת.</span><span class="sxs-lookup"><span data-stu-id="acf8d-127">On the **Delete policy** pane, choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="acf8d-128">הגדרות זמינות</span><span class="sxs-lookup"><span data-stu-id="acf8d-128">Available settings</span></span>

<span data-ttu-id="acf8d-129">הטבלאות הבאות נותנות מידע מפורט אודות הגדרות הזמינות להגנה על קבצי עבודה במכשירים וההגדרות שפקדות כיצד משתמשים ניגשים לקבצי Office מהמכשירים הניידים שלהם.</span><span class="sxs-lookup"><span data-stu-id="acf8d-129">The following tables give detailed information about settings available to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="acf8d-130">לקבלת מידע נוסף, ראה [כיצד תכונות הגנה במפת Microsoft 365 Business Premium להגדרות Intune](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="acf8d-130">For more information, see [How do protection features in Microsoft 365 Business Premium map to Intune settings](map-protection-features-to-intune-settings.md).</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="acf8d-131">הגדרות להגנה על קבצי עבודה</span><span class="sxs-lookup"><span data-stu-id="acf8d-131">Settings that protect work files</span></span>

<span data-ttu-id="acf8d-132">ההגדרות הבאות זמינות כדי להגן על קבצי עבודה במקרה אובדן או גניבה של מכשיר משתמש:</span><span class="sxs-lookup"><span data-stu-id="acf8d-132">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="acf8d-133">הגדרה</span><span class="sxs-lookup"><span data-stu-id="acf8d-133">Setting</span></span>  <br/> |<span data-ttu-id="acf8d-134">תיאור</span><span class="sxs-lookup"><span data-stu-id="acf8d-134">Description</span></span>  <br/> |
|<span data-ttu-id="acf8d-135">מחק קבצי עבודה ממכשיר לא פעיל לאחר מספר הימים הבא</span><span class="sxs-lookup"><span data-stu-id="acf8d-135">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="acf8d-136">אם לא נעשה שימוש במכשיר עבור מספר הימים שתציין כאן, כל קבצי העבודה המאוחסנים במכשיר יימחקו באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="acf8d-136">If a device isn't used for the number of days that you specify here, any work files stored on the device will be deleted automatically.</span></span>  <br/> |
|<span data-ttu-id="acf8d-137">אלץ משתמשים לשמור את כל קבצי העבודה ב- OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="acf8d-137">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="acf8d-138">אם הגדרה זו **היא פועל**, מיקום השמירה הזמין היחיד עבור קבצי עבודה הוא OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="acf8d-138">If this setting is **On**, the only available save location for work files is OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="acf8d-139">הצפן קבצי עבודה</span><span class="sxs-lookup"><span data-stu-id="acf8d-139">Encrypt work files</span></span>  <br/> |<span data-ttu-id="acf8d-140">השאר הגדרה זו במצב **פעיל** כך שקבצי העבודה יהיו מוגנים על-ידי הצפנה.</span><span class="sxs-lookup"><span data-stu-id="acf8d-140">Keep this setting **On** so that work files are protected by encryption.</span></span> <span data-ttu-id="acf8d-141">גם אם המכשיר אובד או נגנב, אף אחד לא יכול לקרוא את נתוני החברה שלך.</span><span class="sxs-lookup"><span data-stu-id="acf8d-141">Even if the device is lost or stolen, no one can read your company data.</span></span>  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="acf8d-142">הגדרות שקובעות כיצד משתמשים ניגשים לקבצי Office במכשירים ניידים</span><span class="sxs-lookup"><span data-stu-id="acf8d-142">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="acf8d-143">ההגדרות הבאות זמינות לניהול אופן הגישה של משתמשים לקבצי עבודה של Office:</span><span class="sxs-lookup"><span data-stu-id="acf8d-143">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="acf8d-144">הגדרה</span><span class="sxs-lookup"><span data-stu-id="acf8d-144">Setting</span></span>  <br/> |<span data-ttu-id="acf8d-145">תיאור</span><span class="sxs-lookup"><span data-stu-id="acf8d-145">Description</span></span>  <br/> |
|<span data-ttu-id="acf8d-146">דרוש מספר זיהוי אישי או טביעת אצבע כדי לגשת ליישומי Office</span><span class="sxs-lookup"><span data-stu-id="acf8d-146">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="acf8d-147">אם הגדרה זו היא **על המשתמשים** חייבים לספק צורה אחרת של אימות, בנוסף לשם המשתמש והסיסמה שלהם, כדי שהם יוכלו להשתמש באפליקציות Office במכשירים הניידים שלהם.</span><span class="sxs-lookup"><span data-stu-id="acf8d-147">If this setting is **On** users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile devices.</span></span><br/> |
|<span data-ttu-id="acf8d-148">אפס מספר זיהוי אישי כשהכניסה נכשלת מספר פעמים זה</span><span class="sxs-lookup"><span data-stu-id="acf8d-148">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="acf8d-149">כדי למנוע ממשתמש לא מורשה לנחש באופן אקראי קוד PIN, הקוד יאופס לאחר מספר כניסות שגויות שאתה תציין.</span><span class="sxs-lookup"><span data-stu-id="acf8d-149">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="acf8d-150">דרוש מהמשתמשים להיכנס שוב לאחר שיישומי Office היו לא פעילים במשך</span><span class="sxs-lookup"><span data-stu-id="acf8d-150">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="acf8d-151">הגדרה זו קובעת כמה זמן המשתמש יכול להיות לא פעיל לפני שהוא מתבקש להיכנס שוב.</span><span class="sxs-lookup"><span data-stu-id="acf8d-151">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="acf8d-152">מנע גישה לקבצי עבודה במכשירים שנפרצו או שבוצעה בהם פעולת ROOT</span><span class="sxs-lookup"><span data-stu-id="acf8d-152">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="acf8d-p105">ייתכן מצב שבו משתמשים מתוחכמים יחזיקו במכשיר שנפרץ או שבוצעה בו פעולת ROOT. כלומר, המשתמש יכול לשנות את מערכת ההפעלה, עובדה שחושפת את המכשיר לתוכנות זדוניות. מכשירים אלה נחסמים כאשר ההגדרה מוגדרת למצב **פעיל**.  </span><span class="sxs-lookup"><span data-stu-id="acf8d-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="acf8d-156">אל תאפשר למשתמשים להעתיק תוכן מאפליקציות Office לאפליקציות אישיות</span><span class="sxs-lookup"><span data-stu-id="acf8d-156">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="acf8d-157">אנחנו מאפשרים זאת כברירת מחדל, אך אם ההגדרה **מופעלת**, המשתמש יכול להעתיק מידע בקובץ עבודה לקובץ אישי.</span><span class="sxs-lookup"><span data-stu-id="acf8d-157">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="acf8d-158">אם ההגדרה **מבוטלת**, למשתמש אין אפשרות להעתיק מידע מקובץ עבודה לאפליקציה אישית או לחשבון אישי.</span><span class="sxs-lookup"><span data-stu-id="acf8d-158">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
