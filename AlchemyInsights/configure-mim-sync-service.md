---
title: MIM sünkroonimise teenuse konfigureerimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481353"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="2a362-102">MIM sünkroonimise teenuse konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="2a362-102">Configure MIM Sync service</span></span>

<span data-ttu-id="2a362-103">Microsoft Identity Manageri (MIM) sünkroonimise teenus on MIM komponent.</span><span class="sxs-lookup"><span data-stu-id="2a362-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="2a362-104">See on tsentraliseeritud kohapealne teenus, mis talletab ja integreerib teabe organisatsioonidele, millel on mitu kohapealset kataloogi ja andmebaasi.</span><span class="sxs-lookup"><span data-stu-id="2a362-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="2a362-105">Võimalik, et saate probleemi lahendada MIM sünkroonimisega, kui probleem on lahendatud hiljutises värskenduses MIM või on mõnest muust jaotisest, mida on kirjeldatud allpool.</span><span class="sxs-lookup"><span data-stu-id="2a362-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="2a362-106">**Soovitatavad toimingud**</span><span class="sxs-lookup"><span data-stu-id="2a362-106">**Recommended steps**</span></span>

1. <span data-ttu-id="2a362-107">Veenduge, et kasutate MIM sünkroonimise hiljutist värskendust ja kontrollite, kas probleem on värskenduses lahendatud, [MIM sünkroonimisel](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) .</span><span class="sxs-lookup"><span data-stu-id="2a362-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="2a362-108">Kui probleem on üldise LDAP-i, Generic SQL-i, Lotus Domino või Web Services Connectori abil, veenduge, et kasutate [geneeriliste konnektorite](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)hiljutist värskendamist.</span><span class="sxs-lookup"><span data-stu-id="2a362-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="2a362-109">Kui MIM sünkroonimisel ilmneb tõrge, lugege võimalike põhjuste määratlemiseks tabelit [käitamise](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) tõrkekoodidest.</span><span class="sxs-lookup"><span data-stu-id="2a362-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="2a362-110">Kui Run peatub **laiendiga dll-erand**, klõpsake neid sõnu, et avada aken **konnektori ruumi objekti atribuudid** , ja klõpsake nuppu **pinu jälg...** lisateabe saamiseks algpõhjuse kohta, nagu on kirjeldatud jaotises [laiend-DLL-erand](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span><span class="sxs-lookup"><span data-stu-id="2a362-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="2a362-111">Kui parool muutmise teatise teenus (PCNS) Component lahendid **tõrge 6025** parooli sünkroonimise ajal sündmuselogi, vaadake [PCNS aruandluse tõrge 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)juhiseid.</span><span class="sxs-lookup"><span data-stu-id="2a362-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="2a362-112">Kui FIM-i teenuse haldusteguri täielik sünkroonimine on aeglane, märkige jaotises tõrkeotsing säte **Automaatne Grow** for tempdb, nagu on kirjeldatud jaotises [tõrkeotsing aeglase või täieliku sünkroonimise](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)korral.</span><span class="sxs-lookup"><span data-stu-id="2a362-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="2a362-113">Kui teil on FIM-i teenuse haldamise agendi abil peatatud-server, kus on ebaõnnestunud loomine-kaudu-veebiteenused, lugege teemat [tugiteenused – teave: ebaõnnestunud-loomine-Via-Web-teenused](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) põhjuste ülevaate saamiseks.</span><span class="sxs-lookup"><span data-stu-id="2a362-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

