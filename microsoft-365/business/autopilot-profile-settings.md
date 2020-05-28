---
title: אודות ההגדרות של פרופיל AutoPilot
f1.keywords:
- NOCSH
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: פרופילי טייס אוטומטי מסייעים לך לשלוט באופן שבו Windows מקבל התקנה בהתקני משתמש. הפרופילים מכילים הגדרות ברירת מחדל ואופציונליות כמו התקנת Cortana.
ms.openlocfilehash: 100de5e9548f901008d3ae154ac5a237ef265ffb
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44401033"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="7fba4-104">אודות ההגדרות של פרופיל AutoPilot</span><span class="sxs-lookup"><span data-stu-id="7fba4-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="7fba4-105">הגדרות פרופיל טייס אוטומטי</span><span class="sxs-lookup"><span data-stu-id="7fba4-105">AutoPilot profile settings</span></span>

<span data-ttu-id="7fba4-106">באפשרותך להשתמש בפרופילי טייס אוטומטי כדי לשלוט באופן ההתקנה של Windows בהתקני משתמש.</span><span class="sxs-lookup"><span data-stu-id="7fba4-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="7fba4-107">הפרופילים מכילים את ההגדרות הבאות.</span><span class="sxs-lookup"><span data-stu-id="7fba4-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="7fba4-108">**תכונות ברירת מחדל של טייס אוטומטי (נדרש) ההוגדרו באופן אוטומטי:**</span><span class="sxs-lookup"><span data-stu-id="7fba4-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="7fba4-109">**הגדרה**</span><span class="sxs-lookup"><span data-stu-id="7fba4-109">**Setting**</span></span>|<span data-ttu-id="7fba4-110">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="7fba4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7fba4-111">דלג קורטנה, OneDrive ורישום OEM</span><span class="sxs-lookup"><span data-stu-id="7fba4-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="7fba4-112">דילוג על ההתקנה של יישומי הצרכן כמו Cortana ו OneDrive אישי.</span><span class="sxs-lookup"><span data-stu-id="7fba4-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="7fba4-113">משתמש ההתקן יכול להתקין אותם מאוחר יותר, כל עוד המשתמש הוא מנהל מקומי בהתקן.</span><span class="sxs-lookup"><span data-stu-id="7fba4-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="7fba4-114">המערכת תדלג על רישום היצרן המקורי מכיוון שההתקן ינוהל על-ידי Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="7fba4-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="7fba4-115">הירשם בניסיון עם מותג החברה שלך</span><span class="sxs-lookup"><span data-stu-id="7fba4-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="7fba4-116">אם לחברה שלך יש [הוסף את מיתוג החברה שלך ל-Microsoft 365 לדף הכניסה](https://docs.microsoft.com/microsoft-365/admin/setup/customize-sign-in-page), משתמש ההתקן יקבל את החוויה הזאת בעת הכניסה.</span><span class="sxs-lookup"><span data-stu-id="7fba4-116">If your company has a [Add your company branding to Microsoft 365 Sign In page](https://docs.microsoft.com/microsoft-365/admin/setup/customize-sign-in-page), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="7fba4-117">הרשמה אוטומטית של MDM עם חשבונות אד-מוגדרים שתצורתם נקבעה.</span><span class="sxs-lookup"><span data-stu-id="7fba4-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="7fba4-118">זהות המשתמש תנוהל על-ידי החברה הפעילה של מיקרוסופט, והמשתמשים יוכלו להיכנס ל-Windows ו-Microsoft 365 עם האישורים העסקיים שלהם ב-Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="7fba4-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Microsoft 365 with their Microsoft 365 Business Premium credentials.</span></span>  <br/> |
   
 <span data-ttu-id="7fba4-119">**הגדרות אופציונליות:**</span><span class="sxs-lookup"><span data-stu-id="7fba4-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="7fba4-120">**הגדרה**</span><span class="sxs-lookup"><span data-stu-id="7fba4-120">**Setting**</span></span>|<span data-ttu-id="7fba4-121">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="7fba4-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7fba4-122">דלג על הגדרות פרטיות (כבוי כברירת מחדל)</span><span class="sxs-lookup"><span data-stu-id="7fba4-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="7fba4-123">אם אפשרות זו מוגדרת כ **-,** משתמש ההתקן לא יראה את הסכם הרשיון עבור ההתקן ו-Windows כאשר הוא יחתום תחילה.</span><span class="sxs-lookup"><span data-stu-id="7fba4-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="7fba4-124">אל תאפשר למשתמש להפוך למנהל המקומי</span><span class="sxs-lookup"><span data-stu-id="7fba4-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="7fba4-125">אם אפשרות זו מוגדרת כ **-,** למשתמש ההתקן לא תהיה אפשרות להתקין יישומים אישיים כלשהם, כגון cortana.</span><span class="sxs-lookup"><span data-stu-id="7fba4-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
   
