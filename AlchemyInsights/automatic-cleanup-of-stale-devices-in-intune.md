---
title: Aegunud seadmete automaatne puhastamine intunes
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554965"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="91409-102">Aegunud seadmete automaatne puhastamine intunes</span><span class="sxs-lookup"><span data-stu-id="91409-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="91409-103">Intune võimaldab administraatoril seadistada ajaintervalli vahemikus 90 ja 270 päeva, pärast mida aegunud seadmed teenusest eemaldatakse.</span><span class="sxs-lookup"><span data-stu-id="91409-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="91409-104">See säte on kogu organisatsioonis ja kui aktiveeritud, jõustub kohe.</span><span class="sxs-lookup"><span data-stu-id="91409-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="91409-105">Kõik seadmed, mida pole Intune ' i serverile üle vaadatud, kustutatakse jäädavalt.</span><span class="sxs-lookup"><span data-stu-id="91409-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="91409-106">**Märkus** Ainult MDM-seadme objektid vastavad selle Kettapuhastuse toimingu tingimustele.</span><span class="sxs-lookup"><span data-stu-id="91409-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="91409-107">Ainult EAS-i seadme objektid on välistatud.</span><span class="sxs-lookup"><span data-stu-id="91409-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="91409-108">Lisateavet selle kohta, millal seade saab seadme puhastamise sätete ja selle oleku alusel kustutamise tingimustele vastavaks, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="91409-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="91409-109">Säte: **seadmete kustutamine pärast viimast sisseregistreerimise kuupäeva: Jah (teatud väärtused (N) määratud päevade lõikes)**</span><span class="sxs-lookup"><span data-stu-id="91409-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="91409-110">Määratud väärtuse (N) põhjal, kui säte on konfigureeritud, kustutab Intune seadme määratud päevade jooksul pärast selle viimase edukat kontrollimist.</span><span class="sxs-lookup"><span data-stu-id="91409-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="91409-111">Säte: **seadmete kustutamine pärast viimast sisseregistreerimise kuupäeva: ei**</span><span class="sxs-lookup"><span data-stu-id="91409-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="91409-112">180 päeva pärast seadme serdi aegumist ja seda ei pikendata, kustutatakse seade.</span><span class="sxs-lookup"><span data-stu-id="91409-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="91409-113">**Märkus** Mõlemal juhul tuleb seade Intune ' is edukalt registreerida.</span><span class="sxs-lookup"><span data-stu-id="91409-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="91409-114">Registreerimine toimub esimese seadme sissemöllimine ja Intune ' i teenusega.</span><span class="sxs-lookup"><span data-stu-id="91409-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="91409-115">Kui seade registreerib edukalt Intune ' i, kuid ei saanud Intune ' i registreerida, kustutatakse seade 270 päeva pärast registreerimist.</span><span class="sxs-lookup"><span data-stu-id="91409-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="91409-116">(90 päeva, et märkida seade tühistatuks ja seejärel teine 180 päeva kirje kustutamiseks.)</span><span class="sxs-lookup"><span data-stu-id="91409-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="91409-117">Ühtegi mehhanismi pole praegu Intune ' i konsoolis, et tuvastada seadme sertide kehtivuse lõppkuupäev.</span><span class="sxs-lookup"><span data-stu-id="91409-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>