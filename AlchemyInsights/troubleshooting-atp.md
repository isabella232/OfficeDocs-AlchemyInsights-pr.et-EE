---
title: Office 365 täiustatud ohutõrje tõrkeotsing
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: b4358fb55a1145833510c6063b520d822f2d1eaf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765009"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="70e13-102">Office 365 täiustatud ohutõrje tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="70e13-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="70e13-103">Kas te teate sõnumi kohaletoimetamise viivituse?</span><span class="sxs-lookup"><span data-stu-id="70e13-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="70e13-104">Kasutada [Dünaamilise tellimise](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) võimalus ATP Safe Attachments poliisil.</span><span class="sxs-lookup"><span data-stu-id="70e13-104">Use the [Dynamic Delivery](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="70e13-105">See aitab vältida sõnumi viivitusi, samal ajal kaitstes adressaadid pahatahtlike faile.</span><span class="sxs-lookup"><span data-stu-id="70e13-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="70e13-106">Kas soovite teavitada Microsofti valepositiivseid või valenegatiivseid?</span><span class="sxs-lookup"><span data-stu-id="70e13-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="70e13-107">Kasuta seda [linki](https://www.microsoft.com/wdsi/filesubmission/) failid analüüsiks.</span><span class="sxs-lookup"><span data-stu-id="70e13-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="70e13-108">Kas teadsite, et saate lubada Safe Links kaitse sisemise meilisõnumid vahel adressaadile oma organisatsioonis?</span><span class="sxs-lookup"><span data-stu-id="70e13-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="70e13-109">Toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="70e13-109">Follow these steps:</span></span>

  1. <span data-ttu-id="70e13-110">Mine [https://protection.office.com](https://protection.office.com) ja logite sisse globaalne administraatori või turvalisuse administraatori konto.</span><span class="sxs-lookup"><span data-stu-id="70e13-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="70e13-111">Valige vasakpoolsel navigeerimispaanil alusel **ohu haldamise** **poliitika** \> **Safe Links**.</span><span class="sxs-lookup"><span data-stu-id="70e13-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="70e13-112">**Saada kogu organisatsiooni** reeglites, valige poliitika ja klõpsake nuppu **Redigeeri**.</span><span class="sxs-lookup"><span data-stu-id="70e13-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="70e13-113">**Rakenda ohutu linke ettevõtte saadetavatele**lubada jaotises **sätted**.</span><span class="sxs-lookup"><span data-stu-id="70e13-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
