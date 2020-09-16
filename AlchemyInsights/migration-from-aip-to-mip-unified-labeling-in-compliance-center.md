---
title: Üleminek AIP-ist kuni MIP/ühtse märgistamiseni vastavuse keskuses
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674322"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="18892-102">Üleminek AIP-ist kuni MIP/ühtse märgistamiseni vastavuse keskuses</span><span class="sxs-lookup"><span data-stu-id="18892-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="18892-103">Üleminekuks AIP-i siltidelt turbe-ja vastavuskontrolli keskuses ühendatud siltidele tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="18892-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="18892-104">**Azure ' i portaalis kaitse aktiveerimine**</span><span class="sxs-lookup"><span data-stu-id="18892-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="18892-105">Kui te pole seda veel teinud, avage uus brauseriaknas ja [logige sisse Azure ' i portaali](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="18892-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="18892-106">Liikuge **Azure ' i teabe kaitse** labale.</span><span class="sxs-lookup"><span data-stu-id="18892-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="18892-107">Näiteks klõpsake menüüs keskus käsku **kõik teenused** ja hakake tippima **teavet** väljale filter.</span><span class="sxs-lookup"><span data-stu-id="18892-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="18892-108">Valige **Azure ' i teabe kaitse**.</span><span class="sxs-lookup"><span data-stu-id="18892-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="18892-109">Kui te pole Azure ' i teabe kaitse Blade ' i varem kasutanud, lugege [lisajuhiseid](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) selle tera lisamiseks portaali.</span><span class="sxs-lookup"><span data-stu-id="18892-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="18892-110">Azure ' i teabe kaitse Blade avamiseks peab teil olema kas Azure ' i [teabe kaitse Premiumi leping](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) või Office 365 leping, mis sisaldab õiguste haldust.</span><span class="sxs-lookup"><span data-stu-id="18892-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="18892-111">Kui teil on üks neist tellimustest, kuid kuvatakse teade selle kohta, et kehtivat tellimust ei leita, [võtke ühendust Microsofti toega](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) või kasutage standardseid kasutajatoe kanaleid.</span><span class="sxs-lookup"><span data-stu-id="18892-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="18892-112">Leidke menüü **Halda** suvandid ja valige **kaitse aktiveerimine**.</span><span class="sxs-lookup"><span data-stu-id="18892-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="18892-113">Klõpsake nuppu **Aktiveeri**ja seejärel kinnitage oma toiming.</span><span class="sxs-lookup"><span data-stu-id="18892-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="18892-114">Kui aktiveerimine on lõpule jõudnud, kuvab teaberiba **aktiveerimine edukalt**.</span><span class="sxs-lookup"><span data-stu-id="18892-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="18892-115">**Azure ' i teabe kaitse siltide migreerimine Office 365 turbe & nõuetele vastavuse keskuses**</span><span class="sxs-lookup"><span data-stu-id="18892-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="18892-116">Veenduge, et olete sisse logitud üldise administraatori õigustega kasutajana.</span><span class="sxs-lookup"><span data-stu-id="18892-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="18892-117">Liikuge **Azure ' i teabe kaitse** labale.</span><span class="sxs-lookup"><span data-stu-id="18892-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="18892-118">Valige menüüst **Halda** suvand **ühendatud silt**.</span><span class="sxs-lookup"><span data-stu-id="18892-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="18892-119">Klõpsake **Azure ' i teabe kaitsega ühendatud sildiga** Blade nuppu **Aktiveeri** ja järgige veebijuhiseid.</span><span class="sxs-lookup"><span data-stu-id="18892-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="18892-120">**Märkus**: Veenduge, et teil oleks enne turbe & ühilduvuse keskuse migreerimise aktiveerimiseks vajalikud load.</span><span class="sxs-lookup"><span data-stu-id="18892-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="18892-121">Lisateavet leiate järgmistest artiklitest:</span><span class="sxs-lookup"><span data-stu-id="18892-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="18892-122">Kas peate Azure ' i teabe kaitse konfigureerimiseks olema üldadministraator või saan anda teistele administraatoritele delegaadi?</span><span class="sxs-lookup"><span data-stu-id="18892-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="18892-123">Oluline teave administratiivsete rollide kohta pärast turbe & nõuetele vastavuse keskuse migreerimist.</span><span class="sxs-lookup"><span data-stu-id="18892-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="18892-124">Lisateavet AIP-i kohta, et ühendatud siltide migreerimine turbe-ja vastavuskontrolli keskusse, leiate teemast [siltide migreerimine](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="18892-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
