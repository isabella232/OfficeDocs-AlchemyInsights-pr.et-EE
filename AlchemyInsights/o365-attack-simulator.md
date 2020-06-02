---
title: 2681 rünnak simulaator Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506734"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="8fc27-102">Rünnak simulaator Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8fc27-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="8fc27-103">Kas teil puudub rünnak simulaator?</span><span class="sxs-lookup"><span data-stu-id="8fc27-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="8fc27-104">Rünnak simulaator nõuab **office 365 täiustatud ohutõrje kava 2 (ATP plaan 2)** või **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="8fc27-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="8fc27-105">Rünnak simulaator **ei** sisaldu Office 365 täiustatud ohutõrje kava 1 (ATP leping 1), Office 365 Enterprise E3 või mis tahes Microsoft 365 apps Business tellimused.</span><span class="sxs-lookup"><span data-stu-id="8fc27-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="8fc27-106">Modelleeritud rünnakute käivitamiseks kasutatav konto nõuab globaalset administraatori või turbeülema õigusi ja mitme teguriga autentimist (MFA).</span><span class="sxs-lookup"><span data-stu-id="8fc27-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="8fc27-107">Rünnaku simulaatori nõuete kohta lisateabe saamiseks vaadake [seda teemat](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="8fc27-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="8fc27-108">Olulised asjad teada **Brute Force parooli** rünnaku simulatsioone:</span><span class="sxs-lookup"><span data-stu-id="8fc27-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="8fc27-109">Kui sihtkontol on MFA lubatud ja parool on õigesti arvatud, ei kuvata kontot ohustena (teine autentimistegur on puudulik).</span><span class="sxs-lookup"><span data-stu-id="8fc27-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="8fc27-110">Paroolifail ei tohi olla suurem kui 10 MB.</span><span class="sxs-lookup"><span data-stu-id="8fc27-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="8fc27-111">Kasutage üks parool rea kohta ja lisage tühi rida (veo tagastamine) pärast viimast parooli loendis.</span><span class="sxs-lookup"><span data-stu-id="8fc27-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="8fc27-112">Olulised asjad, mida teada **Spear phishing** lisada simulatsioone:</span><span class="sxs-lookup"><span data-stu-id="8fc27-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="8fc27-113">Ette nähtud, ei saa anda kohandatud väärtus **phishing logimisserveri URL-i**.</span><span class="sxs-lookup"><span data-stu-id="8fc27-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="8fc27-114">Kui adressaat kasutab sõnumi andmepüügi lubamiseks aruande sõnumi [lisandmoodul](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , te ei pruugi saada teatisi sõnumi (kuna see on simuleeritud rünnak).</span><span class="sxs-lookup"><span data-stu-id="8fc27-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="8fc27-115">Aruanded: pärast simuleeritud rünnak on lõpule jõudnud, võite klõpsata **rünnak üksikasjad** aruande vaatamiseks.</span><span class="sxs-lookup"><span data-stu-id="8fc27-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="8fc27-116">Üksikasjalikke juhiseid ja uusi funktsioone Attack Simulator, vt [rünnak simulaator Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="8fc27-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
