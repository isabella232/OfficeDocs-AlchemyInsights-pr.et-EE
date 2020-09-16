---
title: 2681 Attack Simulator Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759215"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="c5629-102">Rünnaku simulaator Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c5629-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="c5629-103">Kas teil on puudu rünnaku simulaator?</span><span class="sxs-lookup"><span data-stu-id="c5629-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="c5629-104">Attack Simulator nõuab **office 365 täpsema ohu kaitse leping 2 (ATP leping 2)** või **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="c5629-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="c5629-105">Rünnaku simulaator pole **kaasatud office** 365 Advanced ohtu kaitse leping 1 (ATP leping 1), Office 365 Enterprise E3 või mis tahes Microsoft 365 rakendused ettevõtetele mõeldud pakettide jaoks.</span><span class="sxs-lookup"><span data-stu-id="c5629-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="c5629-106">Simuleeritud rünnakute käivitamiseks kasutatav konto peab olema üldadministraator või administraatori õigused ja mitme teguriga autentimine (MFA).</span><span class="sxs-lookup"><span data-stu-id="c5629-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="c5629-107">Lisateavet rünnaku simulaatori nõuete kohta leiate [sellest teemast](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="c5629-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="c5629-108">Tähtsamaid asju teada **Brute Force Password** Attack simulatsioonid:</span><span class="sxs-lookup"><span data-stu-id="c5629-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="c5629-109">Kui TARGETi kontol on MFA lubatud ja parool on õigesti kajastatud, ei kuvata kontot ohustatud kujul (teine autentimine on puudulik).</span><span class="sxs-lookup"><span data-stu-id="c5629-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="c5629-110">Parool ei tohi olla suurem kui 10 MB.</span><span class="sxs-lookup"><span data-stu-id="c5629-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="c5629-111">Kasutage ühte parooli rea kohta ja lisage loendi viimasele paroolile tühi rida (veo tagastus).</span><span class="sxs-lookup"><span data-stu-id="c5629-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="c5629-112">Olulised asjad, mida saab teada **oda andmepüügiga** seotud simulatsioonide kohta.</span><span class="sxs-lookup"><span data-stu-id="c5629-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="c5629-113">Kujunduse järgi ei saa te **andmepüügi sisselogimise serveri URL-i**jaoks kohandatud väärtust anda.</span><span class="sxs-lookup"><span data-stu-id="c5629-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="c5629-114">Kui adressaat kasutab teate saatmiseks [lisandmoodulit luba](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) sõnum andmepüügiks, siis ei pruugi te saada sõnumile teatisi (kuna tegemist on simuleeritud rünnakuga).</span><span class="sxs-lookup"><span data-stu-id="c5629-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="c5629-115">Aruanded: pärast simuleeritud rünnaku lõpulejõudmist võite aruande kuvamiseks klõpsata nuppu **rünnaku üksikasjad** .</span><span class="sxs-lookup"><span data-stu-id="c5629-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="c5629-116">Üksikasjalikud juhised ja uued funktsioonid rakenduses Attack Simulator leiate teemast [rünnaku simulaator Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="c5629-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
