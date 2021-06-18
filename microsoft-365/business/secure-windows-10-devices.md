---
title: אבטחת מכשירים של Windows 10
f1.keywords:
- CSH
ms.author: sharik
author: skjerland
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: למד אודות קביעת התצורה של ההגדרות של מדיניות המכשיר המוגדרת כברירת מחדל שכל מכשיר Windows 10 יקבל בעת הכניסה לחשבון העבודה או בית הספר שלו.
ms.openlocfilehash: 3f85549e722c9aa4196cf50fc02bee2e89506017
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925238"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="fa708-103">אבטחת מכשירים של Windows 10</span><span class="sxs-lookup"><span data-stu-id="fa708-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="fa708-104">מאמר זה חל על Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="fa708-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="fa708-105">ההגדרות שאתה קובע כאן הן חלק ממדיניות ברירת המחדל של המכשיר עבור Windows 10.</span><span class="sxs-lookup"><span data-stu-id="fa708-105">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="fa708-106">כל המשתמשים המחברים מכשיר Windows 10, כולל מכשירים ניידים ומחשבים אישיים, על-ידי כניסה באמצעות חשבון העבודה שלהם יקבלו באופן אוטומטי הגדרות אלה.</span><span class="sxs-lookup"><span data-stu-id="fa708-106">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="fa708-107">אנו ממליצים לקבל את מדיניות ברירת המחדל במהלך ההתקנה ולהוסיף פריטי מדיניות המתמקדים בקבוצות משתמשים ספציפיות במועד מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="fa708-107">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="fa708-108">הגדרות לאבטחת מכשירים של Windows 10</span><span class="sxs-lookup"><span data-stu-id="fa708-108">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="fa708-p102">כברירת מחדל כל ההגדרות מוגדרות ל **פעיל**. ההגדרות הבאות זמינות:</span><span class="sxs-lookup"><span data-stu-id="fa708-p102">By default all settings are **On**. The following settings are available:</span></span>
  


|<span data-ttu-id="fa708-111">הגדרה</span><span class="sxs-lookup"><span data-stu-id="fa708-111">Setting</span></span>  <br/> |<span data-ttu-id="fa708-112">תיאור</span><span class="sxs-lookup"><span data-stu-id="fa708-112">Description</span></span>  <br/> |
|:-----|:-----|
|<span data-ttu-id="fa708-113">עזור בהגנה על מחשבים מפני וירוסים ואיומים אחרים באמצעות האנטי-וירוס של Windows Defender</span><span class="sxs-lookup"><span data-stu-id="fa708-113">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="fa708-114">דרושה הפעלה של האנטי-וירוס של Windows Defender כדי להגן על מחשבים מהסכנות הכרוכות בחיבור לאינטרנט.</span><span class="sxs-lookup"><span data-stu-id="fa708-114">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="fa708-115">עזור בהגנה על מחשבים מפני איומים מבוססי-אינטרנט ב- Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="fa708-115">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="fa708-116">הפעלת הגדרות ב- Microsoft Edge שעוזרות בהגנה על המשתמשים מפני אתרים זדוניים והורדות.</span><span class="sxs-lookup"><span data-stu-id="fa708-116">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="fa708-117">עזור להגן על קבצים ותיקיות במחשבים מפני גישה לא מורשית באמצעות BitLocker</span><span class="sxs-lookup"><span data-stu-id="fa708-117">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="fa708-118">Bitlocker מגן על נתונים על-ידי הצפנת הכוננים הקשיחים של המחשב ומגן מפני חשיפת נתונים אם מחבר אבד או נגנב.</span><span class="sxs-lookup"><span data-stu-id="fa708-118">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen.</span></span> <span data-ttu-id="fa708-119">לקבלת מידע נוסף, ראה [שאלות נפוצות אודות Bitlocker](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions).</span><span class="sxs-lookup"><span data-stu-id="fa708-119">For more information, see [Bitlocker FAQ](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions).</span></span>  <br/> |
|<span data-ttu-id="fa708-120">כבה את מסך המכשיר כאשר הוא לא פעיל למשך פרק זמן זה</span><span class="sxs-lookup"><span data-stu-id="fa708-120">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="fa708-p104">הגדרה זו מוודאת שנתוני החברה מוגנים אם המשתמש אינו פעיל. ייתכן מצב שבו משתמש מסוים עובד במקום ציבורי, למשל בית קפה, שבו הוא מתרחק או שדעתו מוסחת לרגע קט ומשאיר את המכשיר שלו חשוף להצצות אקראיות. הגדרה זו מאפשרת לך לקבוע כמה זמן המשתמש יכול להיות לא פעיל לפני כיבוי המסך.</span><span class="sxs-lookup"><span data-stu-id="fa708-p104">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|