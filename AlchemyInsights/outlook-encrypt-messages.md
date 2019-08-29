---
title: S/MIME Outlook Web
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666836"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="a5543-102">Krüpteerida e-kirju Outlook</span><span class="sxs-lookup"><span data-stu-id="a5543-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="a5543-103">Office 365 sõnumite krüptimiseks põhineb Microsoft Azure Rights Management (Azure RMS), mis on osa Azure'i kaitse.</span><span class="sxs-lookup"><span data-stu-id="a5543-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="a5543-104">Kui teie tellimus hõlmab Azure Rights Management või Azure kaitse, **võite jätta võtma mis tahes meetmeid käsitsi lubamiseks või aktiveerida** õiguste haldamise teenust.</span><span class="sxs-lookup"><span data-stu-id="a5543-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="a5543-105">Klientide tagasiside põhjal me enam võimaldada voolu vahetusreegleid meili krüptimiseks automaatselt väljamineva e-posti, mis sisaldab teatud tüüpi tundlikku teavet teie rentniku vaikimisi.</span><span class="sxs-lookup"><span data-stu-id="a5543-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="a5543-106">Selle asemel pakume üksikasjalikud juhised kuidas saate teha seda ise.</span><span class="sxs-lookup"><span data-stu-id="a5543-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="a5543-107">Transpordireegli krüptida tundliku teabe loomise kohta lisateabe saamiseks vaadake [seda](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="a5543-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="a5543-108">Kui programmi Outlook Web (formerly **OWA**): e-kirja koostamisel klõpsa **kaitse** OWA.</span><span class="sxs-lookup"><span data-stu-id="a5543-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="a5543-109">See kehtib luba "Ei saada edasi".</span><span class="sxs-lookup"><span data-stu-id="a5543-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="a5543-110">Valige **Krüpti** ainult sõnumi krüptimiseks klõpsake **Muuda õigusi** .</span><span class="sxs-lookup"><span data-stu-id="a5543-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="a5543-111">Kui te kasutate **Outlooki klient**: **saata krüptitud sõnumit Outlooki 2013 või 2016 või Outlook 2016 for Mac, valige** > **õigused**, siis valige soovitud kaitse variandi.</span><span class="sxs-lookup"><span data-stu-id="a5543-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="a5543-112">**Krüptitakse automaatselt kõik kirjad** saadetakse teatud adressaatide või väliste organisatsioonidega, peate looma Transpordireegli posti voolu Exchange'i administraatori Center.</span><span class="sxs-lookup"><span data-stu-id="a5543-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="a5543-113">Üksikasjalikud juhised on esitatud [tugiartiklit](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="a5543-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

