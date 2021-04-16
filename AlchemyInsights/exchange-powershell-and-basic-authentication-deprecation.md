---
title: Exchange PowerShell ja põhiautentimise kasutuselt eemaldamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813468"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="df47c-102">Exchange PowerShell ja põhiautentimise kasutuselt eemaldamine</span><span class="sxs-lookup"><span data-stu-id="df47c-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="df47c-103">Uusimat teavet Exchange Online PowerShelliga ühenduse loomise kohta ilma põhiautentimiseta [vaadake siit](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="df47c-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="df47c-104">PowerShelli V2 moodul ei kasuta elementaarautentimist.</span><span class="sxs-lookup"><span data-stu-id="df47c-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="df47c-105">Pange tähele, et elementaarautentimine peab teie klientarvutis endiselt lubatud olema.</span><span class="sxs-lookup"><span data-stu-id="df47c-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="df47c-106">Uus PowerShelli V2 moodul kasutab modernautentimist, et luua ühendus kõigi REST-põhiste V2 cmdlet-käskude lubamiseks.</span><span class="sxs-lookup"><span data-stu-id="df47c-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="df47c-107">Lisaks V2 cmdlet-käskudele pääsete juurde ka vanematele Remote PowerShelli (RPS) cmdlet-käskudele, mis nõuavad Remote PowerShelli seansi loomist.</span><span class="sxs-lookup"><span data-stu-id="df47c-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="df47c-108">Windowsi masinal RPS-i seansi loomiseks on vajalik, et klientarvutis oleks WinRM põhiautentimine lubatud, isegi kui moodul kasutab teenuse autentimiseks modernautentimise mehhanismi.</span><span class="sxs-lookup"><span data-stu-id="df47c-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="df47c-109">WinRM põhiautentimise konveierit kasutatakse modernautentimise tõendite transportimiseks.</span><span class="sxs-lookup"><span data-stu-id="df47c-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="df47c-110">Kui klientarvutis on WinRM põhiautentimine keelatud, jätkavad V2 cmdlet-käsud töötamist (kuid vanemad RPS-i cmdlet-käsud mitte).</span><span class="sxs-lookup"><span data-stu-id="df47c-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
