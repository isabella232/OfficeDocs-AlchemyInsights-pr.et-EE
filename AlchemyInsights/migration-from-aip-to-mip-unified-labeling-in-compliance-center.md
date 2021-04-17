---
title: Migreerimine AIP-st MIP-sse/ühtseks sildistuskeskuses
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825367"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="c05a2-102">Migreerimine AIP-st MIP-sse/ühtseks sildistuskeskuses</span><span class="sxs-lookup"><span data-stu-id="c05a2-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="c05a2-103">Turbe- ja vastavuskeskuses AIP-siltidelt ühtsele sildistusele migreerimiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="c05a2-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="c05a2-104">**Kaitse aktiveerimine Azure'i portaali kaudu**</span><span class="sxs-lookup"><span data-stu-id="c05a2-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="c05a2-105">Kui te pole seda veel teinud, avage uus brauseriaken ja [logige sisse Azure'i portaali.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="c05a2-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="c05a2-106">Liikuge **Azure'i teabekaitse terale.**</span><span class="sxs-lookup"><span data-stu-id="c05a2-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="c05a2-107">Näiteks klõpsake jaoturi menüüs käsku **Kõik teenused** ja hakake **tippima väljale** Filter teksti Teave.</span><span class="sxs-lookup"><span data-stu-id="c05a2-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="c05a2-108">Valige **Azure'i teabekaitse**.</span><span class="sxs-lookup"><span data-stu-id="c05a2-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="c05a2-109">Kui te pole varem Azure'i teabekaitse labale [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) juurde pääsenud, lugege selle lõiketera portaali lisamiseks järgmisi täiendavaid juhiseid.</span><span class="sxs-lookup"><span data-stu-id="c05a2-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="c05a2-110">Azure'i teabekaitse tera avamiseks peab teil olema [Azure'i teabekaitse Premiumi leping](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) või Office 365 leping, mis sisaldab õiguste haldust.</span><span class="sxs-lookup"><span data-stu-id="c05a2-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="c05a2-111">Kui teil on mõni neist tellimustest, kuid kuvatakse teade, et kehtivat tellimust ei leita, pöörduge [Microsofti toe poole](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) või kasutage oma standardseid tugikanaleid.</span><span class="sxs-lookup"><span data-stu-id="c05a2-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="c05a2-112">Otsige üles **menüü haldamissuvandid** ja valige **Kaitse aktiveerimine.**</span><span class="sxs-lookup"><span data-stu-id="c05a2-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="c05a2-113">Klõpsake **nuppu** Aktiveeri ja seejärel kinnitage oma toiming.</span><span class="sxs-lookup"><span data-stu-id="c05a2-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="c05a2-114">Kui aktiveerimine on lõpule viidud, kuvatakse teaberibal teade **Aktiveerimine on edukalt lõpule viidud.**</span><span class="sxs-lookup"><span data-stu-id="c05a2-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="c05a2-115">**Azure'i teabekaitse siltide migreerimine Office 365 turbe- & vastavuskeskusesse**</span><span class="sxs-lookup"><span data-stu-id="c05a2-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="c05a2-116">Veenduge, et olete sisse logitud üldadministraatori õigustega kasutajana.</span><span class="sxs-lookup"><span data-stu-id="c05a2-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="c05a2-117">Liikuge **Azure'i teabekaitse terale.**</span><span class="sxs-lookup"><span data-stu-id="c05a2-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="c05a2-118">Valige **menüüs Halda** käsk **Ühendatud sildistamine**.</span><span class="sxs-lookup"><span data-stu-id="c05a2-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="c05a2-119">Klõpsake **Azure'i teabekaitse – ühtse sildistussaba** nuppu **Aktiveeri** ja täitke veebijuhised.</span><span class="sxs-lookup"><span data-stu-id="c05a2-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="c05a2-120">**Märkus.** Enne turbe- ja vastavuskeskuse migreerimise aktiveerimist veenduge, et teil & õigused.</span><span class="sxs-lookup"><span data-stu-id="c05a2-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="c05a2-121">Lisateavet leiate nendest artiklitest.</span><span class="sxs-lookup"><span data-stu-id="c05a2-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="c05a2-122">Kas teil peab olema Azure'i teabekaitse konfigureerimiseks üldadministraator või saan delegeerida selle teistele administraatoritele?</span><span class="sxs-lookup"><span data-stu-id="c05a2-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="c05a2-123">Oluline teave haldusrollide kohta pärast turbe- ja vastavuskeskusesse & migreerimist.</span><span class="sxs-lookup"><span data-stu-id="c05a2-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="c05a2-124">Lisateavet AIP ühtse sildistuse migreerimise kohta turbe- ja vastavuskeskusesse leiate teemast [Siltide migreerimine.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="c05a2-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
