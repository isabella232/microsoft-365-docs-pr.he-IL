---
title: פתרון בעיות עבור שגיאות במכשיר AutoPilot
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: למד כיצד לפתור שגיאות שייתכן שתראה בעת עבודה עם קבצי התקן טייס אוטומטי ב-Microsoft 365 Business.
ms.openlocfilehash: 7569f18097a1f5959b3dd491958c78886e1e05d6
ms.sourcegitcommit: 41c0bc5cf50f4ca63b4286d1ea0f58ab82984b7a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2020
ms.locfileid: "42547470"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="d04f7-103">פתרון בעיות עבור שגיאות במכשיר AutoPilot</span><span class="sxs-lookup"><span data-stu-id="d04f7-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="d04f7-104">הודעות שגיאה של קובץ התקן</span><span class="sxs-lookup"><span data-stu-id="d04f7-104">Device file error messages</span></span>

<span data-ttu-id="d04f7-105">להלן מידע על חלק מהשגיאות שייתכן שתראה בעת עבודה עם קבצי התקן טייס אוטומטי ב-Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="d04f7-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="d04f7-106">**קוד שגיאה**</span><span class="sxs-lookup"><span data-stu-id="d04f7-106">**Error code**</span></span>|<span data-ttu-id="d04f7-107">**תקן כדי לנסות**</span><span class="sxs-lookup"><span data-stu-id="d04f7-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d04f7-108">גוף בקשה לא חוקי</span><span class="sxs-lookup"><span data-stu-id="d04f7-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="d04f7-109">שגיאה זו אמורה להתרחש לעתים רחוקות, אם אתה רואה שגיאה זו, נסה את הפעולה שנית.</span><span class="sxs-lookup"><span data-stu-id="d04f7-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="d04f7-110">ערך hash של חומרה עבור התקן אינו נכון.</span><span class="sxs-lookup"><span data-stu-id="d04f7-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="d04f7-111">אם אתה רואה שגיאה זו, משמעות הדבר היא שהערך שסיפקת בקובץ ה-CSV עבור קוד ה-hash של התקן אחד אינו נכון.</span><span class="sxs-lookup"><span data-stu-id="d04f7-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="d04f7-112">תחילה, ודא שהערך הוקלד בצורה נכונה.</span><span class="sxs-lookup"><span data-stu-id="d04f7-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="d04f7-113">אם אתה סבור שהערך נכון, אך שגיאה זו עדיין מתרחשת, שאל את ספק החומרה שלך לקבלת עזרה.</span><span class="sxs-lookup"><span data-stu-id="d04f7-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="d04f7-114">התקן שהוקצה לדייר אחר</span><span class="sxs-lookup"><span data-stu-id="d04f7-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="d04f7-115">אם אתה רואה שגיאה זו, משמעות הדבר היא שהערך שסיפקת בקובץ ה-CSV עבור המספר הסידורי או מפתח המוצר של התקן אחד או יותר אינו נכון.</span><span class="sxs-lookup"><span data-stu-id="d04f7-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="d04f7-116">תחילה, ודא שהערך הוקלד בצורה נכונה.</span><span class="sxs-lookup"><span data-stu-id="d04f7-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="d04f7-117">אם אתה סבור שהערך נכון, אך שגיאה זו עדיין מתרחשת, שאל את ספק החומרה שלך לקבלת עזרה.</span><span class="sxs-lookup"><span data-stu-id="d04f7-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="d04f7-118">קובץ ה-CSV מכיל מספר סידורי או מפתח מוצר לא חוקי</span><span class="sxs-lookup"><span data-stu-id="d04f7-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="d04f7-119">אם אתה רואה שגיאה זו, משמעות הדבר היא שההתקן שאתה מנסה לרשום כבר רשום על-ידי ארגון אחר.</span><span class="sxs-lookup"><span data-stu-id="d04f7-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="d04f7-120">כדי לתקן שגיאה זו, שאל את ספק החומרה שלך לקבלת עזרה.</span><span class="sxs-lookup"><span data-stu-id="d04f7-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="d04f7-121">התקן זה אינו נתמך עבור התקנה באמצעות טייס אוטומטי</span><span class="sxs-lookup"><span data-stu-id="d04f7-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="d04f7-122">שגיאה זו פירושה שההתקן אינו עומד בדרישות הפריסה של טייס אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="d04f7-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="d04f7-123">המכשירים צריכים לעמוד בדרישות אלה:</span><span class="sxs-lookup"><span data-stu-id="d04f7-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="d04f7-124">Windows ,10 גירסה 1703 ואילך.</span><span class="sxs-lookup"><span data-stu-id="d04f7-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="d04f7-125">מכשירים חדשים שלא התבצעה באמצעות הניסיון היוצא מהקופסה של Windows.</span><span class="sxs-lookup"><span data-stu-id="d04f7-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="d04f7-126">ההתקן לא נמצא</span><span class="sxs-lookup"><span data-stu-id="d04f7-126">Device not found</span></span>  <br/> |<span data-ttu-id="d04f7-127">שגיאה זו פירושה שהתקן אחד או יותר בקובץ ה-CSV אינו רשום לארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="d04f7-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="d04f7-128">כדי לתקן זאת, בקש עזרה מספק החומרה שלך.</span><span class="sxs-lookup"><span data-stu-id="d04f7-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
