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
ms.openlocfilehash: 90c11caa03249408ba2916d303bcb4a59fbcca8c
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400953"
---
# <a name="device-states"></a><span data-ttu-id="3ed65-103">מצבי המכשיר</span><span class="sxs-lookup"><span data-stu-id="3ed65-103">Device states</span></span>

<span data-ttu-id="3ed65-104">מכשירים ברשימה **פעולות מכשיר** (דף הבית של הניהול \> **פעולות מכשיר**) יכולים לכלול את המצבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="3ed65-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="3ed65-106">**מצב**</span><span class="sxs-lookup"><span data-stu-id="3ed65-106">**Status**</span></span>|<span data-ttu-id="3ed65-107">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="3ed65-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3ed65-108">מנוהל על-ידי Intune</span><span class="sxs-lookup"><span data-stu-id="3ed65-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="3ed65-109">מנוהל על ידי מיקרוסופט 365 עסקים פרימיום.</span><span class="sxs-lookup"><span data-stu-id="3ed65-109">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="3ed65-110">בהמתנה להוצאה משימוש</span><span class="sxs-lookup"><span data-stu-id="3ed65-110">Retire pending</span></span>  <br/> |<span data-ttu-id="3ed65-111">מיקרוסופט 365 עסקים Premium מתכונן להסיר את נתוני החברה מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="3ed65-111">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="3ed65-112">הוצאה משימוש מתבצעת</span><span class="sxs-lookup"><span data-stu-id="3ed65-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="3ed65-113">Microsoft 365 Business Premium מסיר כעת נתוני חברה מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="3ed65-113">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="3ed65-114">הוצאה משימוש נכשלה</span><span class="sxs-lookup"><span data-stu-id="3ed65-114">Retire failed</span></span>  <br/> | <span data-ttu-id="3ed65-115">פעולת הסרת נתוני החברה נכשלה.</span><span class="sxs-lookup"><span data-stu-id="3ed65-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="3ed65-116">פרישה בוטלה</span><span class="sxs-lookup"><span data-stu-id="3ed65-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="3ed65-117">פעולת הפרישה בוטלה.</span><span class="sxs-lookup"><span data-stu-id="3ed65-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="3ed65-118">בהמתנה למחיקה</span><span class="sxs-lookup"><span data-stu-id="3ed65-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="3ed65-119">ממתין להתחלת איפוס להדגרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="3ed65-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="3ed65-120">מחיקה מתבצעת</span><span class="sxs-lookup"><span data-stu-id="3ed65-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="3ed65-121">בוצע איפוס להגדרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="3ed65-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="3ed65-122">מחיקה נכשלה</span><span class="sxs-lookup"><span data-stu-id="3ed65-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="3ed65-123">. לא יכולתי לבצע איפוס של המפעל</span><span class="sxs-lookup"><span data-stu-id="3ed65-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="3ed65-124">ניגוב בוטל</span><span class="sxs-lookup"><span data-stu-id="3ed65-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="3ed65-125">. מחיקת המפעל בוטלה</span><span class="sxs-lookup"><span data-stu-id="3ed65-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="3ed65-126">לא תקין</span><span class="sxs-lookup"><span data-stu-id="3ed65-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="3ed65-127">פעולה ממתינה (או בעיצומה), אך ההתקן לא נרשם במשך 30 + ימים.</span><span class="sxs-lookup"><span data-stu-id="3ed65-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="3ed65-128">בהמתנה למחיקה</span><span class="sxs-lookup"><span data-stu-id="3ed65-128">Delete pending</span></span>  <br/> |<span data-ttu-id="3ed65-129">פעולת המחיקה ממתינה.</span><span class="sxs-lookup"><span data-stu-id="3ed65-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="3ed65-130">התגלה</span><span class="sxs-lookup"><span data-stu-id="3ed65-130">Discovered</span></span>  <br/> |<span data-ttu-id="3ed65-131">מיקרוסופט 365 עסקים Premium זיהה את המכשיר.</span><span class="sxs-lookup"><span data-stu-id="3ed65-131">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
