---
title: הגדרת Microsoft 365 Business Premium
f1.keywords:
- NOCSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: גלה את שלבי ההגדרה עבור Microsoft 365 Business Premium, כולל הוספת תחום ומשתמשים, הגדרת מדיניות אבטחה ועוד.
ms.openlocfilehash: 5b082e78f3dc4067dcce4a96a8088b2347bc3af4
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912569"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="9fd76-103">הגדרת Microsoft 365 Business Premium באשף ההגדרה</span><span class="sxs-lookup"><span data-stu-id="9fd76-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="9fd76-104">צפה בסרטון וידאו זה לקבלת מבט כולל על התקנת Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="9fd76-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="9fd76-105">הוספת התחום, המשתמשים ומדיניות ההגדרה</span><span class="sxs-lookup"><span data-stu-id="9fd76-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="9fd76-106">כאשר אתה רוכש את Microsoft 365 Business Premium, באפשרותך להשתמש בתחום שבבעלותך או לקנות אותו במהלך [ההרשמה](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="9fd76-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="9fd76-107">אם רכשת תחום חדש כאשר נרשמת, התחום שלך מוגדר כולו ובאפשרותך לעבור [להוספת משתמשים ולהקצות רשיונות](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="9fd76-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="9fd76-108">הוספת התחום שלך להתאמה אישית של כניסה</span><span class="sxs-lookup"><span data-stu-id="9fd76-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="9fd76-109">היכנס אל [מרכז הניהול של Microsoft 365](https://admin.microsoft.com) באמצעות אישורי מנהל המערכת הכלליים שלך.</span><span class="sxs-lookup"><span data-stu-id="9fd76-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="9fd76-110">בחר **עבור אל תוכנית ההתקנה** כדי להפעיל את האשף.</span><span class="sxs-lookup"><span data-stu-id="9fd76-110">Choose **Go to setup** to start the wizard.</span></span>

    ![בחר עבור אל תוכנית ההתקנה.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="9fd76-112">בדף **התקן את יישומי Office שלך** , באפשרותך להתקין את היישומים במחשב שלך באופן אופציונלי.</span><span class="sxs-lookup"><span data-stu-id="9fd76-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="9fd76-113">בשלב **הוספת תחום** , הזן את שם התחום שבו ברצונך להשתמש (כגון contoso.com).</span><span class="sxs-lookup"><span data-stu-id="9fd76-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="9fd76-114">אם רכשת תחום במהלך ההרשמה, לא תראה את האפשרות **הוסף שלב זה לתחום** .</span><span class="sxs-lookup"><span data-stu-id="9fd76-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="9fd76-115">עבור אל [הוספת משתמשים](#add-users-and-assign-licenses) במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="9fd76-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![צילום מסך של דף הכניסה התאמה אישית.](../media/adddomain.png)

    
4. <span data-ttu-id="9fd76-117">בצע את השלבים באשף כדי [ליצור רשומות dns בכל ספק אירוח dns עבור Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) שמאמת את בעלותך על התחום.</span><span class="sxs-lookup"><span data-stu-id="9fd76-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="9fd76-118">אם אתה מכיר את מארח התחום שלך, ראה גם [הוראות ספציפיות למארח](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="9fd76-118">If you know your domain host, see also the [host specific instructions](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="9fd76-119">אם ספק האירוח שלך הוא GoDaddy או מארח אחר זמין עם ' [חיבור לתחומים](/office365/admin/get-help-with-domains/domain-connect)', התהליך קל וברצונך להיכנס באופן אוטומטי ולאפשר ל-Microsoft לאמת בשמך.</span><span class="sxs-lookup"><span data-stu-id="9fd76-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![בדף GoDaddy אישור גישה, בחר הרשאה.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="9fd76-121">הוספת משתמשים והקצאת רשיונות</span><span class="sxs-lookup"><span data-stu-id="9fd76-121">Add users and assign licenses</span></span>

<span data-ttu-id="9fd76-122">באפשרותך להוסיף משתמשים באשף, אך באפשרותך גם [להוסיף משתמשים בהמשך](../admin/add-users/add-users.md) מרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="9fd76-122">You can add users in the wizard, but you can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span> <span data-ttu-id="9fd76-123">בנוסף, אם יש לך בקר תחום מקומי, באפשרותך להוסיף משתמשים בעלי [התחברות של תכלת לספירה](/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="9fd76-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="9fd76-124">הוספת משתמשים באשף</span><span class="sxs-lookup"><span data-stu-id="9fd76-124">Add users in the wizard</span></span>

<span data-ttu-id="9fd76-125">כל המשתמשים שתוסיף באשף יוקצה באופן אוטומטי רשיון של Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="9fd76-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![צילום מסך של הדף ' הוספת משתמשים חדשים ' באשף](../media/addnewuserspage.png)

1. <span data-ttu-id="9fd76-127">אם המנוי שלך ל-Microsoft 365 Business Premium מכיל משתמשים קיימים (לדוגמה, אם השתמשת בחיבור של תכלת לספירה), אתה מקבל אפשרות להקצות להם רשיונות כעת.</span><span class="sxs-lookup"><span data-stu-id="9fd76-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="9fd76-128">קדימה, הוסף רשיונות גם להם.</span><span class="sxs-lookup"><span data-stu-id="9fd76-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="9fd76-129">לאחר שהוספת את המשתמשים, תקבל גם אפשרות לשתף אישורים עם המשתמשים החדשים שהוספת.</span><span class="sxs-lookup"><span data-stu-id="9fd76-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="9fd76-130">באפשרותך להדפיס אותם, לשלוח אותם בדואר אלקטרוני או להוריד אותם.</span><span class="sxs-lookup"><span data-stu-id="9fd76-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="9fd76-131">חיבור התחום שלך</span><span class="sxs-lookup"><span data-stu-id="9fd76-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="9fd76-132">אם בחרת להשתמש בתחום. onmicrosoft, או השתמש ב-תכלת AD Connect כדי להגדיר משתמשים, לא תראה שלב זה.</span><span class="sxs-lookup"><span data-stu-id="9fd76-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="9fd76-133">להגדרת שירותים, עליך לעדכן כמה רשומות אצל מארח ה- DNS שלך או אצל רשם התחומים.</span><span class="sxs-lookup"><span data-stu-id="9fd76-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="9fd76-134">אשף ההגדרה מזהה בדרך כלל את הרשם שלך, ומספק לך קישור להוראות מפורטות לעדכון רשומות ה- NS באתר האינטרנט של הרשם.</span><span class="sxs-lookup"><span data-stu-id="9fd76-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="9fd76-135">אם היא אינה [מופיעה, שנה את nameservers כדי להגדיר את Microsoft 365 עם רשם תחומים כלשהו](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md).</span><span class="sxs-lookup"><span data-stu-id="9fd76-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md).</span></span> 

    - <span data-ttu-id="9fd76-136">אם יש לך רשומות DNS קיימות, למשל אתר אינטרנט קיים, אך מארח ה-DNS שלך מופעל עבור ' [חיבור תחום](/office365/admin/get-help-with-domains/domain-connect)', בחר ' **הוסף רשומות עבורי**'.</span><span class="sxs-lookup"><span data-stu-id="9fd76-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="9fd76-137">בדף **בחירת שירותים מקוונים** , קבל את כל ברירות המחדל ובחר **הבא**, ובחר **הרשאה** בעמוד של מארח ה-DNS שלך.</span><span class="sxs-lookup"><span data-stu-id="9fd76-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="9fd76-138">אם יש לך רשומות DNS קיימות עם מארחי DNS אחרים (שאינם זמינים עבור ' חיבור תחום '), מומלץ לנהל רשומות DNS משלך כדי לוודא שהשירותים הקיימים נשארים מחוברים.</span><span class="sxs-lookup"><span data-stu-id="9fd76-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="9fd76-139">ראה [יסודות תחום](/office365/admin/get-help-with-domains/dns-basics) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="9fd76-139">See [domain basics](/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![הפעלת הדף records.](../media/activaterecords.png)

2. <span data-ttu-id="9fd76-141">בצע את השלבים באשף ובדואר האלקטרוני ושירותים אחרים יוגדרו עבורך.</span><span class="sxs-lookup"><span data-stu-id="9fd76-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="9fd76-142">הגנה על הארגון שלך</span><span class="sxs-lookup"><span data-stu-id="9fd76-142">Protect your organization</span></span> 

<span data-ttu-id="9fd76-143">המדיניות שתגדיר באשף מוחלת באופן אוטומטי על [קבוצת אבטחה](/office365/admin/create-groups/compare-groups#security-groups) הנקראת *כל המשתמשים*.</span><span class="sxs-lookup"><span data-stu-id="9fd76-143">The policies you set up in the wizard are applied automatically to a [Security group](/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="9fd76-144">באפשרותך גם ליצור קבוצות נוספות כדי להקצות פריטי מדיניות למרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="9fd76-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="9fd76-145">בנושא **הגדלת ההגנה מפני איומי סייבר מתקדמים**, מומלץ לקבל את ברירות המחדל כדי לאפשר [להגנת האיום של office 365](../security/office-365-security/office-365-atp.md) לסרוק קבצים וקישורים ביישומי office.</span><span class="sxs-lookup"><span data-stu-id="9fd76-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](../security/office-365-security/office-365-atp.md) scan files and links in Office apps.</span></span>

    ![צילום מסך של הדף ' הגדל הגנה '.](../media/increasetreatprotection.png)


2. <span data-ttu-id="9fd76-147">בדף **מנע הדלפות של נתונים רגישים** , קבל את ברירות המחדל להפעלת מניעת אובדן נתונים של office 365 (DLP) כדי לעקוב אחר נתונים רגישים ביישומי office ולמנוע את השיתוף המקרי של הקבצים האלה מחוץ לארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="9fd76-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="9fd76-148">בדף ' **הגנה על נתונים ב-Office למכשירים ניידים** ', השאר את ' ניהול אפליקציות למכשירים ניידים ', הרחב את ההגדרות וסקור אותן ולאחר מכן בחר באפשרות **צור מדיניות ניהול אפליקציות למכשירים ניידים**.</span><span class="sxs-lookup"><span data-stu-id="9fd76-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![צילום מסך של הגנה על נתונים בדף Office למכשירים ניידים.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="9fd76-150">מחשבי Pc של Windows 10 מאובטחים</span><span class="sxs-lookup"><span data-stu-id="9fd76-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="9fd76-151">בסרגל הניווט הימני, בחר **הגדרה** ולאחר מכן, תחת **כניסה ואבטחה**, בחר **Secure Windows 10 מחשבים**.</span><span class="sxs-lookup"><span data-stu-id="9fd76-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="9fd76-152">בחר **' תצוגה** ' כדי להתחיל בעבודה.</span><span class="sxs-lookup"><span data-stu-id="9fd76-152">Choose **View** to get started.</span></span> <span data-ttu-id="9fd76-153">ראה [Secure Windows 10 מחשבים](secure-win-10-pcs.md) לקבלת הוראות מלאות.</span><span class="sxs-lookup"><span data-stu-id="9fd76-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="9fd76-154">פריסת יישומי לקוח של Office 365</span><span class="sxs-lookup"><span data-stu-id="9fd76-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="9fd76-155">אם בחרת להתקין באופן אוטומטי את יישומי Office במהלך ההתקנה, היישומים יותקנו במכשירי Windows 10 לאחר שהמשתמשים נכנסו לאזור התכלת לספירה ממכשירי Windows שלהם, תוך שימוש באישורי העבודה שלהם.</span><span class="sxs-lookup"><span data-stu-id="9fd76-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="9fd76-156">כדי להתקין את Office במכשירים ניידים של iOS או Android, ראה [הגדרת מכשירים ניידים עבור משתמשי Microsoft 365 Business Premium](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="9fd76-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="9fd76-157">באפשרותך גם להתקין את Office בנפרד.</span><span class="sxs-lookup"><span data-stu-id="9fd76-157">You can also install Office individually.</span></span> <span data-ttu-id="9fd76-158">ראה [התקנת Office במחשב PC או Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) לקבלת הוראות.</span><span class="sxs-lookup"><span data-stu-id="9fd76-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="9fd76-159">ראה גם</span><span class="sxs-lookup"><span data-stu-id="9fd76-159">See also</span></span>

[<span data-ttu-id="9fd76-160">סרטוני וידאו של הדרכה של Microsoft 365 for business</span><span class="sxs-lookup"><span data-stu-id="9fd76-160">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)