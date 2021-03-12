---
title: Linkide ja URL-idega seotud probleemid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707878"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="c06f9-102">Linkide ja URL-idega seotud probleemid</span><span class="sxs-lookup"><span data-stu-id="c06f9-102">Issues with links and URLs</span></span>

<span data-ttu-id="c06f9-103">Ümbersuunamise URI/vastuse URL-id (mõlemad avaldised on asendatavad) on URL-id, mida Microsofti identimisplatvorm kasutab rakenduste taotletud sõnede tagastamiseks.</span><span class="sxs-lookup"><span data-stu-id="c06f9-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="c06f9-104">Lisateavet nende URL-ide kohta leiate järgmistest artiklitest:</span><span class="sxs-lookup"><span data-stu-id="c06f9-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="c06f9-105">[Autentimisvood ja rakenduse stsenaariumid](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - teave URI-ide ümbersuunamise kohta lehel **Rakenduse registreerimine** iga stsenaariumi jaoks.</span><span class="sxs-lookup"><span data-stu-id="c06f9-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="c06f9-106">Ümbersuunamise URI/vastuse URL-i kitsendused ja piirangud</span><span class="sxs-lookup"><span data-stu-id="c06f9-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="c06f9-107">**Ma ei tea, kuidas registreerida rakenduse jaoks õige ümbersuunamise URI või vastuse URL**</span><span class="sxs-lookup"><span data-stu-id="c06f9-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="c06f9-108">Kui logite sisse koos arendatava rakendusega ja sisselogimisdialoogis kuvatakse **AADSTS50011: taotluses määratud vastuse URL ei vasta rakenduse jaoks konfigureeritud vastuse URL-idele <your app ID>**, peate oma rakenduse registreerimisele lisama ümbersuunamise URI, mida teie kood kasutas sõne taotluses Microsofti identiteediplatvormile.</span><span class="sxs-lookup"><span data-stu-id="c06f9-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="c06f9-109">Vastuse URL-i lisamiseks minge oma lehel **rakenduse registreerimine** Azure'i portaali vahekaardile **Autentimine** ja lisage kirje jaotises **URI-de ümbersuunamine**.</span><span class="sxs-lookup"><span data-stu-id="c06f9-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="c06f9-110">Sisestatav väärtus sõltub loodava rakenduse tüübist, nagu allpool on kirjeldatud:</span><span class="sxs-lookup"><span data-stu-id="c06f9-110">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="c06f9-111">Ühe lehega rakenduste ja veebirakenduste puhul on vastuse URL teie rakenduse URL.</span><span class="sxs-lookup"><span data-stu-id="c06f9-111">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="c06f9-112">Vaadake [Ühelehelise rakenduse registreerimine](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) või [Veebirakenduse registreerimine Azure'i portaalis](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="c06f9-112">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="c06f9-113">Töölauarakenduste puhul sõltub valitav väärtus järgnevast:</span><span class="sxs-lookup"><span data-stu-id="c06f9-113">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="c06f9-114">platvormist (MacOS erineb Windowsist või Linuxist)</span><span class="sxs-lookup"><span data-stu-id="c06f9-114">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="c06f9-115">viisist, kuidas te loa hankisite (interaktiivselt, seadme koodivooga, integreeritud Windowsi autentimisteenusega (IWA) või kasutajanime/parooliga).</span><span class="sxs-lookup"><span data-stu-id="c06f9-115">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="c06f9-116">Üksikasjad leiate teemast [Töölauarakendused - rakenduse registreerimine - URi ümbersuunamine](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="c06f9-116">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="c06f9-117">Mobiilsideseade rakenduste ümbersuunamise URI sõltub järgnevast:</span><span class="sxs-lookup"><span data-stu-id="c06f9-117">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="c06f9-118">platvormist (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="c06f9-118">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="c06f9-119">rakenduse loomiseks kasutatud teavest (nt komplekti ID iOS-is ning paketi nimi ja allkirja räsiväärtus Androidis). Azure'i portaali rakenduse registreerimine aitab teid.</span><span class="sxs-lookup"><span data-stu-id="c06f9-119">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="c06f9-120">Lisateavet leiate teemast [Platvormi konfigureerimise ja ümbersuunamise URI-d](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="c06f9-120">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="c06f9-121">Veebi-API-d ja mõned hääletud loa hankimise viisid (IWA ja kasutajanimi/parool) ei nõua ümbersuunamise URI-d.</span><span class="sxs-lookup"><span data-stu-id="c06f9-121">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="c06f9-122">**Juurutasin oma veebirakenduse ja juurutatud rakenduse testimisel saan vastuseks URL-i lahknevuse teate**</span><span class="sxs-lookup"><span data-stu-id="c06f9-122">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="c06f9-123">Lisage ümbersuunamise URI-d kõigi nende asukohtade jaoks, kus te oma veebirakendust juurutate.</span><span class="sxs-lookup"><span data-stu-id="c06f9-123">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="c06f9-124">Lisateavet leiate teemast [Registreerige veebirakendused kasutades Azure‘i portaali](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span><span class="sxs-lookup"><span data-stu-id="c06f9-124">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="c06f9-125">Lisage asukohale ümbersuunamise URI kohe pärast seda, kui olete rakenduse selles asukohas juurutanud.</span><span class="sxs-lookup"><span data-stu-id="c06f9-125">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="c06f9-126">**Ma ei saa registreerida piisavalt vastuse URL-e**</span><span class="sxs-lookup"><span data-stu-id="c06f9-126">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="c06f9-127">Olete sõltumatu tarkvaratootja (ISV) ja teil on igale kliendile üks või mitu ümbersuunamise URI.</span><span class="sxs-lookup"><span data-stu-id="c06f9-127">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="c06f9-128">Soovite versioonist ADAL/Azure AD v1.0 migreerida MSAL/Microsofti identimisplatvormile ning te olete jõudnud [maksimaalse ümbersuunamise URI-de arvuni](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="c06f9-128">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="c06f9-129">Probleemi lahendamiseks [lisage ümbersuunamise URI-d teenusesubjektitele](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) mis vastavad igale teie kliendile.</span><span class="sxs-lookup"><span data-stu-id="c06f9-129">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
