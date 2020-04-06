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
search.appverid:
- BCS160
- MET150
- MOE150
description: למד כיצד להגדיר מדיניות גישה מותנית עבור קמפיינים של Microsoft 365 כדי להוסיף אבטחה משמעותית.
ms.openlocfilehash: 26fadecc69486d7931dac069d8f53061592f397f
ms.sourcegitcommit: e525bcf073a61e1350484719a0c3ceb6ff0d8db1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/06/2020
ms.locfileid: "43153765"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="37185-103">הגדרת מדיניות גישה מותנית</span><span class="sxs-lookup"><span data-stu-id="37185-103">Set up Conditional Access policies</span></span>

<span data-ttu-id="37185-104">פריטי מדיניות [גישה מותנים](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) מוסיפים אבטחה משמעותית.</span><span class="sxs-lookup"><span data-stu-id="37185-104">[Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="37185-105">Microsoft מספקת מערכת של פריטי מדיניות של גישה מותנית בסיסית המומלצת עבור כל הלקוחות.</span><span class="sxs-lookup"><span data-stu-id="37185-105">Microsoft provides a set of baseline Conditional Access policies that are recommended for all customers.</span></span> <span data-ttu-id="37185-106">מדיניות בסיסית היא קבוצה של פריטי מדיניות מוגדרים מראש המסייעים להגן על ארגונים מפני התקפות נפוצות רבות.</span><span class="sxs-lookup"><span data-stu-id="37185-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="37185-107">התקפות נפוצות אלה יכולות לכלול תרסיס סיסמה, הפעלה חוזרת ודיוג.</span><span class="sxs-lookup"><span data-stu-id="37185-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="37185-108">מדיניות זו דורשת ממנהלים ומשתמשים להזין סוג שני של אימות (הנקרא אימות מרובה גורמים או משרד המשנה) כאשר מתקיימים תנאים מסוימים.</span><span class="sxs-lookup"><span data-stu-id="37185-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="37185-109">לדוגמה, אם משתמש נכנס ממדינה אחרת, ייתכן שהכניסה תיחשב כמסוכנת והמשתמש חייב לספק סוג נוסף של אימות.</span><span class="sxs-lookup"><span data-stu-id="37185-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="37185-110">כעת, מדיניות בסיסית כוללת את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="37185-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="37185-111">**דרוש למרכז המידע למנהלים** &ndash; מחייב אימות מרובה גורמים עבור תפקידי מנהל המערכת המיוחסים ביותר, כולל מנהל כללי.</span><span class="sxs-lookup"><span data-stu-id="37185-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="37185-112">&ndash; **הגנת משתמש קצה** מחייבת אימות מרובה גורמים עבור משתמשים רק כאשר כניסה היא מסוכנת.</span><span class="sxs-lookup"><span data-stu-id="37185-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="37185-113">&ndash; **חסום אימות מדור קודם** עבור יישומי לקוח ישנים ויישומים חדשים מסוימים אינם משתמשים בפרוטוקולי אימות חדשים ומאובטחים יותר.</span><span class="sxs-lookup"><span data-stu-id="37185-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="37185-114">יישומים ישנים אלה יכולים לעקוף מדיניות גישה מותנית ולקבל גישה בלתי מורשית לסביבה שלך.</span><span class="sxs-lookup"><span data-stu-id="37185-114">These older apps can bypass Conditional Access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="37185-115">מדיניות זו חוסמת את הגישה מלקוחות שאינם תומכים בגישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="37185-115">This policy blocks access from clients that don't support Conditional Access.</span></span> 
- <span data-ttu-id="37185-116">דרוש לתואר &ndash; **שירותי משרד לניהול השירות** מחייב אימות רב-גורמי לגישה לכלי ניהול, כולל פורטל התכלת (היכן שתקבע את תצורת מדיניות בסיסית).</span><span class="sxs-lookup"><span data-stu-id="37185-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="37185-117">Microsoft ממליצה להפוך את כל פריטי המדיניות הבסיסיים לזמינים.</span><span class="sxs-lookup"><span data-stu-id="37185-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="37185-118">לאחר שפריטי מדיניות אלה מופעלים, מנהלים ומשתמשים יתבקשו להירשם לאימות מרובה הגורמים התכלת.</span><span class="sxs-lookup"><span data-stu-id="37185-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="37185-119">לקבלת מידע נוסף אודות פריטי מדיניות אלה, ראה [מהן מדיניות בסיסית](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="37185-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="37185-120">הגדרת מדיניות בסיסית</span><span class="sxs-lookup"><span data-stu-id="37185-120">Set up baseline policies</span></span>

1. <span data-ttu-id="37185-121">עבור אל [הפורטל התכלת](https://portal.azure.com)ונווט אל **הגישה המותנית**של **active Directory** \> .</span><span class="sxs-lookup"><span data-stu-id="37185-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="37185-122">פריטי המדיניות הבסיסיים מפורטים בדף.</span><span class="sxs-lookup"><span data-stu-id="37185-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="37185-123">![דף המפרט פריטי מדיניות בסיסית עבור גישה מותנית.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="37185-123">![Page that lists baseline policies for Conditional Access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="37185-124">עיין בהנחיות הספציפיות הבאות עבור כל מדיניות:</span><span class="sxs-lookup"><span data-stu-id="37185-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="37185-125">דרוש את משרד התואר למנהלים</span><span class="sxs-lookup"><span data-stu-id="37185-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="37185-126">דרוש משרד למשתמש</span><span class="sxs-lookup"><span data-stu-id="37185-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="37185-127">חסום אימות מדור קודם</span><span class="sxs-lookup"><span data-stu-id="37185-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="37185-128">דרוש תואר שירות למען ניהול השירות</span><span class="sxs-lookup"><span data-stu-id="37185-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="37185-129">באפשרותך להגדיר פריטי מדיניות נוספים רבים, כגון דרישת יישומי לקוח מאושרים.</span><span class="sxs-lookup"><span data-stu-id="37185-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="37185-130">לקבלת מידע נוסף, עיין [בתיעוד של גישה מותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="37185-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
