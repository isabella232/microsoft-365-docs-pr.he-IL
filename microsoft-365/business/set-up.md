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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: למד כיצד להגדיר את Microsoft 365 Business.
ms.openlocfilehash: d33839693001f36fbb56541775015f739300b043
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288494"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="dab9d-103">הגדרת העסק של Microsoft 365 באשף ההתקנה</span><span class="sxs-lookup"><span data-stu-id="dab9d-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="dab9d-104">הוספת התחום, המשתמשים והגדרת המדיניות</span><span class="sxs-lookup"><span data-stu-id="dab9d-104">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="dab9d-105">[![תווית כדי ליידע אותך שמרכז הניהול משתנה ובאפשרותך למצוא פרטים נוספים ב-aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="dab9d-105">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="dab9d-106">בעת רכישת Microsoft 365 Business, יש לך את האפשרות להשתמש בתחום שבבעלותך, או לקנות אחד במהלך [ההרשמה](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="dab9d-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="dab9d-107">אם רכשת תחום חדש בעת החתימה, התחום שלך מוגדר ובאפשרותך לעבור [להוספת משתמשים ולהקצות רשיונות](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="dab9d-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="dab9d-108">הוסף את התחום שלך להתאמה אישית של הכניסה</span><span class="sxs-lookup"><span data-stu-id="dab9d-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="dab9d-109">היכנס ל- [Microsoft 365 admin center](https://admin.microsoft.com) באמצעות אישורי המנהל הגלובלי שלך.</span><span class="sxs-lookup"><span data-stu-id="dab9d-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="dab9d-110">בחר **בהוסף תחום** או **הוסף משתמשים** כדי להפעיל את האשף.</span><span class="sxs-lookup"><span data-stu-id="dab9d-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="dab9d-111">אם רכשת תחום במהלך ההרשמה, לא תראה **הוספת שלב בתחום** כאן.</span><span class="sxs-lookup"><span data-stu-id="dab9d-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="dab9d-112">עבור כדי [להוסיף משתמשים](#add-users-and-assign-licenses) במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="dab9d-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![בחר בהוסף תחום.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="dab9d-114">באשף, הזן את שם התחום בו ברצונך להשתמש (כגון contoso.com).</span><span class="sxs-lookup"><span data-stu-id="dab9d-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![צילום מסך של התאמה אישית של דף הכניסה שלך.](media/personalizesignin.png)

    
4. <span data-ttu-id="dab9d-116">בצע את השלבים באשף כדי [ליצור רשומות dns בכל ספק dns המארח עבור Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) המאמת את התחום שלך.</span><span class="sxs-lookup"><span data-stu-id="dab9d-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="dab9d-117">אם אתה מכיר את מארח התחום שלך, ראה גם את [ההנחיות הספציפיות למחשב המארח](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="dab9d-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="dab9d-118">אם ספק האירוח שלך הוא GoDaddy, או מארח אחר הזמין עם [התחברות לקבוצת מחשבים](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), התהליך יהיה פשוט ותתבקש באופן אוטומטי להיכנס ולאפשר למיקרוסופט לבצע אימות בשמך:</span><span class="sxs-lookup"><span data-stu-id="dab9d-118">If your hosting provider is GoDaddy, or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect),the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![בעמוד הרשאה לאישור, בחר באפשרות הרשאת.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="dab9d-120">הוספת משתמשים והקצאת רשיונות</span><span class="sxs-lookup"><span data-stu-id="dab9d-120">Add users and assign licenses</span></span>

<span data-ttu-id="dab9d-121">באפשרותך להוסיף משתמשים באשף, אך באפשרותך גם [להוסיף משתמשים בהמשך](add-users-m365b.md) מרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="dab9d-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="dab9d-122">בנוסף, אם ברשותך בקר תחום מקומי, באפשרותך להוסיף משתמשים בעלי [התקשרות תכלת](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="dab9d-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="dab9d-123">הוספת משתמשים באשף</span><span class="sxs-lookup"><span data-stu-id="dab9d-123">Add users in the wizard</span></span>

<span data-ttu-id="dab9d-124">כל משתמש שתוסיף באשף יוקצה באופן אוטומטי לרשיון עסקי של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="dab9d-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![צילום מסך של הדף ' הוספת משתמשים חדשים ' באשף](media/addnewuserspage.png)

1. <span data-ttu-id="dab9d-126">אם למנוי העסקי שלך ב-Microsoft 365 יש משתמשים קיימים (לדוגמה, אם השתמשת בתכלת AD Connect), תקבל אפשרות להקצות להם רשיונות כעת.</span><span class="sxs-lookup"><span data-stu-id="dab9d-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="dab9d-127">קדימה, הוסף רשיונות גם להם.</span><span class="sxs-lookup"><span data-stu-id="dab9d-127">Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="dab9d-128">לאחר שהוספת את המשתמשים, תהיה לך גם אפשרות לשתף אישורים עם המשתמשים החדשים שהוספת.</span><span class="sxs-lookup"><span data-stu-id="dab9d-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="dab9d-129">באפשרותך להדפיס אותם, לשלוח אותם בדואר אלקטרוני או להוריד אותם.</span><span class="sxs-lookup"><span data-stu-id="dab9d-129">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="dab9d-130">דלג על העברת הודעות דואר אלקטרוני ובחר **הבא** בדף **העברת הודעות דואר אלקטרוני**.</span><span class="sxs-lookup"><span data-stu-id="dab9d-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="dab9d-131">אם אתה עובר מספק דואר אלקטרוני אחר וברצונך להעתיק את הנתונים שלך מאוחר יותר, באפשרותך [להעביר דואר אלקטרוני ואנשי קשר ל-Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="dab9d-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="dab9d-132">חיבור התחום שלך</span><span class="sxs-lookup"><span data-stu-id="dab9d-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="dab9d-133">אם בחרת להשתמש בקבוצת המחשבים onmicrosoft, או בשימוש בתכלת-AD כדי להגדיר משתמשים, לא תראה שלב זה.</span><span class="sxs-lookup"><span data-stu-id="dab9d-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="dab9d-134">להגדרת שירותים, עליך לעדכן כמה רשומות אצל מארח ה- DNS שלך או אצל רשם התחומים.</span><span class="sxs-lookup"><span data-stu-id="dab9d-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="dab9d-135">אשף ההגדרה מזהה בדרך כלל את הרשם שלך, ומספק לך קישור להוראות מפורטות לעדכון רשומות ה- NS באתר האינטרנט של הרשם.</span><span class="sxs-lookup"><span data-stu-id="dab9d-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="dab9d-136">אם לא, [שנה את שרתי הnamםכדי להגדיר את Office 365 עם כל רשם תחום](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="dab9d-136">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="dab9d-137">אם יש לך רשומות DNS קיימות, לדוגמה אתר אינטרנט קיים, אך מארח ה-DNS שלך זמין עבור [התחברות לתחום](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), בחר **באפשרות ' הוסף רשומות**עבורי '.</span><span class="sxs-lookup"><span data-stu-id="dab9d-137">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> 
    - <span data-ttu-id="dab9d-138">אם יש לך רשומות DNS קיימות עם מארחי DNS אחרים (שאינם זמינים עבור התחברות לתחום), תרצה לנהל את רשומות ה-DNS שלך כדי לוודא שהשירותים הקיימים יישארו מחוברים.</span><span class="sxs-lookup"><span data-stu-id="dab9d-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="dab9d-139">לקבלת מידע נוסף, ראה [יסודות קבוצת מחשבים](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .</span><span class="sxs-lookup"><span data-stu-id="dab9d-139">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![חבר את דף התחום שלך עם אני ינהל את רשומות ה-DNS שלי.](media/connectyourdomainpage.png)

2. <span data-ttu-id="dab9d-141">בצע את השלבים באשף ובדואר אלקטרוני ובשירותים אחרים שהוגדרו עבורך.</span><span class="sxs-lookup"><span data-stu-id="dab9d-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="dab9d-142">הגדרת מדיניות אבטחה ותצורות התקנים</span><span class="sxs-lookup"><span data-stu-id="dab9d-142">Set up security policies and device configurations</span></span> 

<span data-ttu-id="dab9d-143">פריטי המדיניות שאתה מגדיר באשף מוחלים באופן אוטומטי על [קבוצת אבטחה](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) הנקראת ' *כל המשתמשים*'.</span><span class="sxs-lookup"><span data-stu-id="dab9d-143">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="dab9d-144">באפשרותך גם ליצור קבוצות נוספות להקצאת פריטי מדיניות במרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="dab9d-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="dab9d-145">בהגנה על **קבצי העבודה שלך במכשירים ניידים** האפשרות **להגן על קבצי עבודה כאשר התקנים אובדים או גנובים מסומנים כברירת** מחדל.</span><span class="sxs-lookup"><span data-stu-id="dab9d-145">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="dab9d-146">יש לך אפשרות להפעיל את **ניהול האופן שבו משתמשים ניגשים לקבצי Office במכשירים ניידים**, ומומלץ לעשות זאת.</span><span class="sxs-lookup"><span data-stu-id="dab9d-146">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![צילום מסך של הגנה על קבצי עבודה בדף התקנים ניידים.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="dab9d-148">הרחב **הגן על קבצי עבודה כאשר התקנים אובדים או גנובים** כדי להציג את [ערכי ברירת המחדל](protect-work-files-on-lost-or-stolen-device.md):</span><span class="sxs-lookup"><span data-stu-id="dab9d-148">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![צילום מסך של ערכי ברירת מחדל להגנה על קבצים בהתקנים אבודים.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="dab9d-150">בחר באפשרות **נהל את אופן הגישה של משתמשים לקבצי Office בהתקנים ניידים** והרחב אותו כדי להציג את [ערכי ברירת המחדל](manage-user-access-on-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="dab9d-150">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="dab9d-151">מומלץ לקבל את ערכי ברירת המחדל במהלך ההתקנה כדי ליצור מדיניות יישומים עבור אנדרואיד, iOS ו-Windows 10 החלים על כל המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="dab9d-151">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="dab9d-152">ניתן ליצור פריטי מדיניות נוספים לאחר השלמת ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="dab9d-152">You can create more policies after setup completes.</span></span>

        ![צילום מסך של הגדרות הגנה עבור קבצי Office בנייד.](media/useraccessonmobile.png)

2. <span data-ttu-id="dab9d-154">השלב האחרון בהגנה על נתונים והתקנים מאפשר לך להגדיר מדיניות לאבטחת התקני Windows 10.</span><span class="sxs-lookup"><span data-stu-id="dab9d-154">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="dab9d-155">הגדרות אלה מוחלות באופן אוטומטי בעת התחברות Windows 10 של משתמש לארגון.</span><span class="sxs-lookup"><span data-stu-id="dab9d-155">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="dab9d-156">באפשרותך להרחיב **התקנים מאובטחים של Windows 10** כדי לראות ולשנות את [ערכי ברירת המחדל](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="dab9d-156">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="dab9d-157">באפשרותך גם לבחור [להתקין באופן אוטומטי את Office](install-office-on-windows-10-during-setup.md) בהתקני Windows 10.</span><span class="sxs-lookup"><span data-stu-id="dab9d-157">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![צילום מסך של הגדרת Windows 10 תצורת התקן הדף.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="dab9d-159">פריסת Office 365 יישומי לקוח</span><span class="sxs-lookup"><span data-stu-id="dab9d-159">Deploy Office 365 client apps</span></span>

<span data-ttu-id="dab9d-160">אם בחרת להתקין באופן אוטומטי יישומי Office במהלך ההתקנה, היישומים יותקנו בהתקני Windows 10 לאחר שהמשתמשים יחתמו לתכלת המחשב מהתקני Windows שלהם עם אישורי העבודה שלהם.</span><span class="sxs-lookup"><span data-stu-id="dab9d-160">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="dab9d-161">כדי להתקין את Office ב-iOS נייד או בהתקני Android, ראה [הגדרת מכשירים ניידים עבור משתמשים עסקיים של Microsoft 365](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="dab9d-161">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="dab9d-162">באפשרותך גם להתקין את Office בנפרד.</span><span class="sxs-lookup"><span data-stu-id="dab9d-162">You can also install Office individually.</span></span> <span data-ttu-id="dab9d-163">ראה [התקנת Office במחשב או במקינטוש](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) לקבלת הוראות.</span><span class="sxs-lookup"><span data-stu-id="dab9d-163">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>
