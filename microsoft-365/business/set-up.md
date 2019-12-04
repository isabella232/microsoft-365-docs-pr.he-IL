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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: למד כיצד להגדיר את Microsoft 365 Business.
ms.openlocfilehash: 0001c2b9962f6cce0be1f77cbf427c68f9ee3249
ms.sourcegitcommit: c5ca71d6feb0f033b50ccd4de816fd59b0925007
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/04/2019
ms.locfileid: "39831302"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="c0d74-103">הגדרת העסק של Microsoft 365 באשף ההתקנה</span><span class="sxs-lookup"><span data-stu-id="c0d74-103">Set up Microsoft 365 Business in the setup wizard</span></span>

<span data-ttu-id="c0d74-104">צפה בסרטון וידאו זה למבט כולל על ההתקנה העסקית של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c0d74-104">Watch this video for an overview of Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

<span data-ttu-id="c0d74-105">אם מצאת את הסרטון הזה מועיל, בדוק את [סידרת ההדרכה המלאה לעסקים קטנים ולאלה החדשים ל-Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="c0d74-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="c0d74-106">הוספת התחום, המשתמשים והגדרת המדיניות</span><span class="sxs-lookup"><span data-stu-id="c0d74-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="c0d74-107">[![תווית המיידעת אותך שמרכז הניהול משתנה ושניתן למצוא פרטים נוספים ב- aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="c0d74-107">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="c0d74-108">בעת רכישת Microsoft 365 Business, יש לך את האפשרות להשתמש בתחום שבבעלותך, או לקנות אחד במהלך [ההרשמה](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="c0d74-108">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="c0d74-109">אם רכשת תחום חדש בעת החתימה, התחום שלך מוגדר ובאפשרותך לעבור [להוספת משתמשים ולהקצות רשיונות](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="c0d74-109">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="c0d74-110">הוסף את התחום שלך להתאמה אישית של הכניסה</span><span class="sxs-lookup"><span data-stu-id="c0d74-110">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="c0d74-111">היכנס ל- [Microsoft 365 admin center](https://admin.microsoft.com) באמצעות אישורי המנהל הגלובלי שלך.</span><span class="sxs-lookup"><span data-stu-id="c0d74-111">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="c0d74-112">בחר באפשרות **עבור אל ההתקנה** כדי להפעיל את האשף.</span><span class="sxs-lookup"><span data-stu-id="c0d74-112">Choose **Go to setup** to start the wizard.</span></span>

    ![בחר באפשרות עבור לכיוונון.](media/gotosetupinadmincenter.png)

3. <span data-ttu-id="c0d74-114">בדף **התקנת היישומים שלך** ב-Office, באפשרותך להתקין את היישומים במחשב שלך באופן אופציונלי.</span><span class="sxs-lookup"><span data-stu-id="c0d74-114">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="c0d74-115">בשלב **הוספת תחום** , הזן את שם התחום בו ברצונך להשתמש (כגון contoso.com).</span><span class="sxs-lookup"><span data-stu-id="c0d74-115">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="c0d74-116">אם רכשת תחום במהלך ההרשמה, לא תראה **הוספת שלב בתחום** כאן.</span><span class="sxs-lookup"><span data-stu-id="c0d74-116">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="c0d74-117">עבור כדי [להוסיף משתמשים](#add-users-and-assign-licenses) במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="c0d74-117">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![צילום מסך של התאמה אישית של דף הכניסה שלך.](media/adddomain.png)

    
4. <span data-ttu-id="c0d74-119">בצע את השלבים באשף כדי [ליצור רשומות dns בכל ספק dns המארח עבור Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) המאמת את התחום שלך.</span><span class="sxs-lookup"><span data-stu-id="c0d74-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="c0d74-120">אם אתה מכיר את מארח התחום שלך, ראה גם את [ההנחיות הספציפיות למחשב המארח](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="c0d74-120">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="c0d74-121">אם ספק האירוח שלך הוא GoDaddy או מארח אחר הזמין עם [התחברות לקבוצת מחשבים](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), התהליך יהיה פשוט ותתבקש באופן אוטומטי להיכנס ולאפשר ל-Microsoft לבצע אימות בשמך.</span><span class="sxs-lookup"><span data-stu-id="c0d74-121">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![בעמוד הרשאה לאישור, בחר באפשרות הרשאת.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="c0d74-123">הוספת משתמשים והקצאת רשיונות</span><span class="sxs-lookup"><span data-stu-id="c0d74-123">Add users and assign licenses</span></span>

<span data-ttu-id="c0d74-124">באפשרותך להוסיף משתמשים באשף, אך באפשרותך גם [להוסיף משתמשים בהמשך](add-users-m365b.md) מרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="c0d74-124">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="c0d74-125">בנוסף, אם ברשותך בקר תחום מקומי, באפשרותך להוסיף משתמשים בעלי [התקשרות תכלת](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="c0d74-125">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="c0d74-126">הוספת משתמשים באשף</span><span class="sxs-lookup"><span data-stu-id="c0d74-126">Add users in the wizard</span></span>

<span data-ttu-id="c0d74-127">כל משתמש שתוסיף באשף יוקצה באופן אוטומטי לרשיון עסקי של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c0d74-127">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![צילום מסך של הדף ' הוספת משתמשים חדשים ' באשף](media/addnewuserspage.png)

1. <span data-ttu-id="c0d74-129">אם למנוי העסקי שלך ב-Microsoft 365 יש משתמשים קיימים (לדוגמה, אם השתמשת בתכלת AD Connect), תקבל אפשרות להקצות להם רשיונות כעת.</span><span class="sxs-lookup"><span data-stu-id="c0d74-129">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="c0d74-130">קדימה, הוסף רשיונות גם להם.</span><span class="sxs-lookup"><span data-stu-id="c0d74-130">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="c0d74-131">לאחר שהוספת את המשתמשים, תקבל גם אפשרות לשתף אישורים עם המשתמשים החדשים שהוספת.</span><span class="sxs-lookup"><span data-stu-id="c0d74-131">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="c0d74-132">באפשרותך להדפיס אותם, לשלוח אותם בדואר אלקטרוני או להוריד אותם.</span><span class="sxs-lookup"><span data-stu-id="c0d74-132">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="c0d74-133">חיבור התחום שלך</span><span class="sxs-lookup"><span data-stu-id="c0d74-133">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="c0d74-134">אם בחרת להשתמש בקבוצת המחשבים onmicrosoft, או בשימוש בתכלת-AD כדי להגדיר משתמשים, לא תראה שלב זה.</span><span class="sxs-lookup"><span data-stu-id="c0d74-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="c0d74-135">להגדרת שירותים, עליך לעדכן כמה רשומות אצל מארח ה- DNS שלך או אצל רשם התחומים.</span><span class="sxs-lookup"><span data-stu-id="c0d74-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="c0d74-136">אשף ההגדרה מזהה בדרך כלל את הרשם שלך, ומספק לך קישור להוראות מפורטות לעדכון רשומות ה- NS באתר האינטרנט של הרשם.</span><span class="sxs-lookup"><span data-stu-id="c0d74-136">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="c0d74-137">אם לא, [שנה את שרתי הnamםכדי להגדיר את Office 365 עם כל רשם תחום](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="c0d74-137">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="c0d74-138">אם יש לך רשומות DNS קיימות, לדוגמה אתר אינטרנט קיים, אך מארח ה-DNS שלך זמין עבור [התחברות לתחום](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), בחר **באפשרות ' הוסף רשומות**עבורי '.</span><span class="sxs-lookup"><span data-stu-id="c0d74-138">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="c0d74-139">בדף **' בחירת שירותים מקוונים** ', קבל את כל ברירות המחדל ובחר באפשרות ' **הבא**' ובחר ' **אישור** ' בדף המארח של DNS.</span><span class="sxs-lookup"><span data-stu-id="c0d74-139">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="c0d74-140">אם יש לך רשומות DNS קיימות עם מארחי DNS אחרים (שאינם זמינים עבור התחברות לתחום), תרצה לנהל את רשומות ה-DNS שלך כדי לוודא שהשירותים הקיימים יישארו מחוברים.</span><span class="sxs-lookup"><span data-stu-id="c0d74-140">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="c0d74-141">לקבלת מידע נוסף, ראה [יסודות קבוצת מחשבים](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) .</span><span class="sxs-lookup"><span data-stu-id="c0d74-141">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![הפעלת דף רשומות.](media/activaterecords.png)

2. <span data-ttu-id="c0d74-143">בצע את השלבים באשף ובדואר אלקטרוני ובשירותים אחרים שהוגדרו עבורך.</span><span class="sxs-lookup"><span data-stu-id="c0d74-143">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="c0d74-144">הגן על הארגון שלך</span><span class="sxs-lookup"><span data-stu-id="c0d74-144">Protect your organization</span></span> 

<span data-ttu-id="c0d74-145">פריטי המדיניות שאתה מגדיר באשף מוחלים באופן אוטומטי על [קבוצת אבטחה](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) הנקראת ' *כל המשתמשים*'.</span><span class="sxs-lookup"><span data-stu-id="c0d74-145">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="c0d74-146">באפשרותך גם ליצור קבוצות נוספות להקצאת פריטי מדיניות במרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="c0d74-146">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="c0d74-147">על **הגנה מפני הגדלת מאיומי סייבר מתקדמים**, מומלץ לקבל את ברירות המחדל כדי לאפשר ל- [Office 365 מראש הגנה על איומים](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) לסרוק קבצים וקישורים ב-office apps.</span><span class="sxs-lookup"><span data-stu-id="c0d74-147">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![צילום מסך של עמוד הגנה מפני הגדלת.](media/increasetreatprotection.png)


2. <span data-ttu-id="c0d74-149">על מנת **למנוע דליפות של דף נתונים רגישים** , קבל את ברירות המחדל כדי להפעיל את מניעת אובדן נתונים של Office 365 (DLP) כדי לעקוב אחר נתונים רגישים ביישומי office ולמנוע את השיתוף המקרי של אלה מחוץ לארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="c0d74-149">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="c0d74-150">בעמוד **הגנה על הנתונים ב-Office for mobile** , השאר את ניהול האפליקציות הניידות, הרחב את ההגדרות וסקור אותן ולאחר מכן בחר באפשרות **צור מדיניות ניהול אפליקציות ניידות**.</span><span class="sxs-lookup"><span data-stu-id="c0d74-150">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![צילום מסך של הגנה על נתונים ב-Office עבור דף נייד.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="c0d74-152">אבטחת Windows 10 מחשבים אישיים</span><span class="sxs-lookup"><span data-stu-id="c0d74-152">Secure Windows 10 PCs</span></span>

<span data-ttu-id="c0d74-153">בניווט השמאלי, בחר **בהגדרה** ולאחר מכן, תחת **שירה ואבטחה**, בחר **באבטחת מחשבי Windows 10 שלך**.</span><span class="sxs-lookup"><span data-stu-id="c0d74-153">On the left nav, select **Setup** and then, under **Sing-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="c0d74-154">בחר **' תצוגה '** כדי להתחיל.</span><span class="sxs-lookup"><span data-stu-id="c0d74-154">Choose **View** to get started.</span></span> <span data-ttu-id="c0d74-155">לקבלת הוראות מלאות, ראה [אבטחת מחשבי Windows 10](secure-win-10-pcs.md) .</span><span class="sxs-lookup"><span data-stu-id="c0d74-155">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="c0d74-156">פריסת Office 365 יישומי לקוח</span><span class="sxs-lookup"><span data-stu-id="c0d74-156">Deploy Office 365 client apps</span></span>

<span data-ttu-id="c0d74-157">אם בחרת להתקין באופן אוטומטי יישומי Office במהלך ההתקנה, היישומים יותקנו בהתקני Windows 10 לאחר שהמשתמשים יחתמו לתכלת לספירה מהתקני Windows שלהם, תוך שימוש באישורי העבודה שלהם.</span><span class="sxs-lookup"><span data-stu-id="c0d74-157">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="c0d74-158">כדי להתקין את Office ב-iOS נייד או בהתקני Android, ראה [הגדרת מכשירים ניידים עבור משתמשים עסקיים של Microsoft 365](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="c0d74-158">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="c0d74-159">באפשרותך גם להתקין את Office בנפרד.</span><span class="sxs-lookup"><span data-stu-id="c0d74-159">You can also install Office individually.</span></span> <span data-ttu-id="c0d74-160">ראה [התקנת Office במחשב או במקינטוש](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) לקבלת הוראות.</span><span class="sxs-lookup"><span data-stu-id="c0d74-160">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="c0d74-161">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="c0d74-161">See also</span></span>

[<span data-ttu-id="c0d74-162">סרטוני הדרכה עסקיים של Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c0d74-162">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
