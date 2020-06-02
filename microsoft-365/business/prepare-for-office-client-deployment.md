---
title: הכנה לפריסת לקוח Office על-ידי Microsoft 365 לעסקים
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: למד כיצד להתקין באופן אוטומטי את יישומי Office 32-bit במחשבי Windows 10 ולעדכן אותם.
ms.openlocfilehash: 2de492914edbde2afe593aac290c4a634b801443
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470946"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="c6a9c-103">הכנה לפריסת לקוח Office על-ידי Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="c6a9c-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

<span data-ttu-id="c6a9c-104">מאמר זה חל על 365 עסקים Premium של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c6a9c-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="c6a9c-105">הכנה להתקנה אוטומטית של יישומי Office במחשבי לקוח</span><span class="sxs-lookup"><span data-stu-id="c6a9c-105">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="c6a9c-106">באפשרותך להשתמש ב-Microsoft 365 Business Premium כדי להתקין באופן אוטומטי את יישומי Office מסוג 32-bit במחשבי Windows 10 ולשמור אותם עדכניים באמצעות עדכונים.</span><span class="sxs-lookup"><span data-stu-id="c6a9c-106">You can use Microsoft 365 Business Premium to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="c6a9c-107">ההתקנה האוטומטית פועלת באופן הטוב ביותר אם המחשב של משתמש הקצה הוא ב-Windows 10 Business ו:</span><span class="sxs-lookup"><span data-stu-id="c6a9c-107">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="c6a9c-108">הוא אינו כולל יישומים שולחניים קיימים של Office (‏Word, ‏Excel, ‏PowerPoint, ‏Outlook, ‏OneNote, ‏Publisher, ‏Access ו- OneDrive).</span><span class="sxs-lookup"><span data-stu-id="c6a9c-108">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="c6a9c-109">או</span><span class="sxs-lookup"><span data-stu-id="c6a9c-109">or</span></span>
    
- <span data-ttu-id="c6a9c-110">מותקנת בו גירסה קיימת של Office מסוג 'לחץ והפעל'.</span><span class="sxs-lookup"><span data-stu-id="c6a9c-110">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="c6a9c-111">כדי לקבוע אם יש לך גירסת 'לחץ והפעל' של Office, בכל יישום של Office, עבור אל **קובץ** \> **חשבון** ( **חשבון Office** ב- Outlook).</span><span class="sxs-lookup"><span data-stu-id="c6a9c-111">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="c6a9c-112">אם אתה רואה **עדכונים של Office** כפי שמוצג באיור הבא, ההתקנה נעשתה על-ידי שימוש בלחיצה-להפעלה.</span><span class="sxs-lookup"><span data-stu-id="c6a9c-112">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="c6a9c-114">**שנהנה מתכונה זו**</span><span class="sxs-lookup"><span data-stu-id="c6a9c-114">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="c6a9c-115">משתמש קצה שהמחשב שלו:</span><span class="sxs-lookup"><span data-stu-id="c6a9c-115">The end user whose PC:</span></span>
  
- <span data-ttu-id="c6a9c-116">**כולל** רישיון משתמש עסקי של Windows 10, 365 פעיל של Microsoft עבור רשיון עסקי, Windows 10 יוצרי עדכונים, והוא מצורף לספריית הפעילים התכולים.</span><span class="sxs-lookup"><span data-stu-id="c6a9c-116">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="c6a9c-117">אין **ברשותך** יישומי Office 64-bit (לדוגמה: Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="c6a9c-117">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="c6a9c-118">אם 64-bit apps Office נדרשים, תכונה זו אינה מתאימה בכלל, משום שאין תמיכה בהפעלת גירסה 64-bit 2016 לחץ-להפעלה של Office מ-Microsoft 365 עבור מסוף ניהול עסקי.</span><span class="sxs-lookup"><span data-stu-id="c6a9c-118">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="c6a9c-119">**אינו כולל** יישומים עצמאיים של Windows Installer (MSI) 2016 (לדוגמה, Visio או Project).</span><span class="sxs-lookup"><span data-stu-id="c6a9c-119">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="c6a9c-120">Microsoft 365 עבור שדרוגים עסקיים Office לגירסת הלחיצה-להפעלה של Office 2016 ושאינה פועלת עם יישומים עצמאיים של Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="c6a9c-120">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="c6a9c-121">הטבלה הבאה מציגה את הפעולה שייתכן כי משתמשי הקצה/מנהלים יצטרכו לנקוט, בהתאם למצב ההתחלה שלהם, לקבל גירסה מוצלחת של 32 סיביות להפעלה של פריסת Office מ-Microsoft 365 עבור מסוף ניהול עסקי.</span><span class="sxs-lookup"><span data-stu-id="c6a9c-121">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span>
  
|<span data-ttu-id="c6a9c-122">**הפעלת מצב ההתקנה של Office**</span><span class="sxs-lookup"><span data-stu-id="c6a9c-122">**Starting Office install status**</span></span>|<span data-ttu-id="c6a9c-123">**פעולה לביצוע לפני Microsoft 365 עבור התקנת Office עסקיים**</span><span class="sxs-lookup"><span data-stu-id="c6a9c-123">**Action to take before Microsoft 365 for business Office install**</span></span>|<span data-ttu-id="c6a9c-124">**מצב סיום**</span><span class="sxs-lookup"><span data-stu-id="c6a9c-124">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c6a9c-125">לא הותקנה חבילת Office</span><span class="sxs-lookup"><span data-stu-id="c6a9c-125">No Office suite installed</span></span>  <br/> |<span data-ttu-id="c6a9c-126">ללא</span><span class="sxs-lookup"><span data-stu-id="c6a9c-126">None</span></span>  <br/> |<span data-ttu-id="c6a9c-127">Office 2016 32-bit מותקן באמצעות ' לחץ להפעלה '</span><span class="sxs-lookup"><span data-stu-id="c6a9c-127">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="c6a9c-128">גירסת 'לחץ והפעל' קיימת של Office מסוג 32 סיביות (2016 או גירסה קודמת) וללא יישומים עצמאיים</span><span class="sxs-lookup"><span data-stu-id="c6a9c-128">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="c6a9c-129">ללא</span><span class="sxs-lookup"><span data-stu-id="c6a9c-129">None</span></span>  <br/> |<span data-ttu-id="c6a9c-130">שדרוג לגירסת 'לחץ והפעל' האחרונה של Office 2016 מסוג 32 סיביות, לפי הצורך **\***</span><span class="sxs-lookup"><span data-stu-id="c6a9c-130">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="c6a9c-131">גירסת לחיצה על הפעלה מסוג 32-bit של Office ולחיצה-להפעלה קיימת, 32-bit או 64-bit של יישומי Office עצמאיים (לדוגמה, Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="c6a9c-131">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="c6a9c-132">ללא</span><span class="sxs-lookup"><span data-stu-id="c6a9c-132">None</span></span>  <br/> |<span data-ttu-id="c6a9c-133">יישומים עצמאיים אינם מושפעים.</span><span class="sxs-lookup"><span data-stu-id="c6a9c-133">Standalone apps aren't affected.</span></span> <span data-ttu-id="c6a9c-134">שדרוג החבילה לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות</span><span class="sxs-lookup"><span data-stu-id="c6a9c-134">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="c6a9c-135">גירסת 'לחץ והפעל' קיימת של Office מסוג 32 סיביות ויישומי Office עצמאיים של MSI מסוג 32 או 64 סיביות (למעט 2016)</span><span class="sxs-lookup"><span data-stu-id="c6a9c-135">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="c6a9c-136">ללא</span><span class="sxs-lookup"><span data-stu-id="c6a9c-136">None</span></span>  <br/> |<span data-ttu-id="c6a9c-137">יישומים עצמאיים אינם מושפעים.</span><span class="sxs-lookup"><span data-stu-id="c6a9c-137">Standalone apps aren't affected.</span></span> <span data-ttu-id="c6a9c-138">שדרוג החבילה לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות</span><span class="sxs-lookup"><span data-stu-id="c6a9c-138">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="c6a9c-139">גירסת 'לחץ והפעל' קיימת של Office מסוג 64 סיביות</span><span class="sxs-lookup"><span data-stu-id="c6a9c-139">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="c6a9c-140">הסר את ההתקנה של יישומי Office 64-bit, אם זה בסדר להחליף אותם ביישומי Office בעלי 32 סיביות</span><span class="sxs-lookup"><span data-stu-id="c6a9c-140">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="c6a9c-141">אם אתה מסיר את יישומי Office מסוג 64 סיביות, גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות מותקנת</span><span class="sxs-lookup"><span data-stu-id="c6a9c-141">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="c6a9c-142">התקנת MSI קיימת של Office 2016 עם או בלי יישומים עצמאיים</span><span class="sxs-lookup"><span data-stu-id="c6a9c-142">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="c6a9c-143">הסרת התקנה של MSI Office 2016.</span><span class="sxs-lookup"><span data-stu-id="c6a9c-143">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="c6a9c-p106">מותקנת גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות. ללא שינוי ביישומים עצמאיים</span><span class="sxs-lookup"><span data-stu-id="c6a9c-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="c6a9c-146">התקנת MSI קיימת של Office 2013 (או גירסה קודמת) ו/או יישומי Office עצמאיים</span><span class="sxs-lookup"><span data-stu-id="c6a9c-146">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="c6a9c-147">ללא</span><span class="sxs-lookup"><span data-stu-id="c6a9c-147">None</span></span>  <br/> |<span data-ttu-id="c6a9c-148">גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות עם התקנת MSI Office קיימת מראש (ויישומים עצמאיים) מתקיימות זו לצד זו</span><span class="sxs-lookup"><span data-stu-id="c6a9c-148">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="c6a9c-149">**(\*) הערה:** לא מתקיים שדרוג לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות עקב באג ידוע.</span><span class="sxs-lookup"><span data-stu-id="c6a9c-149">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="c6a9c-150">. התיקון מתבצע</span><span class="sxs-lookup"><span data-stu-id="c6a9c-150">A fix is in progress.</span></span> 
  
