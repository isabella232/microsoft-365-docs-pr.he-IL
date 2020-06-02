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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: למד אודות מצבי ההתקנים השונים ברשימה פעולות התקן בבית Admin ב-Microsoft 365 עבור עסקים.
ms.openlocfilehash: 64138e2b6ae73c067709cde1912a96615d08ebf1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471178"
---
# <a name="device-states"></a><span data-ttu-id="fa99e-103">מצבי המכשיר</span><span class="sxs-lookup"><span data-stu-id="fa99e-103">Device states</span></span>

<span data-ttu-id="fa99e-104">מאמר זה חל על 365 עסקים Premium של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fa99e-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="fa99e-105">מכשירים ברשימה **פעולות מכשיר** (דף הבית של הניהול \> **פעולות מכשיר**) יכולים לכלול את המצבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="fa99e-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="fa99e-107">**מצב**</span><span class="sxs-lookup"><span data-stu-id="fa99e-107">**Status**</span></span>|<span data-ttu-id="fa99e-108">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="fa99e-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fa99e-109">מנוהל על-ידי Intune</span><span class="sxs-lookup"><span data-stu-id="fa99e-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="fa99e-110">מנוהל על ידי מיקרוסופט 365 עסקים פרימיום.</span><span class="sxs-lookup"><span data-stu-id="fa99e-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="fa99e-111">בהמתנה להוצאה משימוש</span><span class="sxs-lookup"><span data-stu-id="fa99e-111">Retire pending</span></span>  <br/> |<span data-ttu-id="fa99e-112">מיקרוסופט 365 עסקים Premium מתכונן להסיר את נתוני החברה מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="fa99e-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="fa99e-113">הוצאה משימוש מתבצעת</span><span class="sxs-lookup"><span data-stu-id="fa99e-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="fa99e-114">Microsoft 365 Business Premium מסיר כעת נתוני חברה מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="fa99e-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="fa99e-115">הוצאה משימוש נכשלה</span><span class="sxs-lookup"><span data-stu-id="fa99e-115">Retire failed</span></span>  <br/> | <span data-ttu-id="fa99e-116">פעולת הסרת נתוני החברה נכשלה.</span><span class="sxs-lookup"><span data-stu-id="fa99e-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="fa99e-117">פרישה בוטלה</span><span class="sxs-lookup"><span data-stu-id="fa99e-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="fa99e-118">פעולת הפרישה בוטלה.</span><span class="sxs-lookup"><span data-stu-id="fa99e-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="fa99e-119">בהמתנה למחיקה</span><span class="sxs-lookup"><span data-stu-id="fa99e-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="fa99e-120">ממתין להתחלת איפוס להדגרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="fa99e-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="fa99e-121">מחיקה מתבצעת</span><span class="sxs-lookup"><span data-stu-id="fa99e-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="fa99e-122">בוצע איפוס להגדרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="fa99e-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="fa99e-123">מחיקה נכשלה</span><span class="sxs-lookup"><span data-stu-id="fa99e-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="fa99e-124">. לא יכולתי לבצע איפוס של המפעל</span><span class="sxs-lookup"><span data-stu-id="fa99e-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="fa99e-125">ניגוב בוטל</span><span class="sxs-lookup"><span data-stu-id="fa99e-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="fa99e-126">. מחיקת המפעל בוטלה</span><span class="sxs-lookup"><span data-stu-id="fa99e-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="fa99e-127">לא תקין</span><span class="sxs-lookup"><span data-stu-id="fa99e-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="fa99e-128">פעולה ממתינה (או בעיצומה), אך ההתקן לא נרשם במשך 30 + ימים.</span><span class="sxs-lookup"><span data-stu-id="fa99e-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="fa99e-129">בהמתנה למחיקה</span><span class="sxs-lookup"><span data-stu-id="fa99e-129">Delete pending</span></span>  <br/> |<span data-ttu-id="fa99e-130">פעולת המחיקה ממתינה.</span><span class="sxs-lookup"><span data-stu-id="fa99e-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="fa99e-131">התגלה</span><span class="sxs-lookup"><span data-stu-id="fa99e-131">Discovered</span></span>  <br/> |<span data-ttu-id="fa99e-132">מיקרוסופט 365 עסקים Premium זיהה את המכשיר.</span><span class="sxs-lookup"><span data-stu-id="fa99e-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
