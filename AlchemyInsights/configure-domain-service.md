---
title: Domeeni teenuse konfigureerimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885219"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="80006-102">AAD-DS-i või juurutust ei saa lubada</span><span class="sxs-lookup"><span data-stu-id="80006-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="80006-103">Azure AD Domain Service ' i (AAD-DS) probleemi lahendamiseks, mis ei ole lubatud või mida ei saa juurutada, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="80006-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="80006-104">Kui kasutate juba olemasolevat virtuaalset võrku, märkige oma NSG reeglid, mis blokeerivad pordid, mida on vaja portaali AAD-DS sünkroonimiseks https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="80006-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="80006-105">Vaadake, kas selles tõrkeotsingu juhendis on saadaval tõrketeade, et näha, kas teie tõrketeatele on vastatud  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="80006-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="80006-106">Proovige juurutada Azure AD Domain Services uues virtuaalses võrgus.</span><span class="sxs-lookup"><span data-stu-id="80006-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="80006-107">Täitke juhised, kuidas juurutada AAD-DS: [AAD Domain Services loomine ja konfigureerimine](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="80006-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="80006-108">Kui teil on Azure AD Domain Services juurutusega seotud probleeme, lugege teemat [AZURE ad Domain Services tõrkeotsing](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) levinud tõrgete lahendamiseks, mis aitavad teil asjad uuesti tööle saada.</span><span class="sxs-lookup"><span data-stu-id="80006-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="80006-109">**AAD-DS-i ei saa keelata**</span><span class="sxs-lookup"><span data-stu-id="80006-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="80006-110">AAD-DS-i ei saa peatada.</span><span class="sxs-lookup"><span data-stu-id="80006-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="80006-111">Kui soovite hallatava domeeni kasutamise lõpetada, tuleb see kustutada.</span><span class="sxs-lookup"><span data-stu-id="80006-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="80006-112">Hallatava domeeni kustutamiseks vaadake teemat [AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)' i kustutamine.</span><span class="sxs-lookup"><span data-stu-id="80006-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



