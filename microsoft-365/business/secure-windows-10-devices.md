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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: למד אודות קביעת התצורה של ההגדרות של מדיניות ההתקן המוגדרת כברירת מחדל שכל מכשיר Windows 10 יקבל בעת כניסה לחשבון בעבודה או בבית הספר.
ms.openlocfilehash: b586e687d6b61873b77fac8586396ab51fd90b9b
ms.sourcegitcommit: 90efec455336b4cecc06a8cbf0ce287740433523
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/26/2020
ms.locfileid: "46898067"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="90995-103">אבטחת מכשירים של Windows 10</span><span class="sxs-lookup"><span data-stu-id="90995-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="90995-104">מאמר זה חל על Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="90995-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="90995-105">ההגדרות שאתה קובע כאן הן חלק ממדיניות ברירת המחדל של המכשיר עבור Windows 10.</span><span class="sxs-lookup"><span data-stu-id="90995-105">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="90995-106">כל המשתמשים שמחברים מכשיר Windows 10, כולל מכשירים ניידים ומחשבים, על-ידי כניסה באמצעות חשבון העבודה שלהם, יקבלו באופן אוטומטי הגדרות אלה.</span><span class="sxs-lookup"><span data-stu-id="90995-106">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="90995-107">אנו ממליצים לקבל את מדיניות ברירת המחדל במהלך ההתקנה ולהוסיף פריטי מדיניות המתמקדים בקבוצות משתמשים ספציפיות במועד מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="90995-107">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="90995-108">הגדרות לאבטחת מכשירים של Windows 10</span><span class="sxs-lookup"><span data-stu-id="90995-108">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="90995-p102">כברירת מחדל כל ההגדרות מוגדרות ל **פעיל**. ההגדרות הבאות זמינות:</span><span class="sxs-lookup"><span data-stu-id="90995-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="90995-111">הגדרה</span><span class="sxs-lookup"><span data-stu-id="90995-111">Setting</span></span>  <br/> |<span data-ttu-id="90995-112">תיאור</span><span class="sxs-lookup"><span data-stu-id="90995-112">Description</span></span>  <br/> |
|<span data-ttu-id="90995-113">עזור בהגנה על מחשבים מפני וירוסים ואיומים אחרים באמצעות האנטי-וירוס של Windows Defender</span><span class="sxs-lookup"><span data-stu-id="90995-113">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="90995-114">דרושה הפעלה של האנטי-וירוס של Windows Defender כדי להגן על מחשבים מהסכנות הכרוכות בחיבור לאינטרנט.</span><span class="sxs-lookup"><span data-stu-id="90995-114">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="90995-115">עזור בהגנה על מחשבים מפני איומים מבוססי-אינטרנט ב- Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="90995-115">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="90995-116">הפעלת הגדרות ב- Microsoft Edge שעוזרות בהגנה על המשתמשים מפני אתרים זדוניים והורדות.</span><span class="sxs-lookup"><span data-stu-id="90995-116">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="90995-117">כבה את מסך המכשיר כאשר הוא לא פעיל למשך פרק זמן זה</span><span class="sxs-lookup"><span data-stu-id="90995-117">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="90995-p103">הגדרה זו מוודאת שנתוני החברה מוגנים אם המשתמש אינו פעיל. ייתכן מצב שבו משתמש מסוים עובד במקום ציבורי, למשל בית קפה, שבו הוא מתרחק או שדעתו מוסחת לרגע קט ומשאיר את המכשיר שלו חשוף להצצות אקראיות. הגדרה זו מאפשרת לך לקבוע כמה זמן המשתמש יכול להיות לא פעיל לפני כיבוי המסך.</span><span class="sxs-lookup"><span data-stu-id="90995-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="90995-121">אפשר למשתמשים להוריד אפליקציות מ- Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="90995-121">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="90995-p104">הגדרה זו מאפשרת למשתמשים להוריד ולהתקין אפליקציות מ- Microsoft Store. אפליקציות כוללות את כל סוגי התוכן, החל ממשחקים וכלה בכלי פרודוקטיביות, לכן אנו משאירים הגדרה זו במצב **מופעל**, אך ניתן לבטל אותה להשגת אבטחה נוספת.  </span><span class="sxs-lookup"><span data-stu-id="90995-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|