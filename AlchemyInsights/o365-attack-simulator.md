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
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545722"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="1b615-102">Attack Simulator Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1b615-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="1b615-103">Kas teil puudub ründesimulaator?</span><span class="sxs-lookup"><span data-stu-id="1b615-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="1b615-104">Ründesimulaatori **kasutamiseks on vaja Microsoft Defenderit Office 365 2** või Office 365 Enterprise **E5 jaoks.**</span><span class="sxs-lookup"><span data-stu-id="1b615-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="1b615-105">**Ründesimulaatorit ei** kaasata Microsoft Defenderi Office 365 1, Office 365 Enterprise E3 ega Microsoft 365 ettevõtterakendused tellimuste jaoks.</span><span class="sxs-lookup"><span data-stu-id="1b615-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="1b615-106">Simuleeritud rünnakute käivitamiseks kasutav konto nõuab üldadministraatori või turbeadministraatori õigusi ja mitme teguriga autentimist (MFA).</span><span class="sxs-lookup"><span data-stu-id="1b615-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="1b615-107">Lisateavet ründesimulaatori nõuete kohta leiate [sellest teemast.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="1b615-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="1b615-108">Oluline teave **Brute Force Passwordi rünnaku simulatsioonide** kohta.</span><span class="sxs-lookup"><span data-stu-id="1b615-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="1b615-109">Kui sihtkontol on lubatud MFA ja parool arvati õigesti ära, ei kuvata kontot ohustatud kontona (teine autentimistegur pole täielik).</span><span class="sxs-lookup"><span data-stu-id="1b615-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="1b615-110">Paroolifail ei tohi olla suurem kui 10 MB.</span><span class="sxs-lookup"><span data-stu-id="1b615-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="1b615-111">Kasutage ühte parooli rea kohta ja lisage loendis viimase parooli järele tühi rida (tagasijooksu).</span><span class="sxs-lookup"><span data-stu-id="1b615-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="1b615-112">Olulised asjad, mida saate **teada oda andmepüügist, kinnitage** simulatsioonid.</span><span class="sxs-lookup"><span data-stu-id="1b615-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="1b615-113">Vaikimisi ei saa andmepüügilogimisserveri URL-i jaoks **kohandatud väärtust sisestada.**</span><span class="sxs-lookup"><span data-stu-id="1b615-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="1b615-114">Kui adressaat kasutab [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) sõnumi andmepüügiks teatamiseks lisandmoodulit Luba aruandesõnumi lisandmoodul, ei pruugi te sõnumi kohta teatisi saada (kuna see on simuleeritud rünnak).</span><span class="sxs-lookup"><span data-stu-id="1b615-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="1b615-115">Aruanded. Pärast simuleeritud rünnaku lõpule viimist saate aruande **koostamiseks** klõpsata nuppu Rünnaku üksikasjad.</span><span class="sxs-lookup"><span data-stu-id="1b615-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="1b615-116">Üksikasjalikud juhised ja uued funktsioonid ründesimulaatoris leiate teemast [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="1b615-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
