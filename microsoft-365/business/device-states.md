---
title: מצבי המכשיר
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: למד אודות מצבי ההתקנים השונים ברשימה פעולות התקן בבית Admin ב-Microsoft 365 עבור עסקים.
ms.openlocfilehash: 1a66e76dd3a74428923292427b01551db2449e48
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627245"
---
# <a name="device-states"></a><span data-ttu-id="54691-103">מצבי המכשיר</span><span class="sxs-lookup"><span data-stu-id="54691-103">Device states</span></span>

<span data-ttu-id="54691-104">מכשירים ברשימה **פעולות מכשיר** (דף הבית של הניהול \> **פעולות מכשיר**) יכולים לכלול את המצבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="54691-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="54691-106">**מצב**</span><span class="sxs-lookup"><span data-stu-id="54691-106">**Status**</span></span>|<span data-ttu-id="54691-107">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="54691-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="54691-108">מנוהל על-ידי Intune</span><span class="sxs-lookup"><span data-stu-id="54691-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="54691-109">מנוהל על ידי מיקרוסופט 365 עסקים פרימיום.</span><span class="sxs-lookup"><span data-stu-id="54691-109">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="54691-110">בהמתנה להוצאה משימוש</span><span class="sxs-lookup"><span data-stu-id="54691-110">Retire pending</span></span>  <br/> |<span data-ttu-id="54691-111">מיקרוסופט 365 עסקים Premium מתכונן להסיר את נתוני החברה מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="54691-111">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="54691-112">הוצאה משימוש מתבצעת</span><span class="sxs-lookup"><span data-stu-id="54691-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="54691-113">Microsoft 365 Business Premium מסיר כעת נתוני חברה מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="54691-113">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="54691-114">הוצאה משימוש נכשלה</span><span class="sxs-lookup"><span data-stu-id="54691-114">Retire failed</span></span>  <br/> | <span data-ttu-id="54691-115">פעולת הסרת נתוני החברה נכשלה.</span><span class="sxs-lookup"><span data-stu-id="54691-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="54691-116">פרישה בוטלה</span><span class="sxs-lookup"><span data-stu-id="54691-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="54691-117">פעולת הפרישה בוטלה.</span><span class="sxs-lookup"><span data-stu-id="54691-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="54691-118">בהמתנה למחיקה</span><span class="sxs-lookup"><span data-stu-id="54691-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="54691-119">ממתין להתחלת איפוס להדגרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="54691-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="54691-120">מחיקה מתבצעת</span><span class="sxs-lookup"><span data-stu-id="54691-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="54691-121">בוצע איפוס להגדרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="54691-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="54691-122">מחיקה נכשלה</span><span class="sxs-lookup"><span data-stu-id="54691-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="54691-123">. לא יכולתי לבצע איפוס של המפעל</span><span class="sxs-lookup"><span data-stu-id="54691-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="54691-124">ניגוב בוטל</span><span class="sxs-lookup"><span data-stu-id="54691-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="54691-125">. מחיקת המפעל בוטלה</span><span class="sxs-lookup"><span data-stu-id="54691-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="54691-126">לא תקין</span><span class="sxs-lookup"><span data-stu-id="54691-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="54691-127">פעולה ממתינה (או בעיצומה), אך ההתקן לא נרשם במשך 30 + ימים.</span><span class="sxs-lookup"><span data-stu-id="54691-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="54691-128">בהמתנה למחיקה</span><span class="sxs-lookup"><span data-stu-id="54691-128">Delete pending</span></span>  <br/> |<span data-ttu-id="54691-129">פעולת המחיקה ממתינה.</span><span class="sxs-lookup"><span data-stu-id="54691-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="54691-130">התגלה</span><span class="sxs-lookup"><span data-stu-id="54691-130">Discovered</span></span>  <br/> |<span data-ttu-id="54691-131">מיקרוסופט 365 עסקים Premium זיהה את המכשיר.</span><span class="sxs-lookup"><span data-stu-id="54691-131">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
