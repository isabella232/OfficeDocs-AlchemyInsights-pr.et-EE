---
title: 'AIP: poliitikad ei käitudes ootuspäraselt'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506554"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="350f6-102">AIP: poliitikad ei käitudes ootuspäraselt</span><span class="sxs-lookup"><span data-stu-id="350f6-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="350f6-103">Azure ' i teabekaitse: poliitikad ei käitudes ootuspäraselt, vt soovitatud juhised erinevate poliitikafunte:</span><span class="sxs-lookup"><span data-stu-id="350f6-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="350f6-104">Kui teil on visuaalsete märgistuste probleemid, vaadake üle [visuaalsete märgiste kohaldamise](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)korral.</span><span class="sxs-lookup"><span data-stu-id="350f6-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="350f6-105">Kui teil on probleeme automaatse märgistamise, vaadake üle, [Kuidas konfigureerida tingimused automaatse ja soovitatud klassifitseerimise Azure ' i teabekaitse](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ja [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="350f6-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="350f6-106">Kui teil on probleeme Native/Pfile kaitse, vaadake [faili API konfiguratsiooni](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="350f6-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="350f6-107">Kontrollige, kas kasutate hõlmavaid poliitikaid, mis pole õigesti konfigureeritud: [Kuidas konfigureerida Azure ' i teabe kaitse poliitika teatud kasutajatele, kasutades ulatatud poliitikad](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="350f6-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="350f6-108">Kui automaatne märgistamine ei tööta Outlooki sildistatud dokumendi ühendamisel, veenduge, et DRMEncryptProperty pole määratletud siin kirjeldatud: [IRM registrisätted turvalisuse](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="350f6-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="350f6-109">Kui teil on endiselt probleeme, palun koguda Azure ' i teabe kaitse kliendi logid ja kinnitage eksporditud logid sellele piletile.</span><span class="sxs-lookup"><span data-stu-id="350f6-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="350f6-110">Avage Office ' i dokument või looge Outlookis uus e-kiri.</span><span class="sxs-lookup"><span data-stu-id="350f6-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="350f6-111">Klõpsake valikul **kaitse/tundlikkuse**  >  **Spikker ja tagasiside**.</span><span class="sxs-lookup"><span data-stu-id="350f6-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="350f6-112">Klikkige käsul **ekspordi logid**.</span><span class="sxs-lookup"><span data-stu-id="350f6-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="350f6-113">Salvestage logid oma asukoha valikule ja kinnitage need selle teenusetaotlusega.</span><span class="sxs-lookup"><span data-stu-id="350f6-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="350f6-114">Lisaressursid:</span><span class="sxs-lookup"><span data-stu-id="350f6-114">Additional resources:</span></span>

- [<span data-ttu-id="350f6-115">Kuidas konfigureerida sildile visuaalseid märgistusi Azure ' i teabekaitse</span><span class="sxs-lookup"><span data-stu-id="350f6-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="350f6-116">Azure ' i teabekaitse dokumentatsiooni läbivaatamine</span><span class="sxs-lookup"><span data-stu-id="350f6-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="350f6-117">Tundlikkuse siltide kasutamine Office ' i rakendustes</span><span class="sxs-lookup"><span data-stu-id="350f6-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

