---
title: אודות ההגדרות של פרופיל AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: פרופילי טייס אוטומטי מסייעים לך לשלוט באופן שבו Windows מקבל התקנה בהתקני משתמש. הפרופילים מכילים הגדרות ברירת מחדל ואופציונליות כמו התקנת Cortana.
ms.openlocfilehash: eb0d9a95c796909d024db1d061aaeace7d07ed1b
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574577"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="95c67-104">אודות ההגדרות של פרופיל AutoPilot</span><span class="sxs-lookup"><span data-stu-id="95c67-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="95c67-105">הגדרות פרופיל טייס אוטומטי</span><span class="sxs-lookup"><span data-stu-id="95c67-105">AutoPilot profile settings</span></span>

<span data-ttu-id="95c67-106">באפשרותך לשלוט באופן ההתקנה של Windows בהתקני משתמש באמצעות פרופילי הטייס האוטומטי.</span><span class="sxs-lookup"><span data-stu-id="95c67-106">You can control how Windows gets installed on user devices by using the AutoPilot profiles.</span></span> <span data-ttu-id="95c67-107">הפרופילים מכילים את ההגדרות הבאות.</span><span class="sxs-lookup"><span data-stu-id="95c67-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="95c67-108">**תכונות ברירת מחדל של טייס אוטומטי (נדרש) ההוגדרו באופן אוטומטי:**</span><span class="sxs-lookup"><span data-stu-id="95c67-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="95c67-109">**הגדרה**</span><span class="sxs-lookup"><span data-stu-id="95c67-109">**Setting**</span></span>|<span data-ttu-id="95c67-110">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="95c67-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="95c67-111">דלג קורטנה, OneDrive ו-OEM הרישום</span><span class="sxs-lookup"><span data-stu-id="95c67-111">Skip Cortana, OneDrive and OEM registration</span></span>  <br/> |<span data-ttu-id="95c67-112">דילוג על ההתקנה של יישומי הצרכן כמו Cortana ו OneDrive אישי.</span><span class="sxs-lookup"><span data-stu-id="95c67-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="95c67-113">משתמש ההתקן יכול להתקין אותם מאוחר יותר, כל עוד הוא או היא מנהל מקומי במכשיר.</span><span class="sxs-lookup"><span data-stu-id="95c67-113">The device user can install these later as long as he or she is a local admin on the device.</span></span> <span data-ttu-id="95c67-114">המערכת תדלג על רישום היצרן המקורי מכיוון שההתקן ינוהל על-ידי Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="95c67-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="95c67-115">הירשם בניסיון עם מותג החברה שלך</span><span class="sxs-lookup"><span data-stu-id="95c67-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="95c67-116">אם לחברה שלך יש [הוספת מיתוג לחברה שלך לדף הכניסה של Office 365](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), משתמש ההתקן יקבל את החוויה הזאת בעת הכניסה.</span><span class="sxs-lookup"><span data-stu-id="95c67-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="95c67-117">הרשמה אוטומטית של MDM עם חשבונות אד-מוגדרים שתצורתם נקבעה.</span><span class="sxs-lookup"><span data-stu-id="95c67-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="95c67-118">זהות המשתמש תנוהל על-ידי הספריה הפעילה, והמשתמשים יחתמו ל-Windows ו-Office 365 עם האישורים העסקיים של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="95c67-118">The user identity will be managed by Azure Active directory, and the users will sign into Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="95c67-119">**הגדרות אופציונליות:**</span><span class="sxs-lookup"><span data-stu-id="95c67-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="95c67-120">**הגדרה**</span><span class="sxs-lookup"><span data-stu-id="95c67-120">**Setting**</span></span>|<span data-ttu-id="95c67-121">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="95c67-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="95c67-122">דלג על הגדרות פרטיות (כבוי כברירת מחדל)</span><span class="sxs-lookup"><span data-stu-id="95c67-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="95c67-123">אם אפשרות זו מוגדרת כ **-,** משתמש ההתקן לא יראה את הסכם הרשיון עבור ההתקן ו-Windows כאשר הוא יחתום תחילה.</span><span class="sxs-lookup"><span data-stu-id="95c67-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="95c67-124">אל תאפשר למשתמש להפוך למנהל המקומי</span><span class="sxs-lookup"><span data-stu-id="95c67-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="95c67-125">אם אפשרות זו מוגדרת כ **-,** למשתמש ההתקן לא תהיה אפשרות להתקין יישומים אישיים כלשהם, כגון cortana.</span><span class="sxs-lookup"><span data-stu-id="95c67-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span>  <br/> |
   
