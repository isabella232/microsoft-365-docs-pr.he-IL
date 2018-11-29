---
title: מתן אפשרות לניהול מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: למד כיצד להפעיל 365 Microsoft להגן על AD המקומי מצורף התקני Windows 10.
ms.openlocfilehash: 6e66a2c5417c9037232c1ada654d4cac3c520607
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982654"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="fcbde-103">מתן אפשרות לניהול מכשירי Windows 10 המצורפים לתחום על-ידי Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="fcbde-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="fcbde-p101">אם הארגון שלך משתמש Windows Server Active Directory המקומית, באפשרותך להגדיר עסקיים 365 של Microsoft להגנה על התקני Windows 10 שלך, תוך שמירה עדיין גישה למשאבים המקומית המחייבים אימות מקומי. באפשרותך להגדיר זאת על-ידי סינכרון Active Directory שלך עם תכלת הרקיע Active Directory, ואחריו רישום התקני Windows 10 עם AD תכלת הרקיע לבין רושם אותם עבור ניהול התקנים ניידים על-ידי Microsoft 365 עסקיים.</span><span class="sxs-lookup"><span data-stu-id="fcbde-p101">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication. You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="fcbde-106">הגדרת התקני לתחום כדי להיות מנוהל על-ידי Microsoft 365 עסקי</span><span class="sxs-lookup"><span data-stu-id="fcbde-106">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="fcbde-p102">כדי להגדיר את התקנים לתחום של הארגון שלך יועיל להם היכולות שמספק תכלת הרקיע Active Directory בנוסף המקומית Active Directory, באפשרותך ליישם **היברידית AD תכלת הרקיע לחבר התקנים**. אלו הם התקנים המצורפים הן מקומיות של Active Directory ולאחר תכלת הרקיע של Active Directory. היברידית AD תכלת הרקיע מצורף יכול להיות מוגן והתקנים מנוהל על-ידי ביקור 365 Microsoft...</span><span class="sxs-lookup"><span data-stu-id="fcbde-p102">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**. These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory. Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business..</span></span> 
  
<span data-ttu-id="fcbde-110">השלם את השלבים הבאים כדי להפוך את ההתקנים שלך Windows 10 היברידית AD תכלת הרקיע המצורפים ואת מנוהל על-ידי Microsoft 365 עסקיים.</span><span class="sxs-lookup"><span data-stu-id="fcbde-110">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="fcbde-111">כדי לסנכרן שלך משתמשים, קבוצות ואנשי קשר מ- Active Directory המקומי לתוך תכלת הרקיע Active Directory, הפעל את אשף סינכרון הספריות וחבר תכלת הרקיע Active Directory כפי שמתואר [להגדיר סינכרון ספריות עבור Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="fcbde-111">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="fcbde-112">השלבים זהים לחלוטין לעסקים 365 של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fcbde-112">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="fcbde-113">לפני ביצוע שלב 3 כדי לאפשר להתקנים Windows 10 להיות היברידית מצורף AD תכלת הרקיע, עליך לוודא כי אתה עומד בתנאים המוקדמים הבאים:</span><span class="sxs-lookup"><span data-stu-id="fcbde-113">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>
    
   - <span data-ttu-id="fcbde-114">אתה מפעיל את הגירסה העדכנית ביותר של AD תכלת הרקיע להתחבר.</span><span class="sxs-lookup"><span data-stu-id="fcbde-114">You are running the latest version of Azure AD connect.</span></span>
    
   - <span data-ttu-id="fcbde-p103">תכלת הרקיע AD לחבר יש לסנכרן את כל האובייקטים המחשב של ההתקנים שברצונך להיות היברידית AD תכלת הרקיע מצורף. אם האובייקטים המחשב שייך ספציפיים יחידות ארגוניות (OU) ולאחר מכן ודא שיחידות ארגוניות אלה מוגדרות עבור סינכרון ב- AD תכלת הרקיע להתחבר גם.</span><span class="sxs-lookup"><span data-stu-id="fcbde-p103">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined. If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="fcbde-117">רישום קיים לתחום Windows 10 התקנים היברידית Joined AD תכלת הרקיע או להירשם אותם עבור ניהול התקנים ניידים על-ידי Intune (Microsoft 365 עסקי):</span><span class="sxs-lookup"><span data-stu-id="fcbde-117">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="fcbde-p104">בצע את הוראות שלב אחר שלב [כיצד לקבוע תצורה של התקני תכלת הרקיע Active Directory מצורף היברידית](https://go.microsoft.com/fwlink/p/?linkid=872870). פעולה זו תפעיל את הסינכרון של המקומית Active Directory שלך לקבוצת המחשבים של Windows 10 והפוך אותם ענן מוכן.</span><span class="sxs-lookup"><span data-stu-id="fcbde-p104">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870). This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="fcbde-p105">כדי להירשם התקן Windows 10 עבור ניהול התקנים ניידים, ראה [הרשמה התקן Windows 10 עם Intune על-ידי שימוש במדיניות קבוצתית](https://go.microsoft.com/fwlink/p/?linkid=872871) לקבלת הוראות. באפשרותך להגדיר את המדיניות הקבוצתית בכל מחשב מקומי ברמה או עבור פעולות בצובר, באפשרותך ליצור הגדרת מדיניות קבוצתית זו בשרת בקר קבוצת המחשבים שלך.</span><span class="sxs-lookup"><span data-stu-id="fcbde-p105">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions. You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span> 
    

