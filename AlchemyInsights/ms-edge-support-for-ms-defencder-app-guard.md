---
title: Microsoft Edge ' i tugi Microsoft Defenderi rakenduse Guard jaoks
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583579"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="ce61d-102">Microsoft Edge ' i tugi Microsoft Defenderi rakenduse Guard jaoks</span><span class="sxs-lookup"><span data-stu-id="ce61d-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="ce61d-103">Windows 10 ja Microsoft Edge ' i jaoks loodud rakendus valvur kasutab riistvara-isolatsiooni lähenemist, mis võimaldab kasutajal liikuda ebausaldusväärsel saidil isoleeritud Hyper-V-toega konteineri seest, mis eraldatakse hosti operatsioonisüsteemist.</span><span class="sxs-lookup"><span data-stu-id="ce61d-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="ce61d-104">Ettevõtte administraator määratleb usaldusväärsete veebisaitide, pilve ressursside ja sisemiste võrkude loendi.</span><span class="sxs-lookup"><span data-stu-id="ce61d-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="ce61d-105">Kui kasutaja külastab saiti, mida loendis pole, avab Microsoft Edge saidi ümbrises.</span><span class="sxs-lookup"><span data-stu-id="ce61d-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="ce61d-106">See tähendab, et kui sait osutub pahatahtlikuks, jääb vastuvõttev arvuti kaitstud ja ründaja ei pääse ettevõtte andmetele juurde.</span><span class="sxs-lookup"><span data-stu-id="ce61d-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="ce61d-107">Pakendis olevate laienduste installimist toetatakse Microsoft Edge ' i versiooni 81 ja seda saab reguleerida poliitika kaudu.</span><span class="sxs-lookup"><span data-stu-id="ce61d-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="ce61d-108">UpdateURL-aadress, mida kasutatakse ExtensionInstallForcelist poliitikas, tuleks lisada neutraalse ressursina rakenduse Guard kasutatavas võrgu isolatsiooni poliitikas.</span><span class="sxs-lookup"><span data-stu-id="ce61d-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="ce61d-109">Lisateavet leiate teemast Microsoft Edge ' i [tugi Microsoft Defenderi rakenduse Guard jaoks](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="ce61d-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
