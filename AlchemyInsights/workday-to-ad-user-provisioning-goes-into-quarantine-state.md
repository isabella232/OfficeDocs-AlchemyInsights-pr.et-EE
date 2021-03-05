---
title: Tööpäeval AD kasutaja ettevalmistamine läheb karantiini olekusse
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481356"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Tööpäeval AD kasutaja ettevalmistamine läheb karantiini olekusse

**Tööpäeval AD kasutaja ettevalmistamine läheb karantiini olekusse ja REKLAAME ei looda kasutajad**

Tööpäev AD kasutaja ettevalmistamisel on läinud karantiini olekusse ja auditilogi kuvatakse tõrketeade tõrketeade **: OperationsError-SvcErr: ilmnes toimingu tõrge. Kataloogiteenuse jaoks pole ühtegi Superior-viidet konfigureeritud. Kataloogiteenus ei saa seega anda viiteid objektidele väljaspool seda metsa**. See tõrge kuvatakse tavaliselt siis, kui Active Directory ümbris OU pole õigesti määratud või kui **parentDistinguishedName** jaoks kasutatakse avaldiste vastendamisega seotud probleeme.

Märkige ruut **uute kasutajate** jaoks, kui teil on olemas kirjavigu käsitlev parameeter. Veenduge, et määratud OU on teie REKLAAMIs juba olemas. Kui kasutate atribuutide vastendamisel **parentDistinguishedName** , veenduge, et see hindaks alati teadaolevat konteinerit ad-domeenis. Loodud väärtuse kuvamiseks märkige jaotises auditi logid ruut ekspordi sündmus.

Lisateavet tööpäevade automaatseks ettevalmistamiseks konfigureerimise kohta leiate teemast [õpetus: tööpäevade automaatseks](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)ettevalmistamiseks konfigureerimine.

