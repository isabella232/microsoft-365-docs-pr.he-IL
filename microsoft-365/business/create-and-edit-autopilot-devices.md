---
title: יצירה ועריכה של מכשירי AutoPilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: למד כיצד להעלות מכשירים באמצעות AutoPilot Microsoft 365 Business Premium. באפשרותך להקצות פרופיל למכשיר או לקבוצת מכשירים.
ms.openlocfilehash: ae3a760db4b94aac50301685a0c4f468e46ec8e9aa907a1b6fb35e03a9e541f0
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53867040"
---
# <a name="create-and-edit-autopilot-devices"></a>יצירה ועריכה של מכשירי AutoPilot

## <a name="upload-a-list-of-devices"></a>העלאת רשימה של מכשירים

באפשרותך להשתמש במדריך [שלב אחר שלב להעלאת](add-autopilot-devices-and-profile.md) מכשירים, אך באפשרותך גם להעלות מכשירים **בכרטיסיה מכשירים.** 
  
מכשירים חייבים לעמוד בדרישות הבאות:
  
- Windows 10, גירסה 1703 ואילך
    
- מכשירים חדשים שלא עברו Windows חוויה מחוץ לקופסה

1. בתיבת מרכז הניהול של Microsoft 365, בחר  \> **מכשירים AutoPilot**.
  
2. בדף **AutoPilot,** בחר בכרטיסיה **מכשירים** \> **הוסף מכשירים**.
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. בלוח הוספת **מכשירים,** עבור אל קובץ [CSV של רשימת ההתקנים](../admin/misc/device-list.md) שהכנת \> **שמור** \> **סגור**.
    
    באפשרותך לקבל מידע זה מספק החומרה שלך, או להשתמש בקובץ [ה- Script Get-WindowsAutoPilotInfo PowerShell](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) כדי ליצור קובץ CSV. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>הקצאת פרופיל למכשיר או לקבוצה של מכשירים

1. בדף **הכנת Windows,** בחר בכרטיסיה **מכשירים** ובחר את תיבת הסימון לצד מכשיר אחד או יותר. 
    
2. בלוח **מכשיר**, בחר פרופיל מהתפריט הנפתח **פרופיל שהוקצה**. 
    
    אם עדיין אין לך פרופילים, ראה [יצירה ועריכה של פרופילי AutoPilot](create-and-edit-autopilot-profiles.md) לקבלת הוראות. 
