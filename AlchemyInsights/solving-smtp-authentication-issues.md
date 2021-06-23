---
title: SMTP-autentimise ja tõrkeotsingu lubamine
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077647"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="be848-102">SMTP-autentimise ja tõrkeotsingu lubamine</span><span class="sxs-lookup"><span data-stu-id="be848-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="be848-103">Kui soovite postkasti jaoks lubada SMTP-autentimise või saate tõrke "Klient pole autenditud", "Autentimine nurjus" või "SmtpClientAuthentication" koodiga 5.7.57 või 5.7.3 või 5.7.139, kui proovite meilisõnumit edastada, autentides seadme või rakenduse Microsoft 365 abil, tehke probleemi lahendamiseks järgmist kolme toimingut.</span><span class="sxs-lookup"><span data-stu-id="be848-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="be848-104">Keelake [Azure'i turbe vaikesätted,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) kui soovite lubada turbe **vaikesäteteks** **Ei.**</span><span class="sxs-lookup"><span data-stu-id="be848-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="be848-105">a.</span><span class="sxs-lookup"><span data-stu-id="be848-105">a.</span></span> <span data-ttu-id="be848-106">Logige Azure'i portaali sisse turbeadministraatori, tingimusjuurdepääsu administraatori või üldadministraatorina.</span><span class="sxs-lookup"><span data-stu-id="be848-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="be848-107">b.</span><span class="sxs-lookup"><span data-stu-id="be848-107">b.</span></span> <span data-ttu-id="be848-108">Liikuge sirvides Azure Active Directory > **atribuutideni.**</span><span class="sxs-lookup"><span data-stu-id="be848-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="be848-109">c.</span><span class="sxs-lookup"><span data-stu-id="be848-109">c.</span></span> <span data-ttu-id="be848-110">Valige **Halda turbe vaikesätet**.</span><span class="sxs-lookup"><span data-stu-id="be848-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="be848-111">d.</span><span class="sxs-lookup"><span data-stu-id="be848-111">d.</span></span> <span data-ttu-id="be848-112">Määrake **väärtuse Luba turbe vaikesätted** väärtuseks **Ei**.</span><span class="sxs-lookup"><span data-stu-id="be848-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="be848-113">e.</span><span class="sxs-lookup"><span data-stu-id="be848-113">e.</span></span> <span data-ttu-id="be848-114">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="be848-114">Select **Save**.</span></span>

2. <span data-ttu-id="be848-115">[Luba kliendi SMTP-edastus](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) litsentsitud postkastis.</span><span class="sxs-lookup"><span data-stu-id="be848-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="be848-116">a.</span><span class="sxs-lookup"><span data-stu-id="be848-116">a.</span></span> <span data-ttu-id="be848-117">Avage Microsoft 365 halduskeskus Aktiivsed **kasutajad** ja valige kasutaja.</span><span class="sxs-lookup"><span data-stu-id="be848-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="be848-118">b.</span><span class="sxs-lookup"><span data-stu-id="be848-118">b.</span></span> <span data-ttu-id="be848-119">Avage vahekaart Meil ja valige jaotises **Meilirakendused** nupp **Halda meilirakendusi.**</span><span class="sxs-lookup"><span data-stu-id="be848-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="be848-120">d.</span><span class="sxs-lookup"><span data-stu-id="be848-120">d.</span></span> <span data-ttu-id="be848-121">Veenduge, **et autenditud SMTP** oleks märgitud (lubatud).</span><span class="sxs-lookup"><span data-stu-id="be848-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="be848-122">e.</span><span class="sxs-lookup"><span data-stu-id="be848-122">e.</span></span> <span data-ttu-id="be848-123">Valige **Salvesta muudatused**.</span><span class="sxs-lookup"><span data-stu-id="be848-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="be848-124">[Keelake litsentsitud postkastis mitme teguriga autentimine (MFA).](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa)</span><span class="sxs-lookup"><span data-stu-id="be848-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="be848-125">a.</span><span class="sxs-lookup"><span data-stu-id="be848-125">a.</span></span> <span data-ttu-id="be848-126">Avage Microsoft 365 halduskeskus ja valige vasakpoolses navigeerimismenüüs **Kasutajad**  >  **Aktiivsed kasutajad**.</span><span class="sxs-lookup"><span data-stu-id="be848-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="be848-127">b.</span><span class="sxs-lookup"><span data-stu-id="be848-127">b.</span></span> <span data-ttu-id="be848-128">Valige **Mitmikautentimine**.</span><span class="sxs-lookup"><span data-stu-id="be848-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="be848-129">c.</span><span class="sxs-lookup"><span data-stu-id="be848-129">c.</span></span> <span data-ttu-id="be848-130">Valige kasutaja ja keelake **mitme teguriga autentimine.**</span><span class="sxs-lookup"><span data-stu-id="be848-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
