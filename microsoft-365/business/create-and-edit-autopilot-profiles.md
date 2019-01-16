---
title: יצירה ועריכה של פרופילי AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'למד כיצד ליצור, לערוך, למחוק או להסיר פרופילי AutoPilot. '
ms.openlocfilehash: 4658a27e5f2c64a52f8a7d08b3fc13df5e239dc3
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983134"
---
# <a name="create-and-edit-autopilot-profiles"></a>יצירה ועריכה של פרופילי AutoPilot

## <a name="create-a-profile"></a>יצירת פרופיל

פרופיל חל על מכשיר או על קבוצה של מכשירים
  
1. במרכז הניהול של Microsoft 365 Business, בחר **פרוס את Windows באמצעות AutoPilot** בכרטיס **פעולות מכשיר**. 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. בדף **הכנת Windows**, בחר בכרטיסיה **פרופילים** \> **צור פרופיל**.
    
3. בדף **יצירת פרופיל**, הזן שם עבור הפרופיל שיעזור לך לזהות אותו, לדוגמה, שיווק, הפעל את ההגדרה הרצויה (למידע נוסף, ראה [אודות ההגדרות של פרופיל AutoPilot](autopilot-profile-settings.md)), ובחר **שמור**.
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>החלת פרופיל על מכשיר

לאחר שתיצור פרופיל, תוכל להחיל אותו על מכשיר או על קבוצה של מכשירים. תוכל לבחור פרופיל קיים ב[מדריך צעד-אחד-צעד](add-autopilot-devices-and-profile.md), תוכל להחיל אותו על מכשירים חדשים או תוכל להחליף פרופיל קיים עבור מכשיר או קבוצת מכשירים. 
  
1. בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים**. 
    
2. לחץ על תיבת הסימון לצד שם מכשיר בלוח **מכשיר**, בחר פרופיל בתפריט הנפתח **פרופיל שהוקצה** \> **שמור**.
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>עריכה, מחיקה או הסרה של פרופיל

לאחר שהקצית פרופיל למכשיר, תוכל לעדכן אותו גם אם כבר נתת את המכשיר למשתמש. כאשר המכשיר יתחבר לאינטרנט, הוא יוריד את הגירסה העדכנית ביותר של הפרופיל שלך במהלך תהליך ההתקנה. אם המשתמש משחזר את המכשיר שלו את להגדרות ברירת המחדל של היצרן, המכשיר יוריד שוב את העדכונים האחרונים לפרופיל שלך. 
  
### <a name="edit-a-profile"></a>עריכת פרופיל

1. בדף **הכנת Windows**, בחר בכרטיסיה **פרופילים**. 
    
2. לחץ על תיבת הסימון לצד שם מכשיר, ובלוח **פרופיל** עדכן אחת מההגדרות הזמינות \> **שמור**.
    
    אם תבצע פעולות אלה לפני שהמשתמש יחבר את המכשיר לאינטרנט, הפרופיל יוחל על תהליך ההתקנה.
    
### <a name="delete-a-profile"></a>מחיקת פרופיל

1. בדף **הכנת Windows**, בחר בכרטיסיה **פרופילים**. 
    
2. לחץ על תיבת הסימון לצד שם מכשיר, ובלוח **פרופיל** לחץ על **מחק פרופיל** \> **שמור**.
    
    כאשר תמחק פרופיל, הוא יוסר מהכשיר או מקבוצת המכשירים שלהם הוא הוקצה.
    
### <a name="remove-a-profile"></a>הסרת פרופיל

1. בדף **הכנת Windows**, בחר בכרטיסיה **מכשירים**. 
    
2. לחץ על תיבת הסימון לצד שם מכשיר בלוח **מכשיר**, בחר **ללא** בתפריט הנפתח **פרופיל שהוקצה** \> **שמור**.
    