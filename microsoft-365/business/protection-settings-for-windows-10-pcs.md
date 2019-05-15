---
title: קביעת הגדרות הגנה על מכשירים עבור מחשבי PC של Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
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
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: למד אודות ברירת המחדל והגדרות אחרות הזמינות ב- Microsoft Business 365 לאבטחת התקנים Windows 10.
ms.openlocfilehash: 095aa2c2f32c3e7b5a5a4e560ea4bc7124d7146e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074509"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="02ccb-103">קביעת הגדרות הגנה על מכשירים עבור מחשבי PC של Windows 10</span><span class="sxs-lookup"><span data-stu-id="02ccb-103">Set device protection settings for Windows 10 PCs</span></span>

## <a name="secure-windows-10-devices"></a><span data-ttu-id="02ccb-104">אבטחת מכשירים של Windows 10</span><span class="sxs-lookup"><span data-stu-id="02ccb-104">Secure Windows 10 devices</span></span>

<span data-ttu-id="02ccb-105">צפה בסרטון וידאו המסביר כיצד לאבטח מכשירי Windows 10 עם Microsoft 365 Business:</span><span class="sxs-lookup"><span data-stu-id="02ccb-105">View a video on how to secure Windows 10 devices with Microsoft 365 Business:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. <span data-ttu-id="02ccb-106">SGo למרכז admin ב <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="02ccb-106">SGo to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="02ccb-107">נווט השמאלי, בחר **התקנים** \> **מדיניות** \> **הוספה**.</span><span class="sxs-lookup"><span data-stu-id="02ccb-107">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="02ccb-108">בחלונית **הוסף מדיניות**, הזן שם ייחודי עבור מדיניות זו.</span><span class="sxs-lookup"><span data-stu-id="02ccb-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="02ccb-109">תחת **סוג מדיניות**, בחר **תצורת מכשיר Windows 10**.</span><span class="sxs-lookup"><span data-stu-id="02ccb-109">Under **Policy type**, choose **Windows 10 Device Configuration**.</span></span>
    
5. <span data-ttu-id="02ccb-p101">הרחב את **אבטחת מכשירי 10 Windows** \> קבע את תצורת ההגדרות כפי שאתה רוצה. ראה [הגדרות זמינות](#available-settings) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="02ccb-p101">Expand **Secure Windows 10 Devices** \> configure the settings how you would like. See [Available settings](#available-settings) for more information.</span></span> 
    
    <span data-ttu-id="02ccb-112">ניתן להשתמש תמיד בקישור **איפוס הגדרות ברירת מחדל** כדי לחזור להגדרת ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="02ccb-112">You can alway use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. <span data-ttu-id="02ccb-p102">לאחר מכן החלט **מי יקבל הגדרות אלה?** אם אינך מעוניין להשתמש בקבוצת האבטחה המוגדרת כברירת מחדל **כל המשתמשים**, בחר **שינוי**, חפש את קבוצת האבטחה שתקבל הגדרות אלה \> **בחר**.</span><span class="sxs-lookup"><span data-stu-id="02ccb-p102">Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="02ccb-116">לבסוף, בחר **סיום** כדי לשמור את המדיניות והקצה אותה למכשירים.</span><span class="sxs-lookup"><span data-stu-id="02ccb-116">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="02ccb-117">הגדרות זמינות</span><span class="sxs-lookup"><span data-stu-id="02ccb-117">Available settings</span></span>

<span data-ttu-id="02ccb-p103">כברירת מחדל כל ההגדרות מוגדרות ל **פעיל**. ההגדרות הבאות זמינות.</span><span class="sxs-lookup"><span data-stu-id="02ccb-p103">By default all settings are **On**. The following settings are available.</span></span>
  
<span data-ttu-id="02ccb-120">ראה [כיצד תכונות ההגנה של Microsoft 365 Business ממפות להגדרות Intune](map-protection-features-to-intune-settings.md) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="02ccb-120">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
|||
|:-----|:-----|
|<span data-ttu-id="02ccb-121">הגדרה</span><span class="sxs-lookup"><span data-stu-id="02ccb-121">Setting</span></span>  <br/> |<span data-ttu-id="02ccb-122">תיאור</span><span class="sxs-lookup"><span data-stu-id="02ccb-122">Description</span></span>  <br/> |
|<span data-ttu-id="02ccb-123">עזור בהגנה על מחשבים מפני וירוסים ואיומים אחרים באמצעות האנטי-וירוס של Windows Defender</span><span class="sxs-lookup"><span data-stu-id="02ccb-123">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="02ccb-124">דרושה הפעלה של האנטי-וירוס של Windows Defender כדי להגן על מחשבים מהסכנות הכרוכות בחיבור לאינטרנט.</span><span class="sxs-lookup"><span data-stu-id="02ccb-124">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="02ccb-125">עזור בהגנה על מחשבים מפני איומים מבוססי-אינטרנט ב- Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="02ccb-125">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="02ccb-126">הפעלת הגדרות ב- Microsoft Edge שעוזרות בהגנה על המשתמשים מפני אתרים זדוניים והורדות.</span><span class="sxs-lookup"><span data-stu-id="02ccb-126">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="02ccb-127">שימוש בכללים המקטינים את שטח התקיפה של מכשירים</span><span class="sxs-lookup"><span data-stu-id="02ccb-127">Use rules that reduce the attack surface of devices</span></span>  <br/> |<span data-ttu-id="02ccb-p104">כאשר צמצום שטח התקיפה מופעל, הוא עוזר בחסימת פעולות ויישומים המשמשים בדרך כלל תוכניות זדוניות כדי לזהם מכשירים. הגדרה זו זמינה רק אם אנטי-וירוס של Windows Defender מופעל. ראה [צמצום שטחי תקיפה](https://go.microsoft.com/fwlink/?linkid=870417) כדי לקבל מידע נוסף.  </span><span class="sxs-lookup"><span data-stu-id="02ccb-p104">When turned On, attack surface reduction helps block actions and apps typically used by malware to infect devices. This setting is only available if Windows Defender Antivirus is set to On. See [Reduce attack surfaces](https://go.microsoft.com/fwlink/?linkid=870417) to learn more.  </span></span><br/> |
|<span data-ttu-id="02ccb-131">הגנה על תיקיות מפני איומים כגון תוכנת כופר</span><span class="sxs-lookup"><span data-stu-id="02ccb-131">Protect folders from threats such as ransomware</span></span>  <br/> |<span data-ttu-id="02ccb-p105">הגדרה זו משתמשת בגישה מבוקרת לתיקיות כדי להגן על נתוני החברה מפני שינויים על-ידי יישומים חשודים או זדוניים, כגון תוכנות כופר. סוגי יישומים אלה אינם יכולים לבצע שינויים בתיקיות מוגנות. הגדרה זו זמינה רק אם אנטי-וירוס של Windows Defender מופעל. ראה [הגנה על תיקיות עם גישה מבוקרת לתיקיה](https://go.microsoft.com/fwlink/?linkid=870418) כדי לקבל מידע נוסף.  </span><span class="sxs-lookup"><span data-stu-id="02ccb-p105">This setting uses controlled folder access to protect company data from modification by suspicious or malicious apps, such as ransomware. These types of apps are blocked from making changes in protected folders. This setting is only available if Windows Defender Antivirus is set to On. See [Protect folders with COntrolled folder access](https://go.microsoft.com/fwlink/?linkid=870418) to learn more.  </span></span><br/> |
|<span data-ttu-id="02ccb-136">מניעת גישה לרשת של תוכן באינטרנט שעשוי להיות זדוני</span><span class="sxs-lookup"><span data-stu-id="02ccb-136">Prevent network access to potentially malicious content on the Internet</span></span>  <br/> |<span data-ttu-id="02ccb-p106">השתמש בהגדרה זו כדי לחסום חיבורי משתמש יוצאים למיקומי אינטרנט בעלי מוניטין נמוך שעשויים לארח הונאות דיוג, ניצול או תוכן זדוני אחר. הגדרה זו זמינה רק אם אנטי-וירוס של Windows Defender מופעל. ראה [הגנה על הרשת](https://go.microsoft.com/fwlink/?linkid=870419) לקבלת מידע נוסף.  </span><span class="sxs-lookup"><span data-stu-id="02ccb-p106">Use this setting to block outbound user connections to low-reputation Internet locations that may host phishing scams, exploits or other malicious content. This setting is only available if Windows Defender Antivirus is set to On. See [Protect your network](https://go.microsoft.com/fwlink/?linkid=870419) for more information.  </span></span><br/> |
|<span data-ttu-id="02ccb-140">עזור להגן על קבצים ותיקיות במחשבים מפני גישה לא מורשית באמצעות BitLocker</span><span class="sxs-lookup"><span data-stu-id="02ccb-140">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="02ccb-p107">Bitlocker מגן על נתונים על-ידי הצפנת הכוננים הקשיחים של המחשב ומגן מפני חשיפת נתונים אם מחבר אבד או נגנב. ראה [שאלות נפוצות על BitLocker](https://go.microsoft.com/fwlink/?linkid=871000) לקבלת מידע נוסף.  </span><span class="sxs-lookup"><span data-stu-id="02ccb-p107">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen. See [Bitlocker FAQ](https://go.microsoft.com/fwlink/?linkid=871000) for more information.  </span></span><br/> |
|<span data-ttu-id="02ccb-143">אפשר למשתמשים להוריד אפליקציות מ- Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="02ccb-143">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="02ccb-p108">הגדרה זו מאפשרת למשתמשים להוריד ולהתקין אפליקציות מ- Microsoft Store. אפליקציות כוללות את כל סוגי התוכן, החל ממשחקים וכלה בכלי פרודוקטיביות, לכן אנו משאירים הגדרה זו במצב **מופעל**, אך ניתן לבטל אותה להשגת אבטחה נוספת.  </span><span class="sxs-lookup"><span data-stu-id="02ccb-p108">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="02ccb-146">אפשר למשתמשים לגשת ל- Cortana</span><span class="sxs-lookup"><span data-stu-id="02ccb-146">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="02ccb-p109">Cortana יכולה להיות שימושית מאוד! היא יכולה להפעיל או לבטל הגדרות עבורך, לתת הנחיות ולוודא שאתה מגיע בזמן לפגישות, לכן אנו משאירים הגדרה זו במצב **מופעל** כברירת מחדל.  </span><span class="sxs-lookup"><span data-stu-id="02ccb-p109">Cortana can be very helpful! She can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this **On** by default.  </span></span><br/> |
|<span data-ttu-id="02ccb-149">אפשר למשתמשים לקבל עצות ופרסומות בנושא Windows מ- Microsoft</span><span class="sxs-lookup"><span data-stu-id="02ccb-149">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="02ccb-150">העצות של Windows יכולות להיות שימושיות ולעזור למשתמשים להתמצא בעת הפצת התכונות החדשות.</span><span class="sxs-lookup"><span data-stu-id="02ccb-150">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="02ccb-151">עדכן מכשירים של Windows 10 באופן אוטומטי</span><span class="sxs-lookup"><span data-stu-id="02ccb-151">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="02ccb-152">הגדרה זו מוודאת שמכשירי Windows 10 מקבלים באופן אוטומטי את העדכונים האחרונים.</span><span class="sxs-lookup"><span data-stu-id="02ccb-152">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
|<span data-ttu-id="02ccb-153">כבה את מסך המכשיר כשהוא לא פעיל במשך</span><span class="sxs-lookup"><span data-stu-id="02ccb-153">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="02ccb-p110">הגדרה זו מוודאת שנתוני החברה מוגנים אם המשתמש אינו פעיל. ייתכן מצב שבו משתמש מסוים עובד במקום ציבורי, למשל בית קפה, שבו הוא מתרחק או שדעתו מוסחת לרגע קט ומשאיר את המכשיר שלו חשוף להצצות אקראיות. הגדרה זו מאפשרת לך לקבוע כמה זמן המשתמש יכול להיות לא פעיל לפני כיבוי המסך.</span><span class="sxs-lookup"><span data-stu-id="02ccb-p110">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
   
  

