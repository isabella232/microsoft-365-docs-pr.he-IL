---
title: קביעת הגדרות הגנה על מכשירים עבור מחשבי PC של Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: למד אודות ברירת המחדל והגדרות אחרות הזמינות ב- Microsoft Business 365 לאבטחת התקנים Windows 10.
ms.openlocfilehash: ebfe5f59e544b67e5a4f2ecd990031e9221ff8e5
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982144"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="a8877-103">קביעת הגדרות הגנה על מכשירים עבור מחשבי PC של Windows 10</span><span class="sxs-lookup"><span data-stu-id="a8877-103">Set device protection settings for Windows 10 PCs</span></span>

## <a name="secure-windows-10-devices"></a><span data-ttu-id="a8877-104">אבטחת מכשירים של Windows 10</span><span class="sxs-lookup"><span data-stu-id="a8877-104">Secure Windows 10 devices</span></span>

<span data-ttu-id="a8877-105">צפה בסרטון וידאו המסביר כיצד לאבטח מכשירי Windows 10 עם Microsoft 365 Business:</span><span class="sxs-lookup"><span data-stu-id="a8877-105">View a video on how to secure Windows 10 devices with Microsoft 365 Business:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. <span data-ttu-id="a8877-106">היכנס ל- [Microsoft 365 Business](https://portal.office.com) עם אישורים של מנהל מערכת כללי.</span><span class="sxs-lookup"><span data-stu-id="a8877-106">Sign in to [Microsoft 365 Business](https://portal.office.com) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="a8877-107">במרכז הניהול, בכרטיס **כללי מדיניות של מכשיר**, בחר **הוסף מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="a8877-107">in the admin center, on the **Device policies** card, choose **Add policy**.</span></span>
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. <span data-ttu-id="a8877-109">בחלונית **הוסף מדיניות**, הזן שם ייחודי עבור מדיניות זו.</span><span class="sxs-lookup"><span data-stu-id="a8877-109">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="a8877-110">תחת **סוג מדיניות**, בחר **תצורת מכשיר Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="a8877-110">Under **Policy type**, choose **Windows 10 Device Configuration**.</span></span>
    
5. <span data-ttu-id="a8877-p101">הרחב את **אבטחת מכשירי 10 Windows** \> קבע את תצורת ההגדרות כפי שאתה רוצה. ראה [הגדרות זמינות](protection-settings-for-windows-10-pcs.md#bkmk_availablesettings) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="a8877-p101">Expand **Secure Windows 10 Devices** \> configure the settings how you would like. See [Available settings](protection-settings-for-windows-10-pcs.md#bkmk_availablesettings) for more information.</span></span> 
    
    <span data-ttu-id="a8877-113">ניתן להשתמש תמיד בקישור **איפוס הגדרות ברירת מחדל** כדי לחזור להגדרת ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="a8877-113">You can alway use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. <span data-ttu-id="a8877-p102">לאחר מכן החלט **מי יקבל הגדרות אלה?** אם אינך מעוניין להשתמש בקבוצת האבטחה המוגדרת כברירת מחדל **כל המשתמשים**, בחר **שינוי**, חפש את קבוצת האבטחה שתקבל הגדרות אלה \> **בחר**.</span><span class="sxs-lookup"><span data-stu-id="a8877-p102">Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="a8877-117">לבסוף, בחר **סיום** כדי לשמור את המדיניות והקצה אותה למכשירים.</span><span class="sxs-lookup"><span data-stu-id="a8877-117">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="a8877-118">הגדרות זמינות</span><span class="sxs-lookup"><span data-stu-id="a8877-118">Available settings</span></span>

<span data-ttu-id="a8877-p103">כברירת מחדל כל ההגדרות מוגדרות ל **פעיל**. ההגדרות הבאות זמינות.</span><span class="sxs-lookup"><span data-stu-id="a8877-p103">By default all settings are **On**. The following settings are available.</span></span>
  
<span data-ttu-id="a8877-121">ראה [כיצד תכונות ההגנה של Microsoft 365 Business ממפות להגדרות Intune](map-protection-features-to-intune-settings.md) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="a8877-121">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
|||
|:-----|:-----|
|<span data-ttu-id="a8877-122">הגדרה</span><span class="sxs-lookup"><span data-stu-id="a8877-122">Setting</span></span>  <br/> |<span data-ttu-id="a8877-123">תיאור</span><span class="sxs-lookup"><span data-stu-id="a8877-123">Description</span></span>  <br/> |
|<span data-ttu-id="a8877-124">עזור להגן על מחשבי PC מפני וירוסים ואיומים אחרים באמצעות אנטי-וירוס של Windows Defender</span><span class="sxs-lookup"><span data-stu-id="a8877-124">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="a8877-125">דרושה הפעלה של האנטי-וירוס של Windows Defender כדי להגן על מחשבים מהסכנות הכרוכות בחיבור לאינטרנט.</span><span class="sxs-lookup"><span data-stu-id="a8877-125">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="a8877-126">עזור להגן על מחשבי PC מפני איומים מבוססי אינטרנט ב- Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a8877-126">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="a8877-127">הפעלת הגדרות ב- Microsoft Edge שעוזרות בהגנה על המשתמשים מפני אתרים זדוניים והורדות.</span><span class="sxs-lookup"><span data-stu-id="a8877-127">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="a8877-128">שימוש בכללים המקטינים את שטח התקיפה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="a8877-128">Use rules that reduce the attack surface of devices</span></span>  <br/> |<span data-ttu-id="a8877-p104">כאשר צמצום שטח התקיפה מופעל, הוא עוזר בחסימת פעולות ויישומים המשמשים בדרך כלל תוכניות זדוניות כדי לזהם מכשירים. הגדרה זו זמינה רק אם אנטי-וירוס של Windows Defender מופעל. ראה [צמצום שטחי תקיפה](https://go.microsoft.com/fwlink/?linkid=870417) כדי לקבל מידע נוסף.  </span><span class="sxs-lookup"><span data-stu-id="a8877-p104">When turned On, attack surface reduction helps block actions and apps typically used by malware to infect devices. This setting is only available if Windows Defender Antivirus is set to On. See [Reduce attack surfaces](https://go.microsoft.com/fwlink/?linkid=870417) to learn more.  </span></span><br/> |
|<span data-ttu-id="a8877-132">הגנה על תיקיות מפני איומים כגון תוכנת כופר</span><span class="sxs-lookup"><span data-stu-id="a8877-132">Protect folders from threats such as ransomware</span></span>  <br/> |<span data-ttu-id="a8877-p105">הגדרה זו משתמשת בגישה מבוקרת לתיקיות כדי להגן על נתוני החברה מפני שינויים על-ידי יישומים חשודים או זדוניים, כגון תוכנות כופר. סוגי יישומים אלה אינם יכולים לבצע שינויים בתיקיות מוגנות. הגדרה זו זמינה רק אם אנטי-וירוס של Windows Defender מופעל. ראה [הגנה על תיקיות עם גישה מבוקרת לתיקיה](https://go.microsoft.com/fwlink/?linkid=870418) כדי לקבל מידע נוסף.  </span><span class="sxs-lookup"><span data-stu-id="a8877-p105">This setting uses controlled folder access to protect company data from modification by suspicious or malicious apps, such as ransomware. These types of apps are blocked from making changes in protected folders. This setting is only available if Windows Defender Antivirus is set to On. See [Protect folders with COntrolled folder access](https://go.microsoft.com/fwlink/?linkid=870418) to learn more.  </span></span><br/> |
|<span data-ttu-id="a8877-137">מניעת גישה לרשת של תוכן באינטרנט שעשוי להיות זדוני</span><span class="sxs-lookup"><span data-stu-id="a8877-137">Prevent network access to potentially malicious content on the Internet</span></span>  <br/> |<span data-ttu-id="a8877-p106">השתמש בהגדרה זו כדי לחסום חיבורי משתמש יוצאים למיקומי אינטרנט בעלי מוניטין נמוך שעשויים לארח הונאות דיוג, ניצול או תוכן זדוני אחר. הגדרה זו זמינה רק אם אנטי-וירוס של Windows Defender מופעל. ראה [הגנה על הרשת](https://go.microsoft.com/fwlink/?linkid=870419) לקבלת מידע נוסף.  </span><span class="sxs-lookup"><span data-stu-id="a8877-p106">Use this setting to block outbound user connections to low-reputation Internet locations that may host phishing scams, exploits or other malicious content. This setting is only available if Windows Defender Antivirus is set to On. See [Protect your network](https://go.microsoft.com/fwlink/?linkid=870419) for more information.  </span></span><br/> |
|<span data-ttu-id="a8877-141">עזור להגן על קבצים ותיקיות במחשבים מפני גישה לא מורשית באמצעות BitLocker</span><span class="sxs-lookup"><span data-stu-id="a8877-141">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="a8877-p107">Bitlocker מגן על נתונים על-ידי הצפנת הכוננים הקשיחים של המחשב ומגן מפני חשיפת נתונים אם מחבר אבד או נגנב. ראה [שאלות נפוצות על BitLocker](https://go.microsoft.com/fwlink/?linkid=871000) לקבלת מידע נוסף.  </span><span class="sxs-lookup"><span data-stu-id="a8877-p107">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen. See [Bitlocker FAQ](https://go.microsoft.com/fwlink/?linkid=871000) for more information.  </span></span><br/> |
|<span data-ttu-id="a8877-144">אפשר למשתמשים להוריד אפליקציות מ- Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="a8877-144">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="a8877-p108">הגדרה זו מאפשרת למשתמשים להוריד ולהתקין אפליקציות מ- Microsoft Store. אפליקציות כוללות את כל סוגי התוכן, החל ממשחקים וכלה בכלי פרודוקטיביות, לכן אנו משאירים הגדרה זו במצב **מופעל**, אך ניתן לבטל אותה להשגת אבטחה נוספת.  </span><span class="sxs-lookup"><span data-stu-id="a8877-p108">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="a8877-147">אפשר למשתמשים לגשת ל- Cortana</span><span class="sxs-lookup"><span data-stu-id="a8877-147">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="a8877-p109">Cortana יכולה להיות שימושית מאוד! היא יכולה להפעיל או לבטל הגדרות עבורך, לתת הנחיות ולוודא שאתה מגיע בזמן לפגישות, לכן אנו משאירים הגדרה זו במצב **מופעל** כברירת מחדל.  </span><span class="sxs-lookup"><span data-stu-id="a8877-p109">Cortana can be very helpful! She can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this **On** by default.  </span></span><br/> |
|<span data-ttu-id="a8877-150">אפשר למשתמשים לקבל עצות ופרסומות בנושא Windows מ- Microsoft</span><span class="sxs-lookup"><span data-stu-id="a8877-150">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="a8877-151">העצות של Windows יכולות להיות שימושיות ולעזור למשתמשים להתמצא בעת הפצת התכונות החדשות.</span><span class="sxs-lookup"><span data-stu-id="a8877-151">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="a8877-152">עדכן מכשירים של Windows 10 באופן אוטומטי</span><span class="sxs-lookup"><span data-stu-id="a8877-152">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="a8877-153">הגדרה זו מוודאת שמכשירי Windows 10 מקבלים באופן אוטומטי את העדכונים האחרונים.</span><span class="sxs-lookup"><span data-stu-id="a8877-153">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
|<span data-ttu-id="a8877-154">כבה את מסך המכשיר כשהוא לא פעיל במשך</span><span class="sxs-lookup"><span data-stu-id="a8877-154">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="a8877-p110">הגדרה זו מוודאת שנתוני החברה מוגנים אם המשתמש אינו פעיל. ייתכן מצב שבו משתמש מסוים עובד במקום ציבורי, למשל בית קפה, שבו הוא מתרחק או שדעתו מוסחת לרגע קט ומשאיר את המכשיר שלו חשוף להצצות אקראיות. הגדרה זו מאפשרת לך לקבוע כמה זמן המשתמש יכול להיות לא פעיל לפני כיבוי המסך.</span><span class="sxs-lookup"><span data-stu-id="a8877-p110">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
   
  

