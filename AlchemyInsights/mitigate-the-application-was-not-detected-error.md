---
title: Tõrke Rakendust ei leitud lahendamine
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
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836347"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="774a3-102">Tõrke „Rakendust ei leitud“ lahendamine</span><span class="sxs-lookup"><span data-stu-id="774a3-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="774a3-103">Intune’i edastatud rakenduse installimise tõrge „Rakendust ei leitud pärast installimise edukat lõpuleviimist“ võib ilmneda kõigil peamistel OS-i platvormidel (Windows, iOS ja Android).</span><span class="sxs-lookup"><span data-stu-id="774a3-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="774a3-104">Levinumad seda tõrget tekitavad stsenaariumid on järgmised.</span><span class="sxs-lookup"><span data-stu-id="774a3-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="774a3-105">Pärast algset juurutamist värskendati rakendus väljaspool Intune’i (kolmanda osapoole rakenduste poest).</span><span class="sxs-lookup"><span data-stu-id="774a3-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="774a3-106">Näiteks võivad osad rakendused (nt Google Chrome) teha automaatseid värskendusi.</span><span class="sxs-lookup"><span data-stu-id="774a3-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="774a3-107">Kasutaja on rakenduse pärast esialgset installimist desinstallinud.</span><span class="sxs-lookup"><span data-stu-id="774a3-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="774a3-108">Selle probleemi lahendamiseks kõigepealt vaadake mõjutatud seadmed läbi et teha kindlaks tõrke ilmnemise stsenaarium.</span><span class="sxs-lookup"><span data-stu-id="774a3-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="774a3-109">Kui rakendust värskendati väljaspool Intune’i, saab rakenduse käivitamise häälestada rakenduse versiooni ignoreerima.</span><span class="sxs-lookup"><span data-stu-id="774a3-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="774a3-110">Selleks määrake jaotises **Rakenduse konfigureerimine > Rakenduse teave** suvand **Ignoreeri rakendust** valikule **Jah**.</span><span class="sxs-lookup"><span data-stu-id="774a3-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="774a3-111">Sihtklientide jaoks võib olla asjakohane juurutada rakenduse „nagu vaja“ ja tagada, et juurutatud oleks uusim versioon.</span><span class="sxs-lookup"><span data-stu-id="774a3-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="774a3-112">Teise võimalusena on iOS-i platvormil võimalik kasutada funktsiooni **automaatne uuendamine**, mis on seostatud Apple’i mahu ostmise programmiga, mille saab konfigureerida automaatselt värskendama uuele versioonile, kui need avaldatakse.</span><span class="sxs-lookup"><span data-stu-id="774a3-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="774a3-113">Rakenduse installiprobleemide tõrkeotsingu kohta leiate lisateavet teemast [Rakenduse installiprobleemide tõrkeotsing](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="774a3-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
