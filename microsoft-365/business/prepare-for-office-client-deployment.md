---
title: הכנה לפריסת לקוח של Office על-ידי Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: למד כיצד להתקין את יישומי Office של 32 סיביות במחשבים Windows 10 וכיצד במצב עדכני.
ms.openlocfilehash: 20269c493b0e3b5a7deb56a24a5e1a9583ef9d0a
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074649"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="3980e-103">הכנה לפריסת לקוח של Office על-ידי Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="3980e-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="3980e-104">הכנה להתקנה אוטומטית של יישומי Office במחשבי לקוח</span><span class="sxs-lookup"><span data-stu-id="3980e-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="3980e-105">באפשרותך להשתמש ב- Microsoft 365 Business כדי להתקין באופן אוטומטי את יישומי Office בגירסת 32 סיביות במחשבי Windows 10 ולהבטיח שהם עדכניים תמיד בעזרת עדכונים.</span><span class="sxs-lookup"><span data-stu-id="3980e-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps to Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="3980e-106">מוטב שהמחשב של משתמש הקצה יופעל באמצעות Windows 10 Business וכן:</span><span class="sxs-lookup"><span data-stu-id="3980e-106">This works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="3980e-107">הוא אינו כולל יישומים שולחניים קיימים של Office (‏Word, ‏Excel, ‏PowerPoint, ‏Outlook, ‏OneNote, ‏Publisher, ‏Access ו- OneDrive).</span><span class="sxs-lookup"><span data-stu-id="3980e-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="3980e-108">או</span><span class="sxs-lookup"><span data-stu-id="3980e-108">or</span></span>
    
- <span data-ttu-id="3980e-109">מותקנת בו גירסה קיימת של Office מסוג 'לחץ והפעל'.</span><span class="sxs-lookup"><span data-stu-id="3980e-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="3980e-p101">כדי לקבוע אם יש לך גירסת 'לחץ והפעל' של Office, בכל יישום של Office, עבור אל **קובץ** \> **חשבון** ( **חשבון Office** ב- Outlook). אם אתה רואה 'עדכוני Office' כפי שמוצג באיור הבא, פירוש הדבר שההתקנה בוצעה באמצעות 'לחץ והפעל'.</span><span class="sxs-lookup"><span data-stu-id="3980e-p101">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook). If you see Office Updates as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="3980e-113">**מי יפיק תועלת מתכונה זו**</span><span class="sxs-lookup"><span data-stu-id="3980e-113">**Who will benefit from having this feature**</span></span>
  
<span data-ttu-id="3980e-114">משתמש קצה שהמחשב שלו:</span><span class="sxs-lookup"><span data-stu-id="3980e-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="3980e-115">**כולל** רשיון משתמש של Windows 10 Business, רשיון פעיל של Microsoft 365 Business, עדכון Windows 10 ליוצרים ושהמחשב שלו מצורף ל- Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3980e-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="3980e-p102">**אינו כולל** יישומי Office בגירסת 64 סיביות (לדוגמה: Word,‏ Excel,‏ Powerpoint). אם יישומי Office בגירסת 64 סיביות נדרשים, תכונה זו אינה מתאימה כיוון שאין תמיכה בהפעלה של גירסת 64 סיביות מסוג 'לחץ והפעל' של Office 2016 ממסוף הניהול של Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="3980e-p102">**Doesn't have** 64-bit Office apps (example: Word, Excel, Powerpoint). If 64-bit Office apps are required, then this feature is not a good fit because there is no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="3980e-p103">**אינו כולל** יישומים עצמאיים של Windows Installer (MSI) 2016 (לדוגמה, Visio או Project). Microsoft 365 Business משדרג את Office לגירסת 'לחץ והפעל' של Office 2016 וזו אינה מתאימה ליישומים עצמאיים של Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="3980e-p103">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project). Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="3980e-120">הטבלה הבאה מפרטת את הפעולה שייתכן שמשתמשי הקצה/מנהלי המערכת יצטרכו לנקוט, בהתאם למצב ההתחלתי שלהם, כדי להשיג גירסת 'לחץ והפעל' מוצלחת בת 32 סיביות של פריסת Office ממסוף הניהול של Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="3980e-120">The following table details what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="3980e-121">**הפעלת מצב ההתקנה של Office**</span><span class="sxs-lookup"><span data-stu-id="3980e-121">**Starting Office install status**</span></span>|<span data-ttu-id="3980e-122">**הפעולה שיש לנקוט לפני התקנת Office עבור Microsoft 365 Business**</span><span class="sxs-lookup"><span data-stu-id="3980e-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="3980e-123">**מצב סיום**</span><span class="sxs-lookup"><span data-stu-id="3980e-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3980e-124">לא הותקנה חבילת Office</span><span class="sxs-lookup"><span data-stu-id="3980e-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="3980e-125">ללא</span><span class="sxs-lookup"><span data-stu-id="3980e-125">None</span></span>  <br/> |<span data-ttu-id="3980e-126">Office 2016 בגירסת 32 סיביות הותקן באמצעות 'לחץ והפעל'</span><span class="sxs-lookup"><span data-stu-id="3980e-126">Office 2016 32-bit is installed by using click-to-run</span></span>  <br/> |
|<span data-ttu-id="3980e-127">גירסת 'לחץ והפעל' קיימת של Office מסוג 32 סיביות (2016 או גירסה קודמת) וללא יישומים עצמאיים</span><span class="sxs-lookup"><span data-stu-id="3980e-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="3980e-128">ללא</span><span class="sxs-lookup"><span data-stu-id="3980e-128">None</span></span>  <br/> |<span data-ttu-id="3980e-129">שדרוג לגירסת 'לחץ והפעל' האחרונה של Office 2016 מסוג 32 סיביות, לפי הצורך **\***</span><span class="sxs-lookup"><span data-stu-id="3980e-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="3980e-130">גירסת 'לחץ והפעל' קיימת של Office מסוג 32 סיביות או יישומי Office עצמאיים מסוג 32 או 64 סיביות (למשל Visio, ‏Project)</span><span class="sxs-lookup"><span data-stu-id="3980e-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32- or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="3980e-131">ללא</span><span class="sxs-lookup"><span data-stu-id="3980e-131">None</span></span>  <br/> |<span data-ttu-id="3980e-p104">יישומים עצמאיים אינם מושפעים. שדרוג החבילה לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות</span><span class="sxs-lookup"><span data-stu-id="3980e-p104">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="3980e-134">גירסת 'לחץ והפעל' קיימת של Office מסוג 32 סיביות ויישומי Office עצמאיים של MSI מסוג 32 או 64 סיביות (למעט 2016)</span><span class="sxs-lookup"><span data-stu-id="3980e-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="3980e-135">ללא</span><span class="sxs-lookup"><span data-stu-id="3980e-135">None</span></span>  <br/> |<span data-ttu-id="3980e-p105">יישומים עצמאיים אינם מושפעים. שדרוג החבילה לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות</span><span class="sxs-lookup"><span data-stu-id="3980e-p105">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="3980e-138">גירסת 'לחץ והפעל' קיימת של Office מסוג 64 סיביות</span><span class="sxs-lookup"><span data-stu-id="3980e-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="3980e-139">הסרת התקנה של יישומי Office מסוג 64 סיביות, אם זה בסדר להחליף אותה ביישומי Office מסוג 32 סיביות</span><span class="sxs-lookup"><span data-stu-id="3980e-139">Uninstall the 64-bit Office apps, if it is OK to replace it with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="3980e-140">אם אתה מסיר את יישומי Office מסוג 64 סיביות, גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות מותקנת</span><span class="sxs-lookup"><span data-stu-id="3980e-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="3980e-141">התקנת MSI קיימת של Office 2016 עם או בלי יישומים עצמאיים</span><span class="sxs-lookup"><span data-stu-id="3980e-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="3980e-142">הסרת התקנה של MSI Office 2016.</span><span class="sxs-lookup"><span data-stu-id="3980e-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="3980e-p106">מותקנת גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות. ללא שינוי ביישומים עצמאיים</span><span class="sxs-lookup"><span data-stu-id="3980e-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="3980e-145">התקנת MSI קיימת של Office 2013 (או גירסה קודמת) ו/או יישומי Office עצמאיים</span><span class="sxs-lookup"><span data-stu-id="3980e-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="3980e-146">ללא</span><span class="sxs-lookup"><span data-stu-id="3980e-146">None</span></span>  <br/> |<span data-ttu-id="3980e-147">גירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות עם התקנת MSI Office קיימת מראש (ויישומים עצמאיים) מתקיימות זו לצד זו</span><span class="sxs-lookup"><span data-stu-id="3980e-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="3980e-p107">**(\*) הערה:** לא מתקיים שדרוג לגירסת 'לחץ והפעל' של Office 2016 מסוג 32 סיביות עקב באג ידוע. הבעיה תיפתר בקרוב.</span><span class="sxs-lookup"><span data-stu-id="3980e-p107">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug. Fix is in progress.</span></span> 
  


