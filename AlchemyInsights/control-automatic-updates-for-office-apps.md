---
title: Office ' i rakenduste automaatsete värskenduste reguleerimine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438994"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="c8976-102">Office ' i rakenduste automaatsete värskenduste reguleerimine</span><span class="sxs-lookup"><span data-stu-id="c8976-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="c8976-103">Vaikimisi laaditakse Office ' i rakenduste värskendused automaatselt alla ja rakendatakse taustal ilma kasutaja sekkumiseta.</span><span class="sxs-lookup"><span data-stu-id="c8976-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="c8976-104">Administraatorid saavad siiski määrata, kuidas värskendusi Office Update ' i sätete abil rakendada.</span><span class="sxs-lookup"><span data-stu-id="c8976-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="c8976-105">Sätete värskendamine võimaldab administraatoritel lubada või keelata automaatvärskendused, kuvada või peita Office ' i nupp **Värskenda kohe** , määrata värskendamise tähtajad ja muud.</span><span class="sxs-lookup"><span data-stu-id="c8976-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="c8976-106">Üksikasjalikku teavet leiate järgmistest teemadest:</span><span class="sxs-lookup"><span data-stu-id="c8976-106">For detailed information, see:</span></span>

- [<span data-ttu-id="c8976-107">Office ' i värskenduste sätete konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="c8976-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="c8976-108">Office ' i automaatne värskendamine pole lubatud</span><span class="sxs-lookup"><span data-stu-id="c8976-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="c8976-109">Office ' i värskendamise määratlemine pärast selle installimist</span><span class="sxs-lookup"><span data-stu-id="c8976-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="c8976-110">Klientarvutile rakendatud olemasolevate värskenduste sätete vaatamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="c8976-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="c8976-111">Avage registriredaktor, minnes käsule **Start**  >  **Käivita**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="c8976-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="c8976-112">Aktiveerige järgmine asukoht ja vaadake üle Office ' i värskendamise sätted.</span><span class="sxs-lookup"><span data-stu-id="c8976-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="c8976-113">loomine.</span><span class="sxs-lookup"><span data-stu-id="c8976-113">a.</span></span> <span data-ttu-id="c8976-114">HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="c8976-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="c8976-115">b.</span><span class="sxs-lookup"><span data-stu-id="c8976-115">b.</span></span> <span data-ttu-id="c8976-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="c8976-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="c8976-117">**Märkus**  Kui OfficeMgmtCOM võti on seatud, võidakse kuvada **Office '** i  >  **konto**  >  **Office**' i värskenduste kaudu teade "värskendusi haldab teie süsteemiadministraator".</span><span class="sxs-lookup"><span data-stu-id="c8976-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="c8976-118">Lisateavet leiate teemast Microsoft [365 rakenduste värskenduste haldamine Microsoft Endpoint Configuration Manageri abil](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="c8976-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  