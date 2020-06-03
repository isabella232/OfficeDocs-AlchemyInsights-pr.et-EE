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
ms.openlocfilehash: f295e0d7872a13cf47e386343b159e51bc0504de
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508084"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="47467-102">Domeeni nimeserverite värskendamine osutama Microsoftile</span><span class="sxs-lookup"><span data-stu-id="47467-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="47467-103">Märkus. Nimeserveri muudatuste levitamiseks võib vahel kuluda kuni 48 tundi.</span><span class="sxs-lookup"><span data-stu-id="47467-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="47467-104">Domeeni häälestamiseks teenusekomplektis Microsoft 365 tuleb nimeserverid domeeniregistripidaja juures värskendada.</span><span class="sxs-lookup"><span data-stu-id="47467-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="47467-105">Saate nimeserverikirjeid luua või redigeerida domeeniregistraatori juures.</span><span class="sxs-lookup"><span data-stu-id="47467-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="47467-106">Avage domeeniregistraatori veebisait ja otsige sealt ala, kus saate nimeservereid redigeerida.</span><span class="sxs-lookup"><span data-stu-id="47467-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="47467-107">Looge või redigeerige nimeserveri väärtusi, nii et need vastaksid järgmistele aadressidele:</span><span class="sxs-lookup"><span data-stu-id="47467-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="47467-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="47467-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="47467-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="47467-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="47467-110">Salvestage muudatused.</span><span class="sxs-lookup"><span data-stu-id="47467-110">Save changes.</span></span>

<span data-ttu-id="47467-111">Üksikasjalikud juhised leiate ka järgmisest artiklist. [Nimeserverite muutmine mis tahes domeeniregistraatoriga](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="47467-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  