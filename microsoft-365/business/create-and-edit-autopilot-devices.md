---
title: יצירה ועריכה של מכשירי AutoPilot
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
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: למד כיצד להעלות התקנים באמצעות AutoPilot בעסק 365 של Microsoft. באפשרותך להקצות פרופיל התקן או קבוצה של התקנים.
ms.openlocfilehash: fff2dbc6af45ef9d4189f23849d638172c19dfb2
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277030"
---
# <a name="create-and-edit-autopilot-devices"></a>יצירה ועריכה של מכשירי AutoPilot

## <a name="upload-a-list-of-devices"></a>העלאת רשימה של מכשירים

באפשרותך להשתמש ב[מדריך צעד-אחר-צעד](add-autopilot-devices-and-profile.md) כדי להעלות מכשירים, אך ניתן גם להעלות בכרטיסיה **מכשירים**. 
  
המכשירים צריכים לעמוד בדרישות אלה:
  
- Windows ,10 גירסה 1703 ואילך.
    
- מכשירים חדשים שאינם נחשבים כמוצר Windows מוכן לשימוש.

1. במרכז הניהול העסקי של Microsoft 365, בחר **התקנים** \> **AutoPilot** \> **הוספה**.
  
2. בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים** \> **הוסף מכשירים**.
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. בלוח **התקנים הוסף** , דפדף אל [רשימת התקנים קובץ CSV](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) שהכנת \> **שמור** \> **סגור**.
    
    ניתן לקבל מידע זה מספק החומרה, או להשתמש ב[קובץ Script של PowerShell, ‏Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) שייצור קובץ csv. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>הקצאת פרופיל למכשיר או לקבוצה של מכשירים

1. בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים** וסמן את תיבת הסימון לצד מכשיר אחד או יותר. 
    
2. בלוח **מכשיר**, בחר פרופיל מהתפריט הנפתח **פרופיל שהוקצה**. 
    
    אם עדיין אין לך פרופילים, ראה [יצירה ועריכה של פרופילי AutoPilot](create-and-edit-autopilot-profiles.md) לקבלת הוראות. 
    
