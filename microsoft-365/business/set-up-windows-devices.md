---
title: הגדרת מכשירי Windows עבור משתמשי Microsoft 365 Business Premium
f1.keywords:
- CSH
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
- okr_smb
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: למד כיצד להגדיר מכשירי Windows פועלים עם Windows 10 Pro עבור משתמשי Microsoft 365 Business Premium, המאפשרים ניהול מרכזי ופקדי אבטחה.
ms.openlocfilehash: 9c9ffe5bd74d9e9877a87309757c481576ee89d2
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578126"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="81e69-103">הגדרת מכשירי Windows עבור משתמשי Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="81e69-103">Set up Windows devices for Microsoft 365 Business Premium users</span></span>

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="81e69-104">דרישות מוקדמות להגדרת מכשירי Windows עבור משתמשי Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="81e69-104">Prerequisites for setting up Windows devices for Microsoft 365 Business Premium users</span></span>

<span data-ttu-id="81e69-105">כדי שתוכל להגדיר מכשירי Windows עבור משתמשי Microsoft 365 Business Premium, ודא שכל מכשירי Windows פועלים עם Windows 10 Pro, גירסה 1703 (Creators Update).</span><span class="sxs-lookup"><span data-stu-id="81e69-105">Before you can set up Windows devices for Microsoft 365 Business Premium users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update).</span></span> <span data-ttu-id="81e69-106">Windows 10 Pro הוא דרישה מוקדמת לפריסת Windows 10 Business, שהיא קבוצה של שירותי ענן ויכולות ניהול מכשירים המשלים את Windows 10 Pro ותאפשר את פקדי הניהול והאבטחה המרכזיים של Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="81e69-106">Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business Premium.</span></span>
  
<span data-ttu-id="81e69-107">אם יש לך מכשירי Windows פועלים עם Windows 7 Pro , Windows 8 Pro או Windows 8.1 Pro, מנוי Microsoft 365 Business Premium שלך מזכה אותך בשדרוג של Windows 10.</span><span class="sxs-lookup"><span data-stu-id="81e69-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business Premium subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="81e69-108">לקבלת מידע נוסף על שדרוג מכשירי Windows לעדכון Windows 10 ליוצרים, פעל לפי השלבים בנושא זה: [שדרוג מכשירי Windows לעדכון Windows Pro ליוצרים](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="81e69-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="81e69-109">ראה [אימות שהמכשיר מחובר ל- Azure AD](#verify-the-device-is-connected-to-azure-ad) כדי לוודא שהשדרוג מסוים, או כדי לוודא שהשדרוג פעל.</span><span class="sxs-lookup"><span data-stu-id="81e69-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="81e69-110">צפה בסרטון וידאו קצר אודות חיבור Windows ל- Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="81e69-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="81e69-111">אם סרטון וידאו זה היה שימושי עבורך, עיין ב[סדרת ההדרכה המלאה עבור עסקים קטנים ומשתמשים חדשים ב- Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="81e69-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="81e69-112">צירוף מכשירי Windows 10 ל- Azure AD של הארגון שלך</span><span class="sxs-lookup"><span data-stu-id="81e69-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="81e69-113">כאשר כל מכשירי Windows בארגון שלך שודרגו ל- Windows 10 Pro Creators Update או שכבר פועלים Windows 10 Pro Creators Update, באפשרותך להצטרף למכשירים אלה ל- Azure Active Directory של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="81e69-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="81e69-114">לאחר ההצפנה של המכשירים, הם ישודררגו באופן אוטומטי ל- Windows 10 Business, שהוא חלק ממשינוי Microsoft 365 Business Premium שלך.</span><span class="sxs-lookup"><span data-stu-id="81e69-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business Premium subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="81e69-115">עבור מכשיר Windows 10 Pro חדש לגמרי או ששודרג לאחרונה</span><span class="sxs-lookup"><span data-stu-id="81e69-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="81e69-116">עבור מכשיר חדש לגמרי שעדכון Windows 10 Pro ליוצרים פועל בו, או עבור מכשיר ששודרג לעדכון Windows 10 Pro ליוצרים אך לא הוגדר ל- Windows 10, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="81e69-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="81e69-117">עבור על פרטי ההגדרה של מכשיר Windows 10 עד שתגיע לעמוד **כיצד ברצונך להגדיר?**.</span><span class="sxs-lookup"><span data-stu-id="81e69-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="81e69-119">כאן, בחר **הגדר עבור ארגון ולאחר מכן הזן** את שם המשתמש והסיסמה שלך עבור Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="81e69-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business Premium.</span></span> 
    
3. <span data-ttu-id="81e69-120">סיים את הגדרת מכשיר Windows 10.</span><span class="sxs-lookup"><span data-stu-id="81e69-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="81e69-p103">כשתסיים, המשתמש יהיה מחובר ל- Azure AD של הארגון שלך. ראה [אימות שהמכשיר מחובר ל- Azure AD](#verify-the-device-is-connected-to-azure-ad) כדי לוודא.</span><span class="sxs-lookup"><span data-stu-id="81e69-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="81e69-123">עבור מכשיר שכבר מוגדר וש- Windows 10 Pro פועל בו</span><span class="sxs-lookup"><span data-stu-id="81e69-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="81e69-124">**חיבור משתמשים ל- Azure AD:**</span><span class="sxs-lookup"><span data-stu-id="81e69-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="81e69-125">במחשב ה- Windows של המשתמש שלך, שפועל בו Windows 10 Pro, גירסה 1703 (עדכון ליוצרים) (ראה [דרישות מוקדמות](pre-requisites-for-data-protection.md)), לחץ על סמל Windows ולאחר מכן על סמל 'הגדרות'.</span><span class="sxs-lookup"><span data-stu-id="81e69-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="81e69-127">ב **הגדרות**, עבור אל **חשבונות**.</span><span class="sxs-lookup"><span data-stu-id="81e69-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="81e69-129">בדף **המידע שלך**, לחץ על **גישה לחשבון עבודה או בית ספר** \> **התחבר**.</span><span class="sxs-lookup"><span data-stu-id="81e69-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="81e69-131">בתיבת הדו-שיח **הגדר חשבון בעבודה או בבית ספר**, תחת **פעולות חלופיות**, בחר **צרף מכשיר זה ל- Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="81e69-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="81e69-133">בדף **בוא נבצע את תהליך הכניסה**, הזן את החשבון שלך בעבודה או בבית הספר \> **הבא**.</span><span class="sxs-lookup"><span data-stu-id="81e69-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="81e69-134">בדף **הזנת סיסמה**, הזן את הסיסמה שלך \> **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="81e69-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="81e69-136">בדף **ודא שזהו הארגון שלך,** ודא שהמידע נכון ובחר **הצטרף.**</span><span class="sxs-lookup"><span data-stu-id="81e69-136">On the **Make sure this is your organization** page, verify that the information is correct, and choose **Join**.</span></span>
  
   <span data-ttu-id="81e69-137">ב- **אתה מוכן!**</span><span class="sxs-lookup"><span data-stu-id="81e69-137">On the **You're all set!**</span></span> <span data-ttu-id="81e69-138">page, chosse **Done**.</span><span class="sxs-lookup"><span data-stu-id="81e69-138">page, chosse **Done**.</span></span>
  
   ![במסך ודא שזהו הארגון שלך, בחר הצטרף](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="81e69-140">אם העלית קבצים אל OneDrive for Business, סנכרן אותם בחזרה.</span><span class="sxs-lookup"><span data-stu-id="81e69-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="81e69-141">אם השתמשת בכלי של ספקים אחרים להעברת פרופיל וקבצים, סנכרן גם אותם עם הפרופיל החדש.</span><span class="sxs-lookup"><span data-stu-id="81e69-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="81e69-142">אימות שהמכשיר מחובר ל- Azure AD</span><span class="sxs-lookup"><span data-stu-id="81e69-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="81e69-143">כדי לאמת את מצב הסינכרון שלך, **בדף Access** בעבודה  או בבית ספר בהגדרות **,** בחר באזור מחובר אל _ _ כדי לחשוף את הלחצנים מידע \<organization name\> **והתנתק.** </span><span class="sxs-lookup"><span data-stu-id="81e69-143">To verify your sync status, on the **Access work or school** page in **Settings**, select the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**.</span></span> <span data-ttu-id="81e69-144">בחר **מידע כדי** לקבל את מצב הסינכרון שלך.</span><span class="sxs-lookup"><span data-stu-id="81e69-144">Choose **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="81e69-145">בדף מצב **סינכרון,** בחר **סנכרן** כדי לקבל את מדיניות הניהול העדכנית ביותר של מכשירים ניידים למחשב.</span><span class="sxs-lookup"><span data-stu-id="81e69-145">On the **Sync status** page, choose **Sync** to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="81e69-146">כדי להתחיל להשתמש בחשבון Microsoft 365 Business Premium, עבור אל לחצן **התחל** של Windows, לחץ באמצעות לחצן העכבר הימני על תמונת החשבון הנוכחית שלך ולאחר מכן **החלף חשבון**.</span><span class="sxs-lookup"><span data-stu-id="81e69-146">To start using the Microsoft 365 Business Premium account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="81e69-147">היכנס באמצעות הדואר האלקטרוני והסיסמה של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="81e69-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a><span data-ttu-id="81e69-149">ודא שהמחשב משודרג ל- Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="81e69-149">Verify the PC is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="81e69-150">ודא שהתקני Azure AD המצורפים ל- Windows 10 משודרגים ל- Windows 10 Business כחלק ממשינוי Microsoft 365 Business Premium שלך.</span><span class="sxs-lookup"><span data-stu-id="81e69-150">Verify that your Azure AD joined Windows 10 devices are upgraded to Windows 10 Business as part of your Microsoft 365 Business Premium subscription.</span></span>
  
1. <span data-ttu-id="81e69-151">עבור אל **הגדרות** \> **מערכת** \> **אודות**.</span><span class="sxs-lookup"><span data-stu-id="81e69-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="81e69-152">ודא שתחת **מהדורה** מופיע **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="81e69-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="81e69-154">השלבים הבאים</span><span class="sxs-lookup"><span data-stu-id="81e69-154">Next steps</span></span>

<span data-ttu-id="81e69-155">כדי להגדיר את המכשירים הניידים שלך, ראה הגדרת מכשירים ניידים עבור [משתמשי Microsoft 365 Business Premium](set-up-mobile-devices.md), כדי להגדיר מדיניות הגנה על מכשירים או הגנה על יישומים, ראה ניהול [Microsoft 365 לעסקים.](manage.md)</span><span class="sxs-lookup"><span data-stu-id="81e69-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 for business](manage.md).</span></span>
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a><span data-ttu-id="81e69-156">לקבלת מידע נוסף על ההגדרה והשימוש ב- Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="81e69-156">For more on setting up and using Microsoft 365 Business Premium</span></span>

[<span data-ttu-id="81e69-157">סרטוני הדרכה של Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="81e69-157">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
