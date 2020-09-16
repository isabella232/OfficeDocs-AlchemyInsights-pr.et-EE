---
title: Tundlikkuse sildid, mida ei esine
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801180"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="3aa26-102">Tundlikkuse sildid, mida ei esine</span><span class="sxs-lookup"><span data-stu-id="3aa26-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="3aa26-103">Tundlikkuse siltide abil saate oma tundliku sisu klassifitseerida ja kaitsta.</span><span class="sxs-lookup"><span data-stu-id="3aa26-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="3aa26-104">Neid saab luua Microsoft 365 nõuetele vastavuse keskuses, Microsoft 365 Turvakeskus või Microsoft 365 turbe & nõuetele vastavuse Center jaotises klassifitseerimine > tundlikkuse sildid.</span><span class="sxs-lookup"><span data-stu-id="3aa26-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="3aa26-105">Lisateavet selle funktsiooni kohta leiate teemast [tundlikkuse siltide ülevaade](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="3aa26-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="3aa26-106">Kui olete konfigureerinud oma tundlikkuse sildid, kuid neid ei kuvata Microsoft 365 rakendustes, kontrollige järgmist.</span><span class="sxs-lookup"><span data-stu-id="3aa26-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="3aa26-107">Kontrollige, kas tundlikkuse silt on teie soovitud kasutajatele ja rühmadele [avaldatud](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) .</span><span class="sxs-lookup"><span data-stu-id="3aa26-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="3aa26-108">Veenduge, et kasutaja kasutab tundlikke silte toetavat rakendust – vt [dokumendis olevaid tundlikkuse silte](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="3aa26-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="3aa26-109">Kui [migreerite Azure ' i teabe kaitse silte](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), pidage silmas [siin](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)loetletud kaalutlusi.</span><span class="sxs-lookup"><span data-stu-id="3aa26-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="3aa26-110">Andmete kaotsimineku vältimise (DLP) tugi: praegu saab DLP poliitika tingimusena kasutada ainult säilituse silte.</span><span class="sxs-lookup"><span data-stu-id="3aa26-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="3aa26-111">DLP poliitikale mõeldud tundlikkuse siltide tugi pole veel saadaval, kuid me töötame selle kallal.</span><span class="sxs-lookup"><span data-stu-id="3aa26-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="3aa26-112">Kui krüptimine on lubatud tundlikkuse sildil, saate valida, kas soovite teha järgmist.</span><span class="sxs-lookup"><span data-stu-id="3aa26-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="3aa26-113">Õiguse määramine kohe</span><span class="sxs-lookup"><span data-stu-id="3aa26-113">Assign permissions now</span></span>
    - <span data-ttu-id="3aa26-114">Kasutajatele õiguse määramise lubamine</span><span class="sxs-lookup"><span data-stu-id="3aa26-114">Let users assign permissions</span></span>


<span data-ttu-id="3aa26-115">Võimalike probleemide kohta leiate lisateavet teemast [teadaolevad probleemid tundlikkuse siltidega](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="3aa26-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>