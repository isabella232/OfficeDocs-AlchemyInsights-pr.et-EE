---
title: 2609-säilitamine-või-eDiscovery-hoidke
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994058"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="8d032-102">Ei saa kustutada üksusi SharePoint Online ' i või OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="8d032-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="8d032-103">Teie või teie kasutajad ei saa kustutada SharePoint Online ' i või OneDrive for Business üksusi, kuna säilituspoliitika, säilitamise silt või eDiscovery hoida SharePointi OneDrive saidi või mõne kindla üksuse.</span><span class="sxs-lookup"><span data-stu-id="8d032-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="8d032-104">See hõlmab dokumendi, dokumendi versiooni, kausta, dokumenditeegi, loendi, rakenduse, saidi või saidikogumi kustutamist.</span><span class="sxs-lookup"><span data-stu-id="8d032-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="8d032-105">Siin on mõned näited tõrketeadetest, mida võite saada, kui püüate kustutada üksust, mida säilitatakse:</span><span class="sxs-lookup"><span data-stu-id="8d032-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="8d032-106">"Seda saiti ei saa kustutada, kuna see sisaldub eDiscovery Hold-või säilituspoliitikas."</span><span class="sxs-lookup"><span data-stu-id="8d032-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="8d032-107">"See sait on vastavuse poliitika seatud blokeerida kustutamine"</span><span class="sxs-lookup"><span data-stu-id="8d032-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="8d032-108">"Vastavuspoliitika blokeerib praegu selle saidi kustutamise"</span><span class="sxs-lookup"><span data-stu-id="8d032-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="8d032-109">"See saidikogum ei saa kustutada, kuna see sisaldab saite, mis sisalduvad eDiscovery Hold-või säilituspoliitika"</span><span class="sxs-lookup"><span data-stu-id="8d032-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="8d032-110">"Peate kustutama kõik üksused selles kaustas enne kausta kustutamist"</span><span class="sxs-lookup"><span data-stu-id="8d032-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="8d032-111">"Selle üksuse versioone ei saa kustutada, kuna see on kinni-või säilituspoliitika"</span><span class="sxs-lookup"><span data-stu-id="8d032-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="8d032-112">"Üksust ei saa kustutada, kui hoida"</span><span class="sxs-lookup"><span data-stu-id="8d032-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="8d032-113">"Sellele üksusele rakendatud silt takistab selle redigeerimist või kustutamist"</span><span class="sxs-lookup"><span data-stu-id="8d032-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="8d032-114">"Loend ei saa kustutada, kui hoidke või säilituspoliitika"</span><span class="sxs-lookup"><span data-stu-id="8d032-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="8d032-115">"Loendit ei saa kustutada, kui see on blokeeritud või säilituspoliitika on rakendatud"</span><span class="sxs-lookup"><span data-stu-id="8d032-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="8d032-116">Üksuste kustutamiseks ühes neist stsenaariumidest tuleb eemaldada säilituspoliitika, säilitussilt või eDiscovery Hold (või sait tuleb säilituspoliitikast välja jätta).</span><span class="sxs-lookup"><span data-stu-id="8d032-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="8d032-117">Peate kas keelata või välistada vastava Hold, mis põhjustab probleemi.</span><span class="sxs-lookup"><span data-stu-id="8d032-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="8d032-118">Pärast säilituspoliitika või hoidke eemaldamist, võib kuluda kuni 24 tundi muudatuse jõustumiseks.</span><span class="sxs-lookup"><span data-stu-id="8d032-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="8d032-119">Lisateabe saamiseks erinevate säilitamise ja hoidke funktsioone, mida saab rakendada SharePointi saidid ja OneDrive kontod, vaadake ühte järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="8d032-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="8d032-120">Säilituspoliitika ülevaade</span><span class="sxs-lookup"><span data-stu-id="8d032-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="8d032-121">Säilitussiltide ülevaade</span><span class="sxs-lookup"><span data-stu-id="8d032-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="8d032-122">Halda hoiab Advanced eDiscovery</span><span class="sxs-lookup"><span data-stu-id="8d032-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="8d032-123">eDiscovery hoiab</span><span class="sxs-lookup"><span data-stu-id="8d032-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="8d032-124">Pärand saidi sulgemine ja kustutamise poliitikad</span><span class="sxs-lookup"><span data-stu-id="8d032-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
