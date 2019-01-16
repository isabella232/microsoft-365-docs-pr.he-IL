---
title: אימות הגדרות הגנה של אפליקציות במחשבי Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: למד כיצד לאמת את הגדרות ההגנה app עסקיים 365 Microsoft ב- Windows 10 התקנים.
ms.openlocfilehash: f00dd380103ad9498d77b0e8814bace3de168df4
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983294"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="c0b49-103">אימות הגדרות הגנה של אפליקציות במחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="c0b49-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="c0b49-104">ודא שמשתמשים אינם יכולים להעתיק נתונים של החברה לקבצים אישיים במכשירים של החברה</span><span class="sxs-lookup"><span data-stu-id="c0b49-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="c0b49-p101">לאחר שאתה [מגדיר מדיניות הגנה על אפליקציות](protection-settings-for-windows-10-devices.md), עשויות לחלוף כמה שעות בטרם המדיניות תיכנס לתוקף במכשירים של המשתמשים. אם **הפעלת** את ההגדרה **מנע ממשתמשים להעתיק נתוני חברה לקבצים אישיים וכפה עליהם לשמור קבצי עבודה ב- OneDrive for Business** עבור מכשירים השייכים לחברה, תוכל לבדוק זאת במכשירים של המשתמשים לאחר שהם יתחברו ל- Azure AD ויבצעו כניסה.</span><span class="sxs-lookup"><span data-stu-id="c0b49-p101">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices. If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they have connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="c0b49-107">**אימות הגדרות חיבור**</span><span class="sxs-lookup"><span data-stu-id="c0b49-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="c0b49-p102">לאחר להיכנס באמצעות אישורי Microsoft 365 עסקיים להתחבר AD תכלת הרקיע כפי שמתואר [להגדיר התקנים של Windows עבור משתמשים עסקיים 365 של Microsoft](set-up-windows-devices.md), עבור אל **ההגדרות של Windows** \> **חשבונות** \> \*\*Access בעבודה או בבית הספר \*\*. בחר **מחובר \<שם הדייר\> AD תכלת הרקיע**, ולאחר מכן בחר **מידע**.</span><span class="sxs-lookup"><span data-stu-id="c0b49-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="c0b49-111">בדף **מנוהל על-ידי** \<שם הדייר\>, תוכל לראות את **פרטי החיבור** הכוללים **כתובת שרת ניהול** כמו זו המוצגת באיור הבא.</span><span class="sxs-lookup"><span data-stu-id="c0b49-111">On the **Managed by** \<tenant name\> page you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="c0b49-113">**ודא שלא ניתן להדביק נתוני חברה באפליקציה שאינה מנוהלת**</span><span class="sxs-lookup"><span data-stu-id="c0b49-113">**Verify that you cannot paste company data to a non-managed app**</span></span>
  
1. <span data-ttu-id="c0b49-114">פתח את Outlook 2016 שהותקן על-ידי Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c0b49-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="c0b49-115">פתח הודעת דואר אלקטרוני והעתק חלק מהתוכן שלה.</span><span class="sxs-lookup"><span data-stu-id="c0b49-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="c0b49-116">פתח את 'פנקס רשימות' ונסה להדביק את התוכן.</span><span class="sxs-lookup"><span data-stu-id="c0b49-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="c0b49-117">תקבל שגיאה המציינת שהאפליקציה אינה יכולה לגשת לתוכן.</span><span class="sxs-lookup"><span data-stu-id="c0b49-117">You will receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="c0b49-119">עם זאת, תוכל להדביק את אותו תוכן ב- Word 2016.</span><span class="sxs-lookup"><span data-stu-id="c0b49-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="c0b49-120">ודא שמשתמשים אינם יכולים להעתיק נתונים של החברה לקבצים אישיים במכשירים אישיים</span><span class="sxs-lookup"><span data-stu-id="c0b49-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="c0b49-121">**אימות הגדרות חיבור**</span><span class="sxs-lookup"><span data-stu-id="c0b49-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="c0b49-122">במכשיר Windows 10 האישי שבו אתה מחובר בתור משתמש מקומי, עבור אל **הגדרות Windows** ולחץ או הקש על **חשבונות** \> **גישה לחשבון בעבודה או בבית ספר**.</span><span class="sxs-lookup"><span data-stu-id="c0b49-122">On your Windows 10 personal device where you are logged in as a local user, go to **Windows Settings** and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="c0b49-123">תחת **גישה לחשבון בעבודה או בבית ספר**, בחר **התחבר**.</span><span class="sxs-lookup"><span data-stu-id="c0b49-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="c0b49-124">הזן את אישור Microsoft 365 Business שלך בתיבת הדו-שיח **הגדר חשבון בעבודה או בבית ספר** \> **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="c0b49-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="c0b49-125">בדף **גישה לחשבון בעבודה או בבית ספר**, בחר את ה **חשבון בעבודה או בבית ספר** ולאחר מכן בחר **פרטים**.</span><span class="sxs-lookup"><span data-stu-id="c0b49-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Work or school account dalog.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="c0b49-127">בדף **גישה לחשבון עבודה או בית ספר**, תוכל לראות את **פרטי החיבור** הכוללים **כתובת שרת ניהול** כמו זו המוצגת באיור הבא, וכן כוללים את המילים  *wip*  ו-  *mam*  .</span><span class="sxs-lookup"><span data-stu-id="c0b49-127">On the **Access work or school** page you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="c0b49-129">**ודא שלא ניתן להדביק נתוני חברה באפליקציה שאינה מנוהלת**</span><span class="sxs-lookup"><span data-stu-id="c0b49-129">**Verify that you cannot paste company data to a non-managed app**</span></span>
  
1. <span data-ttu-id="c0b49-130">פתח את Outlook 2016 והוסף את חשבון Microsoft 365 Business שלך, אם נדרש; לאחר מכן, היכנס עם אישורי Microsoft 365 Business שלך.</span><span class="sxs-lookup"><span data-stu-id="c0b49-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="c0b49-131">פתח הודעת דואר אלקטרוני והעתק חלק מהתוכן שלה.</span><span class="sxs-lookup"><span data-stu-id="c0b49-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="c0b49-132">פתח את 'פנקס רשימות' ונסה להדביק את התוכן.</span><span class="sxs-lookup"><span data-stu-id="c0b49-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="c0b49-133">תקבל שגיאה המציינת שהאפליקציה אינה יכולה לגשת לתוכן.</span><span class="sxs-lookup"><span data-stu-id="c0b49-133">You will receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="c0b49-135">עם זאת, תוכל להדביק את אותו תוכן ב- Word 2016.</span><span class="sxs-lookup"><span data-stu-id="c0b49-135">You can, however, paste the same content into Word 2016.</span></span>
    

