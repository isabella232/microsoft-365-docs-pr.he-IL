---
title: התקנת Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: למד כיצד להגדיר את Microsoft 365 עסקיים.
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660798"
---
# <a name="set-up-microsoft-365-business"></a><span data-ttu-id="6dbd2-103">התקנת Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="6dbd2-103">Set up Microsoft 365 Business</span></span>

<span data-ttu-id="6dbd2-104">לפני שתתחיל לעבוד, [לקבל ביקור 365 של Microsoft](get-microsoft-365-business.md) לקבלת פרטים, עיין הרשמה.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-104">Before you get started, see [Get Microsoft 365 Business](get-microsoft-365-business.md) for sign-up details.</span></span>

<span data-ttu-id="6dbd2-105">צפה בסרטון [וידאו קצר כיצד להגדיר עסקיים 365 של Microsoft](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) על-ידי שימוש בערכת למעלה אשף, וכאשר אין לך המקומית של Active Directory</span><span class="sxs-lookup"><span data-stu-id="6dbd2-105">Watch a [short video on how to set up Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) by using the set up wizard, and when you don't have an on-premises Active Directory</span></span>
  

## <a name="overview"></a><span data-ttu-id="6dbd2-106">מבט כולל</span><span class="sxs-lookup"><span data-stu-id="6dbd2-106">Overview</span></span>

<span data-ttu-id="6dbd2-107">ניתן לעשות זאת רוב להגדיר השלבים באשף ההתקנה, אך רשומים גם אפשרויות אחרות.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-107">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>

1. <span data-ttu-id="6dbd2-108">[הוסף קבוצת המחשבים שלך](#add-your-domain-to-personalize-sign-in) (אם רכשת את התחום שלך במהלך [להירשם](sign-up.md), שלב זה כבר בוצע.)</span><span class="sxs-lookup"><span data-stu-id="6dbd2-108">[Add your domain](#add-your-domain-to-personalize-sign-in) (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>
2. <span data-ttu-id="6dbd2-109">הוספת משתמשים.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-109">Add users.</span></span> <span data-ttu-id="6dbd2-110">ניתן לעשות זאת באחת משלוש דרכים:</span><span class="sxs-lookup"><span data-stu-id="6dbd2-110">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="6dbd2-111">[אשף ההתקנה](#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-111">In the [setup wizard](#add-users-in-the-wizard).</span></span>
    - <span data-ttu-id="6dbd2-112">השתמש סינכרון ספריות כדי [להוסיף משתמשים באמצעות חיבור AD תכלת הרקיע](#add-users-by-using-azure-ad-connect) אם ברשותך המקומית של Active directory.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-112">Use directory synchronization to [add users by using Azure AD Connect](#add-users-by-using-azure-ad-connect) if you have an on-premises Active directory.</span></span>
    - <span data-ttu-id="6dbd2-113">באפשרותך גם [להוסיף משתמשים מאוחר יותר](add-users-m365b.md) במרכז admin.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
3. <span data-ttu-id="6dbd2-114">הגדרת מדיניות אבטחה וקביעת תצורה של התקנים.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-114">Set up security policies and configure devices.</span></span> <span data-ttu-id="6dbd2-115">ניתן לעשות זאת באחת משלוש דרכים:</span><span class="sxs-lookup"><span data-stu-id="6dbd2-115">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="6dbd2-116">[אשף ההתקנה](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-116">In the [setup wizard](#set-up-policies-in-the-wizard).</span></span>  
    - <span data-ttu-id="6dbd2-117">[מרכז admin](#modify-or-add-policies-in-the-admin-center).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-117">In the [admin center](#modify-or-add-policies-in-the-admin-center).</span></span>
    - <span data-ttu-id="6dbd2-118">[מרכז הניהוליים Intune](https://docs.microsoft.com/intune/what-is-device-management).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-118">In the [Intune admin center](https://docs.microsoft.com/intune/what-is-device-management).</span></span>
4. <span data-ttu-id="6dbd2-119">להגדיר ולנהל התקני Windows 10.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-119">Set up and manage Windows 10 devices.</span></span>

    <span data-ttu-id="6dbd2-120">בעת הצטרפות התקן WIndows 10 כדי AD תכלת הרקיע, כל פריטי המדיניות לקבל שהוחלה עליו.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-120">When you join a WIndows 10 device to Azure AD, all the policies get applied to it.</span></span>
    - <span data-ttu-id="6dbd2-121">קבע תצורות התקן Windows 10 של [אשף ההתקנה](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-121">Set up Windows 10 device configurations in the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="6dbd2-122">לצרף [התקן חדש של Windows 10](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) AD תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-122">Join a [new Windows 10 device](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) to Azure AD.</span></span>
    - <span data-ttu-id="6dbd2-123">צירוף של [התקן Windows 10 קיים](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) כדי AD תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-123">Join an [existing Windows 10 device](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) to Azure AD.</span></span>
1. <span data-ttu-id="6dbd2-124">התקנת Office 365 עסקיים.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-124">Install Office 365 Business.</span></span>
    - <span data-ttu-id="6dbd2-125">באפשרותך להתקין את Office באופן אוטומטי בהתקני Windows באמצעות [אשף ההתקנה](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-125">You can automatically install Office in the Windows devices by using the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="6dbd2-126">באופן אוטומטי [להתקין את Office](auto-install-or-uninstall-office.md) ממרכז admin.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-126">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
    - <span data-ttu-id="6dbd2-127">לאפשר למשתמשים [להתקין את יישומי Office](https://docs.microsoft.com/office365/admin/setup/install-applications) עבור Windows והתקנים.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-127">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
1. <span data-ttu-id="6dbd2-128">הגדרת אבטחה נוספים.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-128">Set up additional security.</span></span>
    - <span data-ttu-id="6dbd2-129">אשף ההתקנה מוסיפה מדיניות כדי לאבטח את ההתקנים שלך, אך באפשרותך גם להנות מהיתרון של יכולות [אבטחה נוספות](#additional-security-settings) כדי מסייע מאובטח נתונים, וחשבונות דוא.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-129">The setup wizard adds policies to secure your devices, but you can also take advantage of [additional security](#additional-security-settings) capabilities to helps secure your data, accounts, and emails.</span></span> 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="6dbd2-130">הוסף את התחום שלך, משתמשים ולהגדיר מדיניות</span><span class="sxs-lookup"><span data-stu-id="6dbd2-130">Add your domain, users and set up policies</span></span>

![כרזה המצביעים על https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="6dbd2-132">בעת רכישת עסקי 365 של Microsoft, יש לך את האפשרות של משתמש תחום בבעלותך, או לקנות אחד במהלך [ההרשמה](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-132">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="6dbd2-133">אם רכשת תחום חדש בעת שנרשמת, התחום שלך הוא קבוצת כל למעלה ובאפשרותך להעביר [הוסף משתמשים והקצה רשיונות](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-133">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="6dbd2-134">הוסף את התחום כדי להתאים אישית את הכניסה</span><span class="sxs-lookup"><span data-stu-id="6dbd2-134">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="6dbd2-135">להיכנס אל [מרכז admin Microsoft 365](https://admin.microsoft.com) באמצעות אישורי ניהול הכללית שלך.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-135">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="6dbd2-136">בחר **הוסף מחשבים** כדי להפעיל את האשף.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-136">Choose **Add a domain** to start the wizard.</span></span>

    ![בחר באפשרות ' הוסף תחום.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="6dbd2-138">באשף, הזן את שם התחום שבו ברצונך להשתמש (כמו contoso.com).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-138">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![צילום מסך של התאמה אישית של דף הכניסה שלך.](media/personalizesignin.png)

    
4. <span data-ttu-id="6dbd2-140">בצע את השלבים באשף [רשומות DNS ליצור אצל כל ספק אירוח DNS עבור Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) מוודא שאתה הבעלים של התחום.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-140">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="6dbd2-141">אם ידוע לך מארח התחום שלך, ראה גם [הוראות ספציפיות של המחשב המארח](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-141">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="6dbd2-142">אם ספק אירוח GoDaddy, התהליך קל, באופן אוטומטי, תתבקש להיכנס ותן Microsoft לאמת בשמך:</span><span class="sxs-lookup"><span data-stu-id="6dbd2-142">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![בדף ' GoDaddy אשר Access, בחר למועדים.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="6dbd2-144">הוספת משתמשים והקצאת רשיונות</span><span class="sxs-lookup"><span data-stu-id="6dbd2-144">Add users and assign licenses</span></span>

<span data-ttu-id="6dbd2-145">באפשרותך להוסיף משתמשים באשף, אך באפשרותך גם [להוסיף משתמשים מאוחר יותר](add-users-m365b.md) במרכז admin.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-145">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="6dbd2-146">בנוסף, אם יש לך בבקר קבוצת מחשבים מקומי, באפשרותך להוסיף משתמשים עם [חיבור AD תכלת הרקיע](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-146">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="6dbd2-147">הוסף משתמשים באשף</span><span class="sxs-lookup"><span data-stu-id="6dbd2-147">Add users in the wizard</span></span>

<span data-ttu-id="6dbd2-148">כל המשתמשים שאתה מוסיף באשף לקבל להקצות רשיון העסק 365 Microsoft באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-148">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>
<span data-ttu-id="6dbd2-149">אם בקר קבוצת מחשבים מקומיים, אתה משתמש ב- Active Directory, ראה [כיצד משתמשים ddd באמצעות חיבור AD תכלת הרקיע](#add-users-by-using-azure-ad-connect).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-149">If you have a local domain controller, and are using Active Directory, see [how to ddd users by using Azure AD Connect](#add-users-by-using-azure-ad-connect).</span></span>

![צילום מסך של הוספת משתמשים הדף החדש באשף](media/addnewuserspage.png)

1. <span data-ttu-id="6dbd2-p106">אם המנוי שלך ל- Microsoft 365 Business כולל משתמשים קיימים (לדוגמה, אם השתמשת ב- Azure AD Connect), תהיה לך אפשרות להקצות להם רשיונות כעת. קדימה, הוסף רשיונות גם להם.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-p106">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you will get an option to assign licenses to them now. Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="6dbd2-153">לאחר שהוספת את המשתמשים, תקבל גם אפשרות לשתף את האישורים עם המשתמשים החדשים שהוספת.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-153">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="6dbd2-154">באפשרותך להדפיס אותם, לשלוח אותם בדואר אלקטרוני או להוריד אותם.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-154">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="6dbd2-155">דלג על העברת הודעות דואר אלקטרוני ובחר **הבא** בדף **העברת הודעות דואר אלקטרוני**.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-155">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="6dbd2-156">אם אתה מעביר מספק דואר אלקטרוני אחר וברצונך להעתיק את הנתונים שלך מאוחר יותר, באפשרותך לבצע [העברת דואר אלקטרוני ואנשי קשר Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-156">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>

#### <a name="add-users-by-using-azure-ad-connect"></a><span data-ttu-id="6dbd2-157">הוסף משתמשים באמצעות חיבור AD תכלת הרקיע</span><span class="sxs-lookup"><span data-stu-id="6dbd2-157">Add users by using Azure AD Connect</span></span>

 <span data-ttu-id="6dbd2-158">אם ברשותך בקר תחום מקומי עם Active Directory, סינכרון למשתמשים עסקיים 365 של Microsoft באמצעות [חיבור AD תכלת הרקיע](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-158">If you have a local domain controller with Active Directory, you synchronize your users with Microsoft 365 Business by using [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span> <span data-ttu-id="6dbd2-159">השלם פעולה זו לפני שתפעיל את אשף ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-159">Complete this before you start the setup wizard.</span></span> <span data-ttu-id="6dbd2-160">באפשרותך להוריד אותו במרכז admin:</span><span class="sxs-lookup"><span data-stu-id="6dbd2-160">You can download it in the admin center:</span></span>

- <span data-ttu-id="6dbd2-161">עבור אל **משתמשים** \> **משתמשים פעילים**, בחר את שלוש הנקודות בראש הדף ולאחר מכן בחר **סינכרון ספריות** להוריד התחבר AD תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-161">Go to **Users** \> **Active users**, select the ellipses on the top of the page and then select **Directory synchronization** to download Azure AD Connect.</span></span>

    ![בדף משתמשים פעילים בחר אליפסות > הספריה snchronization.](media/setupdirsync.png)

    > [!IMPORTANT]
    > <span data-ttu-id="6dbd2-163">אם אתה יוצר משתמשים בדרך זו, עדיין יהיה עליך להקצות רשיונות אותם במרכז admin.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-163">If you create users this way, you will still have to assign licenses to them in the admin center.</span></span>

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a><span data-ttu-id="6dbd2-164">להמשיך לגשת לתחום יישומים והתקנים</span><span class="sxs-lookup"><span data-stu-id="6dbd2-164">Continue to access domain-joined apps and devices</span></span>

<span data-ttu-id="6dbd2-165">אם ברצונך להמשיך לגשת לתחום יישומים והתקנים, קרא את המאמרים הבאים עבור שני בדרך אחרת של הפעלת אשר:</span><span class="sxs-lookup"><span data-stu-id="6dbd2-165">If you want to continue to access domain-joined apps and devices, read the following articles for two different way of enabling that:</span></span>
  
- [<span data-ttu-id="6dbd2-166">מתן אפשרות לניהול מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="6dbd2-166">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>](manage-windows-devices.md)
    - <span data-ttu-id="6dbd2-167">זוהי הדרך המומלצת.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-167">This is the recommended way.</span></span>

- [<span data-ttu-id="6dbd2-168">Access המקומית משאבים ממכשיר מצורף AD תכלת הרקיע ב- Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="6dbd2-168">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>](access-resources.md)

### <a name="connect-your-domain"></a><span data-ttu-id="6dbd2-169">חיבור התחום שלך</span><span class="sxs-lookup"><span data-stu-id="6dbd2-169">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="6dbd2-170">אם בחרת להשתמש בתחום .onmicrosoft, או אם השתמשת תכלת הרקיע AD התחבר כדי להגדיר משתמשים, לא תראה שלב זה.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-170">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="6dbd2-171">להגדרת שירותים, עליך לעדכן כמה רשומות אצל מארח ה- DNS שלך או אצל רשם התחומים.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-171">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="6dbd2-172">אשף ההגדרה מזהה בדרך כלל את הרשם שלך, ומספק לך קישור להוראות מפורטות לעדכון רשומות ה- NS באתר האינטרנט של הרשם.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-172">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="6dbd2-173">אם לא, [שינוי nameservers כדי להגדיר את Office 365 עם כל רשם התחום](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-173">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="6dbd2-174">אם יש לך רשומות DNS קיימות, לדוגמה אתר אינטרנט קיים, ברצונך לנהל רשומות DNS משלך כדי לוודא שהשירותים הקיימים להישאר מחובר.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-174">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="6dbd2-175">ראה [יסודות התחום](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-175">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![לחבר את המחשבים שלך דף עם ניתן לנהל רשומות DNS בעצמי.](media/connectyourdomainpage.png)

2. <span data-ttu-id="6dbd2-177">בצע את השלבים באשף ו דואר אלקטרוני ושירותים אחרים יוגדר עבורך.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-177">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="6dbd2-178">הגדרת מדיניות אבטחה ותצורות התקן</span><span class="sxs-lookup"><span data-stu-id="6dbd2-178">Set up security policies and device configurations</span></span> 

<span data-ttu-id="6dbd2-179">פריטי מדיניות אלה חלות על כל משתמש להעניק רשיון, או קבוצת משתמשים אם תחליט להקצות פריטי מדיניות שונים קבוצת משתמשים.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-179">These policies apply to every user you give a license to, or to a group of users if you decide to assign different policies to a set of users.</span></span>

#### <a name="set-up-policies-in-the-wizard"></a><span data-ttu-id="6dbd2-180">הגדרת מדיניות באשף</span><span class="sxs-lookup"><span data-stu-id="6dbd2-180">Set up policies in the wizard</span></span>

<span data-ttu-id="6dbd2-181">פריטי המדיניות שהגדרת באשף מוחלים באופן אוטומטי [קבוצת אבטחה](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) בשם *כל המשתמשים*.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-181">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span>

1. <span data-ttu-id="6dbd2-182">על **להגן על הקבצים שלך עבודה במכשירים ניידים** האפשרות **הגן על קבצי עבודה כאשר התקנים שאבדו או נגנבו** נבחרת כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-182">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="6dbd2-183">יש לך אפשרות להפעיל **לנהל את האופן שבו משתמשים ניגשים קבצי Office במכשירים ניידים**, ומומלץ זה.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-183">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![קבצי עבודה צילום מסך של הגנה על דף מכשירים ניידים.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="6dbd2-185">אם תרחיב את **הגנת קבצי עבודה כאשר התקנים אבד או נגנב**, [ערכי ברירת המחדל](protect-work-files-on-lost-or-stolen-device.md) הם שנבחרו מראש:</span><span class="sxs-lookup"><span data-stu-id="6dbd2-185">If you expand **Protect work files when devices are lost or stolen**, the [default values](protect-work-files-on-lost-or-stolen-device.md) are pre-selected:</span></span>

        ![צילום מסך של ערכי ברירת מחדל עבור הגנה על קבצים במכשירים אבד.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="6dbd2-187">אם אתה בוחר **לנהל את האופן שבו משתמשים ניגשים קבצי Office במכשירים ניידים** להרחיב אותה, מוצגים [ערכי ברירת מחדל](manage-user-access-on-mobile-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="6dbd2-187">If you select **Manage how users access Office files on mobile devices** and expand it, the [default values](manage-user-access-on-mobile-devices.md) are shown.</span></span> <span data-ttu-id="6dbd2-188">אנו ממליצים לקבל את ערכי ברירת המחדל במהלך ההתקנה כדי ליצור פריטי מדיניות של אפליקציות עבור Android,‏ iOS ו- Windows 10 שחלים על כל המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-188">We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="6dbd2-189">ניתן ליצור פריטי מדיניות נוספים לאחר השלמת ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-189">You can create more policies after setup completes.</span></span>

        ![צילום מסך של הגדרות הגנה עבור קבצי Office על נייד.](media/useraccessonmobile.png)

2. <span data-ttu-id="6dbd2-191">השלב האחרון על להגן על הנתונים ואת התקנים מאפשרת לך להגדיר פריטי מדיניות כדי לאבטח התקני Windows 10.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-191">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="6dbd2-192">הגדרות אלה מוחלים באופן אוטומטי כאשר Windows 10 משתמש מתחבר לארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-192">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="6dbd2-193">באפשרותך להרחיב **התקנים לאבטח Windows 10** כדי לראות ולשנות את [ערכי ברירת המחדל](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-193">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="6dbd2-194">באפשרותך גם [להתקין את Office באופן אוטומטי](install-office-on-windows-10-during-setup.md) במכשירים Windows 10.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-194">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![צילום מסך של הגדרת עמוד תצורת התקן של Windows 10.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a><span data-ttu-id="6dbd2-196">לשנות או להוסיף פריטי מדיניות במרכז admin</span><span class="sxs-lookup"><span data-stu-id="6dbd2-196">Modify or add policies in the admin center</span></span>

<span data-ttu-id="6dbd2-197">ראה [ניהול עסקי 365 Microsoft](manage.md) עבור קישורים לנושאים כיצד להציג ולשנות התקן והגנה על יישום מדיניות, וכיצד להסיר נתונים, או לאפס את התקני משתמש.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-197">See [manage Microsoft 365 Business](manage.md) for links to topics on how to view and modify device and app protection polices, and how to remove data from, or reset user devices.</span></span>

## <a name="deploy-and-manage-windows-10"></a><span data-ttu-id="6dbd2-198">לפרוס ולנהל Windows 10</span><span class="sxs-lookup"><span data-stu-id="6dbd2-198">Deploy and manage Windows 10</span></span>
<span data-ttu-id="6dbd2-199">ראה [הגדרת התקני Windows עבור משתמשים עסקיים 365 Microsoft](set-up-windows-devices.md) כדי להתחבר ידנית AD תכלת הרקיע במהלך ההתקנה עבור מחשבים חדשים, או על-ידי שינוי פרופיל הכניסה עבור המחשבים הקיימים.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-199">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) to manually connect to Azure AD, either during setup for new computers, or by changing sign-in profile for existing computers.</span></span> 

### <a name="use-autopilot-to-set-up-new-devices"></a><span data-ttu-id="6dbd2-200">השתמש Autopilot כדי להגדיר התקנים חדשים</span><span class="sxs-lookup"><span data-stu-id="6dbd2-200">Use Autopilot to set up new devices</span></span>

<span data-ttu-id="6dbd2-201">באפשרותך להשתמש ב- [Windows Autopilot](add-autopilot-devices-and-profile.md) כדי לקבוע מראש של התקנים 10 חלונות **חדשים** עבור משתמש באופן אוטומטי, אך ייתכן שיהיה קל יותר לקבל [שותף](https://www.microsoft.com/solution-providers/search) מי יכול לבצע זאת עבורך.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-201">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="6dbd2-202">באפשרותך גם לעבור לחנות [Microsoft](https://go.microsoft.com/fwlink/?linkid=874598) ובקש טכנולוגיה ענן מומחה להגדיר התקנים חדשים שאתה רוכש עבורך.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-202">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

### <a name="access-on-premises-resources"></a><span data-ttu-id="6dbd2-203">Access המקומית משאבים</span><span class="sxs-lookup"><span data-stu-id="6dbd2-203">Access on-premises resources</span></span>

<span data-ttu-id="6dbd2-204">אם הארגון שלך משתמש Windows Server Active Directory המקומית, באפשרותך להגדיר עסקיים 365 של Microsoft להגנה על התקני Windows 10 שלך, תוך שמירה עדיין גישה למשאבים המקומית המחייבים אימות מקומי.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-204">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="6dbd2-205">בצע את השלבים [אפשר לתחום התקני Windows 10 להיות מנוהל על-ידי Microsoft 365 עסקיים](manage-windows-devices.md) כדי להגדיר זאת.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-205">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="6dbd2-206">זוהי השיטה המועדפת ואת התקנים במצב זה נקראות תכלת הרקיע היברידית AD לחבר התקנים.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-206">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

<span data-ttu-id="6dbd2-207">אם בעסק שלך יש מקומי Active Directory המכילה כמה המקומית משאבים (כגון שיתופי קבצים ומדפסות), באפשרותך להעניק גישה ההתקנים המצורפים AD תכלת הרקיע שלך למשאבים אלה על-ידי ביצוע השלבים כאן: [Access המקומית משאבים מ תכלת הרקיע מצורף AD ההתקן ב- Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-207">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="6dbd2-208">לפרוס יישומי לקוח של Office 365</span><span class="sxs-lookup"><span data-stu-id="6dbd2-208">Deploy Office 365 client apps</span></span>

<span data-ttu-id="6dbd2-209">אם בחרת להתקין באופן אוטומטי יישומי Office ב במהלך ערכת למעלה, apps יתקין בהתקני Windows 10 לאחר שהמשתמשים נרשמו לשירות AD תכלת הרקיע מהתקנים Windows שלהם עם אישורי העבודה שלהם.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-209">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="6dbd2-210">כדי להתקין את Office iOS נייד או התקנים Android, ראה [הגדרת מכשירים ניידים עבור משתמשים עסקיים 365 של Microsoft](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-210">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="6dbd2-211">באפשרותך גם להתקין את Office בנפרד.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-211">You can also install Office individually.</span></span> <span data-ttu-id="6dbd2-212">ראה [התקנת Office במחשב האישי או Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) לקבלת הוראות.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-212">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>

## <a name="additional-security-settings"></a><span data-ttu-id="6dbd2-213">הגדרות אבטחה נוספת</span><span class="sxs-lookup"><span data-stu-id="6dbd2-213">Additional security settings</span></span>

<span data-ttu-id="6dbd2-214">בנוסף אבטחה הגדרת תאימות באשף ההתקנה, באפשרותך גם להגדיר את ההגדרות הנוספות הבאות:</span><span class="sxs-lookup"><span data-stu-id="6dbd2-214">In addition to the security and compliance setting in the setup wizard, you can also set up the following additional settings:</span></span>
  
- <span data-ttu-id="6dbd2-215">**הגנה מפני תוכנות זדוניות דוא**</span><span class="sxs-lookup"><span data-stu-id="6dbd2-215">**Email malware protection**</span></span>
- <span data-ttu-id="6dbd2-216">**מסמכים מצורפים בטוחים איום מתקדם הגנה (ATP)**</span><span class="sxs-lookup"><span data-stu-id="6dbd2-216">**Advanced Threat Protection (ATP) Safe Attachments**</span></span>
- <span data-ttu-id="6dbd2-217">**קישורים מתאימים ATP**</span><span class="sxs-lookup"><span data-stu-id="6dbd2-217">**ATP Safe Links**</span></span>
- <span data-ttu-id="6dbd2-218">**דירה למניעת דיוג**</span><span class="sxs-lookup"><span data-stu-id="6dbd2-218">**APT anti-phishing**</span></span>
- <span data-ttu-id="6dbd2-219">**אחסון בארכיון של Exchange Online**</span><span class="sxs-lookup"><span data-stu-id="6dbd2-219">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="6dbd2-220">**מניעת אובדן נתונים (DLP)**</span><span class="sxs-lookup"><span data-stu-id="6dbd2-220">**Data loss prevention (DLP)**</span></span>
- <span data-ttu-id="6dbd2-221">**הגנה על מידע תכלת הרקיע** (תכנון 1)</span><span class="sxs-lookup"><span data-stu-id="6dbd2-221">**Azure Information Protection** (Plan 1)</span></span>
- <span data-ttu-id="6dbd2-222">**זמינות הפורטל Intune**</span><span class="sxs-lookup"><span data-stu-id="6dbd2-222">**Intune portal availability**</span></span>

<span data-ttu-id="6dbd2-223">כדי לקבל מופעל, ראה [הגדרת מדיניות אבטחה מתקדמות](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="6dbd2-223">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

<span data-ttu-id="6dbd2-224">ראה גם [העליון 10 דרכים לאבטחת העסק 365 Microsoft](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) עבור מפת דרכים של שיטות עבודה מומלצות של אבטחה.</span><span class="sxs-lookup"><span data-stu-id="6dbd2-224">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>