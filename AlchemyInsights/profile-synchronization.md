---
title: Profiilisünkroonimine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320705"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Millal sünkroonitakse minu profiilimuudatused SharePoint kasutajaprofiili rakendusega?

SharePoint Online kasutab Active Directory impordi ajastitööd (AD Import) kasutajate ja rühmade importimiseks kasutajaprofiili rakendusse. 
  
1. AD Import sünkroonib muudatused SharePoint Veebikataloogi poest kasutajaprofiili rakendusse. Neid muudatusi töödeldakse pakettidena.
    
2. Ajastitöö käivitub seni, kuni muudatused sünkroonitakse.
    
**Märkus.** Töö käivitamiseks kulub aega sõltuvalt protsessis tehtud muudatuste arvust. Suur hulk muudatusi võtab kauem aega. Teenusetaseme lepingus (SLA) on sätestatud, et SharePoint Online Directory kasutaja muudatus kajastub kasutajaprofiili rakenduses 24 tunni pärast. 
  
[Lisateave kasutajaprofiili sünkroonimise kohta SharePoint Online'is](https://go.microsoft.com/fwlink/?linkid=875671)
  

