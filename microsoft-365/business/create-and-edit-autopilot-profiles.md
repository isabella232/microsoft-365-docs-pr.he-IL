---
title: יצירה ועריכה של פרופילי AutoPilot
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: למד ליצור, לערוך, למחוק או להסיר פרופילי טייס אוטומטי.
ms.openlocfilehash: 28f5b679d58711d11d9af26dffb7022024b72c79
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065892"
---
# <a name="create-and-edit-autopilot-profiles"></a>יצירה ועריכה של פרופילי AutoPilot

## <a name="create-a-profile"></a>יצירת פרופיל

פרופיל חל על מכשיר או על קבוצה של מכשירים
  
1. במרכז הניהול העסקי של Microsoft 365, בחר **התקנים** \> **טייס אוטומטי**.
  
2. בעמוד **הטייס האוטומטי** , **** בחר בכרטיסיה \> פרופילים **צור פרופיל**.
    
3. בדף **יצירת פרופיל** , הזן שם עבור הפרופיל שמסייע לך לזהות אותו, לדוגמה שיווק. הפעל את ההגדרה הרצויה ולאחר מכן בחר **בשמור**. לקבלת מידע נוסף אודות הגדרות פרופיל טייס אוטומטי, ראה [אודות הגדרות פרופיל טייס אוטומטי](autopilot-profile-settings.md).
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>החלת פרופיל על מכשיר

לאחר יצירת פרופיל, באפשרותך להחילו על התקן או על קבוצת התקנים. באפשרותך לבחור פרופיל קיים [במדריך שלב-אחר-שלב](add-autopilot-devices-and-profile.md) ולהחילו על התקנים חדשים, או להחליף פרופיל קיים עבור התקן או קבוצת התקנים. 
  
1. בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים**. 
    
2. בחר בתיבת הסימון שליד שם התקן, ובחלונית **ההתקן** , בחר פרופיל \> מהרשימה הנפתחת **פרופיל שהוקצה** **שמור**.
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>עריכה, מחיקה או הסרה של פרופיל

לאחר שהקצית פרופיל למכשיר, תוכל לעדכן אותו גם אם כבר נתת את המכשיר למשתמש. כאשר המכשיר יתחבר לאינטרנט, הוא יוריד את הגירסה העדכנית ביותר של הפרופיל שלך במהלך תהליך ההתקנה. אם המשתמש משחזר את המכשיר שלו את להגדרות ברירת המחדל של היצרן, המכשיר יוריד שוב את העדכונים האחרונים לפרופיל שלך. 
  
### <a name="edit-a-profile"></a>עריכת פרופיל

1. בדף **הכנת Windows**, בחר בכרטיסיה **פרופילים**. 
    
2. בחר בתיבת הסימון לצד שם התקן, ובחלונית **הפרופיל** , עדכן כל אחת מההגדרות \> הזמינות **שמור**.
    
    אם תבצע פעולות אלה לפני שהמשתמש יחבר את המכשיר לאינטרנט, הפרופיל יוחל על תהליך ההתקנה.
    
### <a name="delete-a-profile"></a>מחיקת פרופיל

1. בדף **הכנת Windows**, בחר בכרטיסיה **פרופילים**. 
    
2. בחרו בתיבת הסימון שליד שם התקן, ובחלונית ' **פרופיל** ', בחרו ' **מחק** \> **שמור**פרופיל '.
    
    כאשר תמחק פרופיל, הוא יוסר מהכשיר או מקבוצת המכשירים שלהם הוא הוקצה.
    
### <a name="remove-a-profile"></a>הסרת פרופיל

1. בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים**. 
    
2. בחר בתיבת הסימון שליד שם התקן, ובחלונית **ההתקן** , בחר **בללא** מתוך \> **הרשימה**הנפתחת **פרופיל שהוקצתה** .
    
