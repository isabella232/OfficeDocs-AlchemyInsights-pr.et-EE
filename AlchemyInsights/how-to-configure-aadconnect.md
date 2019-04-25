---
title: 646 kuidas seadistada AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399767"
---
# <a name="configure-sync-features"></a><span data-ttu-id="58557-102">Sünkroonimise funktsioonide konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="58557-102">Configure sync features</span></span>

<span data-ttu-id="58557-103">Azure AD ühenduse loomine hõlmab funktsioone, mis on vaikimisi või saate lubada hiljem.</span><span class="sxs-lookup"><span data-stu-id="58557-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="58557-104">Mõni nõuda täiendavaid konfiguratsiooni teatud keskkondades.</span><span class="sxs-lookup"><span data-stu-id="58557-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="58557-105">[Filtreerimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) piirid objektid on sünkroonitud Azure AD.</span><span class="sxs-lookup"><span data-stu-id="58557-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="58557-106">Vaikimisi, kõik kasutajad, kontaktide, rühmade ja Windows 10 arvuti kontod on sünkroonitud.</span><span class="sxs-lookup"><span data-stu-id="58557-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="58557-107">Saate kaasata või välja jätta vastavalt domeenid, organisatsiooniüksused või atribuudid objektid.</span><span class="sxs-lookup"><span data-stu-id="58557-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="58557-108">[Parooli räsi syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sünkroonib parooli räsi asutusesisese Active Directory Azure AD.</span><span class="sxs-lookup"><span data-stu-id="58557-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="58557-109">See võimaldab salasõnade haldus ühes kohas, kuid kasutada sama parooli nii asutusesisese ja pilve keskkondades.</span><span class="sxs-lookup"><span data-stu-id="58557-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="58557-110">Sest Active Directory on usaldusväärne allikas, saate oma parooli poliitika.</span><span class="sxs-lookup"><span data-stu-id="58557-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="58557-111">[Iseteeninduse parooli lähtestada (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) võimaldab kasutajatel oma paroolide lähtestamiseks pilves samas eelnevatega kohapeal paroolipoliitika.</span><span class="sxs-lookup"><span data-stu-id="58557-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="58557-112">[Seadme tagasikirjutusega](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) võimaldab registreeritud seadmed tuleb kirjutada tagasi asutusesisese Active Directory, nii et neid saab kasutada juurdepääsu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="58557-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="58557-113">[Juhusliku oovin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) lubatakse vaikimisi, et vältida liiga palju samaaegseid objekti kustutamist (üle 500 objekti sünkroonimise kohta).</span><span class="sxs-lookup"><span data-stu-id="58557-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="58557-114">Saate muuta seda sätet vastavalt organisatsiooni vajadustele.</span><span class="sxs-lookup"><span data-stu-id="58557-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="58557-115">[Automaatne versioonitäiendus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) on vaikimisi kiire käitiste ja tagada teie versioon Azure AD ühenduse on alati ajakohane.</span><span class="sxs-lookup"><span data-stu-id="58557-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
