---
title: Outlooki töölaua tagasivõtmine või asendamine meilisõnumiga
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663986"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="673d1-102">Outlooki meilisõnumi tagasikutsumine või asendamine</span><span class="sxs-lookup"><span data-stu-id="673d1-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="673d1-103">Administraatorina saate **sõnumeid tagasi kutsuda PowerShelli abil kasutajate nimel**.</span><span class="sxs-lookup"><span data-stu-id="673d1-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="673d1-104">Administreerimiskeskuse sõnumeid ei saa tagasi kutsuda.</span><span class="sxs-lookup"><span data-stu-id="673d1-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="673d1-105">Saate tagasi **kutsuda ainult teie asutuse inimestele saadetud sõnumeid**.</span><span class="sxs-lookup"><span data-stu-id="673d1-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="673d1-106">Kui sõnum saadeti näiteks Gmaili aadressile, ei saa seda enam meelde tuletada.</span><span class="sxs-lookup"><span data-stu-id="673d1-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="673d1-107">Saate tagasi **kutsuda ainult Outlook 2016 arvutist saadetud sõnumeid**.</span><span class="sxs-lookup"><span data-stu-id="673d1-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="673d1-108">Kui kasutaja saadab Outlook for Maci või Outlooki veebirakenduse kaudu sõnumi, ei saa seda enam meelde tuletada.</span><span class="sxs-lookup"><span data-stu-id="673d1-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="673d1-109">Meilisõnumi tagasivõtmiseks või asendamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="673d1-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="673d1-110">Valige Outlooki akna vasakus servas asuval paanil kaust saadetud üksused.</span><span class="sxs-lookup"><span data-stu-id="673d1-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="673d1-111">Topeltklõpsake sõnumit, mille soovite selle avamiseks meelde jätta.</span><span class="sxs-lookup"><span data-stu-id="673d1-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="673d1-112">Valige vahekaart **sõnum** ja seejärel klõpsake nuppu **toimingud**, et  >  **see sõnum tagasi kutsuda**.</span><span class="sxs-lookup"><span data-stu-id="673d1-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="673d1-113">Valige **Kustuta selle sõnumi lugemata eksemplarid** või **Kustuta lugemata eksemplarid ja asendage see uue sõnumiga**ning seejärel valige **OK**.</span><span class="sxs-lookup"><span data-stu-id="673d1-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="673d1-114">Kui saadate asendus-sõnumi, koostage sõnum ja seejärel valige **saada**.</span><span class="sxs-lookup"><span data-stu-id="673d1-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="673d1-115">Sõnumi tagasivõtmise õnnestumine või ebaõnnestumine sõltub Outlooki adressaadi sätetest.</span><span class="sxs-lookup"><span data-stu-id="673d1-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="673d1-116">Lisateavet tagasivõtmise kontrollimise kohta leiate [sellest artiklist](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="673d1-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="673d1-117">Oma asutuse meilisõnumite otsimine ja kustutamine</span><span class="sxs-lookup"><span data-stu-id="673d1-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="673d1-118">Kui te pole üldadministraator, tuleb teie konto lisada sõnumite otsimiseks e-juurdluse halduri rollile või vastavuse otsingu juhtimise rollile.</span><span class="sxs-lookup"><span data-stu-id="673d1-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="673d1-119">Sõnumite kustutamiseks peate liituma organisatsiooni juhtimise rollirühma või otsingu ja likvideerimise rolliga.</span><span class="sxs-lookup"><span data-stu-id="673d1-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="673d1-120">Nende rollide load määratakse [turbe-ja vastavuskontrolli keskuses](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="673d1-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="673d1-121">[Saate luua sisu otsimise](https://docs.microsoft.com/microsoft-365/compliance/content-search) , et leida sõnum, mille soovite kustutada.</span><span class="sxs-lookup"><span data-stu-id="673d1-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="673d1-122">[Looge ühendus turbe-ja vastavuskontrolli keskusega PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="673d1-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="673d1-123">Kui kasutate mitme teguri autentimist, lugege teemat [ühenduse loomine Microsoft 365 turbe ja ühilduvuse keskusega PowerShell, kasutades mitut tegurit autentimine](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="673d1-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>