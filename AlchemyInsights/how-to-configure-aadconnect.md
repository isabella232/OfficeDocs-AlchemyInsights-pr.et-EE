---
title: 646 kuidas konfigureerida AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722531"
---
# <a name="configure-sync-features"></a><span data-ttu-id="5c53d-102">Sünkroonimise funktsioonide konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="5c53d-102">Configure sync features</span></span>

<span data-ttu-id="5c53d-103">Azure AD ühenduse sisaldab mitmeid funktsioone, mis on vaikimisi lubatud või et saate lubada hiljem.</span><span class="sxs-lookup"><span data-stu-id="5c53d-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="5c53d-104">Mõned funktsioonid vajavad täiendavat konfiguratsiooni konkreetses keskkonnas.</span><span class="sxs-lookup"><span data-stu-id="5c53d-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="5c53d-105">[Filtreerimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) piirab objektid SÜNKROONITAKSE Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5c53d-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="5c53d-106">Vaikimisi sünkroonitakse kõik kasutajad, kontaktid, rühmad ja Windows 10 arvutikontod.</span><span class="sxs-lookup"><span data-stu-id="5c53d-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="5c53d-107">Saate objekte lisada või välistada domeenide, organisatsiooniüksused või muude atribuutide alusel.</span><span class="sxs-lookup"><span data-stu-id="5c53d-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="5c53d-108">[Parooli Hash sünkroonimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sünkroonib parooli Hash asutusesisese Active DIRECTORY Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5c53d-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="5c53d-109">See võimaldab parooli haldamine ühes kohas, kuid sama parooli kasutamine nii asutusesisese kui ka pilve keskkondades.</span><span class="sxs-lookup"><span data-stu-id="5c53d-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="5c53d-110">Kuna Active Directory on autoriteetne allikas, saate kasutada oma paroolipoliitikat.</span><span class="sxs-lookup"><span data-stu-id="5c53d-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="5c53d-111">[Iseteeninduse parooli lähtestamine (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) võimaldab kasutajatel lähtestada oma paroolid pilve samas endiselt rakendada oma asutusesisese parooli poliitika.</span><span class="sxs-lookup"><span data-stu-id="5c53d-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="5c53d-112">[Seadme tagasikirja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) võimaldab registreeritud seadmete Azure AD kirjutatakse tagasi asutusesisese Active Directory, et neid saab kasutada tingimuslik juurdepääs.</span><span class="sxs-lookup"><span data-stu-id="5c53d-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="5c53d-113">[Vältida juhuslikku kustutamist](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) on vaikimisi lubatud, et aidata vältida liiga palju samaaegseid objekti kustutamist (rohkem kui 500 objektid sünkroonimise kohta).</span><span class="sxs-lookup"><span data-stu-id="5c53d-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="5c53d-114">Seda sätet saate muuta oma organisatsiooni vajaduste rahuldamiseks.</span><span class="sxs-lookup"><span data-stu-id="5c53d-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="5c53d-115">[Automaatne täiendamine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) on vaikimisi lubatud Express seadmete jaoks ja aitab tagada, et teie Azure AD ühenduse versioon on alati praegune.</span><span class="sxs-lookup"><span data-stu-id="5c53d-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
