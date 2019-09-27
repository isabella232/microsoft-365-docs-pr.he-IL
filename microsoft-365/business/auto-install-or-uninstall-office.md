---
title: התקנה או הסרת התקנה אוטומטית של Office במכשירי Windows 10
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: cbc6bfe5-565a-4fb8-95f0-b06e7b74ac46
description: 'התקן או הסר התקנה של Office בהתקני Windows 10 ממרכז הניהול העסקי של Microsoft 365. '
ms.openlocfilehash: d82ab8292211d1adacba732922bf693dd2157ad6
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287534"
---
# <a name="automatically-install-or-uninstall-office-on-windows-10-devices"></a><span data-ttu-id="5a0c6-103">התקנה או הסרת התקנה אוטומטית של Office במכשירי Windows 10</span><span class="sxs-lookup"><span data-stu-id="5a0c6-103">Automatically install or uninstall Office on Windows 10 devices</span></span>

<span data-ttu-id="5a0c6-104">[![תווית כדי ליידע אותך שמרכז הניהול משתנה ובאפשרותך למצוא פרטים נוספים ב-aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="5a0c6-104">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="5a0c6-105">תוכל להתקין את Office במחשבי PC של Windows 10 בקלות ובמהירות ממרכז הניהול של Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="5a0c6-105">You can quickly and easily install Office to Windows 10 PCs from the Microsoft 365 Business admin center.</span></span>
  
<span data-ttu-id="5a0c6-106">כדי להבין כיצד זה עובד עם יישומי Office שהותקנו בעבר, קרא את [הכנה להתקנת לקוח של Office](prepare-for-office-client-deployment.md) לפני שתתחיל.</span><span class="sxs-lookup"><span data-stu-id="5a0c6-106">To understand how this works with previously installed Office apps, read [Prepare for Office client installation](prepare-for-office-client-deployment.md) before you get started.</span></span> 
  
## <a name="manage-office-deployments"></a><span data-ttu-id="5a0c6-107">ניהול פריסות של Office</span><span class="sxs-lookup"><span data-stu-id="5a0c6-107">Manage Office deployments</span></span>

1. <span data-ttu-id="5a0c6-108">היכנס ל[מרכז הניהול](https://aka.ms/bcsportal) עם אישורים של מנהל מערכת כללי.</span><span class="sxs-lookup"><span data-stu-id="5a0c6-108">Sign in to the [admin center](https://aka.ms/bcsportal) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="5a0c6-109">בכרטיס **מכשירים**, בחר **ניהול פריסת Office**.</span><span class="sxs-lookup"><span data-stu-id="5a0c6-109">On the **Devices** card, choose **Manage Office Deployment**.</span></span>
      <span data-ttu-id="5a0c6-110">אם אינך רואה את כרטיס **פעולות ההתקן** , בדף **הבית** של מרכז הניהול, לחץ על **הוסף** (+) כדי להוסיפו לבית המנהל שלך.</span><span class="sxs-lookup"><span data-stu-id="5a0c6-110">If you do not see the **Device actions** card, in the admin center **Home** page, click **Add** (+) to add it to your admin home.</span></span>
    
    ![Screenshot of the Devices card in the admin center](media/9982e784-dbf9-4a76-a159-bb3e2e5aa23f.png)
  
3. <span data-ttu-id="5a0c6-112">בחלונית **פריסת ניהול Office** שנפתחת, בחר **הוסף קבוצה** ולאחר מכן בחר את הקבוצות שברצונך להשתמש בהן.</span><span class="sxs-lookup"><span data-stu-id="5a0c6-112">On the **Manage Office deployment** pane that opens, choose **Add a group**, then select the groups you want use.</span></span>
    
4. <span data-ttu-id="5a0c6-113">לאחר שהוספת את הקבוצה או הקבוצות שבהן ברצונך להשתמש, מתוך הרשימה הנפתחת **פעולת פריסה**, בחר **התקן את Office מוקדם ככל האפשר** או **הסר את ההתקנה של Office**.</span><span class="sxs-lookup"><span data-stu-id="5a0c6-113">After you have added the group or groups you want to use, from the **Deployment Action** drop-down, select either **Install Office as soon as possible** or **Uninstall Office**.</span></span>
    
    ![In the Manage Office deployment pane, choose either Install Office as soon as possible, or Uninstall Office.](media/00f24a61-1848-40c0-b037-78d726c7d757.png)
  
5. <span data-ttu-id="5a0c6-115">בחר **הבא** \> סקור את ההגדרות ולאחר מכן בחר **אשר**.</span><span class="sxs-lookup"><span data-stu-id="5a0c6-115">Choose **Next** \> review the settings and then choose **Confirm**.</span></span>
    
<span data-ttu-id="5a0c6-116">Office של 32 סיביות יותקן באופן אוטומטי, או שהתקנתו של Office תוסר במכשירים שבבעלות המשתמשים שצוינו על-ידי הקבוצה או הקבוצות שבהן השתמשת.</span><span class="sxs-lookup"><span data-stu-id="5a0c6-116">A 32-bit Office will be automatically installed, or uninstalled in the devices owned by users specified by the group or groups you used.</span></span>
  
<span data-ttu-id="5a0c6-117">כדי לוודא, ניתן לפתוח את מנהל המשימות במחשב שנבחר להתקנת Office ולחפש אחר תהליך 'לחץ והפעל' של Microsoft Office.</span><span class="sxs-lookup"><span data-stu-id="5a0c6-117">To verify you can open the Task Manager on a computer that was selected for an Office install and look for Microsoft Office Click-to-Run process.</span></span>
  


