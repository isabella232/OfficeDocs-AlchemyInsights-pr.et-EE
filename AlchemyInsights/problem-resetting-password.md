---
title: Parooli ennistamise probleem
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694380"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="51383-102">Parooli ennistamise probleemid</span><span class="sxs-lookup"><span data-stu-id="51383-102">Problems resetting password</span></span>

<span data-ttu-id="51383-103">Järgnevalt on toodud mõned probleemid, mis võivad parooli ennistamisel ja võimalike lahenduste leidmisel tekkida.</span><span class="sxs-lookup"><span data-stu-id="51383-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="51383-104">**Mul on probleem, mille parooli lähtestamine pole muudes kategooriates kaetud**</span><span class="sxs-lookup"><span data-stu-id="51383-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="51383-105">Veenduge, et teil on õigus paroole lähtestada.</span><span class="sxs-lookup"><span data-stu-id="51383-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="51383-106">Kasutaja paroole saab lähtestada ainult globaalsete, paroolide ja kasutajate administraatorite jaoks.</span><span class="sxs-lookup"><span data-stu-id="51383-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="51383-107">Globaalsed administraatorid saavad lähtestada ka muud privilegeeritud administraatori paroolid.</span><span class="sxs-lookup"><span data-stu-id="51383-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="51383-108">Veenduge, et mõistate litsentsimise nõudeid.</span><span class="sxs-lookup"><span data-stu-id="51383-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="51383-109">Teie ettevõttes peab olema vähemalt ühe litsentsiga määratud litsents.</span><span class="sxs-lookup"><span data-stu-id="51383-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="51383-110">Ainult pilveteenuse kasutajad – kõik Office 365 (O365) makstud SKU või Azure AD ' i põhifunktsioonid</span><span class="sxs-lookup"><span data-stu-id="51383-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="51383-111">Pilv ja/või kohapealsed kasutajad – Azure AD Premium P1 või P2, Enterprise Mobility + Security (EMS) või Secure produktiivne Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="51383-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="51383-112">Lisateavet litsentsimise nõuete kohta leiate artiklist [litsentsimise nõuded AZURE ad iseteeninduskeskuse parooli lähtestamiseks](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="51383-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="51383-113">**Mul on probleeme parooli lähtestamise poliitika seadmisega**</span><span class="sxs-lookup"><span data-stu-id="51383-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="51383-114">Hiljuti rakendatud poliitikad võivad võtta mitu minutit, et dubleerida kogu andmekeskuste ja lõpp-punkte.</span><span class="sxs-lookup"><span data-stu-id="51383-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="51383-115">Kehaline kaugus andmekeskuse mõjutab ka seda, kui kiiresti muudatusi rakendatakse.</span><span class="sxs-lookup"><span data-stu-id="51383-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="51383-116">Test lõppkasutajaga, mitte administraatoriga ja väikese kasutajate kogumiga piloot.</span><span class="sxs-lookup"><span data-stu-id="51383-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="51383-117">Azure ' i portaalis konfigureeritud poliitikad rakenduvad ainult lõppkasutajatele, mitte administraatoritele.</span><span class="sxs-lookup"><span data-stu-id="51383-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="51383-118">Microsoft jõustab iga Azure ' i administraatori rolli jaoks tugeva vaike-kahe värava parooli lähtestamise poliitika (nt globaalne administraator, kasutajatoe administraator, paroolide haldur jne).</span><span class="sxs-lookup"><span data-stu-id="51383-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="51383-119">Lugege lisateavet [administraatorite poliitikate](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)kohta.</span><span class="sxs-lookup"><span data-stu-id="51383-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="51383-120">**Soovin juurutada parooli lähtestamise, kuid ma ei soovi, et kasutajad ei saaks täiendavat turbeteavet registreerida**</span><span class="sxs-lookup"><span data-stu-id="51383-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="51383-121">Andmete eelasustamine kasutajate jaoks, et nad ei peaks seda tegema!</span><span class="sxs-lookup"><span data-stu-id="51383-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="51383-122">-Administraatorina saate määrata oma kasutajatele telefoni ja meili atribuudid enne, kui käivitate oma organisatsioonile parooli lähtestamise.</span><span class="sxs-lookup"><span data-stu-id="51383-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="51383-123">Seda saate teha API, PowerShelli või Azure AD Connecti abil.</span><span class="sxs-lookup"><span data-stu-id="51383-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="51383-124">Lisateavet leiate siit:</span><span class="sxs-lookup"><span data-stu-id="51383-124">More information here:</span></span>
- [<span data-ttu-id="51383-125">Parooli lähtestamise juurutamine, mis ei nõua kasutajatelt registreerumist</span><span class="sxs-lookup"><span data-stu-id="51383-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="51383-126">Milliseid andmeid parooli lähtestamine kasutab?</span><span class="sxs-lookup"><span data-stu-id="51383-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="51383-127">**Nupp "parooli lähtestamine" on Hall**</span><span class="sxs-lookup"><span data-stu-id="51383-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="51383-128">Teil pole õigust selle kasutaja paroole lähtestada.</span><span class="sxs-lookup"><span data-stu-id="51383-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="51383-129">Kasutaja paroole saab lähtestada ainult globaalsete, paroolide ja kasutajate administraatorite jaoks.</span><span class="sxs-lookup"><span data-stu-id="51383-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="51383-130">Globaalsed administraatorid saavad lähtestada ka muud privilegeeritud administraatori paroolid.</span><span class="sxs-lookup"><span data-stu-id="51383-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="51383-131">**Parooli lähtestamise tera ei kuvata**</span><span class="sxs-lookup"><span data-stu-id="51383-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="51383-132">Teil pole õigust paroole lähtestada.</span><span class="sxs-lookup"><span data-stu-id="51383-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="51383-133">Kasutaja paroole saab lähtestada ainult globaalsete, paroolide ja kasutajate administraatorite jaoks.</span><span class="sxs-lookup"><span data-stu-id="51383-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="51383-134">Globaalsed administraatorid saavad lähtestada ka muud privilegeeritud administraatori paroolid.</span><span class="sxs-lookup"><span data-stu-id="51383-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="51383-135">**Ma ei näe kohapealset integratsiooni Blade parooli lähtestamisel**</span><span class="sxs-lookup"><span data-stu-id="51383-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="51383-136">Kohapealne Integration Blade kuvatakse ainult hübriid-keskkonnas – see tähendab, et kasutate kohapealse kasutaja paroolide manipuleerimiseks parooli tagasikirjutusega.</span><span class="sxs-lookup"><span data-stu-id="51383-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="51383-137">Te ei näe seda tera, kui:</span><span class="sxs-lookup"><span data-stu-id="51383-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="51383-138">Te ei kasuta parooli tagasikirjutusega</span><span class="sxs-lookup"><span data-stu-id="51383-138">You are not using password writeback</span></span>
    - <span data-ttu-id="51383-139">Parooli tagasikirjutusega installi/ühenduvusega on probleeme</span><span class="sxs-lookup"><span data-stu-id="51383-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="51383-140">Azure AD Connecti installi/ühenduvusega on probleeme</span><span class="sxs-lookup"><span data-stu-id="51383-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="51383-141">Lisateavet tagasikirjutusega probleemide lahendamise kohta leiate teemast [parooli tagasikirjutusega tõrkeotsing](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="51383-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="51383-142">**Kasutaja parooli lähtestamine**</span><span class="sxs-lookup"><span data-stu-id="51383-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="51383-143">Logige Azure ' i portaali sisse sobiva administraatorina.</span><span class="sxs-lookup"><span data-stu-id="51383-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="51383-144">Valige kasutajad ja rühmad Blade, valige **Kõik kasutajad**.</span><span class="sxs-lookup"><span data-stu-id="51383-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="51383-145">Valige loendist kasutaja.</span><span class="sxs-lookup"><span data-stu-id="51383-145">Select a user from the list.</span></span>
1. <span data-ttu-id="51383-146">Valitud kasutaja jaoks valige **Ülevaade** ja seejärel klõpsake menüüribal käsku **Lähtesta parool**.</span><span class="sxs-lookup"><span data-stu-id="51383-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="51383-147">Järgige ekraanil kuvatavaid juhiseid.</span><span class="sxs-lookup"><span data-stu-id="51383-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="51383-148">Lähtestatakse ainult Azure ' i portaali toe parooli tagasikirjutusega.</span><span class="sxs-lookup"><span data-stu-id="51383-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="51383-149">**Ma lähtestan kohapealse kasutaja parooli Office 365 administraatori või Office 365 mobiilirakenduse kaudu, kuid kasutaja ei saa ikka sisse logida**</span><span class="sxs-lookup"><span data-stu-id="51383-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="51383-150">Selles portaalis pole parooli tagasikirjutusega toetatud.</span><span class="sxs-lookup"><span data-stu-id="51383-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="51383-151">Lähtestage kasutaja parool uuesti Azure ' i portaalis – portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="51383-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

