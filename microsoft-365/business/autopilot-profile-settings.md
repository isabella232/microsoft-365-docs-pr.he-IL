---
title: אודות ההגדרות של פרופיל AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: פרופילי autoPilot לסייע לך לקבוע כיצד Windows מקבל מותקן במכשירים המשתמש. מכילים פרופילי ברירת מחדל ועל הגדרות אופציונליות לדלג על ההתקנה Cortana.
ms.openlocfilehash: d43a15e5f3dc83596b5c23dd0ceb416b24810298
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32276940"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="5e6e5-104">אודות ההגדרות של פרופיל AutoPilot</span><span class="sxs-lookup"><span data-stu-id="5e6e5-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="5e6e5-105">הגדרות הפרופיל autoPilot</span><span class="sxs-lookup"><span data-stu-id="5e6e5-105">AutoPilot profile settings</span></span>

<span data-ttu-id="5e6e5-106">באפשרותך לקבוע כיצד Windows מקבל מותקן במכשירים המשתמש על-ידי שימוש בפרופילים AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5e6e5-106">You can control how Windows gets installed on user devices by using the AutoPilot profiles.</span></span> <span data-ttu-id="5e6e5-107">הפרופילים מכיל את ההגדרות הבאות.</span><span class="sxs-lookup"><span data-stu-id="5e6e5-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="5e6e5-108">**AutoPilot ברירת המחדל תכונות (נדרש) מוגדרים באופן אוטומטי:**</span><span class="sxs-lookup"><span data-stu-id="5e6e5-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="5e6e5-109">**הגדרה**</span><span class="sxs-lookup"><span data-stu-id="5e6e5-109">**Setting**</span></span>|<span data-ttu-id="5e6e5-110">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="5e6e5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5e6e5-111">דלג על רישום Cortana, OneDrive ו- OEM</span><span class="sxs-lookup"><span data-stu-id="5e6e5-111">Skip Cortana, OneDrive and OEM registration</span></span>  <br/> |<span data-ttu-id="5e6e5-112">מדלג על ההתקנה של יישומים לצרכן כגון Cortana ו- OneDrive אישי.</span><span class="sxs-lookup"><span data-stu-id="5e6e5-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="5e6e5-113">התקן המשתמש יכול להתקין אלה מאוחר יותר כל עוד באפשרותו מנהל מקומי במכשיר.</span><span class="sxs-lookup"><span data-stu-id="5e6e5-113">The device user can install these later as long as he or she is a local admin on the device.</span></span> <span data-ttu-id="5e6e5-114">המערכת מדלגת על רישום היצרן המקורי מכיוון ההתקן ינוהל על-ידי Microsoft 365 עסקיים.</span><span class="sxs-lookup"><span data-stu-id="5e6e5-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="5e6e5-115">להיכנס חוויית עם מותג החברה שלך</span><span class="sxs-lookup"><span data-stu-id="5e6e5-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="5e6e5-116">אם לחברה שלך יש של [התאמה למותג הוספה החברה שלך אל Office 365 כמציע דף כניסה](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), יקבל המשתמש בהתקן זה חוויית בעת הכניסה.</span><span class="sxs-lookup"><span data-stu-id="5e6e5-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="5e6e5-117">MDM הרשמה אוטומטית עם חשבונות AAD שתצורתו נקבעה.</span><span class="sxs-lookup"><span data-stu-id="5e6e5-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="5e6e5-118">זהות משתמש ינוהל על-ידי תכלת הרקיע Active directory ולאחר המשתמשים לבצע כניסה ל- Windows ו- Office 365 עם אישורי Microsoft 365 העסק שלהם.</span><span class="sxs-lookup"><span data-stu-id="5e6e5-118">The user identity will be managed by Azure Active directory, and the users will sign into Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="5e6e5-119">**הגדרות אופציונליות:**</span><span class="sxs-lookup"><span data-stu-id="5e6e5-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="5e6e5-120">**הגדרה**</span><span class="sxs-lookup"><span data-stu-id="5e6e5-120">**Setting**</span></span>|<span data-ttu-id="5e6e5-121">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="5e6e5-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5e6e5-122">דלג על הגדרות פרטיות (מבוטל כברירת מחדל)</span><span class="sxs-lookup"><span data-stu-id="5e6e5-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="5e6e5-123">אם אפשרות זו מוגדרת כ- **On**, המשתמש התקן לא יראו את הסכם הרשיון עבור התקן ו- Windows כאשר הוא או היא חותמים תחילה.</span><span class="sxs-lookup"><span data-stu-id="5e6e5-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="5e6e5-124">אל תאפשר למשתמש להפוך מנהל מקומי</span><span class="sxs-lookup"><span data-stu-id="5e6e5-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="5e6e5-125">אם אפשרות זו מוגדרת כ- **On**, התקן המשתמש לא תהיה אפשרות להתקין יישומים אישיים, כגון Cortana.</span><span class="sxs-lookup"><span data-stu-id="5e6e5-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span>  <br/> |
   
