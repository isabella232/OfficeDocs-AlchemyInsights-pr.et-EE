---
title: Nimeserverite muutmine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706751"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="8a428-102">Domeeni nimeserverite värskendamine osutama Microsoftile</span><span class="sxs-lookup"><span data-stu-id="8a428-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="8a428-103">Märkus. Nimeserveri muudatuste levitamiseks võib vahel kuluda kuni 48 tundi.</span><span class="sxs-lookup"><span data-stu-id="8a428-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="8a428-104">Domeeni häälestamiseks teenusekomplektis Microsoft 365 tuleb nimeserverid domeeniregistripidaja juures värskendada.</span><span class="sxs-lookup"><span data-stu-id="8a428-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="8a428-105">Saate nimeserverikirjeid luua või redigeerida domeeniregistraatori juures.</span><span class="sxs-lookup"><span data-stu-id="8a428-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="8a428-106">Avage domeeniregistraatori veebisait ja otsige sealt ala, kus saate nimeservereid redigeerida.</span><span class="sxs-lookup"><span data-stu-id="8a428-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="8a428-107">Looge või redigeerige nimeserveri väärtusi, nii et need vastaksid järgmistele aadressidele:</span><span class="sxs-lookup"><span data-stu-id="8a428-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="8a428-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="8a428-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="8a428-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="8a428-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="8a428-110">Salvestage muudatused.</span><span class="sxs-lookup"><span data-stu-id="8a428-110">Save changes.</span></span>

<span data-ttu-id="8a428-111">Üksikasjalikud juhised leiate ka järgmisest artiklist. [Nimeserverite muutmine mis tahes domeeniregistraatoriga](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="8a428-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  