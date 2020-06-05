---
title: AIP-sildi poliitikate loomine
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569034"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="a14a2-102">AIP-sildi poliitikate loomine</span><span class="sxs-lookup"><span data-stu-id="a14a2-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="a14a2-103">Azure ' i teabekaitse (AIP) silte saab kasutada koos kõigi andmehulga andmetega, mida organisatsioon tavaliselt loob ja talletab, alates väikseimast isikuandmete liigitust väga konfidentsiaalsete andmete kõrgeimale liigitusele.</span><span class="sxs-lookup"><span data-stu-id="a14a2-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="a14a2-104">Azure ' i teabe kaitse poliitikad rakenduvad Azure Protection (AIP) klassikaline klient ja mitte [AIP ühendatud märgistamise klient](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="a14a2-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="a14a2-105">Saate konfigureerida AIP-i poliitikas mitu elementi, sealhulgas järgmised valikud:</span><span class="sxs-lookup"><span data-stu-id="a14a2-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="a14a2-106">Valik, mille silt võimaldab administraatoritel või kasutajal klassifitseerida ja kaitsta (valikuline) dokumente ja e-kirju</span><span class="sxs-lookup"><span data-stu-id="a14a2-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="a14a2-107">Võimalus jõustada klassifikatsioon, kui kasutajad salvestavad dokumente ja saadavad meili</span><span class="sxs-lookup"><span data-stu-id="a14a2-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="a14a2-108">Võimalus automaatselt Sildista e-kirja, mis põhineb selle manuseid.</span><span class="sxs-lookup"><span data-stu-id="a14a2-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="a14a2-109">Võimalus kontrollida, kas teabekaitse riba kuvatakse Office ' i rakendused</span><span class="sxs-lookup"><span data-stu-id="a14a2-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="a14a2-110">Lisateavet Azure ' i teabekaitse poliitikate kohta leiate teemast: [Azure ' i teabekaitse poliitika ülevaade](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="a14a2-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="a14a2-111">Muud kasulikud ressursid AIP poliitika kohta vt:</span><span class="sxs-lookup"><span data-stu-id="a14a2-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="a14a2-112">Õpetus: Azure ' i teabekaitse poliitikasätete konfigureerimine ja uue sildi loomine</span><span class="sxs-lookup"><span data-stu-id="a14a2-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="a14a2-113">Azure ' i teabe kaitse poliitika konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="a14a2-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="a14a2-114">Tundlikkuse siltide ja nende poliitikate loomine ja konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="a14a2-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="a14a2-115">Kuidas-juhised levinud stsenaariumid, mis kasutavad Azure ' i teabekaitse</span><span class="sxs-lookup"><span data-stu-id="a14a2-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="a14a2-116">Azure ' i teabekaitse dokumentatsiooni läbivaatamine</span><span class="sxs-lookup"><span data-stu-id="a14a2-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="a14a2-117">Azure ' i teabekaitse nõuded</span><span class="sxs-lookup"><span data-stu-id="a14a2-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="a14a2-118">Quick Start juhendaja Azure ' i teabekaitse</span><span class="sxs-lookup"><span data-stu-id="a14a2-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="a14a2-119">Laadige alla Azure ' i teabekaitse klient</span><span class="sxs-lookup"><span data-stu-id="a14a2-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)