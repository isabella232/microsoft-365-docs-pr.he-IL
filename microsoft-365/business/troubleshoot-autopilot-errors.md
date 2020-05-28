---
title: פתרון בעיות עבור שגיאות במכשיר AutoPilot
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: למד כיצד לפתור שגיאות שייתכן שתראה בעת עבודה עם קבצי התקן טייס אוטומטי ב-Microsoft 365 Business Premium.
ms.openlocfilehash: bec5126696ee322db42e4b7c5cd8e0df485ab2c9
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403409"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="c72a2-103">פתרון בעיות עבור שגיאות במכשיר AutoPilot</span><span class="sxs-lookup"><span data-stu-id="c72a2-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="c72a2-104">הודעות שגיאה של קובץ התקן</span><span class="sxs-lookup"><span data-stu-id="c72a2-104">Device file error messages</span></span>

<span data-ttu-id="c72a2-105">הנה מידע על חלק מהשגיאות שאתה עשוי לראות בעת עבודה עם קבצי התקן טייס אוטומטי ב-Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c72a2-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business Premium.</span></span> 
  
|<span data-ttu-id="c72a2-106">**קוד שגיאה**</span><span class="sxs-lookup"><span data-stu-id="c72a2-106">**Error code**</span></span>|<span data-ttu-id="c72a2-107">**תקן כדי לנסות**</span><span class="sxs-lookup"><span data-stu-id="c72a2-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c72a2-108">גוף בקשה לא חוקי</span><span class="sxs-lookup"><span data-stu-id="c72a2-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="c72a2-109">שגיאה זו אמורה להתרחש לעתים רחוקות, אם אתה רואה שגיאה זו, נסה את הפעולה שנית.</span><span class="sxs-lookup"><span data-stu-id="c72a2-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="c72a2-110">ערך hash של חומרה עבור התקן אינו נכון.</span><span class="sxs-lookup"><span data-stu-id="c72a2-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="c72a2-111">אם אתה רואה שגיאה זו, משמעות הדבר היא שהערך שסיפקת בקובץ ה-CSV עבור קוד ה-hash של התקן אחד אינו נכון.</span><span class="sxs-lookup"><span data-stu-id="c72a2-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="c72a2-112">תחילה, ודא שהערך הוקלד בצורה נכונה.</span><span class="sxs-lookup"><span data-stu-id="c72a2-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="c72a2-113">אם אתה סבור שהערך נכון, אך שגיאה זו עדיין מתרחשת, שאל את ספק החומרה שלך לקבלת עזרה.</span><span class="sxs-lookup"><span data-stu-id="c72a2-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="c72a2-114">התקן שהוקצה לדייר אחר</span><span class="sxs-lookup"><span data-stu-id="c72a2-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="c72a2-115">אם אתה רואה שגיאה זו, משמעות הדבר היא שהערך שסיפקת בקובץ ה-CSV עבור המספר הסידורי או מפתח המוצר של התקן אחד או יותר אינו נכון.</span><span class="sxs-lookup"><span data-stu-id="c72a2-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="c72a2-116">תחילה, ודא שהערך הוקלד בצורה נכונה.</span><span class="sxs-lookup"><span data-stu-id="c72a2-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="c72a2-117">אם אתה סבור שהערך נכון, אך שגיאה זו עדיין מתרחשת, שאל את ספק החומרה שלך לקבלת עזרה.</span><span class="sxs-lookup"><span data-stu-id="c72a2-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="c72a2-118">קובץ ה-CSV מכיל מספר סידורי או מפתח מוצר לא חוקי</span><span class="sxs-lookup"><span data-stu-id="c72a2-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="c72a2-119">אם אתה רואה שגיאה זו, משמעות הדבר היא שההתקן שאתה מנסה לרשום כבר רשום על-ידי ארגון אחר.</span><span class="sxs-lookup"><span data-stu-id="c72a2-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="c72a2-120">כדי לתקן שגיאה זו, שאל את ספק החומרה שלך לקבלת עזרה.</span><span class="sxs-lookup"><span data-stu-id="c72a2-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="c72a2-121">התקן זה אינו נתמך עבור התקנה באמצעות טייס אוטומטי</span><span class="sxs-lookup"><span data-stu-id="c72a2-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="c72a2-122">שגיאה זו פירושה שההתקן אינו עומד בדרישות הפריסה של טייס אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="c72a2-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="c72a2-123">המכשירים צריכים לעמוד בדרישות אלה:</span><span class="sxs-lookup"><span data-stu-id="c72a2-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="c72a2-124">Windows ,10 גירסה 1703 ואילך.</span><span class="sxs-lookup"><span data-stu-id="c72a2-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="c72a2-125">מכשירים חדשים שלא התבצעה באמצעות הניסיון היוצא מהקופסה של Windows.</span><span class="sxs-lookup"><span data-stu-id="c72a2-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="c72a2-126">ההתקן לא נמצא</span><span class="sxs-lookup"><span data-stu-id="c72a2-126">Device not found</span></span>  <br/> |<span data-ttu-id="c72a2-127">שגיאה זו פירושה שהתקן אחד או יותר בקובץ ה-CSV אינו רשום לארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="c72a2-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="c72a2-128">כדי לתקן זאת, בקש עזרה מספק החומרה שלך.</span><span class="sxs-lookup"><span data-stu-id="c72a2-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
