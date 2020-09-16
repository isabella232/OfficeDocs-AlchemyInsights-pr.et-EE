---
title: AIP-i siltide poliitikate loomine
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732171"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="65a54-102">AIP-i siltide poliitikate loomine</span><span class="sxs-lookup"><span data-stu-id="65a54-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="65a54-103">Azure Information Protection (AIP) silte saab kasutada kõigi andmete kogumiseks, mida organisatsioon tavaliselt loob ja säilitab isikuandmete väikseima klassifikatsiooni põhjal Väga konfidentsiaalsete andmete kõrgeima klassifikatsiooni.</span><span class="sxs-lookup"><span data-stu-id="65a54-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="65a54-104">Azure ' i teabe kaitsmise poliitika rakendub Azure ' i teabe kaitse (AIP) klassikalisele kliendile, mitte AIP-i  [ühtsele märgistamise kliendile](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="65a54-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="65a54-105">Saate AIP-i poliitikas konfigureerida mitu elementi (sh järgmisi võimalusi).</span><span class="sxs-lookup"><span data-stu-id="65a54-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="65a54-106">Suvand, mille sildil saavad administraatorid või kasutaja klassifitseerida ja kaitsta (valikuline) dokumente ja meilisõnumeid</span><span class="sxs-lookup"><span data-stu-id="65a54-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="65a54-107">Valik jõustada klassifikatsioon, kui kasutajad salvestavad dokumente ja saadavad meilisõnumeid</span><span class="sxs-lookup"><span data-stu-id="65a54-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="65a54-108">Suvand meilisõnumi automaatseks sildistamiseks selle manuste põhjal.</span><span class="sxs-lookup"><span data-stu-id="65a54-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="65a54-109">Suvand, et määrata, kas Office ' i rakendustes kuvatakse teave kaitse riba kohta</span><span class="sxs-lookup"><span data-stu-id="65a54-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="65a54-110">Lisateavet Azure ' i teabeõiguste kaitse poliitikate kohta leiate teemast [Azure ' i teabe kaitse poliitika ülevaade](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="65a54-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="65a54-111">Muid võimalusi AIP-i poliitikate kohta leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="65a54-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="65a54-112">Õpetus: Azure ' i teabe kaitsmise poliitika sätete konfigureerimine ja uue sildi loomine</span><span class="sxs-lookup"><span data-stu-id="65a54-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="65a54-113">Azure ' i teabe kaitse poliitika konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="65a54-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="65a54-114">Tundlikkuse siltide ja nende poliitikate loomine ja konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="65a54-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="65a54-115">Juhised Azure ' i teabeõiguste kaitset kasutavate levinumate stsenaariumite jaoks</span><span class="sxs-lookup"><span data-stu-id="65a54-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="65a54-116">Azure ' i teabe kaitse dokumentatsiooni läbivaatamine</span><span class="sxs-lookup"><span data-stu-id="65a54-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="65a54-117">Azure ' i teabe kaitse nõuded</span><span class="sxs-lookup"><span data-stu-id="65a54-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="65a54-118">Azure ' i teabe kaitse Lühijuhend</span><span class="sxs-lookup"><span data-stu-id="65a54-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="65a54-119">Azure ' i teabe kaitse klientrakenduse allalaadimine</span><span class="sxs-lookup"><span data-stu-id="65a54-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)