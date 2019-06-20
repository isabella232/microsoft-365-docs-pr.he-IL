---
title: להגדיר פריטי מדיניות של גישה מותנית עבור קמפיינים Microsoft 365
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
search.appverid:
- BCS160
- MET150
- MOE150
description: למד כיצד להגדיר פריטי מדיניות של גישה מותנית עבור קמפיינים 365 של Microsoft.
ms.openlocfilehash: 7d8e1f16019d151478aae57b1593b0e0758e5b19
ms.sourcegitcommit: 7e46db0b35c188ee6a7b40ab3eb2d76ff6c101c5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/19/2019
ms.locfileid: "35086335"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="d789c-103">להגדיר פריטי מדיניות של גישה מותנית</span><span class="sxs-lookup"><span data-stu-id="d789c-103">Set up conditional access policies</span></span>

<span data-ttu-id="d789c-104">פריטי מדיניות של [גישה מותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) להוסיף אבטחה נוספת substancial.</span><span class="sxs-lookup"><span data-stu-id="d789c-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="d789c-105">Microsoft מספקת קבוצה של פריטי מדיניות של גישה מותנית בסיסית המומלצים עבור כל הלקוחות.</span><span class="sxs-lookup"><span data-stu-id="d789c-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="d789c-106">מדיניות בסיסית היא ערכה של מדיניות מוגדרת מראש המסייעות בהגנה על ארגונים מפני התקפות נפוצות רבות.</span><span class="sxs-lookup"><span data-stu-id="d789c-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="d789c-107">התקפות נפוצים אלה יכולים לכלול התזה סיסמה, replay ודיוג.</span><span class="sxs-lookup"><span data-stu-id="d789c-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="d789c-108">פריטי מדיניות אלה דורשים מנהלים ומשתמשים להזנת טופס שני של אימות (נקרא אימות רב-גורמי או MFA) כאשר תנאים מסוימים מתקיימים.</span><span class="sxs-lookup"><span data-stu-id="d789c-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="d789c-109">לדוגמה, אם משתמש הכניסה ממדינה אחרת, הכניסה עשויות להיחשב מסוכן ולחץ על המשתמש לספק טופס נוסף של אימות.</span><span class="sxs-lookup"><span data-stu-id="d789c-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="d789c-110">כעת, מדיניות בסיסית כוללות:</span><span class="sxs-lookup"><span data-stu-id="d789c-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="d789c-111">**דרוש MFA עבור מנהלים** — דורש אימות מגורמים רבים עבור תפקידי מנהל מורשה ביותר, כולל מנהל כללי.</span><span class="sxs-lookup"><span data-stu-id="d789c-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="d789c-112">**הגנה על משתמש הקצה** — מחייב אימות מגורמים רבים עבור משתמשים רק בעת-הכניסה היא מסוכנת.</span><span class="sxs-lookup"><span data-stu-id="d789c-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="d789c-113">**אימות דור קודם של בלוק** -יישומים ישנים יותר של הלקוח ואת מספר יישומים חדשים אל תשתמש פרוטוקולי אימות חדשה יותר, בטוחה יותר.</span><span class="sxs-lookup"><span data-stu-id="d789c-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="d789c-114">יישומים ישנים אלה יכולים לעקוף פריטי מדיניות של גישה מותנית ולהשיג גישה לא מורשית לסביבה שלך.</span><span class="sxs-lookup"><span data-stu-id="d789c-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="d789c-115">זו מדיניות חוסם את הגישה מלקוחות שאינם תומכים גישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="d789c-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="d789c-116">**דרוש MFA עבור ניהול שירות** -דורש אימות מגורמים רבים עבור גישה לכלי ניהול, כולל פורטל תכלת הרקיע (בהם לקבוע תצורה של פריטי מדיניות בסיסית).</span><span class="sxs-lookup"><span data-stu-id="d789c-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="d789c-117">Microsoft ממליצה שתפעיל את כל פריטי מדיניות אלה בסיסית.</span><span class="sxs-lookup"><span data-stu-id="d789c-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="d789c-118">לאחר פריטי מדיניות אלה מופעלות, מנהלים ומשתמשים תתבקש לרשום עבור אימות תכלת הרקיע Multii-פקטור.</span><span class="sxs-lookup"><span data-stu-id="d789c-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="d789c-119">לקבלת מידע נוסף אודות מדיניות אלה, ראה [מהן מדיניות בסיסית](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="d789c-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="d789c-120">הגדרת מדיניות בסיסית</span><span class="sxs-lookup"><span data-stu-id="d789c-120">Set up baseline policies</span></span>

1. <span data-ttu-id="d789c-121">מעבר לפורטל [תכלת הרקיע](https://portal.azure.com)ולאחר מכן נווט אל **הספריה הפעילה תכלת הרקיע** \> **Access מותנה**.</span><span class="sxs-lookup"><span data-stu-id="d789c-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="d789c-122">מדיניות בסיסית מפורטים בדף.</span><span class="sxs-lookup"><span data-stu-id="d789c-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="d789c-123">![דף המפרט את מדיניות בסיסית עבור גישה מותנית.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="d789c-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="d789c-124">עיין בהוראות הספציפיות הבאות עבור כל מדיניות:</span><span class="sxs-lookup"><span data-stu-id="d789c-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="d789c-125">דרוש MFA עבור מנהלים</span><span class="sxs-lookup"><span data-stu-id="d789c-125">Require MFA for admins</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="d789c-126">MFA Reequire עבור משתמשים</span><span class="sxs-lookup"><span data-stu-id="d789c-126">Reequire MFA for users</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="d789c-127">אימות דור קודם של בלוק</span><span class="sxs-lookup"><span data-stu-id="d789c-127">Block legacy authentication</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="d789c-128">דרוש MFA עבור ניהול שירות</span><span class="sxs-lookup"><span data-stu-id="d789c-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="d789c-129">באפשרותך להגדיר מדיניות נוספים רבים, כגון דרישת לקוח מאושרת apps.</span><span class="sxs-lookup"><span data-stu-id="d789c-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="d789c-130">עיין [בתיעוד Access מותנה](https://docs.microsoft.com/azure/active-directory/conditional-access/) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="d789c-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>