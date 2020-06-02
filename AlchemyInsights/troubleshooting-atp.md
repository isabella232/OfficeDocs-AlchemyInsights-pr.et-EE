---
title: Tõrkeotsing Office 365 täiustatud ohutõrje
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 7391b3c126d55213881f6b71cb6b5fc72bc68d0f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44512586"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="33630-102">Tõrkeotsing Office 365 täiustatud ohutõrje</span><span class="sxs-lookup"><span data-stu-id="33630-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="33630-103">Kas märkate viivitusi sõnumi kohaletoimetamisega?</span><span class="sxs-lookup"><span data-stu-id="33630-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="33630-104">Kasutage oma ATP turvaliste manuste poliitika [dünaamilise kohaletoimetamise](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) suvandit.</span><span class="sxs-lookup"><span data-stu-id="33630-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="33630-105">See aitab vältida sõnumi viivitusi, kaitstes adressaadid pahatahtlike failide.</span><span class="sxs-lookup"><span data-stu-id="33630-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="33630-106">Kas soovite Microsoftile esitada valeandmeid või valenegatiivseid andmeid?</span><span class="sxs-lookup"><span data-stu-id="33630-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="33630-107">Seda [linki](https://www.microsoft.com/wdsi/filesubmission/) saate kasutada analüüsimiseks failide edastamiseks.</span><span class="sxs-lookup"><span data-stu-id="33630-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="33630-108">Kas teadsite, et saate lubada turvaliste linkide kaitse sisemise meili kaudu, mis saadetakse teie organisatsioonis adressaatide vahel?</span><span class="sxs-lookup"><span data-stu-id="33630-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="33630-109">Tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="33630-109">Follow these steps:</span></span>

  1. <span data-ttu-id="33630-110">[https://protection.office.com](https://protection.office.com)ja logige sisse globaalse administraatori või turbeadministraatori kontoga.</span><span class="sxs-lookup"><span data-stu-id="33630-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="33630-111">Valige jaotises **ohuhalduse**Vasakpoolsel navigeerimispaanil **poliitika** \> **Turvalised lingid**.</span><span class="sxs-lookup"><span data-stu-id="33630-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="33630-112">Poliitika, **mis kehtivad kogu organisatsiooni** jaotises, valige poliitika ja klõpsake nuppu **Redigeeri**.</span><span class="sxs-lookup"><span data-stu-id="33630-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="33630-113">Lubage jaotises **sätted**luba **Rakenda turvalised lingid organisatsioonis saadetud sõnumitele**.</span><span class="sxs-lookup"><span data-stu-id="33630-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
