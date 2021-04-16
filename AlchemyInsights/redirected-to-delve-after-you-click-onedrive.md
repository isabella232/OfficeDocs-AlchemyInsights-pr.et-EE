---
title: OneDrive for Business Web OneDrive suunab ümber Delve'i
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799985"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="ffc80-102">Pärast OneDrive'i klõpsamist delve'i ümbersuunamine</span><span class="sxs-lookup"><span data-stu-id="ffc80-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="ffc80-103">Vaadake meie üksikasjalikku [tõrkeotsingujuhendit.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="ffc80-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="ffc80-104">Selle probleemi lahendamiseks peab administraator andma kasutajatele õiguse luua oma saidi Minu saidid.</span><span class="sxs-lookup"><span data-stu-id="ffc80-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="ffc80-105">Seda seetõttu, et OneDrive for Businessi leht luuakse lehel Minu saidid.</span><span class="sxs-lookup"><span data-stu-id="ffc80-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="ffc80-106">Selle õiguse andmiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="ffc80-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="ffc80-107">Klõpsake SharePointi halduskeskuses nuppu **kasutajaprofiilid.**</span><span class="sxs-lookup"><span data-stu-id="ffc80-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="ffc80-108">Klõpsake **jaotises Inimesed** nuppu **Halda kasutajaõigusi**.</span><span class="sxs-lookup"><span data-stu-id="ffc80-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="ffc80-109">Saate lisada kasutajaid, kes vajavad oma saidi "Minu saidid" loomiseks õigusi.</span><span class="sxs-lookup"><span data-stu-id="ffc80-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="ffc80-110">Vaikimisi on selle sätte sätteks seatud Kõik **peale väliskasutajate.**</span><span class="sxs-lookup"><span data-stu-id="ffc80-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="ffc80-111">Kui olete kasutaja, kasutajad või rühma lisanud, veenduge, et lisatud kasutaja, kasutajad  või rühm on valitud, liikuge kerides jaotisse Õigused ja märkige seejärel ruut Loo isiklik sait (nõutav isikliku talletusruumi, uudistekanali ja jälgitud sisu **jaoks)** kõrval.</span><span class="sxs-lookup"><span data-stu-id="ffc80-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="ffc80-112">Klõpsake **nuppu OK** ja seejärel saate kasutaja saidi loomiseks sirvida OneDrive'i lehele.</span><span class="sxs-lookup"><span data-stu-id="ffc80-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
