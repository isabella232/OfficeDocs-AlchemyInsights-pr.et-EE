---
title: Tundlikkussilte ei kuvata
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207221"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="6997b-102">Tundlikkussilte ei kuvata</span><span class="sxs-lookup"><span data-stu-id="6997b-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="6997b-103">Tundlikkuse sildid võimaldavad teil oma tundliku sisuga sisu klassifitseerida ja kaitsta.</span><span class="sxs-lookup"><span data-stu-id="6997b-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="6997b-104">Neid saab luua Microsoft 365 vastavuse keskus, Microsoft 365 Turvakeskus või Office 365 Security & vastavuse Center jaotises klassifikatsioon > tundlikkuse sildid.</span><span class="sxs-lookup"><span data-stu-id="6997b-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Office 365 Security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="6997b-105">Selle funktsiooni kohta lisateabe saamiseks vaadake [tundlikkuse siltide ülevaade](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="6997b-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="6997b-106">Kui konfigureerisite tundlikkuse silte, kuid neid ei kuvata Office ' i rakendustes, kontrollige järgmist.</span><span class="sxs-lookup"><span data-stu-id="6997b-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="6997b-107">Kinnitage, et tundlikkuse silt on [avaldatud](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) soovitud kasutajatele ja rühmadele.</span><span class="sxs-lookup"><span data-stu-id="6997b-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="6997b-108">Kinnitage, et kasutaja kasutab tundlikkussilte toetavat rakendust – vt [dokumendi tundlikkuse silte](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="6997b-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span></span>

- <span data-ttu-id="6997b-109">Kui [migreerite Azure ' i teabekaitse silte](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), arvestage [siin](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)loetletud kaalutlustega.</span><span class="sxs-lookup"><span data-stu-id="6997b-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="6997b-110">Andmete kadu vältimine (DLP) tugi: praegu ainult Säilitussildid saab kasutada tingimus DLP poliitika.</span><span class="sxs-lookup"><span data-stu-id="6997b-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="6997b-111">Tundlikkuse sildid DLP poliitika tugi ei ole veel saadaval, kuid me töötame selle kallal.</span><span class="sxs-lookup"><span data-stu-id="6997b-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="6997b-112">Kui tundlikkuse sildil on krüptimine lubatud, saate valida kas:</span><span class="sxs-lookup"><span data-stu-id="6997b-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="6997b-113">Määra õigused kohe</span><span class="sxs-lookup"><span data-stu-id="6997b-113">Assign permissions now</span></span>
    - <span data-ttu-id="6997b-114">Luba kasutajatel õigusi määrata</span><span class="sxs-lookup"><span data-stu-id="6997b-114">Let users assign permissions</span></span>


<span data-ttu-id="6997b-115">Võimalike probleemide kohta lisateabe saamiseks vaadake [teadaolevad probleemid tundlikkuse sildid](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="6997b-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>