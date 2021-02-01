---
title: Mandaadiga seotud probleemid
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063627"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="6cbf0-102">Mandaadiga seotud probleemid</span><span class="sxs-lookup"><span data-stu-id="6cbf0-102">Issues with credentials</span></span>

<span data-ttu-id="6cbf0-103">[Microsoft Identity Platform ja oauthi 2,0 Client mandaatide voog](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) kirjeldab, kuidas programmeerida otse OAuthi 2,0 kliendi mandaatide andmise voogu.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="6cbf0-104">**Kuidas hallata rakenduse parooli või serdi mandaati?**</span><span class="sxs-lookup"><span data-stu-id="6cbf0-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="6cbf0-105">Rakenduses Azure CLI saate kasutada [AZ AD Rakenduse mandaati](https://docs.microsoft.com/cli/azure/ad/app/credential) , et kustutada, loetleda või lähtestada rakenduse parooli või serdi mandaati.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="6cbf0-106">**Kuidas saavad kasutajad oma paroolid lähtestada?**</span><span class="sxs-lookup"><span data-stu-id="6cbf0-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="6cbf0-107">Kasutajad peavad oma paroolide lähtestamiseks [registreerima end teenuse parooli lähtestamiseks](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) .</span><span class="sxs-lookup"><span data-stu-id="6cbf0-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="6cbf0-108">Kui kasutaja on registreerunud, saavad nad oma parooli lähtestamiseks järgida selle artikli juhiseid: [töö või kooli parooli lähtestamine](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span><span class="sxs-lookup"><span data-stu-id="6cbf0-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="6cbf0-109">**Kuidas saavad kasutajad oma paroole muuta?**</span><span class="sxs-lookup"><span data-stu-id="6cbf0-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="6cbf0-110">Kasutajad saavad selle artikli juhiseid järgides oma paroole muuta: [parooli muutmine](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="6cbf0-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="6cbf0-111">Nad saavad ka [hallata rakenduse paroole kaheastmeline kinnitamiseks](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span><span class="sxs-lookup"><span data-stu-id="6cbf0-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="6cbf0-112">**Kasutaja saab parooli muutmisel või lähtestamisel tõrketeate**</span><span class="sxs-lookup"><span data-stu-id="6cbf0-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="6cbf0-113">See link annab teavet levinud probleemide kohta, mis võivad tekkida siis, kui kasutaja proovib lähtestada parooli: [levinud probleemid ja nende lahendused](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="6cbf0-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="6cbf0-114">**Mul on probleeme kasutaja parooli ennistamisega**</span><span class="sxs-lookup"><span data-stu-id="6cbf0-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="6cbf0-115">Veenduge, et teil on õigus paroole lähtestada.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="6cbf0-116">*Kasutaja paroole saab lähtestada ainult globaalsete, paroolide ja kasutajate administraatorite jaoks.*</span><span class="sxs-lookup"><span data-stu-id="6cbf0-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="6cbf0-117">Globaalsed administraatorid saavad lähtestada ka muud privilegeeritud administraatori paroolid.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="6cbf0-118">Veenduge, et mõistate litsentsimise nõudeid.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="6cbf0-119">Teie ettevõttes peab olema vähemalt ühe litsentsiga määratud litsents.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="6cbf0-120">**Ainult pilveteenuse kasutajad** – kõik Office 365 (O365) makstud SKU või Azure AD ' i põhifunktsioonid</span><span class="sxs-lookup"><span data-stu-id="6cbf0-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="6cbf0-121">**Pilv ja/või kohapealsed kasutajad** – Azure AD Premium P1 või P2, Enterprise Mobility + Security (EMS) või Secure produktiivne Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="6cbf0-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="6cbf0-122">Lisateavet litsentsimise nõuete kohta leiate teemast [AZURE ad iseteeninduskeskuse parooli lähtestamise litsentsimise nõuded](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span><span class="sxs-lookup"><span data-stu-id="6cbf0-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="6cbf0-123">Kasutaja parooli lähtestamiseks otsige üles Azure AD kasutaja.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="6cbf0-124">Seejärel klõpsake selle kasutaja ülevaates nuppu "Lähtesta parool".</span><span class="sxs-lookup"><span data-stu-id="6cbf0-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="6cbf0-125">**Nupp "parooli lähtestamine" on Hall**</span><span class="sxs-lookup"><span data-stu-id="6cbf0-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="6cbf0-126">Teil pole õigust **selle** kasutaja paroole lähtestada.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="6cbf0-127">*Kasutaja paroole saab lähtestada ainult globaalsete, paroolide ja kasutajate administraatorite jaoks.*</span><span class="sxs-lookup"><span data-stu-id="6cbf0-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="6cbf0-128">Globaalsed administraatorid saavad lähtestada ka muud privilegeeritud administraatori paroolid.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="6cbf0-129">**Parooli lähtestamise tera ei kuvata**</span><span class="sxs-lookup"><span data-stu-id="6cbf0-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="6cbf0-130">Teil pole õigust paroole lähtestada.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="6cbf0-131">*Kasutaja paroole saab lähtestada ainult globaalsete, paroolide ja kasutajate administraatorite jaoks.*</span><span class="sxs-lookup"><span data-stu-id="6cbf0-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="6cbf0-132">Globaalsed administraatorid saavad lähtestada ka muud privilegeeritud administraatori paroolid.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="6cbf0-133">**Ma ei näe kohapealset integratsiooni Blade parooli lähtestamisel**</span><span class="sxs-lookup"><span data-stu-id="6cbf0-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="6cbf0-134">Kohapealne Integration Blade kuvatakse ainult hübriid-keskkonnas – see tähendab, et kasutate kohapealse kasutaja paroolide manipuleerimiseks parooli tagasikirjutusega.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="6cbf0-135">Te ei näe seda tera, kui:</span><span class="sxs-lookup"><span data-stu-id="6cbf0-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="6cbf0-136">Te ei kasuta parooli tagasikirjutusega</span><span class="sxs-lookup"><span data-stu-id="6cbf0-136">You are not using password writeback</span></span>
  - <span data-ttu-id="6cbf0-137">Parooli tagasikirjutusega installi/ühenduvusega on probleeme</span><span class="sxs-lookup"><span data-stu-id="6cbf0-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="6cbf0-138">Azure AD Connecti installi/ühenduvusega on probleeme</span><span class="sxs-lookup"><span data-stu-id="6cbf0-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="6cbf0-139">Lisateavet tagasikirjutusega seotud probleemide tõrkeotsingu kohta leiate teemast [parooli tagasikirjutusega tõrkeotsing](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="6cbf0-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="6cbf0-140">**Kasutaja parooli lähtestamine**</span><span class="sxs-lookup"><span data-stu-id="6cbf0-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="6cbf0-141">Logige Azure ' i portaali sisse sobiva administraatorina.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="6cbf0-142">Valige **kasutajad ja rühmad** Blade, valige **Kõik kasutajad**.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="6cbf0-143">Valige loendist kasutaja.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-143">Select a user from the list.</span></span>
4. <span data-ttu-id="6cbf0-144">Valitud kasutaja jaoks valige **Ülevaade** ja seejärel valige käsuriba käsk **Lähtesta parool**.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="6cbf0-145">Valige nupp **Lähtesta parool** ja järgige ekraanil kuvatavaid juhiseid.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="6cbf0-146">Lähtestatakse ainult **Azure ' i portaali** toe parooli tagasikirjutusega.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="6cbf0-147">**Ma lähtestan kohapealse kasutaja parooli Office 365 administraatori või Office 365 mobiilirakenduse kaudu, kuid kasutaja ei saa ikka sisse logida**</span><span class="sxs-lookup"><span data-stu-id="6cbf0-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="6cbf0-148">Selles portaalis pole parooli tagasikirjutusega toetatud.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="6cbf0-149">Lähtestage kasutaja parool uuesti Azure ' i portaalis.</span><span class="sxs-lookup"><span data-stu-id="6cbf0-149">Reset the user's password again in the Azure portal.</span></span>
