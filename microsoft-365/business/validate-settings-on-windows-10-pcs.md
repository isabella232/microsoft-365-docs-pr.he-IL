---
title: אימות הגדרות הגנה של אפליקציות במחשבי Windows 10
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: למד כיצד לאמת את הגדרות הגנת היישום העסקי של Microsoft 365 בהתקני Windows 10.
ms.openlocfilehash: 5fed2278856f40233b142d3c7c4bc623e3777799
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575467"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="6ab4d-103">אימות הגדרות הגנת התקן במחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="6ab4d-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="6ab4d-104">ודא שמדיניות ההתקנים של Windows 10 מוגדרת</span><span class="sxs-lookup"><span data-stu-id="6ab4d-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="6ab4d-105">לאחר [הגדרת פריטי מדיניות של התקנים](protection-settings-for-windows-10-pcs.md), המדיניות עשויה להימשך שעות ספורות כדי שהמדיניות ייכנסו לתוקף בהתקני המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="6ab4d-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="6ab4d-106">באפשרותך לאשר שהמדיניות השפיעה על-ידי התבוננות במסכים שונים של הגדרות Windows בהתקני המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="6ab4d-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="6ab4d-107">מכיוון שהמשתמשים לא יוכלו לשנות את הגדרות windows Update ו-Windows Defender Antivirus בהתקני Windows 10 שלהם, הרבה אפשרויות אלה יהיה מאפיר.</span><span class="sxs-lookup"><span data-stu-id="6ab4d-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, a lot of those options will be greyed out.</span></span>
  
1. <span data-ttu-id="6ab4d-108">עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **של Windows עדכון** \> **אפשרויות הפעלה** ולוודא כי כל ההגדרות מאפיר.</span><span class="sxs-lookup"><span data-stu-id="6ab4d-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are greyed out.</span></span> 
    
    ![כל האפשרויות הפעלה מחדש מאפיר.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="6ab4d-110">עבור אל **הגדרות** \> \*\* &amp; עדכון אבטחה\*\* \> **Windows עדכן** \> **אפשרויות מתקדמות** ולאשר כי כל ההגדרות מאפיר.</span><span class="sxs-lookup"><span data-stu-id="6ab4d-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are greyed out.</span></span> 
    
    ![אפשרויות העדכונים המתקדמים של Windows כולן החוצה.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="6ab4d-112">עבור אל **הגדרות** \> \*\* &amp; עדכון אבטחה\*\* \> **של Windows update** \> **אפשרויות** \> **מתקדמות בחר את אופן המשלוח של עדכונים**.</span><span class="sxs-lookup"><span data-stu-id="6ab4d-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="6ab4d-113">ודא שאתה יכול לראות את ההודעה (באדום) שההגדרות מסוימות מוסתרות או מנוהלות על-ידי הארגון שלך, וכל האפשרויות מאפיר.</span><span class="sxs-lookup"><span data-stu-id="6ab4d-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are greyed out.</span></span>
    
    ![בחר כיצד עדכונים מועברים לדף מציין שההגדרות מוסתרות או מנוהלות על-ידי הארגון שלך.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="6ab4d-115">כדי לפתוח את מרכז האבטחה של Windows defender, עבור אל **הגדרות** \> \*\* &amp; עדכון אבטחה\*\* \> **windows defender** \> לחץ על **פתח windows Defender אבטחה מרכז** \> **וירוס &amp; הליך משנה הגנת** \> **וירוס &amp; איום הגדרות הגנה**.</span><span class="sxs-lookup"><span data-stu-id="6ab4d-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="6ab4d-116">ודא שכל האפשרויות מאפיר.</span><span class="sxs-lookup"><span data-stu-id="6ab4d-116">Verify that all options are greyed out.</span></span> 
    
    ![הגדרות הגנת הוירוס והאיום מאפיר.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="6ab4d-118">נושאים קרובים</span><span class="sxs-lookup"><span data-stu-id="6ab4d-118">Related Topics</span></span>

[<span data-ttu-id="6ab4d-119">תיעוד ומשאבים עבור Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="6ab4d-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="6ab4d-120">תחילת העבודה עם Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="6ab4d-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="6ab4d-121">ניהול של Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="6ab4d-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="6ab4d-122">קביעת תצורות של מכשירים עבור מחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="6ab4d-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

