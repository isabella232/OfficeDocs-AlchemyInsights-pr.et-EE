---
title: Rakenduste kustutamine või taastamine
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014798"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="8b5aa-102">Rakenduste kustutamine või taastamine</span><span class="sxs-lookup"><span data-stu-id="8b5aa-102">Delete or restore applications</span></span>

<span data-ttu-id="8b5aa-103">**AZURE ad rentniku rakenduse kustutamiseks tehke** järgmist.</span><span class="sxs-lookup"><span data-stu-id="8b5aa-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="8b5aa-104">Valige **AZURE ad portaalis** **Enterprise Applications (Enterprise Applications**).</span><span class="sxs-lookup"><span data-stu-id="8b5aa-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="8b5aa-105">Seejärel otsige üles ja valige rakendus, mille soovite kustutada.</span><span class="sxs-lookup"><span data-stu-id="8b5aa-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="8b5aa-106">Klõpsake vasakpoolse paani jaotises **haldamine** nuppu **Atribuudid**.</span><span class="sxs-lookup"><span data-stu-id="8b5aa-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="8b5aa-107">Valige **Kustuta** ja seejärel valige **Jah** , et kinnitada, et soovite rakenduse Azure AD rentnikult kustutada.</span><span class="sxs-lookup"><span data-stu-id="8b5aa-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="8b5aa-108">Lisateavet rakenduse kustutamise kohta leiate teemast [Kiirjuhend: rakenduse kustutamine Azure Active Directory (AZURE ad) rentniku kaudu](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="8b5aa-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="8b5aa-109">PowerShellis eemaldab cmdlet [-käsk Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) rakenduses Azure Active Directory teatud rakenduse puhverserveri konfiguratsioonid ja saab rakenduse täielikult kustutada, kui see on määratud.</span><span class="sxs-lookup"><span data-stu-id="8b5aa-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="8b5aa-110">**Kustutatud rakenduse saate taastada** PowerShelli abil.</span><span class="sxs-lookup"><span data-stu-id="8b5aa-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="8b5aa-111">Kui rakendus, mille soovite taastada, on tuvastatud, saate selle taastada, kasutades [AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="8b5aa-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
