---
title: S/MIME Outlooki veebirakenduses
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772258"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="d8bf7-102">Meilisõnumite krüptimine Outlookis</span><span class="sxs-lookup"><span data-stu-id="d8bf7-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="d8bf7-103">Microsoft 365 Sõnumite krüptimine on loodud Microsoft Azure ' i õiguste halduses (Azure RMS), mis on osa Azure ' i teabe kaitsest.</span><span class="sxs-lookup"><span data-stu-id="d8bf7-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="d8bf7-104">Kui teie tellimus sisaldab Azure ' i õiguste haldus-või Azure ' i teabe kaitset, **ei pea te õiguste halduse teenuse käsitsi lubamiseks või aktiveerimiseks mingeid toiminguid** tegema.</span><span class="sxs-lookup"><span data-stu-id="d8bf7-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="d8bf7-105">Klientide tagasiside põhjal ei luba me enam Exchange ' i meilivoo reegleid automaatselt krüptida väljaminevaid meilisõnumeid, mis sisaldavad teatud tüüpi delikaatseid andmeid rentniku jaoks vaikimisi.</span><span class="sxs-lookup"><span data-stu-id="d8bf7-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="d8bf7-106">Selle asemel pakume üksikasjalikke juhiseid selle kohta, kuidas saate seda ise teha.</span><span class="sxs-lookup"><span data-stu-id="d8bf7-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="d8bf7-107">Lisateabe saamiseks selle kohta, kuidas luua tundliku teabe krüptimiseks transpordi reeglit, lugege [seda artiklit](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="d8bf7-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="d8bf7-108">Kui kasutate Outlooki veebirakenduses (varem **OWA**): meilisõnumi koostamisel klõpsake lihtsalt nuppu **kaitse** OWA-s.</span><span class="sxs-lookup"><span data-stu-id="d8bf7-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="d8bf7-109">See kehtib "Ära saada edasi" luba.</span><span class="sxs-lookup"><span data-stu-id="d8bf7-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="d8bf7-110">Klõpsake nuppu **Muuda õigusi** ja valige ainult sõnumi krüptimiseks **Krüpti** .</span><span class="sxs-lookup"><span data-stu-id="d8bf7-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="d8bf7-111">Kui kasutate **Outlooki klientrakendust**: krüptitud sõnumi saatmiseks rakendusest Outlook 2013 või 2016 või Outlook 2016 for Mac, valige **Suvandid**  >  **ja**seejärel valige soovitud kaitse suvand.</span><span class="sxs-lookup"><span data-stu-id="d8bf7-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="d8bf7-112">Teatud adressaatidele või väliste partnerite organisatsioonidele saadetavate **meilisõnumite automaatseks krüptimiseks** peate Exchange ' i administreerimiskeskuses looma meilivoo transpordi reegli.</span><span class="sxs-lookup"><span data-stu-id="d8bf7-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="d8bf7-113">[Selles tugiteenuse artiklis](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)on toodud üksikasjalikud juhised.</span><span class="sxs-lookup"><span data-stu-id="d8bf7-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

