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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: למד כיצד לאמת את הגדרות ההגנה על אפליקציות של Microsoft 365 for business שהופעלו במכשירי Windows 10 של המשתמשים שלך.
ms.openlocfilehash: ff99b3a4fce49aebdb5c72f51e46678a7821e186
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912413"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="e2cc7-103">אימות הגדרות הגנה על מכשירים במחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="e2cc7-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="e2cc7-104">אימות ש-Windows 10 מדיניות התקן מוגדרים</span><span class="sxs-lookup"><span data-stu-id="e2cc7-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="e2cc7-105">לאחר [הגדרת מדיניות מכשירים](protection-settings-for-windows-10-pcs.md), ייתכן שיחלפו כמה שעות עד שהמדיניות תיכנס לתוקף של מכשירי משתמשים.</span><span class="sxs-lookup"><span data-stu-id="e2cc7-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="e2cc7-106">באפשרותך לוודא שהמדיניות השפיעה על-ידי התבוננות במסכים שונים של הגדרות Windows במכשירים של המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="e2cc7-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="e2cc7-107">מכיוון שהמשתמשים לא יוכלו לשנות את הגדרות windows Update ו-Windows Defender Antivirus במכשירי Windows 10 שלהם, אפשרויות רבות ייראו באפור.</span><span class="sxs-lookup"><span data-stu-id="e2cc7-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="e2cc7-108">עבור אל  \> **&amp;** \>  \> **אפשרויות הפעלה מחדש** של עדכון אבטחה עבור הגדרות Windows update ואשר שכל ההגדרות מעומעמות.</span><span class="sxs-lookup"><span data-stu-id="e2cc7-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![כל אפשרויות ההפעלה מחדש מעומעמות.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="e2cc7-110">עבור אל  \> האפשרויות המתקדמות של **עדכון &amp; אבטחה** עבור \> **Windows update** \>  ואשר שכל ההגדרות מעומעמות.</span><span class="sxs-lookup"><span data-stu-id="e2cc7-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![האפשרויות ' עדכונים מתקדמים ' של Windows מעומעמות.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="e2cc7-112">עבור אל  \> **&amp;** \> ' אפשרויות מתקדמות ' של עדכוני אבטחה **של Windows update Windows** \>  \> , **בחר כיצד יישלחו עדכונים**.</span><span class="sxs-lookup"><span data-stu-id="e2cc7-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="e2cc7-113">ודא שניתן לראות את ההודעה (באדום) שהגדרות מסוימות מוסתרות או מנוהלות על-ידי הארגון שלך, וכל האפשרויות מעומעמות.</span><span class="sxs-lookup"><span data-stu-id="e2cc7-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![בחר כיצד עדכונים מועברים בדף מציין שההגדרות מוסתרות או מנוהלות על-ידי הארגון שלך.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="e2cc7-115">כדי לפתוח את מרכז האבטחה של windows defender, עבור אל **הגדרות** \> **עדכון &amp; אבטחה** \> **של windows** defender \> לחץ על **פתח את windows defender מרכז** \> **האבטחה וירוסים וירוסים &amp; הגנה** על \> **&amp; הגדרות הגנה** מפני הגנה</span><span class="sxs-lookup"><span data-stu-id="e2cc7-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="e2cc7-116">ודא שכל האפשרויות מעומעמות.</span><span class="sxs-lookup"><span data-stu-id="e2cc7-116">Verify that all options are grayed out.</span></span> 
    
    ![הגדרות הגנה מפני וירוסים ואיומים מעומעמות.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="e2cc7-118">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="e2cc7-118">Related Topics</span></span>

[<span data-ttu-id="e2cc7-119">תיעוד ומשאבים של Microsoft 365 for business</span><span class="sxs-lookup"><span data-stu-id="e2cc7-119">Microsoft 365 for business documentation and resources</span></span>](./index.yml)
  
[<span data-ttu-id="e2cc7-120">תחילת העבודה עם Microsoft 365 for business</span><span class="sxs-lookup"><span data-stu-id="e2cc7-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="e2cc7-121">ניהול Microsoft 365 for business</span><span class="sxs-lookup"><span data-stu-id="e2cc7-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="e2cc7-122">קביעת תצורות של מכשירים עבור מחשבי Windows 10</span><span class="sxs-lookup"><span data-stu-id="e2cc7-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
