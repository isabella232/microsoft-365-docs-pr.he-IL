---
title: אימות הגדרות הגנה של אפליקציות במחשבי Windows 10
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: למד כיצד לאמת את הגדרות ההגנה app עסקיים 365 Microsoft ב- Windows 10 התקנים.
ms.openlocfilehash: 5ab91d65fa7bd40ebc118df217c9711b7bbfe7a4
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32286733"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="d730e-103">אימות הגדרות הגנה התקן במחשבים 10 חלונות</span><span class="sxs-lookup"><span data-stu-id="d730e-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="d730e-104">ודא כי מדיניות התקן Windows 10 מוגדרות</span><span class="sxs-lookup"><span data-stu-id="d730e-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="d730e-105">לאחר [הגדרת פריטי מדיניות של התקנים](protection-settings-for-windows-10-pcs.md), עשוי להימשך עד מספר שעות עבור המדיניות ייכנסו לתוקף במכשירים של המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="d730e-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="d730e-106">באפשרותך לאשר למדיניות ארך אפקט על-ידי התבוננות מסכי הגדרות Windows שונים במכשירים של המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="d730e-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="d730e-107">מאחר למשתמשים לא תהיה אפשרות לשנות את הגדרות Windows Update ו- Windows Defender וירוס בהתקנים שלהם Windows 10, מספר רב של אפשרויות אלה יעומעמו.</span><span class="sxs-lookup"><span data-stu-id="d730e-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, a lot of those options will be greyed out.</span></span>
  
1. <span data-ttu-id="d730e-108">עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **עדכון Windows** \> **אפשרויות הפעלה מחדש** ואשר כל ההגדרות הם greyed החוצה.</span><span class="sxs-lookup"><span data-stu-id="d730e-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are greyed out.</span></span> 
    
    ![כל האפשרויות מחדש הם greyed החוצה.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="d730e-110">עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **עדכון Windows** \> **אפשרויות מתקדמות** ואשר כל ההגדרות הם greyed החוצה.</span><span class="sxs-lookup"><span data-stu-id="d730e-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are greyed out.</span></span> 
    
    ![אפשרויות מתקדמות של Windows של עדכונים הם כל greyed החוצה.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="d730e-112">עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **עדכון Windows** \> **אפשרויות מתקדמות** \> **בחר כיצד העדכונים יועברו**.</span><span class="sxs-lookup"><span data-stu-id="d730e-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="d730e-113">ודא כי באפשרותך לראות את ההודעה (באדום) הגדרות מסוימות הן מוסתרות או מנוהל על-ידי הארגון שלך, ולא כל האפשרויות הם greyed החוצה.</span><span class="sxs-lookup"><span data-stu-id="d730e-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are greyed out.</span></span>
    
    ![בחר כיצד מועברים עדכוני דף מציין הגדרות הן מוסתרות או מנוהל על-ידי הארגון שלך.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="d730e-115">כדי לפתוח את מרכז האבטחה של Windows Defender, עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **Windows Defender** \> לחץ על **פתח את Windows Defender מרכז האבטחה** \> **וירוס &amp; משנה (thread) הגנה** \> **וירוס &amp; איום הגדרות הגנה**.</span><span class="sxs-lookup"><span data-stu-id="d730e-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="d730e-116">ודא כי כל האפשרויות הם greyed החוצה.</span><span class="sxs-lookup"><span data-stu-id="d730e-116">Verify that all options are greyed out.</span></span> 
    
    ![הגדרות ההגנה מפני וירוסים ותוכנות איום הם greyed החוצה.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="d730e-118">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="d730e-118">Related Topics</span></span>

[<span data-ttu-id="d730e-119">תיעוד ומשאבים עבור Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="d730e-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="d730e-120">תחילת העבודה עם Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="d730e-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="d730e-121">ניהול של Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="d730e-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="d730e-122">קביעת תצורות של מכשירים עבור מחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="d730e-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

