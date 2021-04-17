---
title: 'AIP: poliitikad ei käitu ootuspäraselt'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821623"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="3d6ea-102">AIP: poliitikad ei käitu ootuspäraselt</span><span class="sxs-lookup"><span data-stu-id="3d6ea-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="3d6ea-103">Azure'i teabekaitse: poliitikad ei käitu ootuspäraselt, erinevate poliitikaprobleemide kohta leiate järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="3d6ea-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="3d6ea-104">Kui teil on visuaalse märgistusega probleeme, vaadake üle, [kui rakendatakse visuaalseid märgistusi.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="3d6ea-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="3d6ea-105">Kui teil on probleeme automaatse sildistusfunktsiooniga, lugege teemat Kuidas konfigureerida [Azure'i](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) teabekaitse automaatse ja soovitatava liigituse tingimusi ja mida tundliku [loomuga teabetüübid pakuvad.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="3d6ea-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="3d6ea-106">Kui teil on probleeme native/Pfile'i kaitsega, vaadake üle faili [API konfiguratsioon.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="3d6ea-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="3d6ea-107">Kontrollige, kas kasutate ulatusega poliitikaid, mis pole õigesti konfigureeritud: Azure'i teabekaitsepoliitika konfigureerimine kindlate kasutajate jaoks [ulatusega poliitikate abil.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="3d6ea-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="3d6ea-108">Kui sildistatud dokumendi manustamisel ei tööta Outlookis automaatne sildistamine, veenduge, et DRMEncryptProperty pole määratletud [järgmiselt: IRM-i registrisätted turbe jaoks.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="3d6ea-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="3d6ea-109">Kui teil esineb endiselt probleeme, koguge Azure'i teabekaitse kliendi logid ja manustage eksporditud logid sellele piletile.</span><span class="sxs-lookup"><span data-stu-id="3d6ea-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="3d6ea-110">Avage Office'i dokument või looge Outlookis uus meilisõnum.</span><span class="sxs-lookup"><span data-stu-id="3d6ea-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="3d6ea-111">Klõpsake **nuppu Kaitse/tundlikkuse**  >  **spikker ja tagasiside.**</span><span class="sxs-lookup"><span data-stu-id="3d6ea-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="3d6ea-112">Klõpsake **nuppu Ekspordi logid.**</span><span class="sxs-lookup"><span data-stu-id="3d6ea-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="3d6ea-113">Salvestage logid oma asukohavalikusse ja manustage need sellele teenusetaotlusele.</span><span class="sxs-lookup"><span data-stu-id="3d6ea-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="3d6ea-114">Lisaressursid:</span><span class="sxs-lookup"><span data-stu-id="3d6ea-114">Additional resources:</span></span>

- [<span data-ttu-id="3d6ea-115">Azure'i teabekaitse jaoks visuaalsete märgistuste sildi konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="3d6ea-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="3d6ea-116">Azure'i teabekaitse dokumentatsiooni läbivaatamine</span><span class="sxs-lookup"><span data-stu-id="3d6ea-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="3d6ea-117">Tundlikkussiltide kasutamine Microsoft 365 rakendustes</span><span class="sxs-lookup"><span data-stu-id="3d6ea-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

