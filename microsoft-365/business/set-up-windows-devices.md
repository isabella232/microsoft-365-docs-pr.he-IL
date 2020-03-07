---
title: הגדרת מכשירי Windows עבור משתמשים של Microsoft 365 Business
f1.keywords:
- CSH
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: למד כיצד להגדיר התקני Windows שבהם פועל Windows 10 Pro עבור משתמשים עסקיים של Microsoft 365, המאפשרים ניהול מרוכז ובקרת אבטחה.
ms.openlocfilehash: 6ecc45f825a783d9d47c4b069a6021143d96597c
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561159"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a><span data-ttu-id="551f9-103">הגדרת מכשירי Windows עבור משתמשים של Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="551f9-103">Set up Windows devices for Microsoft 365 Business users</span></span>

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-users"></a><span data-ttu-id="551f9-104">דרישות מוקדמות להגדרת התקני Windows עבור משתמשים עסקיים של Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="551f9-104">Prerequisites for setting up Windows devices for Microsoft 365 Business users</span></span>

<span data-ttu-id="551f9-p101">לפני שתוכל להגדיר מכשירי Windows עבור משתמשי Microsoft 365 Business, ודא שבכל מכשירי Windows פועלת מהדורה 1703 של Windows 10 Pro (העדכון ליוצרים). Windows 10 Pro מהווה דרישה מוקדמת לפריסת Windows 10 Business, שהוא קבוצה של שירותי ענן ויכולות ניהול מכשירים שמשלימות את Windows 10 Pro ומאפשרות את ההפעלה של הניהול המרכזי ובקרות האבטחה של Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="551f9-p101">Before you can set up Windows devices for Microsoft 365 Business users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update). Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business.</span></span>
  
<span data-ttu-id="551f9-107">אם יש לך מכשיר Windows עם Windows 7 Pro, ‏Windows 8 Pro או Windows 8.1 Pro, מנוי Microsoft 365 Business שלך מזכה אותך בשדרוג ל- Windows 10.</span><span class="sxs-lookup"><span data-stu-id="551f9-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="551f9-108">לקבלת מידע נוסף על שדרוג מכשירי Windows לעדכון Windows 10 ליוצרים, פעל לפי השלבים בנושא זה: [שדרוג מכשירי Windows לעדכון Windows Pro ליוצרים](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="551f9-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="551f9-109">ראה [אימות ההתקן מחובר לתכלת AD](#verify-the-device-is-connected-to-azure-ad) כדי לוודא שיש לך את השדרוג, או כדי לוודא שהשדרוג עבד.</span><span class="sxs-lookup"><span data-stu-id="551f9-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="551f9-110">צפה בסרטון וידאו קצר אודות חיבור Windows ל-Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="551f9-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="551f9-111">אם סרטון וידאו זה היה שימושי עבורך, עיין ב[סדרת ההדרכה המלאה עבור עסקים קטנים ומשתמשים חדשים ב- Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="551f9-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="551f9-112">צירוף מכשירי Windows 10 ל- Azure AD של הארגון שלך</span><span class="sxs-lookup"><span data-stu-id="551f9-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="551f9-113">כאשר כל התקני Windows בארגון שלך שודרגו ל-Windows 10 Pro יוצרי עדכון או שכבר פועל Windows 10 Pro יוצרי עדכון, אתה יכול להצטרף התקנים אלה לתוך הארגון שלך הפעיל הספריה.</span><span class="sxs-lookup"><span data-stu-id="551f9-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="551f9-114">לאחר הצירוף של המכשירים, הם ישודרגו באופן אוטומטי ל-Windows 10 Business, המהווה חלק ממנוי העסקי של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="551f9-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="551f9-115">עבור מכשיר Windows 10 Pro חדש לגמרי או ששודרג לאחרונה</span><span class="sxs-lookup"><span data-stu-id="551f9-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="551f9-116">עבור מכשיר חדש לגמרי שעדכון Windows 10 Pro ליוצרים פועל בו, או עבור מכשיר ששודרג לעדכון Windows 10 Pro ליוצרים אך לא הוגדר ל- Windows 10, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="551f9-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="551f9-117">עבור על פרטי ההגדרה של מכשיר Windows 10 עד שתגיע לעמוד **כיצד ברצונך להגדיר?**.</span><span class="sxs-lookup"><span data-stu-id="551f9-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="551f9-119">כאן, בחר **הגדרה עבור ארגון** ולאחר מכן הזן את שם המשתמש והסיסמה שלך עבור Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="551f9-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business.</span></span> 
    
3. <span data-ttu-id="551f9-120">סיים את הגדרת מכשיר Windows 10.</span><span class="sxs-lookup"><span data-stu-id="551f9-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="551f9-p103">כשתסיים, המשתמש יהיה מחובר ל- Azure AD של הארגון שלך. ראה [אימות שהמכשיר מחובר ל- Azure AD](#verify-the-device-is-connected-to-azure-ad) כדי לוודא.</span><span class="sxs-lookup"><span data-stu-id="551f9-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="551f9-123">עבור מכשיר שכבר מוגדר וש- Windows 10 Pro פועל בו</span><span class="sxs-lookup"><span data-stu-id="551f9-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="551f9-124">**חיבור משתמשים ל- Azure AD:**</span><span class="sxs-lookup"><span data-stu-id="551f9-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="551f9-125">במחשב ה- Windows של המשתמש שלך, שפועל בו Windows 10 Pro, גירסה 1703 (עדכון ליוצרים) (ראה [דרישות מוקדמות](pre-requisites-for-data-protection.md)), לחץ על סמל Windows ולאחר מכן על סמל 'הגדרות'.</span><span class="sxs-lookup"><span data-stu-id="551f9-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="551f9-127">ב **הגדרות**, עבור אל **חשבונות**.</span><span class="sxs-lookup"><span data-stu-id="551f9-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="551f9-129">בדף **המידע שלך**, לחץ על **גישה לחשבון עבודה או בית ספר** \> **התחבר**.</span><span class="sxs-lookup"><span data-stu-id="551f9-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="551f9-131">בתיבת הדו-שיח **הגדר חשבון בעבודה או בבית ספר**, תחת **פעולות חלופיות**, בחר **צרף מכשיר זה ל- Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="551f9-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="551f9-133">בדף **בוא נבצע את תהליך הכניסה**, הזן את החשבון שלך בעבודה או בבית הספר \> **הבא**.</span><span class="sxs-lookup"><span data-stu-id="551f9-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="551f9-134">בדף **הזנת סיסמה**, הזן את הסיסמה שלך \> **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="551f9-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="551f9-136">ב-ודא שזהו דף **הארגון שלך** , ודא שהמידע נכון ולחץ על **הצטרף**.</span><span class="sxs-lookup"><span data-stu-id="551f9-136">On the **Make sure this is your organization** page, verify that the information is correct, and click **Join**.</span></span>
  
   <span data-ttu-id="551f9-p104">בדף **הכל מוכן!**, לחץ על **סיום**.</span><span class="sxs-lookup"><span data-stu-id="551f9-p104">On the **You're all set!** page, click **Done**.</span></span>
  
   ![On the Make sure this is your organization screen, click Join](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="551f9-140">אם העלית קבצים אל OneDrive for Business, סנכרן אותם בחזרה.</span><span class="sxs-lookup"><span data-stu-id="551f9-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="551f9-141">אם השתמשת בכלי של ספק חיצוני כדי להעביר פרופיל וקבצים, סנכרן גם אותם לפרופיל החדש.</span><span class="sxs-lookup"><span data-stu-id="551f9-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="551f9-142">אימות שהמכשיר מחובר ל- Azure AD</span><span class="sxs-lookup"><span data-stu-id="551f9-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="551f9-p106">כדי לאמת את מצב הסינכרון שלך, בדף **גישה לחשבון עבודה או בית ספר** ב **הגדרות**, לחץ באזור **מחובר ל** _ \<organization name\> _ כדי לחשוף את הלחצנים **מידע** ו **התנתק**. לחץ על **מידע** כדי לקבל את מצב הסינכרון.</span><span class="sxs-lookup"><span data-stu-id="551f9-p106">To verify your sync status, on the **Access work or school** page in **Settings**, click in the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**. Click on **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="551f9-145">בדף 'מצב סינכרון', לחץ על 'סינכרון' כדי לקבל את פריטי מדיניות הניהול העדכניים ביותר של המכשיר הנייד במחשב ה- PC.</span><span class="sxs-lookup"><span data-stu-id="551f9-145">On the Sync status page, click Sync to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="551f9-146">כדי להתחיל להשתמש בחשבון העסקי של Microsoft 365, עבור ללחצן **התחל** של Windows, לחץ לחיצה ימנית על תמונת החשבון הנוכחית שלך ולאחר מכן **החלף חשבון**.</span><span class="sxs-lookup"><span data-stu-id="551f9-146">To start using the Microsoft 365 Business account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="551f9-147">היכנס באמצעות הדואר האלקטרוני והסיסמה של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="551f9-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a><span data-ttu-id="551f9-149">אימות שהמכשיר משודרג ל- Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="551f9-149">Verify the device is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="551f9-150">ודא שמכשירי Windows 10 שהצטרפו ל- Azure AD שודרגו ל- Windows 10 Business כחלק מהמנוי ל- Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="551f9-150">Verify that your Azure AD joined Windows 10 devices were upgraded to Windows 10 Business as part of your Microsoft 365 Business subscription.</span></span>
  
1. <span data-ttu-id="551f9-151">עבור אל **הגדרות** \> **מערכת** \> **אודות**.</span><span class="sxs-lookup"><span data-stu-id="551f9-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="551f9-152">ודא שתחת **מהדורה** מופיע **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="551f9-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="551f9-154">השלבים הבאים</span><span class="sxs-lookup"><span data-stu-id="551f9-154">Next steps</span></span>

<span data-ttu-id="551f9-155">כדי להגדיר את המכשירים הניידים שלך, ראה [הגדרת מכשירים ניידים עבור משתמשי Microsoft 365 Business](set-up-mobile-devices.md). כדי להגדיר כללי מדיניות הגנה למכשירים או ליישומים, ראה [ניהול Microsoft 365 Business](manage.md).</span><span class="sxs-lookup"><span data-stu-id="551f9-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 Business](manage.md).</span></span>
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business"></a><span data-ttu-id="551f9-156">לקבלת פרטים נוספים על הגדרה ושימוש ב-Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="551f9-156">For more on setting up and using Microsoft 365 Business</span></span>

[<span data-ttu-id="551f9-157">סרטוני הדרכה בנושא Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="551f9-157">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
