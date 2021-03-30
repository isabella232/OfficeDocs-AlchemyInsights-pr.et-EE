---
title: API-õigused ja nõusolekuprotsess
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404503"
---
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="2740e-102">API-õigused ja nõusolekuprotsess</span><span class="sxs-lookup"><span data-stu-id="2740e-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="2740e-103">Selleks et teie rakendus pääseks Microsoft Graphis andmetele juurde, peab kasutaja või administraator andma sellele nõusolekuprotsessi kaudu õiged õigused.</span><span class="sxs-lookup"><span data-stu-id="2740e-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="2740e-104">[Microsoft Graphi õiguste viidetes](https://docs.microsoft.com/graph/permissions-reference) loetletakse kõigi Microsoft Graphi API-de põhikomplektiga seotud õigused.</span><span class="sxs-lookup"><span data-stu-id="2740e-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="2740e-105">Samuti annab see juhiseid õiguste kasutamise kohta.</span><span class="sxs-lookup"><span data-stu-id="2740e-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="2740e-106">**Teenusesubjekti häälestamine või värskendamine**</span><span class="sxs-lookup"><span data-stu-id="2740e-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="2740e-107">[Teenuseprintipaali loomine](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – selles artiklis kirjeldatakse, kuidas luua uus servicePrincipal-objekt.</span><span class="sxs-lookup"><span data-stu-id="2740e-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="2740e-108">[Azure AD-&](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) teenusesubjekti loomine portaalis – selles artiklis kirjeldatakse, kuidas luua uus Azure Active Directory (Azure AD) rakendus ja teenusesubjekt, mida saab kasutada rollipõhise juurdepääsu juhtelemendiga.</span><span class="sxs-lookup"><span data-stu-id="2740e-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="2740e-109">[Rakendused & Teenusesubjektid Azure AD-s](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) . Selles artiklis kirjeldatakse Rakenduse registreerimist, rakenduseobjekte ja teenusesubjekte Azure Active Directorys: mis need on, kuidas neid kasutatakse ja kuidas need on omavahel seotud.</span><span class="sxs-lookup"><span data-stu-id="2740e-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="2740e-110">**Rakenduse registreerimise lisamine või värskendamine ja administraatori nõusoleku andmine**</span><span class="sxs-lookup"><span data-stu-id="2740e-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="2740e-111">[Rakenduse registreerimise loomine](https://docs.microsoft.com/graph/api/application-post-applications) – selles artiklis kirjeldatakse, kuidas luua uus rakendusobjekt.</span><span class="sxs-lookup"><span data-stu-id="2740e-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="2740e-112">[Rakenduse registreerimise värskendamine – API-õigused](https://docs.microsoft.com/graph/api/application-update) – selles artiklis kirjeldatakse, kuidas värskendada rakenduseobjekti atribuute.</span><span class="sxs-lookup"><span data-stu-id="2740e-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="2740e-113">[Administraatori nõusoleku andmine](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – administraatori nõusoleku ja nõusoleku andmiseks üldiselt nõuame, et administraator annab selgesõnaliselt nõusoleku.</span><span class="sxs-lookup"><span data-stu-id="2740e-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="2740e-114">[RBAC (beetaversioon)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – rollihalduse ümbris ühtse rollimääratluste ja rolliülesannete jaoks Microsoft 365 RBAC-i pakkujatele, kes toetavad ühte rollimäärangut mitmele subjektile ja mitmele ulatusele.</span><span class="sxs-lookup"><span data-stu-id="2740e-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="2740e-115">See erineb *ressursitüübist rbacApplication.*</span><span class="sxs-lookup"><span data-stu-id="2740e-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="2740e-116">Microsoft Intune on näide sellisest RBAC-pakkujast.</span><span class="sxs-lookup"><span data-stu-id="2740e-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="2740e-117">Intune'i rollimäärangul võib olla subjektide massiiv ja ulatuserühmade massiiv.</span><span class="sxs-lookup"><span data-stu-id="2740e-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="2740e-118">**See on beetaversioon, mis tähendab, et see on alles arenduses ja seda ei soovitata kasutada tootmises.**</span><span class="sxs-lookup"><span data-stu-id="2740e-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>
