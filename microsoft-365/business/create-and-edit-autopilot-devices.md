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
description: למד כיצד להעלות התקנים באמצעות טייס אוטומטי ב-Microsoft 365 Business Premium. באפשרותך להקצות פרופיל להתקן או לקבוצת התקנים.
ms.openlocfilehash: 8c3d029d682ae30444bdc7d30a4790a8f982e0e0
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400993"
---
# <a name="create-and-edit-autopilot-devices"></a>יצירה ועריכה של מכשירי AutoPilot

## <a name="upload-a-list-of-devices"></a>העלאת רשימה של מכשירים

באפשרותך להשתמש [במדריך שלב-אחר-שלב](add-autopilot-devices-and-profile.md) כדי לטעון התקנים, אך באפשרותך גם להעלות התקנים בכרטיסיה ' **התקנים** '. 
  
על התקנים לעמוד בדרישות הבאות:
  
- Windows 10, גירסה 1703 ואילך
    
- מכשירים חדשים שלא עברו חוויה מחוץ לקופסא של Windows

1. במרכז הניהול של Microsoft 365, בחר **התקנים** \> **טייס אוטומטי**.
  
2. בעמוד **הטייס האוטומטי** , בחר בכרטיסיה **התקנים** \> **הוסף התקנים**.
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. בחלונית ' **הוספת התקנים** ', דפדף [לקובץ CSV של רשימת ההתקנים](https://docs.microsoft.com/microsoft-365/admin/misc/device-list) שהכנת \> **לשמירת** \> **הסגירה**.
    
    אתה יכול לקבל את המידע הזה מספק החומרה שלך, או שאתה יכול להשתמש [בסקריפט לקבל-Windowsautopilinfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) כדי ליצור קובץ CSV. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>הקצאת פרופיל למכשיר או לקבוצה של מכשירים

1. בדף ' **הכנת Windows** ', בחר בכרטיסיה ' **התקנים** ' ובחר בתיבת הסימון שליד התקן אחד או יותר. 
    
2. בלוח **מכשיר**, בחר פרופיל מהתפריט הנפתח **פרופיל שהוקצה**. 
    
    אם עדיין אין לך פרופילים, ראה [יצירה ועריכה של פרופילי AutoPilot](create-and-edit-autopilot-profiles.md) לקבלת הוראות. 
    
