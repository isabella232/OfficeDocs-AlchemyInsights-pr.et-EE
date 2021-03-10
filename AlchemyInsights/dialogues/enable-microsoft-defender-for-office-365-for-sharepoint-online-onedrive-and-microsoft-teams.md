---
title: Microsoft Defenderi lubamine Office 365 for SharePoint Online ' i, OneDrive ' i ja Microsoft Teamsi jaoks
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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693246"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="32883-102">Microsoft Defenderi lubamine Office 365 for SharePoint Online ' i, OneDrive ' i ja Microsoft Teamsi jaoks</span><span class="sxs-lookup"><span data-stu-id="32883-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="32883-103">Logige sisse oma üldadministraatori või administraatori mandaadiga, logige sisse teenusekomplekti [Office 365 turbe-ja vastavuskontrolli keskusse](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="32883-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="32883-104">Valige vasakpoolsel paanil **ohu haldus** ja seejärel valige **poliitika**  >  [Turvalised manused](https://protection.office.com/safeattachment).</span><span class="sxs-lookup"><span data-stu-id="32883-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="32883-105">Valige **Lülita Microsoft Defenderi jaoks ette Office 365 SharePointi, OneDrive ' i ja Microsoft teamsi** jaoks ning seejärel valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="32883-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="32883-106">Globaalse administraatorina või SharePoint Online ' i administraatorina käivitage järgmine PowerShelli cmdlet, mille **DisallowInfectedFileDownload** parameeter on seatud väärtusele *True*: [Set-spotenantiga](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="32883-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="32883-107">Teatiste häälestamine tuvastatud failide jaoks</span><span class="sxs-lookup"><span data-stu-id="32883-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="32883-108">Lisateavet leiate teemast [Microsoft Defender for Office 365 SharePointi, OneDrive ' i ja Microsoft teamsi](https://go.microsoft.com/fwlink/?linkid=2092041)jaoks.</span><span class="sxs-lookup"><span data-stu-id="32883-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
