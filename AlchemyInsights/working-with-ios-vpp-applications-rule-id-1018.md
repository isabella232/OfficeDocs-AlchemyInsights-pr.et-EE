---
title: Töötamine iOS VPP taotluste reegli Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364844"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="17930-102">IOS VPP rakenduste töötamine</span><span class="sxs-lookup"><span data-stu-id="17930-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="17930-103">Loe [haldamine Köide-osta programmi Microsoft Intune'iga kaudu ostetud iOS rakendused](https://docs.microsoft.com/intune/vpp-apps-ios) õppida samme, mis funktsioone ja piiranguid Apple Köide osta programm ja toe Microsoft Intune seda kasutada.</span><span class="sxs-lookup"><span data-stu-id="17930-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="17930-104">**Ühiseid teemasid:** "Minu kasutajatele määratud rakendus iOS VPP, kuid installimine nurjus."</span><span class="sxs-lookup"><span data-stu-id="17930-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="17930-105">See juhtub, kui mitu mobiiltelefoni pakkujad ELis kasutatakse ühe VPP märgiks.</span><span class="sxs-lookup"><span data-stu-id="17930-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="17930-106">VPP märkide Apple võib kasutada ainult üks pakkuja.</span><span class="sxs-lookup"><span data-stu-id="17930-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="17930-107">Kui kasutasite märgiks VPP mitme pakkujatega, peab luba Intune uuesti laadida.</span><span class="sxs-lookup"><span data-stu-id="17930-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="17930-108">Install võib ebaõnnestuda ka kui käitiste koguarv ületab mitu litsentsi.</span><span class="sxs-lookup"><span data-stu-id="17930-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="17930-109">Kasutamise aruanne oma litsentside vaatamiseks Ava **Intune Mobile apps** \> **Rakenduse litsentside** lehekülg.</span><span class="sxs-lookup"><span data-stu-id="17930-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="17930-110">Nõuda litsentside kasutamise kohta teabe saamiseks vaadake [selles artiklis.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="17930-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
