---
title: Microsoft Defenderi kasutamine Office 365 anti-phishing Policy
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693241"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="fcff4-102">Microsoft Defenderi kasutamine Office 365 anti-phishing Policy</span><span class="sxs-lookup"><span data-stu-id="fcff4-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="fcff4-103">Need sätted võimaldavad poliitika nimega *domeen ja tegevjuht*.</span><span class="sxs-lookup"><span data-stu-id="fcff4-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="fcff4-104">See poliitika tagab nii kasutaja-kui ka domeeni kaitse ja rakendab seejärel poliitika kõigi domeenis kasutajate vastu võetud meilisõnumite kohta.</span><span class="sxs-lookup"><span data-stu-id="fcff4-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="fcff4-105">Esmalt lisage poliitika loomiseks järgmine teave.</span><span class="sxs-lookup"><span data-stu-id="fcff4-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="fcff4-106">**Nimi**: Domain and CEO **Kirjeldus**: tagab, et tegevjuht ja teie domeeni ei kehastata.</span><span class="sxs-lookup"><span data-stu-id="fcff4-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="fcff4-107">**Rakendatud**: valige **adressaadi Domeen**.</span><span class="sxs-lookup"><span data-stu-id="fcff4-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="fcff4-108">Valige **mõnest** jaotisest nupp **Vali** ja seejärel valige Domeen.</span><span class="sxs-lookup"><span data-stu-id="fcff4-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="fcff4-109">Valige **+ Lisa**.</span><span class="sxs-lookup"><span data-stu-id="fcff4-109">Select **+ Add**.</span></span> <span data-ttu-id="fcff4-110">Märkige loendis selle domeeni nimi (nt *contoso.com*) kõrval olev ruut ja seejärel valige **Lisa**.</span><span class="sxs-lookup"><span data-stu-id="fcff4-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="fcff4-111">Valige **valmis**.</span><span class="sxs-lookup"><span data-stu-id="fcff4-111">Select **Done**.</span></span>
- <span data-ttu-id="fcff4-112">Kui poliitika on loodud, saate poliitika viimistleda järgmiste suvandite abil.</span><span class="sxs-lookup"><span data-stu-id="fcff4-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="fcff4-113">**Kasutajate lisamine kaitsmiseks tehke järgmist.** Selles näites lisage tegevjuhi meiliaadress vähemalt.</span><span class="sxs-lookup"><span data-stu-id="fcff4-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="fcff4-114">**Domeenide lisamine, mida soovite kaitsta**: saate lisada ettevõtte tegevjuhti sisaldava domeeni.</span><span class="sxs-lookup"><span data-stu-id="fcff4-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="fcff4-115">Valige **toimingud**: meilisõnumi **saatmisel kehastanud kasutaja poolt** valige **suuna sõnum ümber teisele** meiliaadressile ja seejärel sisestage selle turvalisuse halduri meiliaadress (nt *securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="fcff4-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="fcff4-116">**Kui meilisõnumid saadetakse kehastava domeeni kaudu**, valige **sõnum karantiinis**.</span><span class="sxs-lookup"><span data-stu-id="fcff4-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="fcff4-117">**Postkasti luure**: Vaikimisi on see suvand valitud, kui loote uue andmepüügi poliitika.</span><span class="sxs-lookup"><span data-stu-id="fcff4-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="fcff4-118">Jätke **see säte parimate** tulemuste saamiseks.</span><span class="sxs-lookup"><span data-stu-id="fcff4-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="fcff4-119">**Usaldusväärsete saatjate ja domeenide lisamine.** Selles näites ära Määratle ühtegi alistamist.</span><span class="sxs-lookup"><span data-stu-id="fcff4-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="fcff4-120">Kui olete oma sätted üle vaadanud, valige **Loo see poliitika** või **Salvesta** vastavalt vajadusele.</span><span class="sxs-lookup"><span data-stu-id="fcff4-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="fcff4-121">Lisateavet leiate teemast [Microsoft 365 anti-andmepüügi poliitikad](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="fcff4-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
