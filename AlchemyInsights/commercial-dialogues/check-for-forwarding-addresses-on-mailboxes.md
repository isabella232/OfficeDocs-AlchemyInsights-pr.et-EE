---
title: Postkastides aadresside edasisaatmise kontrollimine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403307"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="c1964-102">Postkastides aadresside edasisaatmise kontrollimine</span><span class="sxs-lookup"><span data-stu-id="c1964-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="c1964-103">Vahel edastavad häkkerid kasutajate meilisõnumid iseendale, seega kontrollime esmalt, kas postkasti aadressid ja reeglid on edasi saadetud.</span><span class="sxs-lookup"><span data-stu-id="c1964-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="c1964-104">Seejärel kontrollime auditilogisid.</span><span class="sxs-lookup"><span data-stu-id="c1964-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="c1964-105">Edasisaatmisaadresside otsimiseks saate teha nii:</span><span class="sxs-lookup"><span data-stu-id="c1964-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="c1964-106">Valige **Kasutajad**  >  **Aktiivsed kasutajad**.</span><span class="sxs-lookup"><span data-stu-id="c1964-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="c1964-107">Valige kasutaja, kelle kontot on rikutud.</span><span class="sxs-lookup"><span data-stu-id="c1964-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="c1964-108">Laiendage kuvatavas hüpikmenüüs valikut **Meilisätted** ja seejärel klõpsake käsku **Redigeeri** **meilisõnumite edasisaatmiseks.**</span><span class="sxs-lookup"><span data-stu-id="c1964-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="c1964-109">Eemaldage kõik edasisaatmisaadressid, mida te ei tunne.</span><span class="sxs-lookup"><span data-stu-id="c1964-109">Remove any forwarding addresses you don't recognize.</span></span>