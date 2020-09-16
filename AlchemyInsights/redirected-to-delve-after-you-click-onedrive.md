---
title: OneDrive for Business Web OneDrive suunab Delve ' i ümber
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776375"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="2028a-102">Pärast OneDrive ' i klõpsamist suunatakse uuesti Delve ' i</span><span class="sxs-lookup"><span data-stu-id="2028a-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="2028a-103">Lugege meie üksikasjalikku [tõrkeotsingu juhendit](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="2028a-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="2028a-104">Selle probleemi lahendamiseks peab administraator andma kasutajatele õiguse oma saitide saidi loomiseks.</span><span class="sxs-lookup"><span data-stu-id="2028a-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="2028a-105">Selle põhjuseks on see, et minu saitidel luuakse OneDrive for Businessi leht.</span><span class="sxs-lookup"><span data-stu-id="2028a-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="2028a-106">Selle õiguse andmiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="2028a-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="2028a-107">Klõpsake SharePointi administreerimiskeskuses nuppu **kasutajaprofiilid**.</span><span class="sxs-lookup"><span data-stu-id="2028a-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="2028a-108">Klõpsake jaotises **inimesed** nuppu **Halda kasutajaõigusi**.</span><span class="sxs-lookup"><span data-stu-id="2028a-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="2028a-109">Kasutajate lisamine, kes vajavad minu saitide saidi loomiseks õigust.</span><span class="sxs-lookup"><span data-stu-id="2028a-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="2028a-110">Vaikimisi on see säte seatud **kõigile, välja arvatud välised kasutajad**.</span><span class="sxs-lookup"><span data-stu-id="2028a-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="2028a-111">Kui olete lisanud kasutaja, kasutajad või rühma, veenduge, et valitud on valitud kasutaja, kasutajad või rühm, liikuge kerides jaotisse " **permissions** " ja seejärel märkige ruut **Loo isiklik sait (nõutav isiklikuks ladustamiseks, uudistekanali ja järgneb sisu)**.</span><span class="sxs-lookup"><span data-stu-id="2028a-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="2028a-112">Klõpsake nuppu **OK**ja seejärel kasutaja saidi loomiseks sirvige OneDrive ' i lehele.</span><span class="sxs-lookup"><span data-stu-id="2028a-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
