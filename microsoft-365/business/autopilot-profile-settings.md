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
description: פרופילי טייס אוטומטי מסייעים לך לשלוט באופן שבו Windows מותקן במכשירי משתמשים. הפרופילים מכילים ברירות מחדל והגדרות אופציונליות כגון דלג על התקנת Cortana.
ms.openlocfilehash: be10e0e1c8c96ce05aab8526d2010313662ed5f2
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913377"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="4ebdf-104">אודות ההגדרות של פרופיל AutoPilot</span><span class="sxs-lookup"><span data-stu-id="4ebdf-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="4ebdf-105">הגדרות פרופיל טייס אוטומטי</span><span class="sxs-lookup"><span data-stu-id="4ebdf-105">AutoPilot profile settings</span></span>

<span data-ttu-id="4ebdf-106">באפשרותך להשתמש בפרופילי טייס אוטומטי כדי לקבוע כיצד Windows מותקן בהתקני משתמשים.</span><span class="sxs-lookup"><span data-stu-id="4ebdf-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="4ebdf-107">הפרופילים מכילים את ההגדרות הבאות.</span><span class="sxs-lookup"><span data-stu-id="4ebdf-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="4ebdf-108">**תכונות ברירת מחדל של טייס אוטומטי (נדרש) המוגדרות באופן אוטומטי:**</span><span class="sxs-lookup"><span data-stu-id="4ebdf-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="4ebdf-109">**הגדרה**</span><span class="sxs-lookup"><span data-stu-id="4ebdf-109">**Setting**</span></span>|<span data-ttu-id="4ebdf-110">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="4ebdf-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4ebdf-111">דילוג על Cortana, OneDrive ורישום OEM</span><span class="sxs-lookup"><span data-stu-id="4ebdf-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="4ebdf-112">דילוג על התקנת אפליקציות לצרכן כגון Cortana ו-personal OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4ebdf-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="4ebdf-113">משתמש ההתקן יכול להתקין מאוחר יותר, כל עוד המשתמש הוא מנהל מערכת מקומי במכשיר.</span><span class="sxs-lookup"><span data-stu-id="4ebdf-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="4ebdf-114">המערכת תדלג על רישום היצרן המקורי מכיוון שההתקן ינוהל על-ידי Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="4ebdf-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="4ebdf-115">חוויית הכניסה באמצעות המותג של החברה שלך</span><span class="sxs-lookup"><span data-stu-id="4ebdf-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="4ebdf-116">אם לחברה שלך יש [הוספת התאמה למותג של החברה שלך לדף הכניסה של Microsoft 365](../admin/setup/customize-sign-in-page.md), משתמש ההתקן יקבל חוויה זו בעת הכניסה.</span><span class="sxs-lookup"><span data-stu-id="4ebdf-116">If your company has a [Add your company branding to Microsoft 365 Sign In page](../admin/setup/customize-sign-in-page.md), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="4ebdf-117">הרשמה אוטומטית של MDM עם חשבונות שתצורתם נקבעה.</span><span class="sxs-lookup"><span data-stu-id="4ebdf-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="4ebdf-118">זהות המשתמש תנוהל על-ידי תכלת Active Directory, ומשתמשים ייכנסו ל-Windows ו-Microsoft 365 באמצעות אישורי ה-Microsoft 365 Business Premium שלהם.</span><span class="sxs-lookup"><span data-stu-id="4ebdf-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Microsoft 365 with their Microsoft 365 Business Premium credentials.</span></span>  <br/> |
   
 <span data-ttu-id="4ebdf-119">**הגדרות אופציונליות:**</span><span class="sxs-lookup"><span data-stu-id="4ebdf-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="4ebdf-120">**הגדרה**</span><span class="sxs-lookup"><span data-stu-id="4ebdf-120">**Setting**</span></span>|<span data-ttu-id="4ebdf-121">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="4ebdf-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4ebdf-122">דילוג על הגדרות פרטיות (כבוי כברירת מחדל)</span><span class="sxs-lookup"><span data-stu-id="4ebdf-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="4ebdf-123">אם אפשרות זו מוגדרת למצב **מופעל**, משתמש ההתקן לא יראה את הסכם הרשיון עבור ההתקן והחלונות כאשר הוא יופיע לראשונה.</span><span class="sxs-lookup"><span data-stu-id="4ebdf-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="4ebdf-124">אל תאפשר למשתמש להפוך למנהל המערכת המקומי</span><span class="sxs-lookup"><span data-stu-id="4ebdf-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="4ebdf-125">אם אפשרות זו מוגדרת למצב **מופעל**, משתמש ההתקן לא יוכל להתקין אפליקציות אישיות כלשהן, כגון Cortana.</span><span class="sxs-lookup"><span data-stu-id="4ebdf-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
