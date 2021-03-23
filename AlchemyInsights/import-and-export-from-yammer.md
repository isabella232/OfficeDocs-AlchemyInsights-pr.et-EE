---
title: Yammeri importimine ja eksportimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035438"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="c65a1-102">Yammeri importimine ja eksportimine</span><span class="sxs-lookup"><span data-stu-id="c65a1-102">Import and export from Yammer</span></span>

<span data-ttu-id="c65a1-103">**Importimine**</span><span class="sxs-lookup"><span data-stu-id="c65a1-103">**Import**</span></span>

<span data-ttu-id="c65a1-104">Kasutaja – impordi suvandid sõltuvad sellest, kas teie Yammeri võrk on [Microsoft 365 jaoks kohalik režiim](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)või mitte.</span><span class="sxs-lookup"><span data-stu-id="c65a1-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="c65a1-105">**Muu režiim**: kasutajaid saab importida rühmadesse, kasutades [Lisa aadressiraamatust](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (Limit to 100 kasutajad) rühma sätetes või võrgu kaudu, mis kasutab [hulgi värskendust](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) võrgu administraatorina.</span><span class="sxs-lookup"><span data-stu-id="c65a1-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="c65a1-106">**Kohalik režiim**: rühma liikmelisus ja võrgu liikmelisuse toimingud tuleks teostada [Microsoft 365 administraatori portaalist](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portaalist](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)või mõne muu Azure AD suvandi abil.</span><span class="sxs-lookup"><span data-stu-id="c65a1-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="c65a1-107">Emakeelena režiimis olevatel võrkudel pole enam juurdepääsu lahtisele versioonile ja muudele varasematele funktsioonidele.</span><span class="sxs-lookup"><span data-stu-id="c65a1-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c65a1-108">Yammeri ei toetanud kunagi sisu importimist võrgu administraatorilt isegi siis, kui andmete eksportimise funktsiooni kasutati mõnes muus võrgus.</span><span class="sxs-lookup"><span data-stu-id="c65a1-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="c65a1-109">Sisu saab uuesti postitada partnerite lahendused või Yammeri ülejäänud API-d.</span><span class="sxs-lookup"><span data-stu-id="c65a1-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="c65a1-110">**Eksportimine**</span><span class="sxs-lookup"><span data-stu-id="c65a1-110">**Export**</span></span>

<span data-ttu-id="c65a1-111">Võrgu [andmete eksportimine võrgu administraatori](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) kaudu lubab sisu eksportida Yammeri võrkudes (sh sõnumid ja failid).</span><span class="sxs-lookup"><span data-stu-id="c65a1-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="c65a1-112">Manused võivad olla väga suured ja põhjustada eksportimisel olulise aja.</span><span class="sxs-lookup"><span data-stu-id="c65a1-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="c65a1-113">Soovitame aktiivseid võrke eksportida, kasutades [andmete eksportimise API](https://developer.yammer.com/docs/data-export-api) -d iga päev või nädal.</span><span class="sxs-lookup"><span data-stu-id="c65a1-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="c65a1-114">Microsoft support ei paku selleks kohandatud skripte.</span><span class="sxs-lookup"><span data-stu-id="c65a1-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="c65a1-115">Üksikute kasutajate jaoks sisu eksportimiseks on olemas eraldi [üldmääruse eksport](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) .</span><span class="sxs-lookup"><span data-stu-id="c65a1-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>