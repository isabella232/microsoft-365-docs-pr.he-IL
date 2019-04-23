---
title: פתרון בעיות עבור שגיאות במכשיר AutoPilot
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: troubleshooting
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: למד כיצד לפתור בעיות של שגיאות קבצים בהתקן AutoPilot.
ms.openlocfilehash: 9d4a47f78c38d8c076f5b3876a36b6bf46eaaaf3
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32279837"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="405b3-103">פתרון בעיות עבור שגיאות במכשיר AutoPilot</span><span class="sxs-lookup"><span data-stu-id="405b3-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="405b3-104">הודעות שגיאה של קובץ התקן</span><span class="sxs-lookup"><span data-stu-id="405b3-104">Device file error messages</span></span>

<span data-ttu-id="405b3-105">מידע הנה על חלק מן השגיאות עשוי לראות בעת עבודה עם קבצים בהתקן AutoPilot בעסק 365 של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="405b3-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="405b3-106">**קוד שגיאה**</span><span class="sxs-lookup"><span data-stu-id="405b3-106">**Error code**</span></span>|<span data-ttu-id="405b3-107">**תיקון כדי לנסות**</span><span class="sxs-lookup"><span data-stu-id="405b3-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="405b3-108">גוף הבקשה לא חוקי</span><span class="sxs-lookup"><span data-stu-id="405b3-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="405b3-109">שגיאה זו אמור לקרות רק לעתים רחוקות, אם אתה רואה שגיאה זו, נסה את הפעולה שוב.</span><span class="sxs-lookup"><span data-stu-id="405b3-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="405b3-110">ערך ה-hash של החומרה עבור התקן אינו נכון.</span><span class="sxs-lookup"><span data-stu-id="405b3-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="405b3-111">אם אתה רואה שגיאה זו, משמעות הדבר היא כי הערך שסיפקת בקובץ CSV עבור קוד hash של החומרה של התקן אחד אינו נכון.</span><span class="sxs-lookup"><span data-stu-id="405b3-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="405b3-112">תחילה, ודא כי הערך הוקלד כראוי.</span><span class="sxs-lookup"><span data-stu-id="405b3-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="405b3-113">אם אתה סבור כי הערך נכון, אך עדיין קורה שגיאה זו, בקש עזרה ספק החומרה שלך.</span><span class="sxs-lookup"><span data-stu-id="405b3-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="405b3-114">התקן שהוקצו דייר אחר</span><span class="sxs-lookup"><span data-stu-id="405b3-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="405b3-115">אם אתה רואה שגיאה זו, משמעות הדבר היא כי הערך שסיפקת בקובץ CSV עבור המספר הסידורי או את מפתח המוצר של התקן אחד או יותר אינו נכון.</span><span class="sxs-lookup"><span data-stu-id="405b3-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="405b3-116">תחילה, ודא כי הערך הוקלד כראוי.</span><span class="sxs-lookup"><span data-stu-id="405b3-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="405b3-117">אם אתה סבור כי הערך נכון, אך עדיין קורה שגיאה זו, בקש עזרה ספק החומרה שלך.</span><span class="sxs-lookup"><span data-stu-id="405b3-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="405b3-118">קובץ ה-CSV מכילה מספר סידורי לא חוקי או מפתח מוצר</span><span class="sxs-lookup"><span data-stu-id="405b3-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="405b3-119">אם אתה רואה שגיאה זו, פירוש הדבר ההתקן שאתה במהלך ניסיון לרשום כבר רשום על-ידי ארגון אחר.</span><span class="sxs-lookup"><span data-stu-id="405b3-119">If you see this error it means that the device you are tyring to register is already registered by an other organization.</span></span> <span data-ttu-id="405b3-120">כדי לפתור בעיה זו, בקש ספק החומרה שלך לקבלת עזרה.</span><span class="sxs-lookup"><span data-stu-id="405b3-120">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="405b3-121">התקן זה אינו נתמך עבור תוכנית ההתקנה באמצעות AutoPilot</span><span class="sxs-lookup"><span data-stu-id="405b3-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="405b3-122">שגיאה זו פירושה שההתקן אינו עומד בדרישות הפריסה AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="405b3-122">This error means the device does not meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="405b3-123">המכשירים צריכים לעמוד בדרישות אלה:</span><span class="sxs-lookup"><span data-stu-id="405b3-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="405b3-124">Windows ,10 גירסה 1703 ואילך.</span><span class="sxs-lookup"><span data-stu-id="405b3-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="405b3-125">מכשירים חדשים שאינם נחשבים כמוצר Windows מוכן לשימוש.</span><span class="sxs-lookup"><span data-stu-id="405b3-125">New devices that have not been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="405b3-126">התקן לא נמצא</span><span class="sxs-lookup"><span data-stu-id="405b3-126">Device not found</span></span>  <br/> |<span data-ttu-id="405b3-127">שגיאה זו פירושה כי התקן אחד או יותר בקובץ CSV שלך אינו רשום לארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="405b3-127">This error means that one or more devices in your CSV file is not registered to your organization.</span></span> <span data-ttu-id="405b3-128">כדי לפתור בעיה זו, בקש ספק החומרה שלך לקבלת עזרה.</span><span class="sxs-lookup"><span data-stu-id="405b3-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
   
