---
title: מה ההבדל בין ניהול התקן לבין יישומים
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_understand_devices
- BCS365_understand_devices
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
description: למד את ההבדלים בין ניהול התקנים ניידים וניהול אפליקציות ניידות, או MDM ו-אמא.
ms.openlocfilehash: ecb06ffc23823df72f9254d881f6b1dc1b781f59
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/21/2020
ms.locfileid: "45081823"
---
# <a name="difference-between-mdm-and-mam"></a><span data-ttu-id="593de-103">ההבדל בין MDM לבין מאמא</span><span class="sxs-lookup"><span data-stu-id="593de-103">Difference between MDM and MAM</span></span>

<span data-ttu-id="593de-104">מיקרוסופט 365 Business Premium מציעה מספר דרכים להגן על הנתונים העסקיים שלך.</span><span class="sxs-lookup"><span data-stu-id="593de-104">Microsoft 365 Business Premium offers a number of ways for you to protect your business data.</span></span> <span data-ttu-id="593de-105">ראה [סקירה של Microsoft 365 Business Premium](../microsoft-365-business-overview.md) לקבלת פרטים נוספים אודות ההגנות השונות המוגדרות באופן אוטומטי, ומה באפשרותך להגדיר בעצמך להגנה נוספת על העסק שלך.</span><span class="sxs-lookup"><span data-stu-id="593de-105">See [Overview of Microsoft 365 Business Premium](../microsoft-365-business-overview.md) for more about the various protections that are automatically set up, and what you can set up yourself to further protect your business.</span></span> <span data-ttu-id="593de-106">באפשרותך גם להגדיר מדיניות המגינות על התקני Windows 10 ועל הנתונים שבמכשירים הניידים שלך.</span><span class="sxs-lookup"><span data-stu-id="593de-106">You can also set up policies that protect your Windows 10 devices and the data in your mobile devices.</span></span>
<span data-ttu-id="593de-107">[קביעת הגדרות הגנת יישומים עבור התקני Windows 10](../protection-settings-for-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="593de-107">[Set application protection settings for Windows 10 devices](../protection-settings-for-windows-10-devices.md).</span></span>

## <a name="mobile-device-management-or-mdm"></a><span data-ttu-id="593de-108">ניהול התקנים ניידים או MDM</span><span class="sxs-lookup"><span data-stu-id="593de-108">Mobile device management or MDM</span></span>

<span data-ttu-id="593de-109">Microsoft 365 Business Premium מאפשר לך להגדיר פריטי מדיניות המגנים על נתונים בהתקני Windows 10 שלך.</span><span class="sxs-lookup"><span data-stu-id="593de-109">Microsoft 365 Business Premium lets you set up policies that protect data on your Windows 10 devices.</span></span> <span data-ttu-id="593de-110">כאשר התקן נמצא תחת ניהול התקנים ניידים, אתה שולט בכל ההתקן ויכול למחוק ממנו נתונים ולאפס אותו גם להגדרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="593de-110">When a device is under mobile device management, you control the entire device, and can wipe data from it, and also reset it to factory settings.</span></span> <span data-ttu-id="593de-111">לקבלת מידע נוסף, ראה [הגדרת הגדרות הגנת התקן עבור מחשבי Windows 10](../protection-settings-for-windows-10-pcs.md).</span><span class="sxs-lookup"><span data-stu-id="593de-111">For more information, see [Set device protection settings for Windows 10 PCs](../protection-settings-for-windows-10-pcs.md).</span></span>

## <a name="mobile-application-management-or-mam"></a><span data-ttu-id="593de-112">ניהול אפליקציות ניידות או מאמא</span><span class="sxs-lookup"><span data-stu-id="593de-112">Mobile application management or MAM</span></span>

<span data-ttu-id="593de-113">ניהול יישומים ניידים מאפשר לך לשלוט בנתונים העסקיים שלך במכשירים האישיים של המשתמשים שלך, כגון מכשירי אייפון ו אנדרואידים, ו-Win האישי שלהם 10 מחשבים.</span><span class="sxs-lookup"><span data-stu-id="593de-113">Mobile application management lets you control your business data in your users' personal devices, such as iPhones and Androids, and their personal Win 10 computers.</span></span> <span data-ttu-id="593de-114">באפשרותך להשתמש במדיניות ניהול יישומים כדי למנוע מהמשתמשים שלך להעתיק נתונים עסקיים מיישומי Office ליישומים האישיים שלהם.</span><span class="sxs-lookup"><span data-stu-id="593de-114">You can use application management policies to prevent your users from copying business data from Office apps to their personal apps.</span></span> <span data-ttu-id="593de-115">באפשרותך גם להסיר את כל הנתונים מיישומי Office בהתקנים האישיים שלהם.</span><span class="sxs-lookup"><span data-stu-id="593de-115">You can also remove all data from the Office apps on their personal devices.</span></span> <span data-ttu-id="593de-116">לקבלת מידע נוסף, ראה [קביעת הגדרות הגנת אפליקציות עבור מכשירי Android או iOS](../app-protection-settings-for-android-and-ios.md) [וקביעת הגדרות הגנת יישומים עבור מכשירי Windows 10](../protection-settings-for-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="593de-116">For more information, see [Set app protection settings for Android or iOS devices](../app-protection-settings-for-android-and-ios.md) and [Set application protection settings for Windows 10 devices](../protection-settings-for-windows-10-devices.md).</span></span>
