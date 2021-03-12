---
title: Koopia komplekt
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713747"
---
# <a name="replica-set"></a><span data-ttu-id="620c1-102">Koopia komplekt</span><span class="sxs-lookup"><span data-stu-id="620c1-102">Replica set</span></span>

<span data-ttu-id="620c1-103">AADDS nimetatakse ka hallatavaks domeeniks.</span><span class="sxs-lookup"><span data-stu-id="620c1-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="620c1-104">See on tegelikult kaks domeenikontrollerit, mida tagaserveris käitab ja hooldab.</span><span class="sxs-lookup"><span data-stu-id="620c1-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="620c1-105">Kaks DCs sisaldavad ühte peamist DC-d ja ühte replikatsiooni DC-d.</span><span class="sxs-lookup"><span data-stu-id="620c1-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="620c1-106">Varundid AADDS (hallatav Domeen) on Azure ' i platvormi hallatav automatiseeritud protsess.</span><span class="sxs-lookup"><span data-stu-id="620c1-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="620c1-107">Kui probleem on teie hallatavas domeenis, aitab Azure ' i tugi teil taastada varukoopia põhjal.</span><span class="sxs-lookup"><span data-stu-id="620c1-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="620c1-108">Loote iga koopia virtuaalses võrgus.</span><span class="sxs-lookup"><span data-stu-id="620c1-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="620c1-109">Iga virtuaalne võrk peab olema ühendatud kõigi muude virtuaalsete võrkudega, mis majutavad hallatava domeeni koopia komplekti.</span><span class="sxs-lookup"><span data-stu-id="620c1-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="620c1-110">Selle konfiguratsiooniga luuakse võrgusilma võrgu topoloogia, mis toetab kataloogi replikatsiooni.</span><span class="sxs-lookup"><span data-stu-id="620c1-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="620c1-111">Virtual Network saab toetada mitut koopia komplekti, kui iga koopia komplekt on mõnes muus virtuaalses alamvõrgus.</span><span class="sxs-lookup"><span data-stu-id="620c1-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="620c1-112">Lisateavet koopiakomplekti kohta leiate teemast [Concepts replica komplektid](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span><span class="sxs-lookup"><span data-stu-id="620c1-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
