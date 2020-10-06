---
title: Tingimusliku juurdepääsu jälgimine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366424"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="a9f6b-102">Exchange ' i tingimisi juurdepääsu jälgimine</span><span class="sxs-lookup"><span data-stu-id="a9f6b-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="a9f6b-103">Juurdepääsuõigusega kasutajatele antakse teatise meilisõnum, kui need ei vasta teie asutuse juurdepääsu nõuetele.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="a9f6b-104">Lahendamiseks soovitame teha ühte või mitut järgmistest lahendustest.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="a9f6b-105">Kui eeldatakse, et seade on registreeritud, Soovitage kasutajal minna ettevõtte portaali rakendusse ja veenduge, et see kuvatakse ettevõtte portaalis.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="a9f6b-106">Kui seda ei juhtu, peaks kasutaja seadme registreerima.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="a9f6b-107">Azure ' i portaalis avage > seadme nõuetele vastavuse häälestamine.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="a9f6b-108">Klõpsake jaotises kuvar nuppu seadme nõuetele vastavus.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="a9f6b-109">Vaadake seadme nõuetele vastavuse aruandeid, et veenduda, kas kasutaja seade on märgitud nõuetele vastavaks.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="a9f6b-110">Azure ' i portaalis avage > seadme nõuetele vastavuse häälestamine.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="a9f6b-111">Klõpsake jaotises haldamine nuppu poliitikad.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-111">Under Manage, click Policies.</span></span> <span data-ttu-id="a9f6b-112">Veenduge, et nõuetele vastavuse poliitikate loendis oleks teie kasutaja seadmele määratud profiil.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="a9f6b-113">Kui profiili pole määratud, ei saa Intune kinnitada seadme nõuetele vastavuse olekut.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="a9f6b-114">Kasutaja tingimusliku juurdepääsu määramise redigeerimine.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="a9f6b-115">Azure ' i portaalis Avage **Intune**  >  **tingimusjuurdepääsu**  >  **poliitikate**häälestamine.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="a9f6b-116">Valige loendist poliitika.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="a9f6b-117">Klõpsake nuppu kasutajad ja rühmad.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-117">Click Users and groups.</span></span>
4. <span data-ttu-id="a9f6b-118">Kellegile teatud poliitika suunamiseks lisage need loendisse kaasa.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="a9f6b-119">Kui soovite tagada, et isik on poliitikast välja jäetud, lisage need loendisse välista.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="a9f6b-120">Kasulikud lingid:</span><span class="sxs-lookup"><span data-stu-id="a9f6b-120">Helpful links:</span></span>

[<span data-ttu-id="a9f6b-121">Seadme nõuetele vastavuse ülevaade</span><span class="sxs-lookup"><span data-stu-id="a9f6b-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="a9f6b-122">Tõrkeotsing CA</span><span class="sxs-lookup"><span data-stu-id="a9f6b-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="a9f6b-123">Tõrkeotsingu poliitika</span><span class="sxs-lookup"><span data-stu-id="a9f6b-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="a9f6b-124">Seadme nõuetele vastavuse jälgimine</span><span class="sxs-lookup"><span data-stu-id="a9f6b-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="a9f6b-125">Märkus: need toimingud on abiks ainult Azure Active Directory tõrkeotsingul.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="a9f6b-126">Samuti on võimalik sulgeda seade, mis blokeerib juurdepääsu Exchange ' i poliitikaga.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="a9f6b-127">Lisateavet Exchange ' i seadmete halduse kohta leiate [siit](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="a9f6b-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
