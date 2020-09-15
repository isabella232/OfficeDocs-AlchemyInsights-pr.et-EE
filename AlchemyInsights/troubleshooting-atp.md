---
title: Office 365 täiustatud ohtude kaitse tõrkeotsing
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658910"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="9a778-102">Office 365 täiustatud ohtude kaitse tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="9a778-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="9a778-103">Kas teate kohaletoimetamisega viivitatakse?</span><span class="sxs-lookup"><span data-stu-id="9a778-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="9a778-104">Kasutage oma ATP turvaliste manuste poliitikas [dünaamilist kohaletoimetamise](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) võimalust.</span><span class="sxs-lookup"><span data-stu-id="9a778-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="9a778-105">See aitab vältida sõnumite viivitusi, kaitstes samal ajal adressaate pahatahtlike failide eest.</span><span class="sxs-lookup"><span data-stu-id="9a778-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="9a778-106">Kas soovite Microsoftile teatada valedest positiivsetest või valedest negatiivist?</span><span class="sxs-lookup"><span data-stu-id="9a778-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="9a778-107">Kasutage seda [linki](https://www.microsoft.com/wdsi/filesubmission/) , et esitada analüüsimiseks faile.</span><span class="sxs-lookup"><span data-stu-id="9a778-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="9a778-108">Kas teadsite, et saate lubada turvaliste linkide kaitse oma asutuse adressaatidele saadetavate sisemiste meilisõnumite jaoks?</span><span class="sxs-lookup"><span data-stu-id="9a778-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="9a778-109">Tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="9a778-109">Follow these steps:</span></span>

  1. <span data-ttu-id="9a778-110">Avage [https://protection.office.com](https://protection.office.com) ja logige sisse üldise administraatori või administraatori kontoga.</span><span class="sxs-lookup"><span data-stu-id="9a778-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="9a778-111">Valige vasakpoolsel navigeerimispaanil jaotises **ohu haldamine**valik **poliitika** \> **Turvalised lingid**.</span><span class="sxs-lookup"><span data-stu-id="9a778-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="9a778-112">Valige jaotises **kogu organisatsioon rakendatav** poliitika ja klõpsake nuppu **Redigeeri**.</span><span class="sxs-lookup"><span data-stu-id="9a778-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="9a778-113">Jaotises **sätted**lubage **organisatsioonis saadetavate sõnumite turvaliste linkide rakendamine**.</span><span class="sxs-lookup"><span data-stu-id="9a778-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
