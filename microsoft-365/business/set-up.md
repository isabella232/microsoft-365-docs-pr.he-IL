---
title: התקנת Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
ms.openlocfilehash: 42a35810531b6abd5b22e5fdbce2c0cfea57b8d7
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074589"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="f6dbd-103">הגדרת Microsoft 365 עסקיים באשף ההתקנה</span><span class="sxs-lookup"><span data-stu-id="f6dbd-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="f6dbd-104">הוסף את התחום שלך, משתמשים, ולהגדיר מדיניות</span><span class="sxs-lookup"><span data-stu-id="f6dbd-104">Add your domain, users, and set up policies</span></span>

![כרזה המצביעים על https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="f6dbd-106">בעת רכישת עסקי 365 של Microsoft, יש לך את האפשרות של משתמש תחום בבעלותך, או לקנות אחד במהלך [ההרשמה](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="f6dbd-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="f6dbd-107">אם רכשת תחום חדש בעת שנרשמת, התחום שלך הוא קבוצת כל למעלה ובאפשרותך להעביר [הוסף משתמשים והקצה רשיונות](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="f6dbd-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="f6dbd-108">הוסף את התחום כדי להתאים אישית את הכניסה</span><span class="sxs-lookup"><span data-stu-id="f6dbd-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="f6dbd-109">להיכנס אל [מרכז admin Microsoft 365](https://admin.microsoft.com) באמצעות אישורי ניהול הכללית שלך.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="f6dbd-110">בחרו ' **הוסף תחום** או **הוסף משתמשים** כדי להפעיל את האשף.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="f6dbd-111">אם רכשת תחום במהלך ההרשמה, יהיה באפשרותך לא ראה **להוסיף תחום** שלב כאן.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="f6dbd-112">עבור לדף [הוספת משתמשים](#add-users-and-assign-licenses) במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![בחר באפשרות ' הוסף תחום.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="f6dbd-114">באשף, הזן את שם התחום שבו ברצונך להשתמש (כמו contoso.com).</span><span class="sxs-lookup"><span data-stu-id="f6dbd-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![צילום מסך של התאמה אישית של דף הכניסה שלך.](media/personalizesignin.png)

    
4. <span data-ttu-id="f6dbd-116">בצע את השלבים באשף [רשומות DNS ליצור אצל כל ספק אירוח DNS עבור Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) מוודא שאתה הבעלים של התחום.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="f6dbd-117">אם ידוע לך מארח התחום שלך, ראה גם [הוראות ספציפיות של המחשב המארח](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="f6dbd-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="f6dbd-118">אם ספק אירוח GoDaddy, התהליך קל, באופן אוטומטי, תתבקש להיכנס ותן Microsoft לאמת בשמך:</span><span class="sxs-lookup"><span data-stu-id="f6dbd-118">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![בדף ' GoDaddy אשר Access, בחר למועדים.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="f6dbd-120">הוספת משתמשים והקצאת רשיונות</span><span class="sxs-lookup"><span data-stu-id="f6dbd-120">Add users and assign licenses</span></span>

<span data-ttu-id="f6dbd-121">באפשרותך להוסיף משתמשים באשף, אך באפשרותך גם [להוסיף משתמשים מאוחר יותר](add-users-m365b.md) במרכז admin.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="f6dbd-122">בנוסף, אם יש לך בבקר קבוצת מחשבים מקומי, באפשרותך להוסיף משתמשים עם [חיבור AD תכלת הרקיע](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="f6dbd-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="f6dbd-123">הוסף משתמשים באשף</span><span class="sxs-lookup"><span data-stu-id="f6dbd-123">Add users in the wizard</span></span>

<span data-ttu-id="f6dbd-124">כל המשתמשים שאתה מוסיף באשף לקבל להקצות רשיון העסק 365 Microsoft באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![צילום מסך של הוספת משתמשים הדף החדש באשף](media/addnewuserspage.png)

1. <span data-ttu-id="f6dbd-126">אם המנוי Microsoft 365 העסק שלך כולל משתמשים קיימים (לדוגמה, אם השתמשת תכלת הרקיע התחבר AD), תקבל אפשרות להקצות רשיונות אותם כעת.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="f6dbd-127">קדימה, הוסף רשיונות גם להם.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-127">Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="f6dbd-128">לאחר שהוספת את המשתמשים, תקבל גם אפשרות לשתף את האישורים עם המשתמשים החדשים שהוספת.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="f6dbd-129">באפשרותך להדפיס אותם, לשלוח אותם בדואר אלקטרוני או להוריד אותם.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-129">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="f6dbd-130">דלג על העברת הודעות דואר אלקטרוני ובחר **הבא** בדף **העברת הודעות דואר אלקטרוני**.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="f6dbd-131">אם אתה מעביר מספק דואר אלקטרוני אחר וברצונך להעתיק את הנתונים שלך מאוחר יותר, באפשרותך לבצע [העברת דואר אלקטרוני ואנשי קשר Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="f6dbd-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="f6dbd-132">חיבור התחום שלך</span><span class="sxs-lookup"><span data-stu-id="f6dbd-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="f6dbd-133">אם בחרת להשתמש בתחום .onmicrosoft, או אם השתמשת תכלת הרקיע AD התחבר כדי להגדיר משתמשים, לא תראה שלב זה.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="f6dbd-134">להגדרת שירותים, עליך לעדכן כמה רשומות אצל מארח ה- DNS שלך או אצל רשם התחומים.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="f6dbd-135">אשף ההגדרה מזהה בדרך כלל את הרשם שלך, ומספק לך קישור להוראות מפורטות לעדכון רשומות ה- NS באתר האינטרנט של הרשם.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="f6dbd-136">אם לא, [שינוי nameservers כדי להגדיר את Office 365 עם כל רשם התחום](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="f6dbd-136">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="f6dbd-137">אם יש לך רשומות DNS קיימות, לדוגמה אתר אינטרנט קיים, ברצונך לנהל רשומות DNS משלך כדי לוודא שהשירותים הקיימים להישאר מחובר.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-137">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="f6dbd-138">ראה [יסודות התחום](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-138">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![לחבר את המחשבים שלך דף עם ניתן לנהל רשומות DNS בעצמי.](media/connectyourdomainpage.png)

2. <span data-ttu-id="f6dbd-140">בצע את השלבים באשף ו דואר אלקטרוני ושירותים אחרים יוגדר עבורך.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-140">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="f6dbd-141">הגדרת מדיניות אבטחה ותצורות התקן</span><span class="sxs-lookup"><span data-stu-id="f6dbd-141">Set up security policies and device configurations</span></span> 

<span data-ttu-id="f6dbd-142">פריטי המדיניות שהגדרת באשף מוחלים באופן אוטומטי [קבוצת אבטחה](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) בשם *כל המשתמשים*.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-142">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="f6dbd-143">באפשרותך גם ליצור קבוצות נוספות כדי להקצות פריטי מדיניות כדי במרכז admin.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-143">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="f6dbd-144">על **להגן על הקבצים שלך עבודה במכשירים ניידים** האפשרות **הגן על קבצי עבודה כאשר התקנים שאבדו או נגנבו** נבחרת כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-144">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="f6dbd-145">יש לך אפשרות להפעיל **לנהל את האופן שבו משתמשים ניגשים קבצי Office במכשירים ניידים**, ומומלץ זה.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-145">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![קבצי עבודה צילום מסך של הגנה על דף מכשירים ניידים.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="f6dbd-147">הרחב את **הגנת קבצי עבודה כאשר התקנים שאבדו או נגנבו** כדי להציג את [ערכי ברירת המחדל](protect-work-files-on-lost-or-stolen-device.md):</span><span class="sxs-lookup"><span data-stu-id="f6dbd-147">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![צילום מסך של ערכי ברירת מחדל עבור הגנה על קבצים במכשירים אבד.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="f6dbd-149">בחר **לנהל את האופן שבו משתמשים ניגשים קבצי Office במכשירים ניידים** והרחב אותו כדי להציג את [ערכי ברירת המחדל](manage-user-access-on-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="f6dbd-149">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="f6dbd-150">אנו ממליצים כי אתה מקבל את ערכי ברירת המחדל במהלך ההתקנה כדי ליצור פריטי מדיניות יישומים עבור Android, iOS ו- Windows 10 החלות על כל המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-150">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="f6dbd-151">ניתן ליצור פריטי מדיניות נוספים לאחר השלמת ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-151">You can create more policies after setup completes.</span></span>

        ![צילום מסך של הגדרות הגנה עבור קבצי Office על נייד.](media/useraccessonmobile.png)

2. <span data-ttu-id="f6dbd-153">השלב האחרון על להגן על הנתונים ואת התקנים מאפשרת לך להגדיר פריטי מדיניות כדי לאבטח התקני Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-153">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="f6dbd-154">הגדרות אלה מוחלים באופן אוטומטי כאשר Windows 10 משתמש מתחבר לארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-154">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="f6dbd-155">באפשרותך להרחיב **התקנים לאבטח Windows 10** כדי לראות ולשנות את [ערכי ברירת המחדל](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="f6dbd-155">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="f6dbd-156">באפשרותך גם [להתקין את Office באופן אוטומטי](install-office-on-windows-10-during-setup.md) במכשירים Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-156">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![צילום מסך של הגדרת עמוד תצורת התקן של Windows 10.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="f6dbd-158">לפרוס יישומי לקוח של Office 365</span><span class="sxs-lookup"><span data-stu-id="f6dbd-158">Deploy Office 365 client apps</span></span>

<span data-ttu-id="f6dbd-159">אם בחרת להתקין באופן אוטומטי יישומי Office ב במהלך ערכת למעלה, apps יתקין בהתקני Windows 10 לאחר שהמשתמשים נרשמו לשירות AD תכלת הרקיע מהתקנים Windows שלהם עם אישורי העבודה שלהם.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-159">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="f6dbd-160">כדי להתקין את Office iOS נייד או התקנים Android, ראה [הגדרת מכשירים ניידים עבור משתמשים עסקיים 365 של Microsoft](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="f6dbd-160">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="f6dbd-161">באפשרותך גם להתקין את Office בנפרד.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-161">You can also install Office individually.</span></span> <span data-ttu-id="f6dbd-162">ראה [התקנת Office במחשב האישי או Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) לקבלת הוראות.</span><span class="sxs-lookup"><span data-stu-id="f6dbd-162">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>
