---
title: 'AIP-skanner: paigaldamine ja konfigureerimine'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357661"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="7fb61-102">AIP-skanner: paigaldamine ja konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="7fb61-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="7fb61-103">**AIP skanneri installimiseks järgige soovitatud juhiseid**.</span><span class="sxs-lookup"><span data-stu-id="7fb61-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="7fb61-104">Kui täiendate ja ei tee puhast installi, veenduge, et olete järginud juhiseid [Azure ' i teabe kaitse skanneri](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) ja ühendatud märgistamise kliendi täiendamine, vaadake [Azure ' i teabe kaitse skanneri täiendamine](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="7fb61-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="7fb61-105">Veenduge, et te järgite kõiki [tulemüüride ja võrgu infrastruktuuri seadete nõudeid](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="7fb61-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="7fb61-106">Veenduge, et teie [poliitikad on seatud](https://docs.microsoft.com/azure/information-protection/configure-policy) automaatne märgistamine või on vaikimisi silt poliitika.</span><span class="sxs-lookup"><span data-stu-id="7fb61-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="7fb61-107">Veenduge, et vastav failitüüp on konfigureeritud sildi/kaitse puhul, nagu on kirjeldatud [Azure ' i teabekaitse kliendi toetatud failitüüpide](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)puhul.</span><span class="sxs-lookup"><span data-stu-id="7fb61-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="7fb61-108">Lisaks, kui soovite muuta vaikekäitumist, järgige neid juhiseid: [muuta failide vaikimisi kaitse tase](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="7fb61-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="7fb61-109">Veenduge, et skanneri teenuse käivitamiseks konfigureeritud kasutajakontole on juurdepääsuõigused kõigile konfigureeritud hoidlates.</span><span class="sxs-lookup"><span data-stu-id="7fb61-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="7fb61-110">Kui teil esineb endiselt probleeme, siis eksportike skanneri logid ja lisage need oma toe pilet.</span><span class="sxs-lookup"><span data-stu-id="7fb61-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="7fb61-111">**Ekspordi Azure ' i teabe kaitse skanner logid**</span><span class="sxs-lookup"><span data-stu-id="7fb61-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="7fb61-112">Liikuge%localappdata%\Microsoft\MSIP skanneri teenust käitavas kasutajakonteksti all.</span><span class="sxs-lookup"><span data-stu-id="7fb61-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="7fb61-113">ZIP kogu sisu MSIP kausta.</span><span class="sxs-lookup"><span data-stu-id="7fb61-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="7fb61-114">Salvestage logid oma asukoha valikule ja kinnitage need oma teenustaotlusele.</span><span class="sxs-lookup"><span data-stu-id="7fb61-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="7fb61-115">Võite kasutada ka [ekspordi-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="7fb61-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="7fb61-116">**Lisateabe saamiseks vt**:</span><span class="sxs-lookup"><span data-stu-id="7fb61-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="7fb61-117">Azure ' i teabekaitse skanneri juurutamine failide automaatseks klassifitseerimiseks ja kaitsmiseks</span><span class="sxs-lookup"><span data-stu-id="7fb61-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="7fb61-118">Määrake ja kasutage Set-AIPAuthentication loa parameeter</span><span class="sxs-lookup"><span data-stu-id="7fb61-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="7fb61-119">Tuvastustsükli käivitamine ja skanneri aruannete vaatamine</span><span class="sxs-lookup"><span data-stu-id="7fb61-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="7fb61-120">Azure ' i teabekaitse dokumentatsiooni läbivaatamine</span><span class="sxs-lookup"><span data-stu-id="7fb61-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="7fb61-121">Azure ' i teabekaitse nõuded</span><span class="sxs-lookup"><span data-stu-id="7fb61-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="7fb61-122">Laadige alla Azure ' i teabekaitse klient</span><span class="sxs-lookup"><span data-stu-id="7fb61-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
