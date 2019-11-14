---
title: יצירה ועריכה של מכשירי AutoPilot
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
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: למד כיצד להעלות התקנים באמצעות טייס אוטומטי ב-Microsoft 365 Business. באפשרותך להקצות פרופיל להתקן או לקבוצת התקנים.
ms.openlocfilehash: 1dd6b1a574166379e29465bf3699e47e3b155e0b
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320257"
---
# <a name="create-and-edit-autopilot-devices"></a>יצירה ועריכה של מכשירי AutoPilot

## <a name="upload-a-list-of-devices"></a>העלאת רשימה של מכשירים

באפשרותך להשתמש [במדריך שלב-אחר-שלב](add-autopilot-devices-and-profile.md) כדי לטעון התקנים, אך באפשרותך גם להעלות התקנים בכרטיסיה ' **התקנים** '. 
  
על התקנים לעמוד בדרישות הבאות:
  
- Windows 10, גירסה 1703 ואילך
    
- מכשירים חדשים שלא עברו חוויה מחוץ לקופסא של Windows

1. במרכז הניהול העסקי של Microsoft 365, בחר **התקנים** \> **טייס אוטומטי**.
  
2. בעמוד **הטייס האוטומטי** , בחר \> בכרטיסיה **התקנים** **הוספת התקנים**.
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. בחלונית **' הוספת התקנים** ', דפדף [לקובץ CSV של רשימת ההתקנים](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) שהכנת \> **לשמירת** \> **הסגירה**.
    
    אתה יכול לקבל את המידע הזה מספק החומרה שלך, או שאתה יכול להשתמש [בסקריפט לקבל-Windowsautopilinfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) כדי ליצור קובץ CSV. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>הקצאת פרופיל למכשיר או לקבוצה של מכשירים

1. בדף ' **הכנת Windows** ', בחר בכרטיסיה ' **התקנים** ' ובחר בתיבת הסימון שליד התקן אחד או יותר. 
    
2. בלוח **מכשיר**, בחר פרופיל מהתפריט הנפתח **פרופיל שהוקצה**. 
    
    אם עדיין אין לך פרופילים, ראה [יצירה ועריכה של פרופילי AutoPilot](create-and-edit-autopilot-profiles.md) לקבלת הוראות. 
    
