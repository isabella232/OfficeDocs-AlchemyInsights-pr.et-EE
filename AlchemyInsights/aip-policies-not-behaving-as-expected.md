---
title: 'AIP: poliitika ei käitu ootuspäraselt'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663185"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="83e2d-102">AIP: poliitika ei käitu ootuspäraselt</span><span class="sxs-lookup"><span data-stu-id="83e2d-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="83e2d-103">Azure ' i teabe kaitse: poliitikad, mis ei toimi ootuspäraselt, leiate järgmistest teemast Soovitatavad juhised.</span><span class="sxs-lookup"><span data-stu-id="83e2d-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="83e2d-104">Kui teil on probleeme visuaalse märgistusega, vaadake [visuaalse märgistuse rakendamisel](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="83e2d-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="83e2d-105">Kui teil on automaatse sildistamisega probleeme, vaadake, [Kuidas konfigureerida Azure ' i teabe kaitse automaatse ja soovitatava klassifikatsiooni tingimusi](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ning [milliseid tundlikke teabe tüüpe otsida](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="83e2d-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="83e2d-106">Kui teil on emakeelena/Pfile kaitsega probleeme, vaadake läbi selle [API konfiguratsioon](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="83e2d-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="83e2d-107">Kontrollige, kas kasutate ulatusega poliitikaid, mida pole õigesti konfigureeritud: [Kuidas konfigureerida Azure ' i teabe kaitsmise poliitika kindlate kasutajate jaoks ulatusega poliitikate abil](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="83e2d-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="83e2d-108">Kui siltidega dokumendi manustamisel ei tööta automaatne sildistamine Outlooki jaoks, veenduge, et DRMEncryptProperty poleks määratletud, nagu on kirjeldatud siin: [turbe IRM-i registrisätete sätted](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="83e2d-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="83e2d-109">Kui teil esineb endiselt probleeme, palume koguda Azure ' i teabeõiguste kaitse kliendi logisid ja lisada eksporditud logid sellele pilet.</span><span class="sxs-lookup"><span data-stu-id="83e2d-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="83e2d-110">Avage Office ' i dokument või looge Outlookis Uus meilisõnum.</span><span class="sxs-lookup"><span data-stu-id="83e2d-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="83e2d-111">Klõpsake nuppu **kaitse/tundlikkuse**  >  **Spikker ja tagasiside**.</span><span class="sxs-lookup"><span data-stu-id="83e2d-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="83e2d-112">Klõpsake nuppu **ekspordi logid**.</span><span class="sxs-lookup"><span data-stu-id="83e2d-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="83e2d-113">Salvestage logid oma asukoha valikusse ja lisage need selle teenuse taotlusele.</span><span class="sxs-lookup"><span data-stu-id="83e2d-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="83e2d-114">Lisaressursid:</span><span class="sxs-lookup"><span data-stu-id="83e2d-114">Additional resources:</span></span>

- [<span data-ttu-id="83e2d-115">Azure ' i teabe kaitsmiseks mõeldud visuaalsete märkide sildi konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="83e2d-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="83e2d-116">Azure ' i teabe kaitse dokumentatsiooni läbivaatamine</span><span class="sxs-lookup"><span data-stu-id="83e2d-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="83e2d-117">Microsoft 365 rakenduste tundlikkuse siltide kasutamine</span><span class="sxs-lookup"><span data-stu-id="83e2d-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

