---
title: Kaitse tagasihajutusega rünnaku eest
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035411"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="bf9d9-102">Kaitse tagasihajutusega rünnaku eest</span><span class="sxs-lookup"><span data-stu-id="bf9d9-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="bf9d9-103">Tagasihajutusega on mitte-kohaletoimetamise aruanded (tuntud ka kui NDR või põrge sõnumid), mida te ei saatnud.</span><span class="sxs-lookup"><span data-stu-id="bf9d9-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="bf9d9-104">Rämpsposti saatjad (Paroodiad) saatja **:** nende sõnumite aadressid ja sageli kasutavad nad tõelisi meiliaadresse nende sõnumite usaldusväärsuse tagamiseks.</span><span class="sxs-lookup"><span data-stu-id="bf9d9-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="bf9d9-105">Seega, kui rämpsposti saatjad saadavad paratamatult sõnumeid Olematutele adressaatidele, meelitatakse sihtkoha meiliserver selle asemel, et tagastada ebakohane sõnum NDR-i, mis on adressaadile saatja **:** aadress.</span><span class="sxs-lookup"><span data-stu-id="bf9d9-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="bf9d9-106">Lisateavet leiate [EOP tagasihajutusega](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="bf9d9-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="bf9d9-107">**Tagasihajutusega kaitse lubamine**</span><span class="sxs-lookup"><span data-stu-id="bf9d9-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="bf9d9-108">Tagasihajutusega kaitse lubamiseks järgige allolevat teed.</span><span class="sxs-lookup"><span data-stu-id="bf9d9-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="bf9d9-109">**protection.office.com > ohtu juhtimise > poliitika > antispam > valige rämpsmeili filtri poliitika ja Redigeeri poliitika > rämpsposti atribuudid > märgi rämpspostiks > NDR tagasihajutusega > seadke selle väärtuseks "sees"**</span><span class="sxs-lookup"><span data-stu-id="bf9d9-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="bf9d9-110">Kui arvate, et konto on ohustatud, lugege järgmist.</span><span class="sxs-lookup"><span data-stu-id="bf9d9-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="bf9d9-111">Ohustatud meilikontole vastamine</span><span class="sxs-lookup"><span data-stu-id="bf9d9-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="bf9d9-112">Blokeeritud kasutajate eemaldamine Office 365 piiratud kasutajate portaalist</span><span class="sxs-lookup"><span data-stu-id="bf9d9-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



