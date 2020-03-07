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
description: למד אודות מצבי ההתקנים השונים ברשימה פעולות התקן בבית Admin ב-Microsoft 365 Business.
ms.openlocfilehash: bed1610814ca0d60adb4b4b3d0018e3e7e6d763f
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/07/2020
ms.locfileid: "42560819"
---
# <a name="device-states"></a><span data-ttu-id="601f2-103">מצבי המכשיר</span><span class="sxs-lookup"><span data-stu-id="601f2-103">Device states</span></span>

<span data-ttu-id="601f2-104">מכשירים ברשימה **פעולות מכשיר** (דף הבית של הניהול \> **פעולות מכשיר**) יכולים לכלול את המצבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="601f2-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="601f2-106">**מצב**</span><span class="sxs-lookup"><span data-stu-id="601f2-106">**Status**</span></span>|<span data-ttu-id="601f2-107">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="601f2-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="601f2-108">מנוהל על-ידי Intune</span><span class="sxs-lookup"><span data-stu-id="601f2-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="601f2-109">מנוהל על-ידי Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="601f2-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="601f2-110">בהמתנה להוצאה משימוש</span><span class="sxs-lookup"><span data-stu-id="601f2-110">Retire pending</span></span>  <br/> |<span data-ttu-id="601f2-111">Microsoft 365 Business מתכונן להסרת נתוני החברה מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="601f2-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="601f2-112">הוצאה משימוש מתבצעת</span><span class="sxs-lookup"><span data-stu-id="601f2-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="601f2-113">Microsoft 365 Business מסיר כעת את נתוני החברה מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="601f2-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="601f2-114">הוצאה משימוש נכשלה</span><span class="sxs-lookup"><span data-stu-id="601f2-114">Retire failed</span></span>  <br/> | <span data-ttu-id="601f2-115">פעולת הסרת נתוני החברה נכשלה.</span><span class="sxs-lookup"><span data-stu-id="601f2-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="601f2-116">פרישה בוטלה</span><span class="sxs-lookup"><span data-stu-id="601f2-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="601f2-117">פעולת הפרישה בוטלה.</span><span class="sxs-lookup"><span data-stu-id="601f2-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="601f2-118">בהמתנה למחיקה</span><span class="sxs-lookup"><span data-stu-id="601f2-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="601f2-119">ממתין להתחלת איפוס להדגרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="601f2-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="601f2-120">מחיקה מתבצעת</span><span class="sxs-lookup"><span data-stu-id="601f2-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="601f2-121">בוצע איפוס להגדרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="601f2-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="601f2-122">מחיקה נכשלה</span><span class="sxs-lookup"><span data-stu-id="601f2-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="601f2-123">. לא יכולתי לבצע איפוס של המפעל</span><span class="sxs-lookup"><span data-stu-id="601f2-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="601f2-124">ניגוב בוטל</span><span class="sxs-lookup"><span data-stu-id="601f2-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="601f2-125">. מחיקת המפעל בוטלה</span><span class="sxs-lookup"><span data-stu-id="601f2-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="601f2-126">לא תקין</span><span class="sxs-lookup"><span data-stu-id="601f2-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="601f2-127">פעולה ממתינה (או בעיצומה), אך ההתקן לא נרשם במשך 30 + ימים.</span><span class="sxs-lookup"><span data-stu-id="601f2-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="601f2-128">בהמתנה למחיקה</span><span class="sxs-lookup"><span data-stu-id="601f2-128">Delete pending</span></span>  <br/> |<span data-ttu-id="601f2-129">פעולת המחיקה ממתינה.</span><span class="sxs-lookup"><span data-stu-id="601f2-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="601f2-130">התגלה</span><span class="sxs-lookup"><span data-stu-id="601f2-130">Discovered</span></span>  <br/> |<span data-ttu-id="601f2-131">Microsoft 365 Business זיהה את המכשיר.</span><span class="sxs-lookup"><span data-stu-id="601f2-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
