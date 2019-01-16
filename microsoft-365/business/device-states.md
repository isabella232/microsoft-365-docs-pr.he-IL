---
title: מצבי המכשיר
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: למד אודות מצבי ההתקן ב- Microsoft 365 Business.
ms.openlocfilehash: bd6f1ad7f7671d9616fd14d477dfcfb164ff6bd0
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982904"
---
# <a name="device-states"></a><span data-ttu-id="f355a-103">מצבי המכשיר</span><span class="sxs-lookup"><span data-stu-id="f355a-103">Device states</span></span>

## <a name="device-states"></a><span data-ttu-id="f355a-104">מצבי המכשיר</span><span class="sxs-lookup"><span data-stu-id="f355a-104">Device states</span></span>

<span data-ttu-id="f355a-105">מכשירים ברשימה **פעולות מכשיר** (דף הבית של הניהול \> **פעולות מכשיר**) יכולים לכלול את המצבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="f355a-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="f355a-107">**מצב**</span><span class="sxs-lookup"><span data-stu-id="f355a-107">**Status**</span></span>|<span data-ttu-id="f355a-108">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="f355a-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f355a-109">מנוהל על-ידי Intune</span><span class="sxs-lookup"><span data-stu-id="f355a-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="f355a-110">מנוהל על-ידי Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="f355a-110">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="f355a-111">בהמתנה להוצאה משימוש</span><span class="sxs-lookup"><span data-stu-id="f355a-111">Retire pending</span></span>  <br/> |<span data-ttu-id="f355a-112">Microsoft 365 Business מתכונן להסרת נתוני החברה מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="f355a-112">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="f355a-113">הוצאה משימוש מתבצעת</span><span class="sxs-lookup"><span data-stu-id="f355a-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="f355a-114">Microsoft 365 Business מסיר כעת את נתוני החברה מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="f355a-114">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="f355a-115">הוצאה משימוש נכשלה</span><span class="sxs-lookup"><span data-stu-id="f355a-115">Retire failed</span></span>  <br/> | <span data-ttu-id="f355a-116">פעולת הסרת נתוני החברה נכשלה.</span><span class="sxs-lookup"><span data-stu-id="f355a-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="f355a-117">הוצאה משימוש בוטלה</span><span class="sxs-lookup"><span data-stu-id="f355a-117">Retire cancelled</span></span>  <br/> |<span data-ttu-id="f355a-118">פעולת ההוצאה משימוש בוטלה.</span><span class="sxs-lookup"><span data-stu-id="f355a-118">Retire action was cancelled.</span></span>  <br/> |
|<span data-ttu-id="f355a-119">בהמתנה למחיקה</span><span class="sxs-lookup"><span data-stu-id="f355a-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="f355a-120">ממתין להתחלת איפוס להדגרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="f355a-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="f355a-121">מחיקה מתבצעת</span><span class="sxs-lookup"><span data-stu-id="f355a-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="f355a-122">בוצע איפוס להגדרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="f355a-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="f355a-123">מחיקה נכשלה</span><span class="sxs-lookup"><span data-stu-id="f355a-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="f355a-124">לא הייתה אפשרות לבצע איפוס להגדרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="f355a-124">Couldn't perform factory reset.</span></span>  <br/> |
|<span data-ttu-id="f355a-125">מחיקה בוטלה</span><span class="sxs-lookup"><span data-stu-id="f355a-125">Wipe cancelled</span></span>  <br/> |<span data-ttu-id="f355a-126">מחיקה להגדרות היצרן בוטלה.</span><span class="sxs-lookup"><span data-stu-id="f355a-126">Factory wipe was cancelled.</span></span>  <br/> |
|<span data-ttu-id="f355a-127">לא תקין</span><span class="sxs-lookup"><span data-stu-id="f355a-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="f355a-128">המשמעות היא שפעולה ממתינה (או מתבצעת) אך לא בוצעה פעולת צ'ק אין למכשיר במשך למעלה מ- 30 יום.</span><span class="sxs-lookup"><span data-stu-id="f355a-128">This means that an action is pending (or in progress) but the device has not checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="f355a-129">בהמתנה למחיקה</span><span class="sxs-lookup"><span data-stu-id="f355a-129">Delete pending</span></span>  <br/> |<span data-ttu-id="f355a-130">פעולת המחיקה ממתינה.</span><span class="sxs-lookup"><span data-stu-id="f355a-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="f355a-131">התגלה</span><span class="sxs-lookup"><span data-stu-id="f355a-131">Discovered</span></span>  <br/> |<span data-ttu-id="f355a-132">Microsoft 365 Business זיהה את המכשיר.</span><span class="sxs-lookup"><span data-stu-id="f355a-132">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
