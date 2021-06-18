---
title: אימות הגדרות הגנה על אפליקציות עבור Windows 10 אישיים
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
description: למד כיצד לוודא שהגדרות Microsoft 365 הגנה על אפליקציות עסקיות השפיעו על מכשירי Windows 10 המשתמשים שלך.
ms.openlocfilehash: 464a246a0da65dcffeb70946287ce4fa0e67ae7c
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925258"
---
# <a name="validate-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="fa13d-103">אימות הגדרות הגנה על מכשיר עבור Windows 10 אישיים</span><span class="sxs-lookup"><span data-stu-id="fa13d-103">Validate device protection settings for Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="fa13d-104">ודא שמדיניות Windows 10 מוגדרת</span><span class="sxs-lookup"><span data-stu-id="fa13d-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="fa13d-105">לאחר הגדרת [מדיניות מכשירים,](protection-settings-for-windows-10-pcs.md)ייתכן שיקח עד כמה שעות עד שהמדיניות תיתוקף במכשירים של המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="fa13d-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="fa13d-106">באפשרותך לאשר שמדיניות זו השפיעה על-ידי Windows הגדרות שונים במכשירים של המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="fa13d-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="fa13d-107">מאחר שהמשתמשים לא יוכלו לשנות את הגדרות Windows עדכון אנטי-וירוס של Windows Defender במכשירי Windows 10 שלהם, אפשרויות רבות יהיו באפור.</span><span class="sxs-lookup"><span data-stu-id="fa13d-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="fa13d-108">עבור אל **הגדרות** \> **עדכון אבטחה &amp; Windows** \> **אפשרויות עדכון** \> **מחדש ואשר** שכל ההגדרות מופיעות באפור.</span><span class="sxs-lookup"><span data-stu-id="fa13d-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![כל אפשרויות ההפעלה מחדש מופיעות באפור.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="fa13d-110">עבור אל **הגדרות** \> **עדכון &amp; אבטחה** Windows \> **אפשרויות** מתקדמות \> **ואשר** שכל ההגדרות מופיעות באפור.</span><span class="sxs-lookup"><span data-stu-id="fa13d-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Windows אפשרויות עדכונים מתקדמים מופיעות באפור.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="fa13d-112">עבור אל **הגדרות** \> **עדכון אבטחה &amp; Windows** \> **אפשרויות מתקדמות** \> **בחר** כיצד \> **ישלחו עדכונים**.</span><span class="sxs-lookup"><span data-stu-id="fa13d-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="fa13d-113">אשר כי באפשרותך לראות את ההודעה (באדום) שהגדרות מסוימות מוסתרות או מנוהלות על-ידי הארגון שלך, וכל האפשרויות מופיעות באפור.</span><span class="sxs-lookup"><span data-stu-id="fa13d-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![בחר כיצד הדף מועבר מציין שההגדרות מוסתרות או מנוהלות על-ידי הארגון שלך.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="fa13d-115">כדי לפתוח את מרכז Windows Defender אבטחה, עבור **אל הגדרות** עדכון אבטחה Windows Defender לחץ על פתח את Windows Defender אבטחה מרכז האבטחה הגנה מפני הליכי משנה של \> **&amp;** \>  \>  \> **&amp;** \> **&amp; וירוסים הגדרות הגנה מפני איומים.**</span><span class="sxs-lookup"><span data-stu-id="fa13d-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="fa13d-116">ודא שכל האפשרויות מופיעות באפור.</span><span class="sxs-lookup"><span data-stu-id="fa13d-116">Verify that all options are grayed out.</span></span> 
    
    ![הגדרות ההגנה מפני וירוסים ואיומים מופיעות באפור.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="fa13d-118">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="fa13d-118">Related Topics</span></span>

[<span data-ttu-id="fa13d-119">Microsoft 365 עבור תיעוד ומשאבים עסקיים</span><span class="sxs-lookup"><span data-stu-id="fa13d-119">Microsoft 365 for business documentation and resources</span></span>](./index.yml)
  
[<span data-ttu-id="fa13d-120">תחילת העבודה עם Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="fa13d-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="fa13d-121">ניהול Microsoft 365 לעסקים</span><span class="sxs-lookup"><span data-stu-id="fa13d-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="fa13d-122">קביעת תצורות של מכשירים עבור מחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="fa13d-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
