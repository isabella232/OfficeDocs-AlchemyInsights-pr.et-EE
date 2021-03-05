---
title: Postkastidele aadresside edasisaatmise kontrollimine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481805"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="a5420-102">Postkastidele aadresside edasisaatmise kontrollimine</span><span class="sxs-lookup"><span data-stu-id="a5420-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="a5420-103">Mõnikord edastavad häkkerid kasutajate meilisõnumeid ise, nii et kõigepealt kontrollime postkasti aadresse ja reegleid.</span><span class="sxs-lookup"><span data-stu-id="a5420-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="a5420-104">Siis kontrollime auditi logisid.</span><span class="sxs-lookup"><span data-stu-id="a5420-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="a5420-105">Aadresside edasisaatmise kontrollimiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="a5420-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="a5420-106">**Kasutajate**  >  **Aktiivsete kasutajate** valimine.</span><span class="sxs-lookup"><span data-stu-id="a5420-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="a5420-107">Valige kasutaja, kelle konto on ohustatud.</span><span class="sxs-lookup"><span data-stu-id="a5420-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="a5420-108">Laiendage kuvatavas hüpik jaotist **meili sätted** ja seejärel klõpsake käsku **Redigeeri** **meilisõnumite edasisaatmiseks**.</span><span class="sxs-lookup"><span data-stu-id="a5420-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="a5420-109">Eemaldage kõik edasisaadetavate aadressid, mida te ei tunne.</span><span class="sxs-lookup"><span data-stu-id="a5420-109">Remove any forwarding addresses you don't recognize.</span></span>