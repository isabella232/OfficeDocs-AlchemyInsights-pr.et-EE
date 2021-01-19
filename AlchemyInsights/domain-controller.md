---
title: Domeenikontroller
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900872"
---
# <a name="domain-controller"></a><span data-ttu-id="fce2e-102">Domeenikontroller</span><span class="sxs-lookup"><span data-stu-id="fce2e-102">Domain controller</span></span>

<span data-ttu-id="fce2e-103">**AAD-DS-i või juurutust ei saa lubada**</span><span class="sxs-lookup"><span data-stu-id="fce2e-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="fce2e-104">Azure AD Domain Service ' i (AAD-DS) probleemi lahendamiseks, mis ei ole lubatud või mida ei saa juurutada, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="fce2e-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="fce2e-105">Kui kasutate juba olemasolevat virtuaalset võrku, märkige oma NSG reeglid, mis blokeerivad pordid, mida on vaja portaali AAD-DS sünkroonimiseks https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="fce2e-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="fce2e-106">Vaadake, kas selles tõrkeotsingu juhendis on saadaval tõrketeade, et näha, kas teie tõrketeatele on vastatud  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="fce2e-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="fce2e-107">Proovige juurutada Azure AD Domain Services uues virtuaalses võrgus.</span><span class="sxs-lookup"><span data-stu-id="fce2e-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="fce2e-108">Täitke juhised selle kohta, kuidas juurutada AAD-DS-i, mis on saadaval aadressil [juhendaja AZURE ad Domain Services loomiseks](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="fce2e-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="fce2e-109">Kui teil on Azure AD Domain Services juurutusega seotud probleeme, lugege teemat [AZURE ad Domain Services tõrkeotsing](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) levinud tõrgete lahendamiseks, mis aitavad teil asjad uuesti tööle saada.</span><span class="sxs-lookup"><span data-stu-id="fce2e-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="fce2e-110">**AAD-DS-i ei saa keelata**</span><span class="sxs-lookup"><span data-stu-id="fce2e-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="fce2e-111">AAD-DS-i ei saa peatada.</span><span class="sxs-lookup"><span data-stu-id="fce2e-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="fce2e-112">Kui soovite hallatava domeeni kasutamise lõpetada, tuleb see kustutada.</span><span class="sxs-lookup"><span data-stu-id="fce2e-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="fce2e-113">Kui teil tekib probleeme, Lahendage levinud tõrketeated ja seotud tõrkeotsingu toimingud, et aidata teil asju uuesti käivitada, lugege teemat [Azure Active Directory Domain Services tõrkeotsing](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="fce2e-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
