---
title: Teenuse osutamise teenuse konfigureerimine
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481853"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="c1114-102">Teenuse osutamise teenuse konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="c1114-102">Configuring the Provision service</span></span>

<span data-ttu-id="c1114-103">Kui soovite, et automatiseeritud kasutaja ettevalmistamine töötaks, on Azure AD-s vaja kehtivaid mandaate, mis võimaldavad tal luua ühenduse tööpäevaga veebiteenuste API</span><span class="sxs-lookup"><span data-stu-id="c1114-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="c1114-104">Lisaks kinnitatakse, et kui kasutaja saab luua ühenduse AD-domeeniga seotud Azure AD Connecti agendiga, siis kinnitab see, et tööpäeval töötav nupp Test Connection to AD Useri ettevalmistamine.</span><span class="sxs-lookup"><span data-stu-id="c1114-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="c1114-105">Kui Azure ' i portaalis kuvatakse mandaadi salvestamisel tõrge, järgige allpool soovitatud juhiseid.</span><span class="sxs-lookup"><span data-stu-id="c1114-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="c1114-106">Veenduge, et olete konfigureerinud tööpäevade integreerimise süsteemi kasutajakonto, nagu on näidatud jaotises õpetus, et [konfigureerida integratsiooni süsteemi kasutaja tööpäevas](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="c1114-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="c1114-107">Veenduge, et Azure AD Connecti ettevalmistamine agendi teenus töötab ja töötab teie kohapealses Windowsi serveris teenuste halduskonsooli abil.</span><span class="sxs-lookup"><span data-stu-id="c1114-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="c1114-108">Samuti saate kontrollida agendi olekut Azure ' i portaalis, klõpsates nuppu Kuva kohapealsed agendid.</span><span class="sxs-lookup"><span data-stu-id="c1114-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="c1114-109">Veenduge, et sisestate välja "tööpäevade username" väärtuse, kasutades vormingut username@workday-rentniku nimi.</span><span class="sxs-lookup"><span data-stu-id="c1114-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="c1114-110">Kui tööpäev – rentniku nimi on puudu, siis tööpäevade autentimine nurjub.</span><span class="sxs-lookup"><span data-stu-id="c1114-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="c1114-111">Kui konfigureerite integratsiooni tööpäevade rakendamise rentniku jaoks, arvestage oma tööpäevade rentniku ajastatud seisakute tundi.</span><span class="sxs-lookup"><span data-stu-id="c1114-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="c1114-112">Tööpäeval on planeeritud aeg selle rakendamiseks rentnike jaoks nädalavahetustel (tavaliselt reede õhtul kuni laupäeva hommikul) ja Ühenduvus ebaõnnestumised selle seisakute aknas on teadaolev probleem, mis automaatselt lahendatakse kohe, kui rakendamise rentnikud on tagasi võrgus.</span><span class="sxs-lookup"><span data-stu-id="c1114-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="c1114-113">Harvadel juhtudel võite seda viga näha ka juhul, kui selle integreerimise süsteemi kasutaja parool on rentniku värskendamise tõttu muudetud või kui konto on lukustatud või aegunud olekus.</span><span class="sxs-lookup"><span data-stu-id="c1114-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="c1114-114">Palun kontrolli oma tööpäevade administraatoriga integreerimise süsteemi kasutaja olekut.</span><span class="sxs-lookup"><span data-stu-id="c1114-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="c1114-115">Lisateavet tööpäevade automaatseks ettevalmistamiseks konfigureerimise kohta leiate teemast [õpetus: tööpäevade automaatseks](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)ettevalmistamiseks konfigureerimine.</span><span class="sxs-lookup"><span data-stu-id="c1114-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
