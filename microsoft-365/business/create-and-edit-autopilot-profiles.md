---
title: יצירה ועריכה של פרופילי AutoPilot
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'למד ליצור, לערוך, למחוק או להסיר פרופילי טייס אוטומטי. '
ms.openlocfilehash: 8fae8af5e7aa7b866745d0b34a4fe11862de6e9d
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287774"
---
# <a name="create-and-edit-autopilot-profiles"></a>יצירה ועריכה של פרופילי AutoPilot

## <a name="create-a-profile"></a>יצירת פרופיל

פרופיל חל על מכשיר או על קבוצה של מכשירים
  
1. במרכז הניהול העסקי של Microsoft 365, בחר **התקנים** \> **טייס אוטומטי**.
  
2. בעמוד **הטייס האוטומטי** , **** בחר בכרטיסיה \> פרופילים **צור פרופיל**.
    
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
    
