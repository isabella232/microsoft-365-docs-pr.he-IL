---
title: יצירה ועריכה של מכשירי AutoPilot
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: למד כיצד להעלות מכשירים באמצעות טייס אוטומטי ב-Microsoft 365 Business Premium. באפשרותך להקצות פרופיל למכשיר או לקבוצת מכשירים.
ms.openlocfilehash: 910abb98b94b749177b04cd12c766f82d348e379
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913397"
---
# <a name="create-and-edit-autopilot-devices"></a>יצירה ועריכה של מכשירי AutoPilot

## <a name="upload-a-list-of-devices"></a>העלאת רשימה של מכשירים

באפשרותך להשתמש [במדריך שלב אחר שלב](add-autopilot-devices-and-profile.md) להעלאת מכשירים, אך ניתן גם להעלות מכשירים בכרטיסיה ' **מכשירים** '. 
  
המכשירים חייבים לעמוד בדרישות אלה:
  
- Windows 10, גירסה 1703 ואילך
    
- מכשירים חדשים שאינם מותקנים בחוויית Windows out-of-box

1. במרכז הניהול של Microsoft 365, בחר **מכשירים** \> **טייס אוטומטי**.
  
2. בדף **הטייס האוטומטי** , בחר את הכרטיסיה **מכשירים** \> **הוסף מכשירים**.
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. בלוח **הוספת מכשירים** , אתר את [קובץ ה-CSV של רשימת](../admin/misc/device-list.md) המכשירים שהכנת \> **שמור** \> **בסגירה**.
    
    באפשרותך לקבל מידע זה מספק החומרה, או להשתמש [בסקריפט get-Windowsautopilotinfohttps PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) כדי ליצור קובץ CSV. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>הקצאת פרופיל למכשיר או לקבוצה של מכשירים

1. בדף **הכנת Windows** , בחר את הכרטיסיה **התקנים** ובחר את תיבת הסימון לצד התקן אחד או יותר. 
    
2. בלוח **מכשיר**, בחר פרופיל מהתפריט הנפתח **פרופיל שהוקצה**. 
    
    אם עדיין אין לך פרופילים, ראה [יצירה ועריכה של פרופילי AutoPilot](create-and-edit-autopilot-profiles.md) לקבלת הוראות. 
