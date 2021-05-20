---
title: Välistuste konfigureerimine Microsoft Defenderi ATP skannimiseks
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
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543681"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="b5d64-102">Välistuste konfigureerimine Microsoft Defenderi ATP skannimiseks</span><span class="sxs-lookup"><span data-stu-id="b5d64-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="b5d64-103">Üldiselt saate teatud faililaiendid ja kaustaasukohad skannitud failidest Microsoft Defenderi ATP välistada.</span><span class="sxs-lookup"><span data-stu-id="b5d64-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="b5d64-104">Samuti saate konfigureerida teatud protsessides avatud failide välistamised.</span><span class="sxs-lookup"><span data-stu-id="b5d64-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="b5d64-105">Lisateavet leiate teemast Välistamiste konfigureerimine [ja valideerimine](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) faililaiendi ja kausta asukoha alusel ning Protsessides avatud [failide välistamiste konfigureerimine.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="b5d64-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="b5d64-106">Windows **Server 2016 ja 2019** välistamiste konfigureerimiseks lugege [teemat Microsoft Defenderi viirusetõrje-serveri Windows konfigureerimine.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="b5d64-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="b5d64-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="b5d64-107">**Mac**</span></span>

<span data-ttu-id="b5d64-108">Lisateavet toetatud välistamistüüpide ja Maci välistamiste loendi konfigureerimise kohta leiate teemast [Toetatud](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) välistamistüübid [ja Välistamiste loendi konfigureerimine.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="b5d64-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="b5d64-109">**Märkus** Välistamiste loendeid saate valideerida ka EICAR-i testifaili abil.</span><span class="sxs-lookup"><span data-stu-id="b5d64-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="b5d64-110">Lisateavet leiate teemast Välistamiste [loendite valideerimine EICAR-i testifaili abil.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="b5d64-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="b5d64-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="b5d64-111">**Linux**</span></span>

<span data-ttu-id="b5d64-112">Lisateavet toetatud välistamistüüpide ja Linuxi välistamiste loendi [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) konfigureerimise kohta leiate artiklitest Toetatud välistamistüübid ja [Linuxi jaoks Microsoft Defenderi ATP välistamiste konfigureerimine ja valideerimine.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="b5d64-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="b5d64-113">**Märkus** Välistamiste loendeid saate valideerida ka EICAR-i testifaili abil.</span><span class="sxs-lookup"><span data-stu-id="b5d64-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="b5d64-114">Lisateavet leiate teemast Välistamiste [loendite valideerimine EICAR-i testifaili abil.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="b5d64-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 