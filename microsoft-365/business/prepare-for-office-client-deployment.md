---
title: הכנה לפריסת לקוח של Office על-ידי Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: למד כיצד להתקין באופן אוטומטי את יישומי Office 32-bit במחשבי Windows 10 ולעדכן אותם.
ms.openlocfilehash: 0f8cd7df49ad627b190fad6737ec95a6d64d99d0
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065104"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="c0e56-103">הכנה לפריסת לקוח של Office על-ידי Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="c0e56-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="c0e56-104">הכנה להתקנה אוטומטית של יישומי Office במחשבי לקוח</span><span class="sxs-lookup"><span data-stu-id="c0e56-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="c0e56-105">באפשרותך להשתמש ב-Microsoft 365 Business כדי להתקין באופן אוטומטי את יישומי Office מסוג 32-bit במחשבי Windows 10 ולשמור אותם עדכניים באמצעות עדכונים.</span><span class="sxs-lookup"><span data-stu-id="c0e56-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="c0e56-106">ההתקנה האוטומטית פועלת באופן הטוב ביותר אם המחשב של משתמש הקצה הוא ב-Windows 10 Business ו:</span><span class="sxs-lookup"><span data-stu-id="c0e56-106">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="c0e56-107">הוא אינו כולל יישומים שולחניים קיימים של Office (‏Word, ‏Excel, ‏PowerPoint, ‏Outlook, ‏OneNote, ‏Publisher, ‏Access ו- OneDrive).</span><span class="sxs-lookup"><span data-stu-id="c0e56-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="c0e56-108">או</span><span class="sxs-lookup"><span data-stu-id="c0e56-108">or</span></span>
    
- <span data-ttu-id="c0e56-109">מותקנת בו גירסה קיימת של Office מסוג 'לחץ והפעל'.</span><span class="sxs-lookup"><span data-stu-id="c0e56-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="c0e56-110">כדי לקבוע אם יש לך גירסת 'לחץ והפעל' של Office, בכל יישום של Office, עבור אל **קובץ** \> **חשבון** ( **חשבון Office** ב- Outlook).</span><span class="sxs-lookup"><span data-stu-id="c0e56-110">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="c0e56-111">אם אתה רואה **עדכונים של Office** כפי שמוצג באיור הבא, ההתקנה נעשתה על-ידי שימוש בלחיצה-להפעלה.</span><span class="sxs-lookup"><span data-stu-id="c0e56-111">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="c0e56-113">**שנהנה מתכונה זו**</span><span class="sxs-lookup"><span data-stu-id="c0e56-113">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="c0e56-114">משתמש קצה שהמחשב שלו:</span><span class="sxs-lookup"><span data-stu-id="c0e56-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="c0e56-115">**כולל** רשיון משתמש של Windows 10 Business, רשיון פעיל של Microsoft 365 Business, עדכון Windows 10 ליוצרים ושהמחשב שלו מצורף ל- Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c0e56-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="c0e56-116">אין **ברשותך** יישומי Office 64-bit (לדוגמה: Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="c0e56-116">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="c0e56-117">אם 64-bit apps Office נדרשים, תכונה זו אינה מתאימה בכלל, משום שאין תמיכה בהפעלת גירסה 64-bit 2016 לחץ-להפעלה של Office מתוך מסוף מנהל העסקים של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c0e56-117">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="c0e56-118">**אינו כולל** יישומים עצמאיים של Windows Installer (MSI) 2016 (לדוגמה, Visio או Project).</span><span class="sxs-lookup"><span data-stu-id="c0e56-118">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="c0e56-119">Microsoft 365 עסקים שדרוגים Office לגירסת הלחיצה-אל-הפעל של Office 2016 ושאינה פועלת עם יישומים עצמאיים של Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="c0e56-119">Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="c0e56-120">הטבלה הבאה מציגה את הפעולה שייתכן שמשתמשי הקצה/מנהלים יצטרכו לבצע, בהתאם למצב ההתחלה שלהם, לקבל גירסה מוצלחת של 32 סיביות להפעלה של פריסת Office ממסוף הניהול העסקי של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c0e56-120">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="c0e56-121">**הפעלת מצב ההתקנה של Office**</span><span class="sxs-lookup"><span data-stu-id="c0e56-121">**Starting Office install status**</span></span>|<span data-ttu-id="c0e56-122">**הפעולה שיש לנקוט לפני התקנת Office עבור Microsoft 365 Business**</span><span class="sxs-lookup"><span data-stu-id="c0e56-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="c0e56-123">**מצב סיום**</span><span class="sxs-lookup"><span data-stu-id="c0e56-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c0e56-124">לא הותקנה חבילת Office</span><span class="sxs-lookup"><span data-stu-id="c0e56-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="c0e56-125">ללא</span><span class="sxs-lookup"><span data-stu-id="c0e56-125">None</span></span>  <br/> |<span data-ttu-id="c0e56-126">Office 2016 32-bit מותקן באמצעות ' לחץ להפעלה '</span><span class="sxs-lookup"><span data-stu-id="c0e56-126">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="c0e56-127">גירסת 'לחץ והפעל' קיימת של Office מסוג 32 סיביות (2016 או גירסה קודמת) וללא יישומים עצמאיים</span><span class="sxs-lookup"><span data-stu-id="c0e56-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="c0e56-128">ללא</span><span class="sxs-lookup"><span data-stu-id="c0e56-128">None</span></span>  <br/> |<span data-ttu-id="c0e56-129">שדרוג לגירסת 'לחץ והפעל' האחרונה של Office 2016 מסוג 32 סיביות, לפי הצורך **\***</span><span class="sxs-lookup"><span data-stu-id="c0e56-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="c0e56-130">גירסת לחיצה על הפעלה מסוג 32-bit של Office ולחיצה-להפעלה קיימת, 32-bit או 64-bit של יישומי Office עצמאיים (לדוגמה, Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="c0e56-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="c0e56-131">ללא</span><span class="sxs-lookup"><span data-stu-id="c0e56-131">None</span></span>  <br/> |<span data-ttu-id="c0e56-132">יישומים עצמאיים אינם מושפעים.</span><span class="sxs-lookup"><span data-stu-id="c0e56-132">Standalone apps aren't affected.</span></span> <span data-ttu-id="c0e56-133">שדרוג החבילה לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות</span><span class="sxs-lookup"><span data-stu-id="c0e56-133">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="c0e56-134">גירסת 'לחץ והפעל' קיימת של Office מסוג 32 סיביות ויישומי Office עצמאיים של MSI מסוג 32 או 64 סיביות (למעט 2016)</span><span class="sxs-lookup"><span data-stu-id="c0e56-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="c0e56-135">ללא</span><span class="sxs-lookup"><span data-stu-id="c0e56-135">None</span></span>  <br/> |<span data-ttu-id="c0e56-136">יישומים עצמאיים אינם מושפעים.</span><span class="sxs-lookup"><span data-stu-id="c0e56-136">Standalone apps aren't affected.</span></span> <span data-ttu-id="c0e56-137">שדרוג החבילה לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות</span><span class="sxs-lookup"><span data-stu-id="c0e56-137">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="c0e56-138">גירסת 'לחץ והפעל' קיימת של Office מסוג 64 סיביות</span><span class="sxs-lookup"><span data-stu-id="c0e56-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="c0e56-139">הסר את ההתקנה של יישומי Office 64-bit, אם זה בסדר להחליף אותם ביישומי Office בעלי 32 סיביות</span><span class="sxs-lookup"><span data-stu-id="c0e56-139">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="c0e56-140">אם אתה מסיר את יישומי Office מסוג 64 סיביות, גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות מותקנת</span><span class="sxs-lookup"><span data-stu-id="c0e56-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="c0e56-141">התקנת MSI קיימת של Office 2016 עם או בלי יישומים עצמאיים</span><span class="sxs-lookup"><span data-stu-id="c0e56-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="c0e56-142">הסרת התקנה של MSI Office 2016.</span><span class="sxs-lookup"><span data-stu-id="c0e56-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="c0e56-p106">מותקנת גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות. ללא שינוי ביישומים עצמאיים</span><span class="sxs-lookup"><span data-stu-id="c0e56-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="c0e56-145">התקנת MSI קיימת של Office 2013 (או גירסה קודמת) ו/או יישומי Office עצמאיים</span><span class="sxs-lookup"><span data-stu-id="c0e56-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="c0e56-146">ללא</span><span class="sxs-lookup"><span data-stu-id="c0e56-146">None</span></span>  <br/> |<span data-ttu-id="c0e56-147">גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות עם התקנת MSI Office קיימת מראש (ויישומים עצמאיים) מתקיימות זו לצד זו</span><span class="sxs-lookup"><span data-stu-id="c0e56-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="c0e56-148">**(\*) הערה:** לא מתקיים שדרוג לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות עקב באג ידוע.</span><span class="sxs-lookup"><span data-stu-id="c0e56-148">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="c0e56-149">. התיקון מתבצע</span><span class="sxs-lookup"><span data-stu-id="c0e56-149">A fix is in progress.</span></span> 
  
