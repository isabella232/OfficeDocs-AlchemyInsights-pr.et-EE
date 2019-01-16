---
title: Töötamine iOS VPP taotluste reegli Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286068"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="3445a-102">IOS VPP rakenduste töötamine</span><span class="sxs-lookup"><span data-stu-id="3445a-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="3445a-103">Loe [haldamine Köide-osta programmi Microsoft Intune'iga kaudu ostetud iOS rakendused](https://docs.microsoft.com/intune/vpp-apps-ios) õppida samme, mis funktsioone ja piiranguid Apple Köide osta programm ja toe Microsoft Intune seda kasutada.</span><span class="sxs-lookup"><span data-stu-id="3445a-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="3445a-104">**Ühiseid teemasid:** "Minu kasutajatele määratud rakendus iOS VPP, kuid installimine nurjus."</span><span class="sxs-lookup"><span data-stu-id="3445a-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="3445a-p101">See juhtub, kui mitu mobiiltelefoni pakkujad ELis kasutatakse ühe VPP märgiks. VPP märkide Apple võib kasutada ainult üks pakkuja. Kui kasutasite märgiks VPP mitme pakkujatega, peab luba Intune uuesti laadida.</span><span class="sxs-lookup"><span data-stu-id="3445a-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="3445a-p102">Install võib ebaõnnestuda ka kui käitiste koguarv ületab mitu litsentsi. Kasutamise aruanne oma litsentside vaatamiseks Ava **Intune Mobile apps** \> **Rakenduse litsentside** lehekülg. Nõuda litsentside kasutamise kohta teabe saamiseks vaadake [selles artiklis.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="3445a-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

