---
title: Meilisõnumi edastamine, kui esitate võrgu sõnumi ID
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744239"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="33af0-102">Meilisõnumi edastamine, kui esitate võrgu sõnumi ID</span><span class="sxs-lookup"><span data-stu-id="33af0-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="33af0-103">Valige hüpik **Uus edastus** **meiliaadress** ja **võrgu sõnumi ID**.</span><span class="sxs-lookup"><span data-stu-id="33af0-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="33af0-104">Meilisõnumi sõnumi ID leidmiseks Outlookis tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="33af0-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="33af0-105">Meilisõnumi avamiseks topeltklõpsake seda.</span><span class="sxs-lookup"><span data-stu-id="33af0-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="33af0-106">Valige **failiatribuudid**  >  .</span><span class="sxs-lookup"><span data-stu-id="33af0-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="33af0-107">Avage Notepad või tühi Wordi dokument ja seejärel kopeerige ja kleepige väljale **Interneti-päised** leitud sisu parema nähtavuse huvides.</span><span class="sxs-lookup"><span data-stu-id="33af0-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="33af0-108">Otsige väli **X-MS-Exchange-Organization-Network-Message-ID** .</span><span class="sxs-lookup"><span data-stu-id="33af0-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="33af0-109">Väärtus pärast **:** on teie edastuse jaoks vajalik ID.</span><span class="sxs-lookup"><span data-stu-id="33af0-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="33af0-110">Valige jaotises **adressaadid**, kui meilisõnumid, mis on selle meilisõnumi kõigi adressaatide kaustas Rämpspost, nuppu **Vali kõik**.</span><span class="sxs-lookup"><span data-stu-id="33af0-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="33af0-111">Kui mitte, valige ainult probleemist teatanud kasutaja.</span><span class="sxs-lookup"><span data-stu-id="33af0-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="33af0-112">Valige **jaotises põhjus**, kui valite suvandi oleks **blokeeritud**, kas sõnum oleks pidanud olema **rämpspostiks**, **andmepüügiks** või **ründevaraks** blokeeritud ja seejärel valige **Edasta**.</span><span class="sxs-lookup"><span data-stu-id="33af0-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="33af0-113">Lisateavet leiate teemast [rämpsposti, Phish, URL-ide ja failide Microsoftile skannimiseks edastamine](https://go.microsoft.com/fwlink/?linkid=2101479).</span><span class="sxs-lookup"><span data-stu-id="33af0-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
