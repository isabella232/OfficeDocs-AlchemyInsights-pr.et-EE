---
title: Tingimusjuurdepääsu Intune Accessi jälgimine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427425"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="ff0f9-102">Tingimusjuurdepääsu Intune Accessi jälgimine</span><span class="sxs-lookup"><span data-stu-id="ff0f9-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="ff0f9-103">Juurdepääsuõigusega kasutajatele antakse teatise meilisõnum, kui need ei vasta teie asutuse juurdepääsu nõuetele.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="ff0f9-104">Lahendamiseks soovitame teha ühte või mitut järgmistest lahendustest.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="ff0f9-105">Kui eeldatakse, et seade on registreeritud, Soovitage kasutajal minna ettevõtte portaali rakendusse ja veenduge, et see kuvatakse ettevõtte portaalis.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="ff0f9-106">Kui seda ei juhtu, peab kasutaja seadme registreerima.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="ff0f9-107">Avage Azure ' i portaalis   >  **seadme nõuetele vastavuse** häälestamine.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="ff0f9-108">Seadme nõuetele vastavuse aruannete vaatamiseks veendumaks, et kasutaja seade on märgitud nõuetele vastavaks, klõpsake jaotises **kuvar** nuppu **seadme vastavus**.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="ff0f9-109">Avage Azure ' i portaalis   >  **seadme nõuetele vastavuse** häälestamine.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="ff0f9-110">Klõpsake jaotises **haldamine** nuppu **poliitikad**.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="ff0f9-111">Veenduge, et nõuetele vastavuse poliitikate loendis oleks teie kasutaja seadmele määratud profiil.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="ff0f9-112">Kui profiili pole määratud, ei saa Intune kinnitada seadme nõuetele vastavuse olekut.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="ff0f9-113">Kasutaja tingimusliku juurdepääsu määramise redigeerimine.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="ff0f9-114">Liikuge Azure ' i portaalis lehele  >  **tingimusjuurdepääsu**  >  **poliitikate** häälestamine, valige loendist poliitika ja klõpsake nuppu **kasutajad ja rühmad**.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="ff0f9-115">Kellegile teatud poliitika suunamiseks lisage need **loendisse kaasa**.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="ff0f9-116">Kui soovite tagada, et isik on poliitikast välja jäetud, lisage need loendisse **välista**.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="ff0f9-117">**Kasulikud lingid:**</span><span class="sxs-lookup"><span data-stu-id="ff0f9-117">**Helpful links:**</span></span>

- [<span data-ttu-id="ff0f9-118">Seadme nõuetele vastavuse ülevaade</span><span class="sxs-lookup"><span data-stu-id="ff0f9-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="ff0f9-119">Tõrkeotsing CA</span><span class="sxs-lookup"><span data-stu-id="ff0f9-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="ff0f9-120">Tõrkeotsingu poliitika</span><span class="sxs-lookup"><span data-stu-id="ff0f9-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="ff0f9-121">Seadme nõuetele vastavuse jälgimine</span><span class="sxs-lookup"><span data-stu-id="ff0f9-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="ff0f9-122">Need toimingud on abiks ainult Azure Active Directory tõrkeotsingul.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="ff0f9-123">Samuti on võimalik sulgeda seade, mis blokeerib juurdepääsu Exchange ' i poliitikaga.</span><span class="sxs-lookup"><span data-stu-id="ff0f9-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="ff0f9-124">Lisateavet Exchange ' i seadmete halduse kohta leiate [**siit**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="ff0f9-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
