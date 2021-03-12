---
title: Microsoft Defenderi ATP-skannimise erandite konfigureerimine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713571"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="5242d-102">Microsoft Defenderi ATP-skannimise erandite konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="5242d-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="5242d-103">Üldiselt saate Microsoft Defenderi ATP-st skannitud teatud laiendite ja kaustade asukohad välistada.</span><span class="sxs-lookup"><span data-stu-id="5242d-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="5242d-104">Saate ka konfigureerida teatud protsessidega avatavate failide välistused.</span><span class="sxs-lookup"><span data-stu-id="5242d-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="5242d-105">Lisateavet leiate teemast [laiendite ja kaustade asukoha põhjal välistamine ja valideerimise](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) tühistamine ning [protsesside kaudu avatud failide eemaldamise välistamine](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="5242d-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="5242d-106">**Windows server 2016 ja 2019** erandite konfigureerimiseks lugege artiklit [Microsoft Defenderi viirusetõrje väljaarvamiste konfigureerimine Windows serveris](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="5242d-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="5242d-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="5242d-107">**Mac**</span></span>

<span data-ttu-id="5242d-108">Lisateavet toetatud tõrjutuse tüüpide ja Mac-arvutis erandite loendi konfigureerimise kohta leiate teemast [toetatud välistamise tüübid](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) ja [nende kõrvaldamise loendi konfigureerimine](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="5242d-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="5242d-109">**Märkus** Saate EICAR abil kinnitada ka erandite loendeid.</span><span class="sxs-lookup"><span data-stu-id="5242d-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="5242d-110">Lisateavet leiate teemast EICAR-i [testimise failidega seotud loendite kinnitamine](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="5242d-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="5242d-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="5242d-111">**Linux**</span></span>

<span data-ttu-id="5242d-112">Lisateavet toetatud tõrjutuse tüüpide ja Linuxi jaoks mõeldud erandite loendi konfigureerimise kohta leiate teemast [toetatud tõrjutuse tüübid](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) ja [konfigureerimine ning valideerimine Microsoft Defenderi ATP for Linuxis](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="5242d-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="5242d-113">**Märkus** Saate EICAR abil kinnitada ka erandite loendeid.</span><span class="sxs-lookup"><span data-stu-id="5242d-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="5242d-114">Lisateavet leiate teemast EICAR-i [testimise failidega seotud loendite kinnitamine](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="5242d-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 