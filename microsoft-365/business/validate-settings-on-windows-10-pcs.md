---
title: אימות הגדרות הגנה של אפליקציות במחשבי Windows 10
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: למד כיצד לוודא שהגדרות ההגנה על אפליקציה של Microsoft 365 לעסקים השפיעו על מכשירי Windows 10 של המשתמשים שלך.
ms.openlocfilehash: fcb463fd98f692f7d4802689e0c03fe4e3e648a1
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579841"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="636bf-103">אימות הגדרות הגנה על מכשיר במחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="636bf-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="636bf-104">ודא שמדיניות המכשיר של Windows 10 מוגדרת</span><span class="sxs-lookup"><span data-stu-id="636bf-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="636bf-105">לאחר הגדרת [מדיניות מכשירים,](protection-settings-for-windows-10-pcs.md)ייתכן שיקח עד כמה שעות עד שהמדיניות תיתוקף במכשירים של המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="636bf-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="636bf-106">באפשרותך לאשר שמדיניות זו השפיעה על-ידי התסתכלות על מסכי הגדרות Windows השונים במכשירים של המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="636bf-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="636bf-107">מאחר שהמשתמשים לא יוכלו לשנות את הגדרות האנטי-וירוס של Windows Update ו- Windows Defender במכשירי Windows 10 שלהם, אפשרויות רבות יהיו באפור.</span><span class="sxs-lookup"><span data-stu-id="636bf-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="636bf-108">עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **אפשרויות הפעלה מחדש** של Windows Update \>  ואשר שכל ההגדרות מופיעות באפור.</span><span class="sxs-lookup"><span data-stu-id="636bf-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![כל אפשרויות ההפעלה מחדש מופיעות באפור.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="636bf-110">עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **אפשרויות Windows Update** \> **Advanced** ואשר שכל ההגדרות מופיעות באפור.</span><span class="sxs-lookup"><span data-stu-id="636bf-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![אפשרויות העדכונים המתקדמות של Windows מופיעות באפור.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="636bf-112">עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **אפשרויות מתקדמות של Windows Update** \>  \> **בחר כיצד ישלחו עדכונים.**</span><span class="sxs-lookup"><span data-stu-id="636bf-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="636bf-113">אשר כי באפשרותך לראות את ההודעה (באדום) שהגדרות מסוימות מוסתרות או מנוהלות על-ידי הארגון שלך, וכל האפשרויות מופיעות באפור.</span><span class="sxs-lookup"><span data-stu-id="636bf-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![בחר כיצד הדף מועבר מציין שההגדרות מוסתרות או מנוהלות על-ידי הארגון שלך.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="636bf-115">כדי לפתוח את מרכז האבטחה של Windows Defender, עבור **אל** הגדרות עדכון אבטחה \> **&amp;** Windows \> **Defender, לחץ** על פתח את הגדרות ההגנה מפני איומים מפני וירוסים של מרכז האבטחה של Windows \>  \> **&amp;** \> **&amp;** Defender.</span><span class="sxs-lookup"><span data-stu-id="636bf-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="636bf-116">ודא שכל האפשרויות מופיעות באפור.</span><span class="sxs-lookup"><span data-stu-id="636bf-116">Verify that all options are grayed out.</span></span> 
    
    ![הגדרות ההגנה מפני וירוסים ואיומים מופיעות באפור.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="636bf-118">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="636bf-118">Related Topics</span></span>

[<span data-ttu-id="636bf-119">תיעוד ומשאבים של Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="636bf-119">Microsoft 365 for business documentation and resources</span></span>](./index.yml)
  
[<span data-ttu-id="636bf-120">תחילת העבודה עם Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="636bf-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="636bf-121">ניהול Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="636bf-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="636bf-122">קביעת תצורות של מכשירים עבור מחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="636bf-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
