---
title: הגדרת מדיניות גישה מותנית עבור קמפיינים של Microsoft 365
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
search.appverid:
- BCS160
- MET150
- MOE150
description: למד כיצד להגדיר מדיניות גישה מותנית עבור קמפיינים של Microsoft 365.
ms.openlocfilehash: 31f3b7f3678671af3b5ca3947dec37041b226fac
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575637"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="0666f-103">הגדרת מדיניות גישה מותנית</span><span class="sxs-lookup"><span data-stu-id="0666f-103">Set up conditional access policies</span></span>

<span data-ttu-id="0666f-104">פריטי מדיניות [גישה מותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) מוסיפים אבטחה נוספת בחומר החומר.</span><span class="sxs-lookup"><span data-stu-id="0666f-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="0666f-105">Microsoft מספקת מערכת של פריטי מדיניות גישה מותנית בסיסית המומלצת עבור כל הלקוחות.</span><span class="sxs-lookup"><span data-stu-id="0666f-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="0666f-106">מדיניות בסיסית היא קבוצה של פריטי מדיניות מוגדרים מראש המסייעים להגן על ארגונים מפני התקפות נפוצות רבות.</span><span class="sxs-lookup"><span data-stu-id="0666f-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="0666f-107">התקפות נפוצות אלה יכולות לכלול תרסיס סיסמה, הפעלה חוזרת ודיוג.</span><span class="sxs-lookup"><span data-stu-id="0666f-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="0666f-108">מדיניות זו דורשת ממנהלים ומשתמשים להזין סוג שני של אימות (הנקרא אימות מרובה גורמים או משרד המשנה) כאשר מתקיימים תנאים מסוימים.</span><span class="sxs-lookup"><span data-stu-id="0666f-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="0666f-109">לדוגמה, אם משתמש נכנס ממדינה אחרת, ייתכן שהכניסה תיחשב כמסוכנת והמשתמש חייב לספק סוג נוסף של אימות.</span><span class="sxs-lookup"><span data-stu-id="0666f-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="0666f-110">כעת, מדיניות בסיסית כוללת את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="0666f-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="0666f-111">**דרוש את משרד המידע למנהלים** – מחייב אימות רב-גורמי עבור תפקידי מנהל המערכת המיוחסים ביותר, כולל מנהל כללי.</span><span class="sxs-lookup"><span data-stu-id="0666f-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="0666f-112">**הגנת משתמש קצה** -מחייב אימות רב-גורמי עבור משתמשים רק כאשר כניסה מסוכנת.</span><span class="sxs-lookup"><span data-stu-id="0666f-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="0666f-113">**חסום אימות מדור קודם** — יישומי לקוח מבוגרים ויישומים חדשים מסוימים אינם משתמשים בפרוטוקולי אימות חדשים ומאובטחים יותר.</span><span class="sxs-lookup"><span data-stu-id="0666f-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="0666f-114">יישומים ישנים אלה יכולים לעקוף מדיניות גישה מותנית ולהשיג גישה בלתי מורשית לסביבה שלך.</span><span class="sxs-lookup"><span data-stu-id="0666f-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="0666f-115">מדיניות זו חוסמת את הגישה מלקוחות שאינם תומכים בגישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="0666f-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="0666f-116">**דרוש את משרד העבודה עבור ניהול השירות** – מחייב אימות רב-גורמי לגישה לכלי ניהול, כולל פורטל התכלת (שם תקבע מדיניות בסיסית).</span><span class="sxs-lookup"><span data-stu-id="0666f-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="0666f-117">Microsoft ממליצה להפוך את כל פריטי המדיניות הבסיסיים לזמינים.</span><span class="sxs-lookup"><span data-stu-id="0666f-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="0666f-118">לאחר שפריטי מדיניות אלה מופעלים, מנהלים ומשתמשים יתבקשו להירשם לאימות מרובה הגורמים התכלת.</span><span class="sxs-lookup"><span data-stu-id="0666f-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="0666f-119">לקבלת מידע נוסף אודות פריטי מדיניות אלה, ראה [מהן מדיניות בסיסית](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="0666f-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="0666f-120">הגדרת מדיניות בסיסית</span><span class="sxs-lookup"><span data-stu-id="0666f-120">Set up baseline policies</span></span>

1. <span data-ttu-id="0666f-121">עבור אל [הפורטל התכלת](https://portal.azure.com)ונווט אל **הגישה המותנית**של **active Directory** \> .</span><span class="sxs-lookup"><span data-stu-id="0666f-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="0666f-122">פריטי המדיניות הבסיסיים מפורטים בדף.</span><span class="sxs-lookup"><span data-stu-id="0666f-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="0666f-123">![דף המפרט מדיניות בסיסית עבור גישה מותנית.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="0666f-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="0666f-124">עיין בהנחיות הספציפיות הבאות עבור כל מדיניות:</span><span class="sxs-lookup"><span data-stu-id="0666f-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="0666f-125">דרוש את משרד התואר למנהלים</span><span class="sxs-lookup"><span data-stu-id="0666f-125">Require MFA for admins</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="0666f-126">דרוש משרד למשתמש</span><span class="sxs-lookup"><span data-stu-id="0666f-126">Require MFA for users</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="0666f-127">חסום אימות מדור קודם</span><span class="sxs-lookup"><span data-stu-id="0666f-127">Block legacy authentication</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="0666f-128">דרוש תואר שירות למען ניהול השירות</span><span class="sxs-lookup"><span data-stu-id="0666f-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="0666f-129">באפשרותך להגדיר פריטי מדיניות נוספים רבים, כגון דרישת יישומי לקוח מאושרים.</span><span class="sxs-lookup"><span data-stu-id="0666f-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="0666f-130">לקבלת מידע נוסף, עיין [בתיעוד הגישה המותנה](https://docs.microsoft.com/azure/active-directory/conditional-access/) .</span><span class="sxs-lookup"><span data-stu-id="0666f-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>