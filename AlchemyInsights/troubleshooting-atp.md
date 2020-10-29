---
title: Microsoft Defenderi tõrkeotsing Office 365 jaoks
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
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801439"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="d3506-102">Microsoft Defenderi tõrkeotsing Office 365 jaoks</span><span class="sxs-lookup"><span data-stu-id="d3506-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="d3506-103">Kas teate kohaletoimetamisega viivitatakse?</span><span class="sxs-lookup"><span data-stu-id="d3506-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="d3506-104">Kasutage oma ATP turvaliste manuste poliitikas [dünaamilist kohaletoimetamise](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) võimalust.</span><span class="sxs-lookup"><span data-stu-id="d3506-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="d3506-105">See aitab vältida sõnumite viivitusi, kaitstes samal ajal adressaate pahatahtlike failide eest.</span><span class="sxs-lookup"><span data-stu-id="d3506-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="d3506-106">Kas soovite Microsoftile teatada valedest positiivsetest või valedest negatiivist?</span><span class="sxs-lookup"><span data-stu-id="d3506-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="d3506-107">Kasutage seda [linki](https://www.microsoft.com/wdsi/filesubmission/) , et esitada analüüsimiseks faile.</span><span class="sxs-lookup"><span data-stu-id="d3506-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="d3506-108">Kas teadsite, et saate lubada turvaliste linkide kaitse oma asutuse adressaatidele saadetavate sisemiste meilisõnumite jaoks?</span><span class="sxs-lookup"><span data-stu-id="d3506-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="d3506-109">Tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="d3506-109">Follow these steps:</span></span>

  1. <span data-ttu-id="d3506-110">Avage [https://protection.office.com](https://protection.office.com) ja logige sisse üldise administraatori või administraatori kontoga.</span><span class="sxs-lookup"><span data-stu-id="d3506-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="d3506-111">Valige vasakpoolsel navigeerimispaanil jaotises **ohu haldamine** valik **poliitika** \> **Turvalised lingid** .</span><span class="sxs-lookup"><span data-stu-id="d3506-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="d3506-112">Valige jaotises **kogu organisatsioon rakendatav** poliitika ja klõpsake nuppu **Redigeeri** .</span><span class="sxs-lookup"><span data-stu-id="d3506-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="d3506-113">Jaotises **sätted** lubage **organisatsioonis saadetavate sõnumite turvaliste linkide rakendamine** .</span><span class="sxs-lookup"><span data-stu-id="d3506-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
