---
title: הגדלת הגנת האיום עבור Microsoft 365 Business Premium
f1.keywords:
- NOCSH
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
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: הגדר תכונות תאימות כדי למנוע אובדן נתונים ולסייע בשמירה על מידע רגיש של הלקוחות שלך והלקוח שלך.
ms.openlocfilehash: e210787718025c5df29af8d4a2283291dcecc2a8
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912529"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="f34c0-103">הגדרת תכונות תאימות</span><span class="sxs-lookup"><span data-stu-id="f34c0-103">Set up compliance features</span></span>

<span data-ttu-id="f34c0-104">ה-Microsoft 365 Business Premium מגיע עם תכונות להגנה על הנתונים והמכשירים שלך, ומסייע לך לשמור על מידע רגיש ומאובטח של הלקוחות שלך.</span><span class="sxs-lookup"><span data-stu-id="f34c0-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="f34c0-105">הגדרת תכונות של DLP</span><span class="sxs-lookup"><span data-stu-id="f34c0-105">Set up DLP features</span></span>

<span data-ttu-id="f34c0-106">ראה [יצירת מדיניות DLP מתבנית](../compliance/create-a-dlp-policy-from-a-template.md) לקבלת דוגמה לגבי אופן הגדרת מדיניות להגנה מפני הגנה על אובדן נתונים אישיים.</span><span class="sxs-lookup"><span data-stu-id="f34c0-106">See [Create a DLP policy from a template](../compliance/create-a-dlp-policy-from-a-template.md) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="f34c0-107">DLP מגיע עם תבניות מדיניות רבות מוכנות לשימוש עבור אזורים רבים ושונים.</span><span class="sxs-lookup"><span data-stu-id="f34c0-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="f34c0-108">לדוגמה, הנתונים הכספיים של אוסטרליה, חוק קנדה מידע אישי, הנתונים הפיננסיים של ארצות הברית וכן הלאה.</span><span class="sxs-lookup"><span data-stu-id="f34c0-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="f34c0-109">גלה [מהן תבניות מדיניות DLP הכוללות](../compliance/what-the-dlp-policy-templates-include.md) רשימה מלאה.</span><span class="sxs-lookup"><span data-stu-id="f34c0-109">See [What the DLP policy templates include](../compliance/what-the-dlp-policy-templates-include.md) for a full list.</span></span> <span data-ttu-id="f34c0-110">ניתן להפוך את כל התבניות האלה לזמינות בדומה לדוגמה של תבנית PII.</span><span class="sxs-lookup"><span data-stu-id="f34c0-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="f34c0-111">הגדרת שמירה בדואר אלקטרוני באמצעות אחסון בארכיון של Exchange Online</span><span class="sxs-lookup"><span data-stu-id="f34c0-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="f34c0-112">תכונות רשיון **לאחסון בארכיון של Exchange Online** עוזרות לשמור על תאימות וסטנדרטים תקינים על-ידי שימור תוכן דואר אלקטרוני עבור גילוי אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="f34c0-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="f34c0-113">היא גם מסייעת לצמצם את הסיכון אם קיימת תביעה משפטית, ומספקת דרך לשחזר נתונים לאחר פרצת אבטחה או כאשר עליך לשחזר פריטים שנמחקו.</span><span class="sxs-lookup"><span data-stu-id="f34c0-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="f34c0-114">באפשרותך להשתמש בחסימה לצורך תביעה משפטית כדי לשמר את כל תוכן המשתמש, או להשתמש במדיניות שמירה כדי להתאים אישית את מה שברצונך לשמר.</span><span class="sxs-lookup"><span data-stu-id="f34c0-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="f34c0-115">**חסימה לצורך תביעה משפטית:** באפשרותך לשמור את כל תוכן תיבת הדואר, כולל פריטים שנמחקו על-ידי הצבת תיבת דואר כולה של משתמש בחסימה לצורך תביעה משפטית.</span><span class="sxs-lookup"><span data-stu-id="f34c0-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="f34c0-116">כדי למקם תיבת דואר בחסימה לצורך תביעה משפטית, במרכז הניהול:</span><span class="sxs-lookup"><span data-stu-id="f34c0-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="f34c0-117">בניווט הימני, **עבור אל משתמשים** \> **פעילים**.</span><span class="sxs-lookup"><span data-stu-id="f34c0-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="f34c0-118">בחר משתמש שאת תיבת הדואר שלו ברצונך למקם בחסימה לצורך תביעה משפטית.</span><span class="sxs-lookup"><span data-stu-id="f34c0-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="f34c0-119">בחלונית המשתמש, הרחב את **הגדרות דואר** וליד **הגדרות נוספות**, בחר באפשרות **ערוך מאפייני Exchange**.</span><span class="sxs-lookup"><span data-stu-id="f34c0-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="f34c0-120">בדף תיבת הדואר של המשתמש, בחר \* \* תכונות תיבת דואר \* \* בניווט הימני ולאחר מכן בחר **באפשרות הפוך קישור לזמין** תחת חסימה לצורך **תביעה משפטית**.</span><span class="sxs-lookup"><span data-stu-id="f34c0-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="f34c0-121">בתיבת הדו חסימה לצורך **תביעה משפטית** , באפשרותך לציין את משך החסימה של הליטיגציה בשדה **משך החזקת הליטיגציה** .</span><span class="sxs-lookup"><span data-stu-id="f34c0-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="f34c0-122">השאר את השדה ריק אם ברצונך להציב חסימה אינסופית.</span><span class="sxs-lookup"><span data-stu-id="f34c0-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="f34c0-123">באפשרותך גם להוסיף הערות ולנתב את בעלי תיבת הדואר לאתר אינטרנט שייתכן שתצטרך להסביר מידע נוסף אודות החסימה לצורך תביעה משפטית.</span><span class="sxs-lookup"><span data-stu-id="f34c0-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="f34c0-124">\>**שמור**.</span><span class="sxs-lookup"><span data-stu-id="f34c0-124">\> **Save**.</span></span>
    
<span data-ttu-id="f34c0-125">**שמירה:** באפשרותך להפוך מדיניות שמירה מותאמת אישית לזמינה, לדוגמה, כדי לשמר עבור פרק זמן ספציפי או למחוק תוכן לצמיתות בסוף תקופת השמירה.</span><span class="sxs-lookup"><span data-stu-id="f34c0-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="f34c0-126">לקבלת מידע נוסף, ראה [מבט כולל על מדיניות שמירה](../compliance/retention.md).</span><span class="sxs-lookup"><span data-stu-id="f34c0-126">To learn more, see [Overview of retention policies](../compliance/retention.md).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="f34c0-127">הגדרת תוויות רגישות</span><span class="sxs-lookup"><span data-stu-id="f34c0-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="f34c0-128">תוויות רגישות מגיעות עם הגנה על מידע תכלת (AIP) תוכנית 1, ומסייעות לך לסווג, ובאופן אופציונלי להגן על המסמכים והודעות הדואר האלקטרוני שלך, על-ידי החלת תוויות.</span><span class="sxs-lookup"><span data-stu-id="f34c0-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="f34c0-129">ניתן להחיל תוויות באופן אוטומטי על-ידי מנהלי מערכת המגדירים כללים ותנאים, באופן ידני על-ידי משתמשים, או באמצעות שילוב שבו משתמשים מקבלים המלצות.</span><span class="sxs-lookup"><span data-stu-id="f34c0-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="f34c0-130">כדי להגדיר תוויות רגישות, הצג [וידאו יצירה וניהול של תוויות רגישות](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) .</span><span class="sxs-lookup"><span data-stu-id="f34c0-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="f34c0-131">התקנת הלקוח תכלת להגנת המידע באופן ידני</span><span class="sxs-lookup"><span data-stu-id="f34c0-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="f34c0-132">כדי להתקין באופן ידני את לקוח AIP:</span><span class="sxs-lookup"><span data-stu-id="f34c0-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="f34c0-133">**הורדAzinfoProtection_UL.exe** [ממרכז ההורדות של Microsoft](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="f34c0-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="f34c0-134">באפשרותך לוודא שההתקנה פעלה על-ידי הצגת מסמך Word ובדיקה שהאפשרות **רגישות** זמינה בכרטיסיה **בית** .</span><span class="sxs-lookup"><span data-stu-id="f34c0-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="f34c0-135">![הרשימה הנפתחת של הכרטיסיה ' הגנה ' במסמך Word.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="f34c0-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="f34c0-136">לקבלת מידע נוסף, ראה [התקנת הלקוח](/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="f34c0-136">For more information, see [Install the client](/azure/information-protection/infoprotect-tutorial-step3).</span></span>