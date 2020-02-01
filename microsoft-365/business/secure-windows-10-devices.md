---
title: אבטחת מכשירים של Windows 10
f1.keywords:
- CSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4WindowsConfig
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
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: 'למד אודות ברירת המחדל והגדרות אחרות לאבטחת התקני Windows 10. '
ms.openlocfilehash: 9560bb4e299dba8f92d435a64670261b0e7e0290
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593444"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="0d180-103">אבטחת מכשירים של Windows 10</span><span class="sxs-lookup"><span data-stu-id="0d180-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="0d180-104">ההגדרות שאתה קובע כאן הן חלק ממדיניות ברירת המחדל של המכשיר עבור Windows 10.</span><span class="sxs-lookup"><span data-stu-id="0d180-104">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="0d180-105">כל המשתמשים המחברים התקן Windows 10, כולל מכשירים ניידים ומחשבים אישיים, על-ידי כניסה באמצעות חשבון העבודה שלהם יקבלו באופן אוטומטי הגדרות אלה.</span><span class="sxs-lookup"><span data-stu-id="0d180-105">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="0d180-106">אנו ממליצים לקבל את מדיניות ברירת המחדל במהלך ההתקנה ולהוסיף פריטי מדיניות המתמקדים בקבוצות משתמשים ספציפיות במועד מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="0d180-106">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="0d180-107">הגדרות לאבטחת מכשירים של Windows 10</span><span class="sxs-lookup"><span data-stu-id="0d180-107">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="0d180-p102">כברירת מחדל כל ההגדרות מוגדרות ל **פעיל**. ההגדרות הבאות זמינות:</span><span class="sxs-lookup"><span data-stu-id="0d180-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="0d180-110">הגדרה</span><span class="sxs-lookup"><span data-stu-id="0d180-110">Setting</span></span>  <br/> |<span data-ttu-id="0d180-111">תיאור</span><span class="sxs-lookup"><span data-stu-id="0d180-111">Description</span></span>  <br/> |
|<span data-ttu-id="0d180-112">עזור בהגנה על מחשבים מפני וירוסים ואיומים אחרים באמצעות האנטי-וירוס של Windows Defender</span><span class="sxs-lookup"><span data-stu-id="0d180-112">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="0d180-113">דרושה הפעלה של האנטי-וירוס של Windows Defender כדי להגן על מחשבים מהסכנות הכרוכות בחיבור לאינטרנט.</span><span class="sxs-lookup"><span data-stu-id="0d180-113">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="0d180-114">עזור בהגנה על מחשבים מפני איומים מבוססי-אינטרנט ב- Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="0d180-114">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="0d180-115">הפעלת הגדרות ב- Microsoft Edge שעוזרות בהגנה על המשתמשים מפני אתרים זדוניים והורדות.</span><span class="sxs-lookup"><span data-stu-id="0d180-115">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="0d180-116">כבה את מסך המכשיר כאשר הוא לא פעיל למשך פרק זמן זה</span><span class="sxs-lookup"><span data-stu-id="0d180-116">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="0d180-p103">הגדרה זו מוודאת שנתוני החברה מוגנים אם המשתמש אינו פעיל. ייתכן מצב שבו משתמש מסוים עובד במקום ציבורי, למשל בית קפה, שבו הוא מתרחק או שדעתו מוסחת לרגע קט ומשאיר את המכשיר שלו חשוף להצצות אקראיות. הגדרה זו מאפשרת לך לקבוע כמה זמן המשתמש יכול להיות לא פעיל לפני כיבוי המסך.</span><span class="sxs-lookup"><span data-stu-id="0d180-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="0d180-120">אפשר למשתמשים להוריד אפליקציות מ- Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="0d180-120">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="0d180-p104">הגדרה זו מאפשרת למשתמשים להוריד ולהתקין אפליקציות מ- Microsoft Store. אפליקציות כוללות את כל סוגי התוכן, החל ממשחקים וכלה בכלי פרודוקטיביות, לכן אנו משאירים הגדרה זו במצב **מופעל**, אך ניתן לבטל אותה להשגת אבטחה נוספת.  </span><span class="sxs-lookup"><span data-stu-id="0d180-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="0d180-123">אפשר למשתמשים לגשת ל- Cortana</span><span class="sxs-lookup"><span data-stu-id="0d180-123">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="0d180-124">Cortana יכולה להיות שימושית מאוד!</span><span class="sxs-lookup"><span data-stu-id="0d180-124">Cortana can be very helpful!</span></span> <span data-ttu-id="0d180-125">Cortana יכול להפעיל או לבטל הגדרות עבורך, לתת הוראות, ולוודא שאתה בזמן לפגישות, אז אנחנו שומרים על הגדרה זו על כברירת **מחדל** .</span><span class="sxs-lookup"><span data-stu-id="0d180-125">Cortana can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this setting **On** by default.</span></span>  <br/> |
|<span data-ttu-id="0d180-126">אפשר למשתמשים לקבל עצות ופרסומות בנושא Windows מ- Microsoft</span><span class="sxs-lookup"><span data-stu-id="0d180-126">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="0d180-127">העצות של Windows יכולות להיות שימושיות ולעזור למשתמשים להתמצא בעת הפצת התכונות החדשות.</span><span class="sxs-lookup"><span data-stu-id="0d180-127">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="0d180-128">עדכן מכשירים של Windows 10 באופן אוטומטי</span><span class="sxs-lookup"><span data-stu-id="0d180-128">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="0d180-129">הגדרה זו מוודאת שמכשירי Windows 10 מקבלים באופן אוטומטי את העדכונים האחרונים.</span><span class="sxs-lookup"><span data-stu-id="0d180-129">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
   

