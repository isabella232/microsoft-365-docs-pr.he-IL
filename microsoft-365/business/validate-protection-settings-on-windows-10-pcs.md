---
title: אימות הגדרות הגנה של אפליקציות במחשבי Windows 10
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: למד כיצד לאמת את הגדרות הגנת היישום העסקי של Microsoft 365 בהתקני Windows 10.
ms.openlocfilehash: 577921f7f33eafbbe652dcf825a145d89f1ff556
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42057249"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="54889-103">אימות הגדרות הגנה של אפליקציות במחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="54889-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="54889-104">ודא שמשתמשים אינם יכולים להעתיק נתונים של החברה לקבצים אישיים במכשירים של החברה</span><span class="sxs-lookup"><span data-stu-id="54889-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="54889-105">לאחר שאתה [מגדיר מדיניות הגנה על אפליקציות](protection-settings-for-windows-10-devices.md), עשויות לחלוף כמה שעות בטרם המדיניות תיכנס לתוקף במכשירים של המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="54889-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="54889-106">אם **הפעלת את** **הנתונים של החברה ' מנע ממשתמשים להעתיק ' לקבצים אישיים ולאלץ אותם לשמור קבצי עבודה בכונן אחד עבור** הגדרות עסקיות עבור התקנים בבעלות חברה, באפשרותך לבדוק זאת בהתקן המשתמש לאחר ההתחברות למודעה ולחתימה ב-.</span><span class="sxs-lookup"><span data-stu-id="54889-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="54889-107">**אימות הגדרות חיבור**</span><span class="sxs-lookup"><span data-stu-id="54889-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="54889-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span><span class="sxs-lookup"><span data-stu-id="54889-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="54889-111">בדף ' **מנוהל על-ידי** \<שם\> דייר ', באפשרותך לראות את **מידע החיבור** הכולל **כתובת שרת ניהול** כמו זו המוצגת באיור הבא.</span><span class="sxs-lookup"><span data-stu-id="54889-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="54889-113">**ודא שלא ניתן להדביק נתוני חברה ביישום שאינו מנוהל**</span><span class="sxs-lookup"><span data-stu-id="54889-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="54889-114">פתח את Outlook 2016 שהותקן על-ידי Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="54889-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="54889-115">פתח הודעת דואר אלקטרוני והעתק חלק מהתוכן שלה.</span><span class="sxs-lookup"><span data-stu-id="54889-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="54889-116">פתח את 'פנקס רשימות' ונסה להדביק את התוכן.</span><span class="sxs-lookup"><span data-stu-id="54889-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="54889-117">תקבל שגיאה המציינת כי ליישום אין אפשרות לגשת לתוכן.</span><span class="sxs-lookup"><span data-stu-id="54889-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="54889-119">עם זאת, תוכל להדביק את אותו תוכן ב- Word 2016.</span><span class="sxs-lookup"><span data-stu-id="54889-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="54889-120">ודא שמשתמשים אינם יכולים להעתיק נתונים של החברה לקבצים אישיים במכשירים אישיים</span><span class="sxs-lookup"><span data-stu-id="54889-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="54889-121">**אימות הגדרות חיבור**</span><span class="sxs-lookup"><span data-stu-id="54889-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="54889-122">בהתקן האישי של windows 10 שבו אתה מחובר כמשתמש מקומי, עבור אל **הגדרות Windows**ולחץ או הקש על **חשבון** \> **גישה לעבודה או בית ספר**.</span><span class="sxs-lookup"><span data-stu-id="54889-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="54889-123">תחת **גישה לחשבון בעבודה או בבית ספר**, בחר **התחבר**.</span><span class="sxs-lookup"><span data-stu-id="54889-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="54889-124">הזן את אישור Microsoft 365 Business שלך בתיבת הדו-שיח **הגדר חשבון בעבודה או בבית ספר** \> **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="54889-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="54889-125">בדף **גישה לחשבון בעבודה או בבית ספר**, בחר את ה **חשבון בעבודה או בבית ספר** ולאחר מכן בחר **פרטים**.</span><span class="sxs-lookup"><span data-stu-id="54889-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![לחץ או הקש על מידע בתיבת הדו עבודה או חשבון בית ספר.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="54889-127">בדף **עבודה או בית ספר של Access** , באפשרותך לראות את **מידע החיבור** הכולל **כתובת שרת ניהול** כגון האחת המוצגת באיור הבא, וכוללת את המילים *wip* *ואמא* בתוך.</span><span class="sxs-lookup"><span data-stu-id="54889-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="54889-129">**ודא שלא ניתן להדביק נתוני חברה ביישום שאינו מנוהל**</span><span class="sxs-lookup"><span data-stu-id="54889-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="54889-130">פתח את Outlook 2016 והוסף את חשבון Microsoft 365 Business שלך, אם נדרש; לאחר מכן, היכנס עם אישורי Microsoft 365 Business שלך.</span><span class="sxs-lookup"><span data-stu-id="54889-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="54889-131">פתח הודעת דואר אלקטרוני והעתק חלק מהתוכן שלה.</span><span class="sxs-lookup"><span data-stu-id="54889-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="54889-132">פתח את 'פנקס רשימות' ונסה להדביק את התוכן.</span><span class="sxs-lookup"><span data-stu-id="54889-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="54889-133">תקבל שגיאה המציינת ש-App אינו יכול לגשת לתוכן.</span><span class="sxs-lookup"><span data-stu-id="54889-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="54889-135">עם זאת, תוכל להדביק את אותו תוכן ב- Word 2016.</span><span class="sxs-lookup"><span data-stu-id="54889-135">You can, however, paste the same content into Word 2016.</span></span>
    

