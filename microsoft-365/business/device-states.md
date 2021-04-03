---
title: מצבי המכשיר
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: למד אודות מצבי המכשיר השונים ברשימה פעולות מכשירים בבית מנהל מערכת ב- Microsoft 365 לעסקים.
ms.openlocfilehash: e6f1b428413d094e0a1ce3afb026528074038736
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578466"
---
# <a name="device-states"></a><span data-ttu-id="f88cc-103">מצבי המכשיר</span><span class="sxs-lookup"><span data-stu-id="f88cc-103">Device states</span></span>

<span data-ttu-id="f88cc-104">מאמר זה חל על Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="f88cc-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="f88cc-105">מכשירים ברשימה **פעולות מכשיר** (דף הבית של הניהול \> **פעולות מכשיר**) יכולים לכלול את המצבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="f88cc-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="f88cc-107">**מצב**</span><span class="sxs-lookup"><span data-stu-id="f88cc-107">**Status**</span></span>|<span data-ttu-id="f88cc-108">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="f88cc-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f88cc-109">מנוהל על-ידי Intune</span><span class="sxs-lookup"><span data-stu-id="f88cc-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="f88cc-110">מנוהל על-ידי Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="f88cc-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="f88cc-111">בהמתנה להוצאה משימוש</span><span class="sxs-lookup"><span data-stu-id="f88cc-111">Retire pending</span></span>  <br/> |<span data-ttu-id="f88cc-112">Microsoft 365 Business Premium מתכונן להסיר נתוני חברה מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="f88cc-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="f88cc-113">הוצאה משימוש מתבצעת</span><span class="sxs-lookup"><span data-stu-id="f88cc-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="f88cc-114">Microsoft 365 Business Premium מסיר כעת נתוני חברה מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="f88cc-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="f88cc-115">הוצאה משימוש נכשלה</span><span class="sxs-lookup"><span data-stu-id="f88cc-115">Retire failed</span></span>  <br/> | <span data-ttu-id="f88cc-116">פעולת הסרת נתוני החברה נכשלה.</span><span class="sxs-lookup"><span data-stu-id="f88cc-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="f88cc-117">התבטל</span><span class="sxs-lookup"><span data-stu-id="f88cc-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="f88cc-118">פעולת הפרישה בוטלה.</span><span class="sxs-lookup"><span data-stu-id="f88cc-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="f88cc-119">בהמתנה למחיקה</span><span class="sxs-lookup"><span data-stu-id="f88cc-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="f88cc-120">ממתין להתחלת איפוס להדגרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="f88cc-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="f88cc-121">מחיקה מתבצעת</span><span class="sxs-lookup"><span data-stu-id="f88cc-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="f88cc-122">בוצע איפוס להגדרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="f88cc-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="f88cc-123">מחיקה נכשלה</span><span class="sxs-lookup"><span data-stu-id="f88cc-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="f88cc-124">לא היתה אפשרות לאפס את היצרן.</span><span class="sxs-lookup"><span data-stu-id="f88cc-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="f88cc-125">מחק בוטל</span><span class="sxs-lookup"><span data-stu-id="f88cc-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="f88cc-126">ניגוב היצרן בוטל.</span><span class="sxs-lookup"><span data-stu-id="f88cc-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="f88cc-127">לא תקין</span><span class="sxs-lookup"><span data-stu-id="f88cc-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="f88cc-128">פעולה ממתינה (או מתבצעת), אך המכשיר לא מחובר במשך 30+ ימים.</span><span class="sxs-lookup"><span data-stu-id="f88cc-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="f88cc-129">בהמתנה למחיקה</span><span class="sxs-lookup"><span data-stu-id="f88cc-129">Delete pending</span></span>  <br/> |<span data-ttu-id="f88cc-130">פעולת המחיקה ממתינה.</span><span class="sxs-lookup"><span data-stu-id="f88cc-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="f88cc-131">התגלה</span><span class="sxs-lookup"><span data-stu-id="f88cc-131">Discovered</span></span>  <br/> |<span data-ttu-id="f88cc-132">Microsoft 365 Business Premium זיהה את המכשיר.</span><span class="sxs-lookup"><span data-stu-id="f88cc-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
