---
title: Kasutajate halduse probleemid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035531"
---
# <a name="user-management-issues"></a>Kasutajate halduse probleemid

**Mis juhtub rakendusega praegune määratud kasutajad, kui ma keelan atribuudi "kasutaja määramine on nõutav" (selle atribuudi seadmine pole)?**

**Nõutud kasutaja ülesande** keelamine ei mõjuta praegu määratud kasutajaid. Selle atribuudi keelamine lubab ainult kõigil kasutajatel rakendusele juurde pääseda. Kõik loetletud kasutajad ja rakenduse rühmadele määratud kasutajad jäävad endiselt kehtima.

- Rakenduse piiramiseks kindlate kasutajate kogumiga lugege teemat [AZURE ad ' i rakenduse piiramine kasutajate kogumiga – Microsoft Identity Platform | Microsoft docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Kasutajate ja rühmade määramiseks rakenduses Azure Active Directory (Azure AD) Azure ' i portaalis või PowerShelli abil leiate [lisateavet teemast rakenduse User määrang haldamine rakenduses Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Rakenduse loomise ja haldamise õiguse delegeerimise kohta leiate teavet teemast [delegaadi rakenduse halduse administraatoriõigused – AZURE ad | Microsoft docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Teatud Enterprise ' i rakenduste peitmine kasutajate hulgast** – järgmiste toimingute abil saate peita kõik Microsoft 365 rakendused **MyApps** paanilt. Rakendused on endiselt nähtavad Office 365 portaalis.

 1. Logige Azure ' i portaali sisse oma kataloogi globaalse administraatorina. 
 2. Valige **Azure Active Directory**. 
 3. Valige **Kasutajad**. 
 4. Valige **kasutaja sätted**. 
 5. Klõpsake jaotises **Enterprise Applications (Enterprise Applications**) nuppu **Halda, kuidas lõppkasutajad rakendusi käivitada ja vaadata** 
 6. **Kasutajatele saab office 365 portaalis vaadata ainult office 365 rakendusi**, klõpsake nuppu **Jah**. 
 7. Klõpsake nuppu **Salvesta**. 
 8. Lisateavet leiate teemast [ettevõtte rakenduse peitmine kasutaja AZURE ad rakenduses | Microsoft docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Kui pakute tarkvara teenusena (SaaS) mitmele organisatsioonile, saate oma rakenduse konfigureerida nii, et see aktsepteeriks sisselogimisi mis tahes Azure Active Directory (Azure AD) rentniku kaudu. Selle konfiguratsiooni nimi on "mitme rentniku taotluse koostamine". Mis tahes Azure AD rentniku kasutajad saavad teie rakendusse sisse logida pärast seda, kui olete oma konto kasutamisega oma kontoga nõustunud. Lisateavet leiate teemast [AZURE ad kasutajate sisselogimise rakendused – Microsoft Identity Platform | Microsoft docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Kuidas saab lõppkasutaja kasutada rakendust, kui ta on rakendusele määratud?**

Iga rakenduses Enterprise Application Blade on link lõppkasutajatele juurdepääsemiseks. Kasutajad pääsevad rakenduse kaudu **Myapps** portaali kaudu juurde ka lihtsal viisil.

- **Kas soovite teada, milliseid rakendusi ja tüüpi rakendusi kasutajad kasutavad?**

Saate alla laadida viimase 30 päeva **portal.azure.com > Azure Active directory> Signins> alla laadida aruandeid**.

- Siit saate teada, kuidas [anda rakenduse rentniku jaoks administraatorile nõusolekut](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) ja [konfigureerida, kuidas lõppkasutajad rakendustega nõustuvad](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Saate teada, [Kuidas nõusolek toimib](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) ja [haldab rakenduste nõusolekut](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


