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
ms.openlocfilehash: d7c9cfee2ef00e4ebe231a28ccca185c10f53c6b
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403017"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="f4725-103">הגדרת מדיניות גישה מותנית</span><span class="sxs-lookup"><span data-stu-id="f4725-103">Set up conditional access policies</span></span>

<span data-ttu-id="f4725-104">פריטי מדיניות [גישה מותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) מוסיפים אבטחה משמעותית.</span><span class="sxs-lookup"><span data-stu-id="f4725-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="f4725-105">Microsoft מספקת מערכת של פריטי מדיניות גישה מותנית בסיסית המומלצת עבור כל הלקוחות.</span><span class="sxs-lookup"><span data-stu-id="f4725-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="f4725-106">מדיניות בסיסית היא קבוצה של פריטי מדיניות מוגדרים מראש המסייעים להגן על ארגונים מפני התקפות נפוצות רבות.</span><span class="sxs-lookup"><span data-stu-id="f4725-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="f4725-107">התקפות נפוצות אלה יכולות לכלול תרסיס סיסמה, הפעלה חוזרת ודיוג.</span><span class="sxs-lookup"><span data-stu-id="f4725-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="f4725-108">מדיניות זו דורשת ממנהלים ומשתמשים להזין סוג שני של אימות (הנקרא אימות מרובה גורמים או משרד המשנה) כאשר מתקיימים תנאים מסוימים.</span><span class="sxs-lookup"><span data-stu-id="f4725-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="f4725-109">לדוגמה, אם משתמש נכנס ממדינה אחרת, ייתכן שהכניסה תיחשב כמסוכנת והמשתמש חייב לספק סוג נוסף של אימות.</span><span class="sxs-lookup"><span data-stu-id="f4725-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="f4725-110">כעת, מדיניות בסיסית כוללת את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="f4725-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="f4725-111">**דרוש את משרד התואר למנהלים** &ndash; מחייב אימות רב-גורמי עבור תפקידי מנהל המערכת המיוחסים ביותר, כולל מנהל כללי.</span><span class="sxs-lookup"><span data-stu-id="f4725-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="f4725-112">הגנת משתמש **קצה** &ndash; מחייב אימות רב-גורמי עבור משתמשים רק כאשר כניסה מסוכנת.</span><span class="sxs-lookup"><span data-stu-id="f4725-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="f4725-113">**חסום אימות** &ndash; מדור קודם יישומי לקוח ישנים ויישומים חדשים מסוימים אינם משתמשים בפרוטוקולי אימות חדשים ומאובטחים יותר.</span><span class="sxs-lookup"><span data-stu-id="f4725-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="f4725-114">יישומים ישנים אלה יכולים לעקוף מדיניות גישה מותנית ולהשיג גישה בלתי מורשית לסביבה שלך.</span><span class="sxs-lookup"><span data-stu-id="f4725-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="f4725-115">מדיניות זו חוסמת את הגישה מלקוחות שאינם תומכים בגישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="f4725-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="f4725-116">**דרוש משרד לניהול** &ndash; שירות מחייב אימות רב-גורמי לקבלת גישה לכלי ניהול, כולל פורטל תכלת (שם תקבע את תצורת מדיניות בסיסית).</span><span class="sxs-lookup"><span data-stu-id="f4725-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="f4725-117">Microsoft ממליצה להפוך את כל פריטי המדיניות הבסיסיים לזמינים.</span><span class="sxs-lookup"><span data-stu-id="f4725-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="f4725-118">לאחר שפריטי מדיניות אלה מופעלים, מנהלים ומשתמשים יתבקשו להירשם לאימות מרובה הגורמים התכלת.</span><span class="sxs-lookup"><span data-stu-id="f4725-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="f4725-119">לקבלת מידע נוסף אודות פריטי מדיניות אלה, ראה [מהן מדיניות בסיסית](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="f4725-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="f4725-120">הגדרת מדיניות בסיסית</span><span class="sxs-lookup"><span data-stu-id="f4725-120">Set up baseline policies</span></span>

1. <span data-ttu-id="f4725-121">עבור [לפורטל התכלת](https://portal.azure.com)ונווט אל **Azure Active Directory** \> **הגישה המותנית**של active Directory.</span><span class="sxs-lookup"><span data-stu-id="f4725-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="f4725-122">פריטי המדיניות הבסיסיים מפורטים בדף.</span><span class="sxs-lookup"><span data-stu-id="f4725-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="f4725-123">![דף המפרט מדיניות בסיסית עבור גישה מותנית.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="f4725-123">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="f4725-124">עיין בהנחיות הספציפיות הבאות עבור כל מדיניות:</span><span class="sxs-lookup"><span data-stu-id="f4725-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="f4725-125">דרוש את משרד התואר למנהלים</span><span class="sxs-lookup"><span data-stu-id="f4725-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="f4725-126">דרוש משרד למשתמש</span><span class="sxs-lookup"><span data-stu-id="f4725-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="f4725-127">חסום אימות מדור קודם</span><span class="sxs-lookup"><span data-stu-id="f4725-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="f4725-128">דרוש תואר שירות למען ניהול השירות</span><span class="sxs-lookup"><span data-stu-id="f4725-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="f4725-129">באפשרותך להגדיר פריטי מדיניות נוספים רבים, כגון דרישת יישומי לקוח מאושרים.</span><span class="sxs-lookup"><span data-stu-id="f4725-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="f4725-130">לקבלת מידע נוסף, עיין [בתיעוד של גישה מותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="f4725-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
