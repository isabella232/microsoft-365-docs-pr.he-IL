---
title: מצבי המכשיר
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: למד אודות מצבי ההתקן ב- Microsoft 365 Business.
ms.openlocfilehash: 06e5c800e6a104785c1fd0724223e05d7729722e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072719"
---
# <a name="device-states"></a><span data-ttu-id="93af9-103">מצבי המכשיר</span><span class="sxs-lookup"><span data-stu-id="93af9-103">Device states</span></span>

## <a name="device-states"></a><span data-ttu-id="93af9-104">מצבי המכשיר</span><span class="sxs-lookup"><span data-stu-id="93af9-104">Device states</span></span>

<span data-ttu-id="93af9-105">מכשירים ברשימה **פעולות מכשיר** (דף הבית של הניהול \> **פעולות מכשיר**) יכולים לכלול את המצבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="93af9-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="93af9-107">**מצב**</span><span class="sxs-lookup"><span data-stu-id="93af9-107">**Status**</span></span>|<span data-ttu-id="93af9-108">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="93af9-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="93af9-109">מנוהל על-ידי Intune</span><span class="sxs-lookup"><span data-stu-id="93af9-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="93af9-110">מנוהל על-ידי Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="93af9-110">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="93af9-111">בהמתנה להוצאה משימוש</span><span class="sxs-lookup"><span data-stu-id="93af9-111">Retire pending</span></span>  <br/> |<span data-ttu-id="93af9-112">Microsoft 365 Business מתכונן להסרת נתוני החברה מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="93af9-112">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="93af9-113">הוצאה משימוש מתבצעת</span><span class="sxs-lookup"><span data-stu-id="93af9-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="93af9-114">Microsoft 365 Business מסיר כעת את נתוני החברה מהמכשיר.</span><span class="sxs-lookup"><span data-stu-id="93af9-114">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="93af9-115">הוצאה משימוש נכשלה</span><span class="sxs-lookup"><span data-stu-id="93af9-115">Retire failed</span></span>  <br/> | <span data-ttu-id="93af9-116">פעולת הסרת נתוני החברה נכשלה.</span><span class="sxs-lookup"><span data-stu-id="93af9-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="93af9-117">הוצאה משימוש בוטלה</span><span class="sxs-lookup"><span data-stu-id="93af9-117">Retire cancelled</span></span>  <br/> |<span data-ttu-id="93af9-118">פעולת ההוצאה משימוש בוטלה.</span><span class="sxs-lookup"><span data-stu-id="93af9-118">Retire action was cancelled.</span></span>  <br/> |
|<span data-ttu-id="93af9-119">בהמתנה למחיקה</span><span class="sxs-lookup"><span data-stu-id="93af9-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="93af9-120">ממתין להתחלת איפוס להדגרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="93af9-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="93af9-121">מחיקה מתבצעת</span><span class="sxs-lookup"><span data-stu-id="93af9-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="93af9-122">בוצע איפוס להגדרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="93af9-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="93af9-123">מחיקה נכשלה</span><span class="sxs-lookup"><span data-stu-id="93af9-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="93af9-124">לא הייתה אפשרות לבצע איפוס להגדרות היצרן.</span><span class="sxs-lookup"><span data-stu-id="93af9-124">Couldn't perform factory reset.</span></span>  <br/> |
|<span data-ttu-id="93af9-125">מחיקה בוטלה</span><span class="sxs-lookup"><span data-stu-id="93af9-125">Wipe cancelled</span></span>  <br/> |<span data-ttu-id="93af9-126">מחיקה להגדרות היצרן בוטלה.</span><span class="sxs-lookup"><span data-stu-id="93af9-126">Factory wipe was cancelled.</span></span>  <br/> |
|<span data-ttu-id="93af9-127">לא תקין</span><span class="sxs-lookup"><span data-stu-id="93af9-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="93af9-128">המשמעות היא שפעולה ממתינה (או מתבצעת) אך לא בוצעה פעולת צ'ק אין למכשיר במשך למעלה מ- 30 יום.</span><span class="sxs-lookup"><span data-stu-id="93af9-128">This means that an action is pending (or in progress) but the device has not checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="93af9-129">בהמתנה למחיקה</span><span class="sxs-lookup"><span data-stu-id="93af9-129">Delete pending</span></span>  <br/> |<span data-ttu-id="93af9-130">פעולת המחיקה ממתינה.</span><span class="sxs-lookup"><span data-stu-id="93af9-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="93af9-131">התגלה</span><span class="sxs-lookup"><span data-stu-id="93af9-131">Discovered</span></span>  <br/> |<span data-ttu-id="93af9-132">Microsoft 365 Business זיהה את המכשיר.</span><span class="sxs-lookup"><span data-stu-id="93af9-132">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
