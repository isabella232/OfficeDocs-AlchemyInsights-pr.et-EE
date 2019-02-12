---
title: ADFS Föderatsiooni sertifikaadi kuni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 55529265d2356a911624026107fb639f93e29abd
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925376"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="4cb87-102">ADFS Föderatsiooni sertifikaadi kuni</span><span class="sxs-lookup"><span data-stu-id="4cb87-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="4cb87-103">Probleemi lahendamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="4cb87-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="4cb87-p101">Microsoft Azure Active Directory moodul jaoks Windows PowerShelli installimine arvutisse (kui moodul pole juba installitud). Selleks lähen [haldamine Windows PowerShelli abil Azure AD](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="4cb87-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="4cb87-106">Järgige selle "stsenaarium 1: AD FS luba sisselogimise sert aegunud" osa ["Ilmnes probleem saidile" tõrge, kui välise kasutaja logib sisse Office 365, Azure, või Intune ADFS](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="4cb87-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="4cb87-107">Järgige [Kuidas uuendada või remont ühendatud Domeen Office 365, Azure, või Intune seadeid](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="4cb87-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="4cb87-108">Föderatsiooni sertifikaatide uuendamise kohta lisateabe saamiseks vt [Office 365 ja Azure Active Directory Renew Föderatsiooni tunnistused](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="4cb87-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    

