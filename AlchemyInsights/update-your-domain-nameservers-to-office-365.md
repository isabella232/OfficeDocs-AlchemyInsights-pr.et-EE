---
title: Domeeni nimeserverite värskendamine Office 365 jaoks
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742171"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="f4b64-102">Domeeni nimeserverite värskendamine Office 365 jaoks</span><span class="sxs-lookup"><span data-stu-id="f4b64-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="f4b64-103">Märkus. Nimeserveri muudatuste levitamiseks võib vahel kuluda kuni 48 tundi.</span><span class="sxs-lookup"><span data-stu-id="f4b64-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="f4b64-104">Domeeni häälestamiseks teenusekomplektis Office 365 tuleb nimeserverid domeeniregistripidaja juures värskendada.</span><span class="sxs-lookup"><span data-stu-id="f4b64-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="f4b64-105">Saate nimeserverikirjeid luua või redigeerida domeeniregistraatori juures.</span><span class="sxs-lookup"><span data-stu-id="f4b64-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="f4b64-106">Avage domeeniregistraatori veebisait ja otsige sealt ala, kus saate nimeservereid redigeerida.</span><span class="sxs-lookup"><span data-stu-id="f4b64-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="f4b64-107">Looge või redigeerige nimeserveri väärtusi, nii et need vastaksid järgmistele aadressidele:</span><span class="sxs-lookup"><span data-stu-id="f4b64-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="f4b64-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="f4b64-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="f4b64-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="f4b64-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="f4b64-110">Salvestage muudatused.</span><span class="sxs-lookup"><span data-stu-id="f4b64-110">Save changes.</span></span>

<span data-ttu-id="f4b64-111">Üksikasjalikud juhised leiate ka järgmisest artiklist. [Nimeserverite muutmine teenuskomplekti Office 365 häälestamiseks mis tahes domeeniregistraatoriga](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="f4b64-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  