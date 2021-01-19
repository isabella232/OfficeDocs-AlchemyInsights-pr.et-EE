---
title: Rakendustesse sisselogimisega seotud probleemid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900873"
---
# <a name="issues-signing-in-to-applications"></a>Rakendustesse sisselogimisega seotud probleemid

Kasutaja sisselogimisega seotud probleemide põhjuse või diagnoosimise tuvastamiseks tehke järgmist.

1. Käivitage [sisselogimise diagnostika](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Analüüsitud sündmuse otsimine, sisestades andmed, mis on seotud kasutaja, rakenduse, sisselogimise aja, päringu ID või korrelatsiooni ID-ga.
3. Vaadake üle diagnostilised tulemused, kus on näha, mis juhtus ja milliseid toiminguid saab teha muudatuste tegemiseks, kui on vaja muudatusi teha.

Järgmised on mõned levinud probleemid, mis võivad rakendustesse sisselogimisel ilmneda.

1. Teil või kasutajal **on AZURE ad Logi sisse logida, kuid kuvatakse ootamatu viip** – lugege artiklit [ootamatute nõusolekute küsimine, kui logite](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) rakendusse sisse ja [ootamatu tõrge rakenduse nõusoleku](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)andmisel.
2. Teie või kasutaja **on rakenduse otse sisse loginud, kuid te ei saa seda deeplink kohandatud portaali või Accessi paneeli kaudu sisse logida**. lugege teemat [rakenduse Azure AD minu rakendused sisselogimisega seotud probleemide tõrkeotsing](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Teie või kasutaja **on AZURE ad Logi sisse loginud, kuid rakendus kuvab tõrketeate ja ei lase kasutajal end sisse logida**: probleem on selles, et rakendus ei nõustunud Azure AD ' i välja antud vastusega. Tõrkeotsingu tegemiseks tehke [järgmist](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) .
4. Teie või kasutaja **ei saa sisse logida rakendusse "mitte-Galerii", mis on konfigureeritud parooliga ühekordse sisselogimise** korral: tõrkeotsinguks järgige allolevaid [juhiseid.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
5. Teie või kasutaja **ei saa sisse logida AZURE ad Gallery rakendusse, mis on konfigureeritud parooliga ühekordse sisselogimise korral**, [tehke tõrkeotsinguks järgmist.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
6. Teie või kasutaja **ei saa Microsofti rakendusse sisse logida**: tõrkeotsinguks järgige [järgmisi juhiseid](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) .
7. Teie või kasutaja **ei saa sisse logida väliseks ühekordseks sisselogimiseks konfigureeritud mitte-Galerii rakendusse**: tõrkeotsinguks järgige [järgmisi juhiseid](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) .
8. Te või kasutaja **ei saa sisse logida AZURE ad Gallery rakendusse, mis on konfigureeritud ühendatud ühekordse sisselogimise jaoks**, [tehke tõrkeotsinguks järgmist.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)
9. Teie või kasutaja **ei saa kohandatud rakendusse sisse logida**: tõrkeotsinguks [toimige](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) järgmiselt.
10. Teie või kasutaja **ei saa AZURE ad Application puhverserveri kaudu asutusesisesesse rakendusse sisse logida**: tõrkeotsinguks järgige [järgmisi juhiseid](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) .

