---
title: Seadme tagasikirjutusega
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256749"
---
# <a name="device-writeback"></a><span data-ttu-id="e13f7-102">Seadme tagasikirjutusega</span><span class="sxs-lookup"><span data-stu-id="e13f7-102">Device Writeback</span></span>

<span data-ttu-id="e13f7-103">Seadme tagasikirjutusega kasutatakse järgmistel juhtudel.</span><span class="sxs-lookup"><span data-stu-id="e13f7-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="e13f7-104">[Windowsi Hello ärirakenduse lubamine hübriid-serdi usaldatavuse juurutamise abil](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="e13f7-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="e13f7-105">Luba tingimuslik juurdepääs seadmetele, mis põhinevad ADFS (2012 R2 või uuem) kaitstud rakendustel (tuginedes osapoole Trust)</span><span class="sxs-lookup"><span data-stu-id="e13f7-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="e13f7-106">Seadme tagasikirjutusega jaoks on vaja Azure AD Premiumi tellimust.</span><span class="sxs-lookup"><span data-stu-id="e13f7-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="e13f7-107">See tagab täiendava turvalisuse ja kindluse, et juurdepääsu rakendustele antakse ainult usaldusväärsetele seadmetele.</span><span class="sxs-lookup"><span data-stu-id="e13f7-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="e13f7-108">Lisateavet tingimusjuurdepääsu kohta leiate teemast [riski haldamine tingimusliku juurdepääsuga](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) ja [asutusesisese tingimusjuurdepääsu häälestamine Azure Active Directory seadme registreerimise abil](https://docs.microsoft.com/azure/active-directory/devices/overview).</span><span class="sxs-lookup"><span data-stu-id="e13f7-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="e13f7-109">Seadmete tagasikirjutusega lubamise kohta leiate lisateavet artiklist [seadme tagasikirjutusega lubamine](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span><span class="sxs-lookup"><span data-stu-id="e13f7-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
