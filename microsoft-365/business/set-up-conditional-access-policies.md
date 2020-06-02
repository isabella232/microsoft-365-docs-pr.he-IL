---
title: הגדרת מדיניות גישה מותנית עבור קמפיינים של Microsoft 365
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: למד כיצד להגדיר מדיניות גישה מותנית עבור קמפיינים של Microsoft 365 כדי להוסיף אבטחה משמעותית.
ms.openlocfilehash: 58ee760877ee2fd7e53ef9463242657ab66a2b6e
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470646"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="59fa3-103">הגדרת מדיניות גישה מותנית</span><span class="sxs-lookup"><span data-stu-id="59fa3-103">Set up conditional access policies</span></span>

<span data-ttu-id="59fa3-104">מאמר זה חל על 365 עסקים Premium של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="59fa3-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="59fa3-105">פריטי מדיניות [גישה מותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) מוסיפים אבטחה משמעותית.</span><span class="sxs-lookup"><span data-stu-id="59fa3-105">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="59fa3-106">Microsoft מספקת מערכת של פריטי מדיניות גישה מותנית בסיסית המומלצת עבור כל הלקוחות.</span><span class="sxs-lookup"><span data-stu-id="59fa3-106">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="59fa3-107">מדיניות בסיסית היא קבוצה של פריטי מדיניות מוגדרים מראש המסייעים להגן על ארגונים מפני התקפות נפוצות רבות.</span><span class="sxs-lookup"><span data-stu-id="59fa3-107">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="59fa3-108">התקפות נפוצות אלה יכולות לכלול תרסיס סיסמה, הפעלה חוזרת ודיוג.</span><span class="sxs-lookup"><span data-stu-id="59fa3-108">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="59fa3-109">מדיניות זו דורשת ממנהלים ומשתמשים להזין סוג שני של אימות (הנקרא אימות מרובה גורמים או משרד המשנה) כאשר מתקיימים תנאים מסוימים.</span><span class="sxs-lookup"><span data-stu-id="59fa3-109">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="59fa3-110">לדוגמה, אם משתמש נכנס ממדינה אחרת, ייתכן שהכניסה תיחשב כמסוכנת והמשתמש חייב לספק סוג נוסף של אימות.</span><span class="sxs-lookup"><span data-stu-id="59fa3-110">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="59fa3-111">כעת, מדיניות בסיסית כוללת את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="59fa3-111">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="59fa3-112">**דרוש את משרד התואר למנהלים** &ndash; מחייב אימות רב-גורמי עבור תפקידי מנהל המערכת המיוחסים ביותר, כולל מנהל כללי.</span><span class="sxs-lookup"><span data-stu-id="59fa3-112">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="59fa3-113">הגנת משתמש **קצה** &ndash; מחייב אימות רב-גורמי עבור משתמשים רק כאשר כניסה מסוכנת.</span><span class="sxs-lookup"><span data-stu-id="59fa3-113">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="59fa3-114">**חסום אימות** &ndash; מדור קודם יישומי לקוח ישנים ויישומים חדשים מסוימים אינם משתמשים בפרוטוקולי אימות חדשים ומאובטחים יותר.</span><span class="sxs-lookup"><span data-stu-id="59fa3-114">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="59fa3-115">יישומים ישנים אלה יכולים לעקוף מדיניות גישה מותנית ולהשיג גישה בלתי מורשית לסביבה שלך.</span><span class="sxs-lookup"><span data-stu-id="59fa3-115">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="59fa3-116">מדיניות זו חוסמת את הגישה מלקוחות שאינם תומכים בגישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="59fa3-116">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="59fa3-117">**דרוש משרד לניהול** &ndash; שירות מחייב אימות רב-גורמי לקבלת גישה לכלי ניהול, כולל פורטל תכלת (שם תקבע את תצורת מדיניות בסיסית).</span><span class="sxs-lookup"><span data-stu-id="59fa3-117">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="59fa3-118">Microsoft ממליצה להפוך את כל פריטי המדיניות הבסיסיים לזמינים.</span><span class="sxs-lookup"><span data-stu-id="59fa3-118">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="59fa3-119">לאחר שפריטי מדיניות אלה מופעלים, מנהלים ומשתמשים יתבקשו להירשם לאימות מרובה הגורמים התכלת.</span><span class="sxs-lookup"><span data-stu-id="59fa3-119">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="59fa3-120">לקבלת מידע נוסף אודות פריטי מדיניות אלה, ראה [מהן מדיניות בסיסית](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="59fa3-120">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="59fa3-121">הגדרת מדיניות בסיסית</span><span class="sxs-lookup"><span data-stu-id="59fa3-121">Set up baseline policies</span></span>

1. <span data-ttu-id="59fa3-122">עבור [לפורטל התכלת](https://portal.azure.com)ונווט אל **Azure Active Directory** \> **הגישה המותנית**של active Directory.</span><span class="sxs-lookup"><span data-stu-id="59fa3-122">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="59fa3-123">פריטי המדיניות הבסיסיים מפורטים בדף.</span><span class="sxs-lookup"><span data-stu-id="59fa3-123">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="59fa3-124">![דף המפרט מדיניות בסיסית עבור גישה מותנית.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="59fa3-124">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="59fa3-125">עיין בהנחיות הספציפיות הבאות עבור כל מדיניות:</span><span class="sxs-lookup"><span data-stu-id="59fa3-125">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="59fa3-126">דרוש את משרד התואר למנהלים</span><span class="sxs-lookup"><span data-stu-id="59fa3-126">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="59fa3-127">דרוש משרד למשתמש</span><span class="sxs-lookup"><span data-stu-id="59fa3-127">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="59fa3-128">חסום אימות מדור קודם</span><span class="sxs-lookup"><span data-stu-id="59fa3-128">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="59fa3-129">דרוש תואר שירות למען ניהול השירות</span><span class="sxs-lookup"><span data-stu-id="59fa3-129">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="59fa3-130">באפשרותך להגדיר פריטי מדיניות נוספים רבים, כגון דרישת יישומי לקוח מאושרים.</span><span class="sxs-lookup"><span data-stu-id="59fa3-130">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="59fa3-131">לקבלת מידע נוסף, עיין [בתיעוד של גישה מותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="59fa3-131">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
