---
title: Litsentsimata toote tõrgete lahendamine
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
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737949"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="19dc6-102">Tõrked "litsentsimata toote" lahendamise näpunäited</span><span class="sxs-lookup"><span data-stu-id="19dc6-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="19dc6-103">Litsentsimata toote tõrgete lahendamiseks proovige teha järgmist.</span><span class="sxs-lookup"><span data-stu-id="19dc6-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="19dc6-104">Vaadake, kas teie tellimuse olek on aegunud.</span><span class="sxs-lookup"><span data-stu-id="19dc6-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="19dc6-105">Veenduge, et teil on tellimus, mis lubab kliendi litsentse (nt Microsoft 365 Apps for Business või Business Premium), ja veenduge, [et kasutajal on määratud litsents](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="19dc6-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="19dc6-106">Veenduge, et kasutaja on Office ' isse sisse loginud sama kontoga, millele on määratud litsents.</span><span class="sxs-lookup"><span data-stu-id="19dc6-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="19dc6-107">Vaadake, kas teenusel on [teenuse seisund](https://docs.microsoft.com/office365/enterprise/view-service-health) , et näha, kas teenusega on seotud mõni teadaolev probleem.</span><span class="sxs-lookup"><span data-stu-id="19dc6-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="19dc6-108">Kontrollige oma tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Microsoft 365 rakendusi Interneti-ühenduse jaoks.</span><span class="sxs-lookup"><span data-stu-id="19dc6-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="19dc6-109">Vaadake teemat [URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="19dc6-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="19dc6-110">Võite proovida ka järgmisi tõrkeotsingu toiminguid.</span><span class="sxs-lookup"><span data-stu-id="19dc6-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="19dc6-111">Avage Office ' i rakendus ja [logige välja](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) mis tahes olemasolevast kasutajakontost.</span><span class="sxs-lookup"><span data-stu-id="19dc6-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="19dc6-112">[Eemaldage](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) Office ' i litsents ja [määrake see uuesti](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ning seejärel [logige Office ' isse](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) sisse mõjutatud kasutajakonto kaudu.</span><span class="sxs-lookup"><span data-stu-id="19dc6-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="19dc6-113">Käivitage [aktiveerimise tõrkeotsija](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="19dc6-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="19dc6-114">[Lähtestage Office ' i aktiveerimise olek](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="19dc6-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="19dc6-115">[Office ' i võrgus parandamise](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span><span class="sxs-lookup"><span data-stu-id="19dc6-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="19dc6-116">Täiendavad tõrkeotsingu lahendused leiate järgmistest teemadest:</span><span class="sxs-lookup"><span data-stu-id="19dc6-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="19dc6-117">Litsentsimata toote ja aktiveerimisega seotud tõrketeated Office’is</span><span class="sxs-lookup"><span data-stu-id="19dc6-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="19dc6-118">Office’i aktiveerimisel kuvatakse tõrketeade: „Kahjuks ei saa teie kontoga ühendust luua. Proovige hiljem uuesti.“</span><span class="sxs-lookup"><span data-stu-id="19dc6-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)