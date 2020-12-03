---
title: Parooli tagasikirjutamise lubamine Azure AD Connectis
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560436"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="e7ca1-102">Parooli tagasikirjutamise lubamine Azure AD Connectis</span><span class="sxs-lookup"><span data-stu-id="e7ca1-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="e7ca1-103">Selleks et lubada iseteeninduslikku paroolilähtestuse tagasikirjutamist, peate esmalt Azure AD Connectis lubama tagasikirjutamise võimaluse.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="e7ca1-104">Tehke Azure AD Connecti serveri kaudu järgmised toimingud.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="e7ca1-105">Logige sisse Azure AD Connecti serverisse ja käivitage **Azure AD Connecti** konfigureerimisviisard.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="e7ca1-106">Klõpsake lehel **Tere tulemast** nuppu **Konfigureeri**.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="e7ca1-107">Lehel **Lisaülesanded** valige **Kohanda sünkroonimissuvandeid** ja seejärel klõpsake nuppu **Edasi**.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="e7ca1-108">Lehel **Loo ühendus Azure AD-ga** sisestage oma Azure’i rentniku üldadministraatori identimisteave ja seejärel klõpsake nuppu **Edasi**.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="e7ca1-109">Filtreerimislehtedel **Ühenda kataloogid** ja **Domeen/OÜ** klõpsake nuppu **Edasi**.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="e7ca1-110">Lehel **Valikulised funktsioonid** märkige valiku **Parooli tagasikirjutamine** kõrval olev kastike ja klõpsake nuppu **Edasi**.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="e7ca1-111">Lehel **Konfigureerimiseks valmis** klõpsake nuppu **Konfigureeri** ja oodake, kuni protsess lõpeb.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="e7ca1-112">Kui näete, et konfigureerimine on lõppenud, klõpsake nuppu **Välju**.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="e7ca1-113">Kui parooli tagasikirjutamine on Azure AD Connectis lubatud, konfigureerige Azure AD SSPR-i tagasikirjutamine.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="e7ca1-114">SSPR-is parooli tagasikirjutamise lubamiseks tehke järgmised toimingud.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="e7ca1-115">Logige üldadministraatori kontot kasutades sisse Microsoft Azure’i portaali.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="e7ca1-116">Otsige üles **Azure Active Directory** ja valige see, klõpsake valikut **Paroolilähtestus** ning seejärel valikut **Kohapealne integreerimine**.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="e7ca1-117">Määrake küsimuse **Soovite paroole tagasi kirjutada oma kohapealsesse kataloogi?** vastuseks **Jah**.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="e7ca1-118">Määrake küsimuse **Lubate kasutajatel kontosid lukust avada ilma oma parooli lähtestamata?** vastuseks **Jah**.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="e7ca1-119">Kui olete valmis, klõpsake nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-119">When ready, click **Save**.</span></span>

<span data-ttu-id="e7ca1-120">Lisateavet leiate artiklist [Kuidas lubada Azure Active Directoryil iseteeninduslikku paroolilähtestuse tagasikirjutamist kohapealsesse keskkonda](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="e7ca1-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="e7ca1-121">Kui administraator lähtestab Azure’i portaalis kasutaja parooli ja see on väliskasutaja või parool räsisünkroonitud, kirjutatakse parool tagasi kohapealsesse keskkonda.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="e7ca1-122">Seda funktsiooni ei toetata praegu Office’i haldusportaalis.</span><span class="sxs-lookup"><span data-stu-id="e7ca1-122">This functionality is currently not supported in the Office Admin portal.</span></span>