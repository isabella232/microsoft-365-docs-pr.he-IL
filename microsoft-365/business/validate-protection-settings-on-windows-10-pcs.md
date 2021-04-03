---
title: אימות הגדרות הגנה של אפליקציות במחשבי Windows 10
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: אמת את הגדרות ההגנה על אפליקציית Microsoft 365 Business Premium במכשירי Windows 10 וודא שמשתמשים אינם יכולים להעתיק נתוני חברה לקבצים אישיים או ליישומים שאינם מנוהלים.
ms.openlocfilehash: e319ffa5149f055b5de45078facc8899acffc223
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579861"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="b0081-103">אימות הגדרות הגנה של אפליקציות במחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="b0081-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="b0081-104">ודא שמשתמשים אינם יכולים להעתיק נתונים של החברה לקבצים אישיים במכשירים של החברה</span><span class="sxs-lookup"><span data-stu-id="b0081-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="b0081-105">לאחר שאתה [מגדיר מדיניות הגנה על אפליקציות](protection-settings-for-windows-10-devices.md), עשויות לחלוף כמה שעות בטרם המדיניות תיכנס לתוקף במכשירים של המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="b0081-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="b0081-106">אם הפכת את **ההגדרה** מנע ממשתמשים להעתיק נתוני חברה לקבצים אישיים ולאלץ אותם לשמור קבצי עבודה ב- **OneDrive for Business** עבור מכשירים בבעלות החברה, באפשרותך לבדוק זאת במכשיר של המשתמש לאחר שהם התחברו ל- Azure AD והינם מחוברים.</span><span class="sxs-lookup"><span data-stu-id="b0081-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="b0081-107">**אימות הגדרות חיבור**</span><span class="sxs-lookup"><span data-stu-id="b0081-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="b0081-108">לאחר שתיתחבר באמצעות אישורי Microsoft 365 Business Premium ותתחבר ל- Azure AD כמתואר בהגדיר מכשירי Windows עבור [משתמשי Microsoft 365 Business Premium](set-up-windows-devices.md), עבור אל חשבונות הגדרות **Windows** Access עבודה או \>  \> **בית ספר.**</span><span class="sxs-lookup"><span data-stu-id="b0081-108">After you sign in with Microsoft 365 Business Premium credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**.</span></span> <span data-ttu-id="b0081-109">בחר **מחובר \<tenant name\> ל- Azure AD** ולאחר מכן בחר **מידע**.</span><span class="sxs-lookup"><span data-stu-id="b0081-109">Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="b0081-111">בדף **מנוהל על-ידי,** באפשרותך לראות את פרטי החיבור הכוללים כתובת \<tenant name\> שרת **ניהול,** כמו זו המוצגת באיור הבא. </span><span class="sxs-lookup"><span data-stu-id="b0081-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="b0081-113">**ודא שלא ניתן להדביק נתוני חברה באפליקציה לא מנוהלת**</span><span class="sxs-lookup"><span data-stu-id="b0081-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="b0081-114">פתח את Outlook 2016 שהותקן על-ידי Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="b0081-114">Open Outlook 2016 that was installed by Microsoft 365 Business Premium.</span></span>
    
2. <span data-ttu-id="b0081-115">פתח הודעת דואר אלקטרוני והעתק חלק מהתוכן שלה.</span><span class="sxs-lookup"><span data-stu-id="b0081-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="b0081-116">פתח את 'פנקס רשימות' ונסה להדביק את התוכן.</span><span class="sxs-lookup"><span data-stu-id="b0081-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="b0081-117">תקבל שגיאה המציין שלאפליקציה אין אפשרות לגשת לתוכן.</span><span class="sxs-lookup"><span data-stu-id="b0081-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="b0081-119">עם זאת, תוכל להדביק את אותו תוכן ב- Word 2016.</span><span class="sxs-lookup"><span data-stu-id="b0081-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="b0081-120">ודא שמשתמשים אינם יכולים להעתיק נתונים של החברה לקבצים אישיים במכשירים אישיים</span><span class="sxs-lookup"><span data-stu-id="b0081-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="b0081-121">**אימות הגדרות חיבור**</span><span class="sxs-lookup"><span data-stu-id="b0081-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="b0081-122">במכשיר האישי שלך ב- Windows 10 שבו אתה מחובר כמשתמש מקומי, עבור אל **הגדרות Windows** ולאחר מכן לחץ או הקש על **חשבונות** Access בעבודה או \> **בבית ספר**.</span><span class="sxs-lookup"><span data-stu-id="b0081-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="b0081-123">תחת **גישה לחשבון בעבודה או בבית ספר**, בחר **התחבר**.</span><span class="sxs-lookup"><span data-stu-id="b0081-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="b0081-124">הזן את אישור Microsoft 365 Business Premium שלך בתיבת **הדו-שיח הגדרת חשבון בעבודה או בבית** ספר \> **היכנס.**</span><span class="sxs-lookup"><span data-stu-id="b0081-124">Enter your Microsoft 365 Business Premium credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="b0081-125">בדף **גישה לחשבון בעבודה או בבית ספר**, בחר את ה **חשבון בעבודה או בבית ספר** ולאחר מכן בחר **פרטים**.</span><span class="sxs-lookup"><span data-stu-id="b0081-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![לחץ או הקש על מידע בתיבת הדו-שיח חשבון בעבודה או בבית ספר.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="b0081-127">בדף **Access בעבודה** או בבית ספר, באפשרותך  לראות את פרטי החיבור הכוללים כתובת **שרת** ניהול, כמו זו המוצגת באיור הבא, וכוללת את המילים *wip* *ו- mam* בתוך.</span><span class="sxs-lookup"><span data-stu-id="b0081-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="b0081-129">**ודא שלא ניתן להדביק נתוני חברה באפליקציה לא מנוהלת**</span><span class="sxs-lookup"><span data-stu-id="b0081-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="b0081-130">פתח את Outlook 2016 והוסף את חשבון Microsoft 365 Business Premium שלך במקרה הצורך והירשם באמצעות אישורי Microsoft 365 Business Premium שלך.</span><span class="sxs-lookup"><span data-stu-id="b0081-130">Open Outlook 2016 and add your Microsoft 365 Business Premium account if necessary and sign in with your Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="b0081-131">פתח הודעת דואר אלקטרוני והעתק חלק מהתוכן שלה.</span><span class="sxs-lookup"><span data-stu-id="b0081-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="b0081-132">פתח את 'פנקס רשימות' ונסה להדביק את התוכן.</span><span class="sxs-lookup"><span data-stu-id="b0081-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="b0081-133">תקבל שגיאה שמציין ש- App לא יכול לגשת לתוכן.</span><span class="sxs-lookup"><span data-stu-id="b0081-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="b0081-135">עם זאת, תוכל להדביק את אותו תוכן ב- Word 2016.</span><span class="sxs-lookup"><span data-stu-id="b0081-135">You can, however, paste the same content into Word 2016.</span></span>
    

