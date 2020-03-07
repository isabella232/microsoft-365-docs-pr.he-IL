---
title: אימות הגדרות הגנה של אפליקציות במחשבי Windows 10
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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: למד כיצד לוודא שהגדרות ההגנה של היישום Business 365 של Microsoft השפעתם על התקני Windows 10 של המשתמשים שלך.
ms.openlocfilehash: 47977f8d79eb6dbb2f4d087af8f8ad7da4313c61
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/07/2020
ms.locfileid: "42560679"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="8e920-103">אימות הגדרות הגנת התקן במחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="8e920-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="8e920-104">ודא שמדיניות ההתקנים של Windows 10 מוגדרת</span><span class="sxs-lookup"><span data-stu-id="8e920-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="8e920-105">לאחר [הגדרת פריטי מדיניות של התקנים](protection-settings-for-windows-10-pcs.md), המדיניות עשויה להימשך שעות ספורות כדי שהמדיניות ייכנסו לתוקף בהתקני המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="8e920-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="8e920-106">באפשרותך לאשר שהמדיניות השפיעה על-ידי התבוננות במסכים שונים של הגדרות Windows בהתקני המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="8e920-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="8e920-107">מאחר שהמשתמשים לא יוכלו לשנות את הגדרות windows Update ו-Windows Defender Antivirus בהתקני Windows 10 שלהם, אפשרויות רבות יופיעו באפור.</span><span class="sxs-lookup"><span data-stu-id="8e920-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="8e920-108">עבור אל **' הגדרות** \> \*\* &amp; עדכון אבטחה\*\* \> **של Windows עדכון** \> **אפשרויות הפעלה מחדש** ולוודא שכל ההגדרות אפורות.</span><span class="sxs-lookup"><span data-stu-id="8e920-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![כל האפשרויות הפעלה מחדש מאפורות.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="8e920-110">עבור אל **הגדרות** \> \*\* &amp; עדכון אבטחה\*\* \> **Windows עדכן** \> **אפשרויות מתקדמות** וודא כי כל ההגדרות אפורות.</span><span class="sxs-lookup"><span data-stu-id="8e920-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![אפשרויות העדכונים המתקדמים של Windows מאפורות כולן.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="8e920-112">עבור אל **הגדרות** \> \*\* &amp; עדכון אבטחה\*\* \> **של Windows update** \> **אפשרויות** \> **מתקדמות בחר את אופן המשלוח של עדכונים**.</span><span class="sxs-lookup"><span data-stu-id="8e920-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="8e920-113">ודא כי באפשרותך לראות את ההודעה (באדום) שההגדרות מסוימות מוסתרות או מנוהלות על-ידי הארגון שלך וכל האפשרויות מאפורות.</span><span class="sxs-lookup"><span data-stu-id="8e920-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![בחר כיצד עדכונים מועברים לדף מציין שההגדרות מוסתרות או מנוהלות על-ידי הארגון שלך.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="8e920-115">כדי לפתוח את מרכז האבטחה של Windows defender, עבור אל **הגדרות** \> \*\* &amp; עדכון אבטחה\*\* \> **windows defender** \> לחץ על **פתח windows Defender אבטחה מרכז** \> **וירוס &amp; הגנת הליך** \> הגנה \*\*איום וירוס &amp; \*\*.</span><span class="sxs-lookup"><span data-stu-id="8e920-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="8e920-116">ודא שכל האפשרויות מעומעמת.</span><span class="sxs-lookup"><span data-stu-id="8e920-116">Verify that all options are grayed out.</span></span> 
    
    ![הגדרות הגנת הווירוס והאיום מאפורות.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="8e920-118">נושאים קרובים</span><span class="sxs-lookup"><span data-stu-id="8e920-118">Related Topics</span></span>

[<span data-ttu-id="8e920-119">תיעוד ומשאבים עבור Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="8e920-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="8e920-120">תחילת העבודה עם Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="8e920-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="8e920-121">ניהול של Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="8e920-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="8e920-122">קביעת תצורות של מכשירים עבור מחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="8e920-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

