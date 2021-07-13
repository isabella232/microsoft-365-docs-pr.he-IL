---
title: הגדרת Windows עבור Microsoft 365 Business Premium המשתמשים
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
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: הגדר Windows פועלים Windows 10 Pro עבור Microsoft 365 Business Premium המשתמשים, ומאפשרים ניהול מרכזי ופקדי אבטחה.
ms.openlocfilehash: a911414b1a7abef259f4c5fffbdd48e07f9ebfdd
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/12/2021
ms.locfileid: "53393358"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="dde03-103">הגדרת Windows עבור Microsoft 365 Business Premium המשתמשים</span><span class="sxs-lookup"><span data-stu-id="dde03-103">Set up Windows devices for Microsoft 365 Business Premium users</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="dde03-104">לפני שתתחיל</span><span class="sxs-lookup"><span data-stu-id="dde03-104">Before you begin</span></span>

<span data-ttu-id="dde03-105">כדי שתוכל להגדיר Windows עבור משתמשי Microsoft 365 Business Premium, ודא שכל מכשירי Windows פועלים Windows 10 Pro, גירסה 1703 (Creators Update).</span><span class="sxs-lookup"><span data-stu-id="dde03-105">Before you can set up Windows devices for Microsoft 365 Business Premium users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update).</span></span> <span data-ttu-id="dde03-106">Windows 10 Pro היא דרישה מוקדמת לפריסת Windows 10 Business, שהיא ערכה של שירותי ענן ויכולות לניהול מכשירים המשלים את Windows 10 Pro ולאפשר את פקדי הניהול והאבטחה המרכזיים של Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="dde03-106">Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business Premium.</span></span>
  
<span data-ttu-id="dde03-107">אם יש לך Windows פועלים Windows 7 Pro, Windows 8 Pro או Windows 8.1 Pro, המנוי Microsoft 365 Business Premium שלך מקנה לך Windows 10 שדרוג.</span><span class="sxs-lookup"><span data-stu-id="dde03-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business Premium subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="dde03-108">לקבלת מידע נוסף על שדרוג מכשירי Windows לעדכון Windows 10 ליוצרים, פעל לפי השלבים בנושא זה: [שדרוג מכשירי Windows לעדכון Windows Pro ליוצרים](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="dde03-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="dde03-109">ראה [אימות שהמכשיר מחובר ל- Azure AD](#verify-the-device-is-connected-to-azure-ad) כדי לוודא שהשדרוג מסוים, או כדי לוודא שהשדרוג פעל.</span><span class="sxs-lookup"><span data-stu-id="dde03-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

## <a name="watch-connect-your-pc-to-microsoft-365-business"></a><span data-ttu-id="dde03-110">צפה: התחברות למחשב שלך כדי Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="dde03-110">Watch: Connect your PC to Microsoft 365 Business</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="dde03-111">אם סרטון וידאו זה היה שימושי עבורך, עיין ב[סדרת ההדרכה המלאה עבור עסקים קטנים ומשתמשים חדשים ב- Microsoft 365](../business-video/index.yml).</span><span class="sxs-lookup"><span data-stu-id="dde03-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](../business-video/index.yml).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="dde03-112">צירוף מכשירי Windows 10 ל- Azure AD של הארגון שלך</span><span class="sxs-lookup"><span data-stu-id="dde03-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="dde03-113">כאשר כל Windows בארגון שלך שודרגו לעדכון Windows 10 Pro ליוצרים או שכבר פועלים Windows 10 Pro Creators Update, באפשרותך להצטרף למכשירים אלה ל- Azure Active Directory של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="dde03-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="dde03-114">לאחר ההצטרפות של המכשירים, הם ישודררגו באופן אוטומטי ל- Windows 10 Business, שהוא חלק Microsoft 365 Business Premium שלך.</span><span class="sxs-lookup"><span data-stu-id="dde03-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business Premium subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="dde03-115">עבור מכשיר Windows 10 Pro חדש לגמרי או ששודרג לאחרונה</span><span class="sxs-lookup"><span data-stu-id="dde03-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="dde03-116">עבור מכשיר חדש לגמרי שעדכון Windows 10 Pro ליוצרים פועל בו, או עבור מכשיר ששודרג לעדכון Windows 10 Pro ליוצרים אך לא הוגדר ל- Windows 10, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="dde03-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="dde03-117">עבור על פרטי ההגדרה של מכשיר Windows 10 עד שתגיע לעמוד **כיצד ברצונך להגדיר?**.</span><span class="sxs-lookup"><span data-stu-id="dde03-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="dde03-119">כאן, בחר **הגדר עבור ארגון ולאחר מכן הזן** את שם המשתמש והסיסמה שלך עבור Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="dde03-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business Premium.</span></span> 
    
3. <span data-ttu-id="dde03-120">סיים את הגדרת מכשיר Windows 10.</span><span class="sxs-lookup"><span data-stu-id="dde03-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="dde03-p103">כשתסיים, המשתמש יהיה מחובר ל- Azure AD של הארגון שלך. ראה [אימות שהמכשיר מחובר ל- Azure AD](#verify-the-device-is-connected-to-azure-ad) כדי לוודא.</span><span class="sxs-lookup"><span data-stu-id="dde03-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="dde03-123">עבור מכשיר שכבר מוגדר וש- Windows 10 Pro פועל בו</span><span class="sxs-lookup"><span data-stu-id="dde03-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="dde03-124">**חיבור משתמשים ל- Azure AD:**</span><span class="sxs-lookup"><span data-stu-id="dde03-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="dde03-125">במחשב ה- Windows של המשתמש שלך, שפועל בו Windows 10 Pro, גירסה 1703 (עדכון ליוצרים) (ראה [דרישות מוקדמות](pre-requisites-for-data-protection.md)), לחץ על סמל Windows ולאחר מכן על סמל 'הגדרות'.</span><span class="sxs-lookup"><span data-stu-id="dde03-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="dde03-127">ב **הגדרות**, עבור אל **חשבונות**.</span><span class="sxs-lookup"><span data-stu-id="dde03-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="dde03-129">בדף **המידע שלך**, לחץ על **גישה לחשבון עבודה או בית ספר** \> **התחבר**.</span><span class="sxs-lookup"><span data-stu-id="dde03-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="dde03-131">בתיבת הדו-שיח **הגדר חשבון בעבודה או בבית ספר**, תחת **פעולות חלופיות**, בחר **צרף מכשיר זה ל- Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="dde03-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="dde03-133">בדף **בוא נבצע את תהליך הכניסה**, הזן את החשבון שלך בעבודה או בבית הספר \> **הבא**.</span><span class="sxs-lookup"><span data-stu-id="dde03-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="dde03-134">בדף **הזנת סיסמה**, הזן את הסיסמה שלך \> **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="dde03-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="dde03-136">בדף **ודא שזהו הארגון שלך,** ודא שהמידע נכון ובחר **הצטרף.**</span><span class="sxs-lookup"><span data-stu-id="dde03-136">On the **Make sure this is your organization** page, verify that the information is correct, and choose **Join**.</span></span>
  
   <span data-ttu-id="dde03-137">ב- **אתה מוכן!**</span><span class="sxs-lookup"><span data-stu-id="dde03-137">On the **You're all set!**</span></span> <span data-ttu-id="dde03-138">page, chosse **Done**.</span><span class="sxs-lookup"><span data-stu-id="dde03-138">page, chosse **Done**.</span></span>
  
   ![במסך ודא שזהו הארגון שלך, בחר הצטרף](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="dde03-140">אם העלית קבצים אל OneDrive for Business, סנכרן אותם בחזרה.</span><span class="sxs-lookup"><span data-stu-id="dde03-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="dde03-141">אם השתמשת בכלי של ספקים אחרים להעברת פרופיל וקבצים, סנכרן גם אותם עם הפרופיל החדש.</span><span class="sxs-lookup"><span data-stu-id="dde03-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="dde03-142">אימות שהמכשיר מחובר ל- Azure AD</span><span class="sxs-lookup"><span data-stu-id="dde03-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="dde03-143">כדי לאמת את מצב הסינכרון שלך, **בדף Access** בעבודה או בבית ספר **ב- הגדרות**, בחר באזור **מחובר** ל_ _ כדי לחשוף את \<organization name\> הלחצנים מידע **והתנתק.** </span><span class="sxs-lookup"><span data-stu-id="dde03-143">To verify your sync status, on the **Access work or school** page in **Settings**, select the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**.</span></span> <span data-ttu-id="dde03-144">בחר **מידע כדי** לקבל את מצב הסינכרון שלך.</span><span class="sxs-lookup"><span data-stu-id="dde03-144">Choose **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="dde03-145">בדף מצב **סינכרון,** בחר **סנכרן** כדי לקבל את מדיניות הניהול העדכנית ביותר של מכשירים ניידים למחשב.</span><span class="sxs-lookup"><span data-stu-id="dde03-145">On the **Sync status** page, choose **Sync** to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="dde03-146">כדי להתחיל להשתמש בחשבון Microsoft 365 Business Premium, עבור אל לחצן Windows **התחל,** לחץ באמצעות לחצן העכבר הימני על תמונת החשבון הנוכחית ולאחר מכן **עבור לחשבון**.</span><span class="sxs-lookup"><span data-stu-id="dde03-146">To start using the Microsoft 365 Business Premium account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="dde03-147">היכנס באמצעות הדואר האלקטרוני והסיסמה של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="dde03-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a><span data-ttu-id="dde03-149">ודא שהמחשב משודרג ל- Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="dde03-149">Verify the PC is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="dde03-150">ודא שהתקני Azure AD המצורפים Windows 10 שלך משודרגים ל- Windows 10 Business כחלק Microsoft 365 Business Premium שלך.</span><span class="sxs-lookup"><span data-stu-id="dde03-150">Verify that your Azure AD joined Windows 10 devices are upgraded to Windows 10 Business as part of your Microsoft 365 Business Premium subscription.</span></span>
  
1. <span data-ttu-id="dde03-151">עבור אל **הגדרות** \> **מערכת** \> **אודות**.</span><span class="sxs-lookup"><span data-stu-id="dde03-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="dde03-152">ודא שתחת **מהדורה** מופיע **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="dde03-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="dde03-154">השלבים הבאים</span><span class="sxs-lookup"><span data-stu-id="dde03-154">Next steps</span></span>

<span data-ttu-id="dde03-155">כדי להגדיר את המכשירים הניידים שלך, ראה הגדרת [מכשירים ניידים עבור משתמשי Microsoft 365 Business Premium](set-up-mobile-devices.md), כדי להגדיר מדיניות הגנה על מכשירים או הגנה [על יישומים, ראה ניהול Microsoft 365 לעסקים.](manage.md)</span><span class="sxs-lookup"><span data-stu-id="dde03-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 for business](manage.md).</span></span>
  
## <a name="related-content"></a><span data-ttu-id="dde03-156">תוכן קשור</span><span class="sxs-lookup"><span data-stu-id="dde03-156">Related content</span></span>

<span data-ttu-id="dde03-157">[Microsoft 365 הדרכה לעסקים](../business-video/index.yml) (דף קישור)</span><span class="sxs-lookup"><span data-stu-id="dde03-157">[Microsoft 365 for business training videos](../business-video/index.yml) (link page)</span></span>
