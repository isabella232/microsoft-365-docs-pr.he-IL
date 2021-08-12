---
title: יצירה ועריכה של פרופילי AutoPilot
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: למד כיצד ליצור פרופיל AutoPilot ולהחיל אותו על מכשיר, וכן לערוך או למחוק פרופיל או להסיר פרופיל ממכשיר.
ms.openlocfilehash: d2a3038346b7879006dc2eb50ebe2e70cc6fae92c020a38465cec9d468c638b2
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53797213"
---
# <a name="create-and-edit-autopilot-profiles"></a>יצירה ועריכה של פרופילי AutoPilot

## <a name="create-a-profile"></a>יצירת פרופיל

פרופיל חל על מכשיר או על קבוצה של מכשירים
  
1. בתיבת מרכז הניהול של Microsoft 365, בחר  \> **מכשירים AutoPilot**.
  
2. בדף **AutoPilot,** בחר את הכרטיסיה **פרופילים** \> **צור פרופיל**.
    
3. בדף **יצירת פרופיל,** הזן שם עבור הפרופיל שמסייע לך לזהות אותו, לדוגמה Marketing. הפעל את ההגדרה הרצויה ולאחר מכן בחר **שמור**. לקבלת מידע נוסף אודות הגדרות פרופיל AutoPilot, ראה [אודות הגדרות פרופיל AutoPilot](autopilot-profile-settings.md).
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>החלת פרופיל על מכשיר

לאחר יצירת פרופיל, באפשרותך להחיל אותו על מכשיר או על קבוצת מכשירים. באפשרותך לבחור פרופיל קיים במדריך [שלב אחר](add-autopilot-devices-and-profile.md) שלב ולהחיל אותו על מכשירים חדשים, או להחליף פרופיל קיים עבור מכשיר או קבוצת מכשירים. 
  
1. בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים**. 
    
2. בחר את תיבת הסימון לצד שם מכשיר, ובלוח **המכשיר,**  בחר פרופיל מהרשימה הנפתחת פרופיל מוקצה \> **שמור**.
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>עריכה, מחיקה או הסרה של פרופיל

לאחר שהקצית פרופיל למכשיר, תוכל לעדכן אותו גם אם כבר נתת את המכשיר למשתמש. כאשר המכשיר יתחבר לאינטרנט, הוא יוריד את הגירסה העדכנית ביותר של הפרופיל שלך במהלך תהליך ההתקנה. אם המשתמש משחזר את המכשיר שלו את להגדרות ברירת המחדל של היצרן, המכשיר יוריד שוב את העדכונים האחרונים לפרופיל שלך. 
  
### <a name="edit-a-profile"></a>עריכת פרופיל

1. בדף **הכנת Windows**, בחר בכרטיסיה **פרופילים**. 
    
2. בחר את תיבת הסימון לצד שם מכשיר, ובלוח **פרופיל, עדכן** אחת מההגדרות הזמינות \> **שמור**.
    
    אם תבצע פעולות אלה לפני שהמשתמש יחבר את המכשיר לאינטרנט, הפרופיל יוחל על תהליך ההתקנה.
    
### <a name="delete-a-profile"></a>מחיקת פרופיל

1. בדף **הכנת Windows**, בחר בכרטיסיה **פרופילים**. 
    
2. בחר את תיבת הסימון לצד שם מכשיר, ובחלונית פרופיל, **בחר** מחק **שמירת** \> **פרופיל**.
    
    כאשר תמחק פרופיל, הוא יוסר מהכשיר או מקבוצת המכשירים שלהם הוא הוקצה.
    
### <a name="remove-a-profile"></a>הסרת פרופיל

1. בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים**. 
    
2. בחר את תיבת הסימון לצד שם מכשיר, ובלוח **המכשיר,** בחר **ללא** מהרשימה הנפתחת פרופיל מוקצה  \> **שמור**.
    
