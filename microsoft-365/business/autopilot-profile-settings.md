---
title: אודות ההגדרות של פרופיל AutoPilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: פרופילי AutoPilot עוזרים לך לשלוט באופן ההתקנה של Windows במכשירי משתמש. הפרופילים מכילים הגדרות ברירת מחדל והגדרות אופציונליות, כמו דלג על התקנת Cortana.
ms.openlocfilehash: 86f8718131f0a0b93e18e65e39e02e7d65aded1a
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578506"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="16448-104">אודות ההגדרות של פרופיל AutoPilot</span><span class="sxs-lookup"><span data-stu-id="16448-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="16448-105">הגדרות פרופיל AutoPilot</span><span class="sxs-lookup"><span data-stu-id="16448-105">AutoPilot profile settings</span></span>

<span data-ttu-id="16448-106">באפשרותך להשתמש בפרופילי AutoPilot כדי לשלוט באופן ההתקנה של Windows במכשירי משתמש.</span><span class="sxs-lookup"><span data-stu-id="16448-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="16448-107">הפרופילים מכילים את ההגדרות הבאות.</span><span class="sxs-lookup"><span data-stu-id="16448-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="16448-108">**תכונות ברירת המחדל של AutoPilot (נדרש) המוגדרות באופן אוטומטי:**</span><span class="sxs-lookup"><span data-stu-id="16448-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="16448-109">**הגדרה**</span><span class="sxs-lookup"><span data-stu-id="16448-109">**Setting**</span></span>|<span data-ttu-id="16448-110">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="16448-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="16448-111">דלג על רישום Cortana , OneDrive ו- OEM</span><span class="sxs-lookup"><span data-stu-id="16448-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="16448-112">מדלג על ההתקנה של יישומי צריכה, כמו Cortana ו- OneDrive אישי.</span><span class="sxs-lookup"><span data-stu-id="16448-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="16448-113">משתמש המכשיר יכול להתקין תקנות אלה מאוחר יותר כל עוד המשתמש הוא מנהל מערכת מקומי במכשיר.</span><span class="sxs-lookup"><span data-stu-id="16448-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="16448-114">המערכת דילגה על רישום היצרן המקורי מכיוון שהמכשיר ינוהל על-ידי Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="16448-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="16448-115">חוויית כניסה באמצעות מותג החברה שלך</span><span class="sxs-lookup"><span data-stu-id="16448-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="16448-116">אם לחברה שלך יש דף הוסף את המיתוג של החברה שלך לדף כניסה של [Microsoft 365](../admin/setup/customize-sign-in-page.md), משתמש המכשיר מקבל חוויה זו בעת הכניסה.</span><span class="sxs-lookup"><span data-stu-id="16448-116">If your company has a [Add your company branding to Microsoft 365 Sign In page](../admin/setup/customize-sign-in-page.md), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="16448-117">הרשמה אוטומטית של MDM עם חשבונות AAD שהוגדרו.</span><span class="sxs-lookup"><span data-stu-id="16448-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="16448-118">זהות המשתמש תנוהל על-ידי Azure Active Directory, והמשתמשים יירשם ל- Windows ול- Microsoft 365 עם אישורי Microsoft 365 Business Premium שלהם.</span><span class="sxs-lookup"><span data-stu-id="16448-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Microsoft 365 with their Microsoft 365 Business Premium credentials.</span></span>  <br/> |
   
 <span data-ttu-id="16448-119">**הגדרות אופציונליות:**</span><span class="sxs-lookup"><span data-stu-id="16448-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="16448-120">**הגדרה**</span><span class="sxs-lookup"><span data-stu-id="16448-120">**Setting**</span></span>|<span data-ttu-id="16448-121">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="16448-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="16448-122">דלג על הגדרות הפרטיות (כבוי כברירת מחדל)</span><span class="sxs-lookup"><span data-stu-id="16448-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="16448-123">אם אפשרות זו מוגדרת **ל'פועל',** משתמש המכשיר לא יראה את הסכם הרשיון עבור המכשיר ו- Windows כאשר הוא נכנס לראשונה.</span><span class="sxs-lookup"><span data-stu-id="16448-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="16448-124">אל תאפשר למשתמש להפוך למנהל המערכת המקומי</span><span class="sxs-lookup"><span data-stu-id="16448-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="16448-125">אם אפשרות זו מוגדרת **ל'הפעל',** משתמש המכשיר לא יוכל להתקין אפליקציות אישיות, כגון Cortana.</span><span class="sxs-lookup"><span data-stu-id="16448-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
