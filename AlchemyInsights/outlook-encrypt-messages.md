---
title: S/MIME Outlookis veebis
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511504"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="a30f1-102">E-kirjade krüptimine Outlookis</span><span class="sxs-lookup"><span data-stu-id="a30f1-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="a30f1-103">Microsoft 365 sõnumi krüptimine on loodud Microsoft Azure Rights Management (Azure RMS), mis on osa Azure ' i teabekaitse.</span><span class="sxs-lookup"><span data-stu-id="a30f1-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="a30f1-104">Kui teie tellimus sisaldab Azure ' i õiguste haldust või Azure ' i Teabekaitset, ei ole õiguste halduse teenuse **käsitsi lubamiseks või aktiveerimiseks vaja toiminguid** teha.</span><span class="sxs-lookup"><span data-stu-id="a30f1-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="a30f1-105">Kliendi tagasiside põhjal ei saa me enam lubada Exchange ' i meilivoolu reegleid automaatselt krüptida Väljamineva meili, mis sisaldab teatud tüüpi tundlikku teavet teie rentnikus vaikimisi.</span><span class="sxs-lookup"><span data-stu-id="a30f1-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="a30f1-106">Selle asemel pakume üksikasjalikke juhiseid selle kohta, kuidas te saate seda ise teha.</span><span class="sxs-lookup"><span data-stu-id="a30f1-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="a30f1-107">Lisateabe saamiseks selle kohta, kuidas luua transpordireegel tundliku teabe krüptimiseks, lugege [seda artiklit](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="a30f1-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="a30f1-108">Kui kasutate Outlook Web (endine **OWA**): koostamisel e-kirja, klõpsake lihtsalt **kaitsta** OWA.</span><span class="sxs-lookup"><span data-stu-id="a30f1-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="a30f1-109">See kehtib "ära Edasta" luba.</span><span class="sxs-lookup"><span data-stu-id="a30f1-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="a30f1-110">Klõpsake nuppu **Muuda luba** ja valige **Krüpti** ainult sõnumi krüptimiseks.</span><span class="sxs-lookup"><span data-stu-id="a30f1-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="a30f1-111">Kui kasutate **Outlooki kliendi**: krüptitud sõnumi saatmiseks Outlook 2013 või 2016 või Outlook 2016 for Mac, valige **Suvandid**  >  **permissions**, seejärel valige kaitse valik, mida vajate.</span><span class="sxs-lookup"><span data-stu-id="a30f1-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="a30f1-112">**Automaatselt krüptida kõik saadetud e-posti** teatud adressaatidele või väliste partnerite organisatsioonidele, peate looma voog transpordi reegel Exchange ' i halduskeskus.</span><span class="sxs-lookup"><span data-stu-id="a30f1-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="a30f1-113">Üksikasjalikud juhised on antud [tugiteenuste artiklis](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="a30f1-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

