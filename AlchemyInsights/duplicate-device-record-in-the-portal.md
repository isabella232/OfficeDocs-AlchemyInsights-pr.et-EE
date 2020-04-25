---
title: Portaalis seadme kirje dubleerimine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789685"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="9f440-102">Portaalis seadme kirje dubleerimine</span><span class="sxs-lookup"><span data-stu-id="9f440-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="9f440-103">Kui seade ei raporteeri Configuration Manageri saidile kaashalduse olekut õigesti, võite näha portaalis seadme jaoks kahte kirjet.</span><span class="sxs-lookup"><span data-stu-id="9f440-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="9f440-104">Seadme kaashalduse oleku kontrollimiseks vaadake Configuration Manageri konsoolis seadme veergu **Kaashallatud**.</span><span class="sxs-lookup"><span data-stu-id="9f440-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="9f440-105">Kui veerg pole nähtav, võite selle lisada, paremklõpsates mõnda veerupäist ja valides selle loendist.</span><span class="sxs-lookup"><span data-stu-id="9f440-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="9f440-106">Suvandi Kaashallatav väärtus peab olema **Jah**.</span><span class="sxs-lookup"><span data-stu-id="9f440-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="9f440-107">Kui väärtus on **Ei**, avage klientrakenduses Configuration Manageri kliendi aplett ja kontrollige vahekaardil Üldine atribuuti **Kaashaldus**.</span><span class="sxs-lookup"><span data-stu-id="9f440-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="9f440-108">Kui väärtus on **Lubatud**, näitab see halduspunkti kliendisuhtuse probleeme.</span><span class="sxs-lookup"><span data-stu-id="9f440-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="9f440-109">Vaadake seadmes logi **CcmMessaging.log**, et uurida võimalikke ühenduvuse probleeme.</span><span class="sxs-lookup"><span data-stu-id="9f440-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="9f440-110">Kui väärtus on **Keelatud** ja seade on registreeritud Intune’is, veenduge, et seade oleks saanud kaashalduse poliitika, vaadates seadmes läbi logi **CoManagementHandler.log**.</span><span class="sxs-lookup"><span data-stu-id="9f440-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
