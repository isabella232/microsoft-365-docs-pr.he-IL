---
title: פתרון בעיות עבור שגיאות במכשיר AutoPilot
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: למד כיצד לפתור שגיאות שאתה עשוי לראות בעת עבודה עם קבצי מכשיר AutoPilot ב- Microsoft 365 Business Premium.
ms.openlocfilehash: 1078ab74b07952e4bb565555a081b98ecce9db5c
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578086"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="4434b-103">פתרון בעיות עבור שגיאות במכשיר AutoPilot</span><span class="sxs-lookup"><span data-stu-id="4434b-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="4434b-104">הודעות שגיאה של קובץ מכשיר</span><span class="sxs-lookup"><span data-stu-id="4434b-104">Device file error messages</span></span>

<span data-ttu-id="4434b-105">להלן מידע על חלק מהשגיאות שאתה עשוי לראות בעת עבודה עם קבצי מכשיר AutoPilot ב- Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="4434b-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business Premium.</span></span> 
  
|<span data-ttu-id="4434b-106">**קוד שגיאה**</span><span class="sxs-lookup"><span data-stu-id="4434b-106">**Error code**</span></span>|<span data-ttu-id="4434b-107">**תקן כדי לנסות**</span><span class="sxs-lookup"><span data-stu-id="4434b-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4434b-108">גוף בקשה לא חוקי</span><span class="sxs-lookup"><span data-stu-id="4434b-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="4434b-109">שגיאה זו אמורה להתרחש לעתים רחוקות, אם אתה רואה שגיאה זו, נסה את הפעולה שוב.</span><span class="sxs-lookup"><span data-stu-id="4434b-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="4434b-110">ערך Hash של חומרה עבור מכשיר אינו נכון.</span><span class="sxs-lookup"><span data-stu-id="4434b-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="4434b-111">אם אתה רואה שגיאה זו, משמעות הדבר היא שהערך שסופק בקובץ ה- CSV עבור קוד ה- Hash של החומרה של מכשיר אחד אינו נכון.</span><span class="sxs-lookup"><span data-stu-id="4434b-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="4434b-112">תחילה, ודא שהערך הוקלדה כראוי.</span><span class="sxs-lookup"><span data-stu-id="4434b-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="4434b-113">אם אתה סבור שהערך נכון, אך שגיאה זו עדיין מתרחשת, בקש עזרה מספק החומרה.</span><span class="sxs-lookup"><span data-stu-id="4434b-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="4434b-114">מכשיר שהוקצה לדייר אחר</span><span class="sxs-lookup"><span data-stu-id="4434b-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="4434b-115">אם אתה רואה שגיאה זו, פירוש הדבר שהערך שסופק בקובץ ה- CSV עבור המספר הסידורי או מפתח המוצר של מכשיר אחד או יותר אינו נכון.</span><span class="sxs-lookup"><span data-stu-id="4434b-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="4434b-116">תחילה, ודא שהערך הוקלדה כראוי.</span><span class="sxs-lookup"><span data-stu-id="4434b-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="4434b-117">אם אתה סבור שהערך נכון, אך שגיאה זו עדיין מתרחשת, בקש עזרה מספק החומרה.</span><span class="sxs-lookup"><span data-stu-id="4434b-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="4434b-118">קובץ ה- CSV מכיל מספר סידורי לא חוקי או מפתח מוצר לא חוקי</span><span class="sxs-lookup"><span data-stu-id="4434b-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="4434b-119">אם אתה רואה שגיאה זו, פירוש הדבר שהמכשיר שאתה מנסה לרשום כבר רשום על-ידי ארגון אחר.</span><span class="sxs-lookup"><span data-stu-id="4434b-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="4434b-120">כדי לפתור שגיאה זו, בקש עזרה מספק החומרה שלך.</span><span class="sxs-lookup"><span data-stu-id="4434b-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="4434b-121">התקן זה אינו נתמך עבור הגדרה באמצעות AutoPilot</span><span class="sxs-lookup"><span data-stu-id="4434b-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="4434b-122">שגיאה זו פירושה שההתקן אינו לעמוד בדרישות הפריסה של AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="4434b-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="4434b-123">המכשירים צריכים לעמוד בדרישות אלה:</span><span class="sxs-lookup"><span data-stu-id="4434b-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="4434b-124">Windows ,10 גירסה 1703 ואילך.</span><span class="sxs-lookup"><span data-stu-id="4434b-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="4434b-125">מכשירים חדשים שלא עברו את החוויה 'מחוץ ל- Windows'.</span><span class="sxs-lookup"><span data-stu-id="4434b-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="4434b-126">המכשיר לא נמצא</span><span class="sxs-lookup"><span data-stu-id="4434b-126">Device not found</span></span>  <br/> |<span data-ttu-id="4434b-127">שגיאה זו פירושה שמכשיר אחד או יותר בקובץ ה- CSV שלך אינו רשום בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="4434b-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="4434b-128">כדי לפתור בעיה זו, בקש עזרה מספק החומרה שלך.</span><span class="sxs-lookup"><span data-stu-id="4434b-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
