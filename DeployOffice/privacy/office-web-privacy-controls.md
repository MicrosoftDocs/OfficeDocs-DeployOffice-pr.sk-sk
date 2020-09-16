---
title: Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office na webe s nastaveniami politiky
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
audience: ITPro
ms.topic: article
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection: Ent_O365
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
description: V tomto článku získajú správcovia služieb Office informácie o postupoch spravovania nastavení ochrany osobných údajov pre aplikácie Office na webe.
hideEdit: true
ms.openlocfilehash: b5131d5ffc09b28a3b5731a417fcd6d383fb7d01
ms.sourcegitcommit: da41d41b443c8392c96e64a4d2fc674957abddf5
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/11/2020
ms.locfileid: "47431985"
---
# <a name="use-policy-settings-to-manage-privacy-controls-for-office-for-the-web-applications"></a><span data-ttu-id="3824c-103">Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office na webe s nastaveniami politiky</span><span class="sxs-lookup"><span data-stu-id="3824c-103">Use policy settings to manage privacy controls for Office for the web applications</span></span>

> [!NOTE]
> <span data-ttu-id="3824c-104">Ak si chcete pozrieť zoznam produktov balíka Office, na ktorý sa vzťahujú tieto informácie o ochrane osobných údajov, pozrite si tému [Ovládacie prvky na ochranu osobných údajov dostupné pre produkty balíka Office](products-versions-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="3824c-104">For a list of Office products covered by this privacy information, see [Privacy controls available for Office products](products-versions-privacy-controls.md).</span></span>

<span data-ttu-id="3824c-105">Ako správca vašej organizácie môžete určiť, či majú vaši používatelia možnosť používať voliteľné online funkcie pri používaní Office na webe, ako je napríklad Word na webe alebo PowerPoint na webe.</span><span class="sxs-lookup"><span data-stu-id="3824c-105">As an administrator for your organization, you can control whether your users have the choice to use optional connected experiences when they use Office for the web applications, such as Word for the web or PowerPoint for the web.</span></span> <span data-ttu-id="3824c-106">Táto možnosť je k dispozícii pre používateľov len v prípade, že keď používajú aplikácie Office na webe, sú prihlásení pomocou pracovného alebo školského konta.</span><span class="sxs-lookup"><span data-stu-id="3824c-106">This choice is available to your users only if they're signed in with their work or school account when they use Office for the web applications.</span></span> <span data-ttu-id="3824c-107">Pomocou nastavenia politiky *Povoliť používanie dodatočných voliteľných pripojených funkcií v Office* môžete určiť, či budú mať vaši používatelia možnosť používať voliteľné online funkcie.</span><span class="sxs-lookup"><span data-stu-id="3824c-107">To control whether your users have the choice to use optional connected experiences, you use the *Allow the use of additional optional connected experiences in Office* policy setting.</span></span>

## <a name="overview-of-optional-connected-experiences"></a><span data-ttu-id="3824c-108">Prehľad voliteľných online funkcií</span><span class="sxs-lookup"><span data-stu-id="3824c-108">Overview of optional connected experiences</span></span>

<span data-ttu-id="3824c-109">Voliteľne online funkcie sú cloudové služby, ktoré sú k dispozícii pre používateľov, keď používajú aplikáciu Office.</span><span class="sxs-lookup"><span data-stu-id="3824c-109">Optional connected experiences are cloud-backed services that are available to your users when they’re using Office.</span></span> <span data-ttu-id="3824c-110">Príkladmi voliteľných online funkcií je vytvorenie kartogramu v Exceli alebo vloženie obrázka online do wordového dokumentu, pretože obe využívajú možnosti poskytované technológiou Microsoft Bing.</span><span class="sxs-lookup"><span data-stu-id="3824c-110">Examples of optional connected experiences include creating a map chart in Excel or inserting an online picture into your Word document, both of which rely on services provided by Microsoft Bing.</span></span> <span data-ttu-id="3824c-111">Používanie týchto cloudových služieb je voliteľné.</span><span class="sxs-lookup"><span data-stu-id="3824c-111">The use of these cloud-backed services is optional.</span></span> 

<span data-ttu-id="3824c-112">Na voliteľné pripojené funkcie sa nevzťahuje komerčná zmluva vašej spoločnosti so spoločnosťou Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3824c-112">Optional connected experiences are not covered by your organization’s commercial agreement with Microsoft.</span></span> <span data-ttu-id="3824c-113">Voliteľné pripojené funkcie ponúka priamo spoločnosť Microsoft a riadia sa [zmluvou o poskytovaní služieb spoločnosti Microsoft](https://www.microsoft.com/servicesagreement).</span><span class="sxs-lookup"><span data-stu-id="3824c-113">Instead, optional connected experiences are offered by Microsoft directly to your users and are governed by the [Microsoft Services Agreement](https://www.microsoft.com/servicesagreement).</span></span> <span data-ttu-id="3824c-114">V niektorých prípadoch sa prostredníctvom týchto voliteľných funkcií poskytujú obsah alebo funkcie tretích strán a môžu sa na ne vzťahovať aj ďalšie podmienky.</span><span class="sxs-lookup"><span data-stu-id="3824c-114">In some cases, third-party content or functionality are provided through these optional connected experiences and other terms may also apply.</span></span>

<span data-ttu-id="3824c-115">Niektoré voliteľné online funkcie nemusia byť dostupné v aplikáciách Office na webe, ale sú dostupné pri používaní oných verzií aplikácie Office, napríklad počítačovej verzie na zariadení so systémom Windows.</span><span class="sxs-lookup"><span data-stu-id="3824c-115">Some optional connected experiences might not be available in Office for the web applications, but are available when using other versions of Office, such as the desktop version on a device running Windows.</span></span>

<span data-ttu-id="3824c-116">Ďalšie informácie sa nachádzajú v téme [Prehľad voliteľných online funkcií v balíku Office](optional-connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="3824c-116">For more information, see [Overview of optional connected experiences in Office](optional-connected-experiences.md).</span></span>

## <a name="configure-the-policy-setting-by-using-the-office-cloud-policy-service"></a><span data-ttu-id="3824c-117">Konfigurácia nastavenia politiky pomocou služby politiky Office v cloude</span><span class="sxs-lookup"><span data-stu-id="3824c-117">Configure the policy setting by using the Office cloud policy service</span></span>

<span data-ttu-id="3824c-118">Pomocou nastavenia politiky *Povoliť používanie dodatočných voliteľných pripojených funkcií v Office* môžete určiť, či budú mať vaši používatelia možnosť používať voliteľné online funkcie.</span><span class="sxs-lookup"><span data-stu-id="3824c-118">You can use the *Allow the use of additional optional connected experiences in Office* policy setting to control whether your users have the choice to use optional connected experiences.</span></span> <span data-ttu-id="3824c-119">Ak chcete nakonfigurovať nastavenie politiky pre aplikácie Office pre web, musíte použiť [službu politiky Office v cloude](../overview-office-cloud-policy-service.md).</span><span class="sxs-lookup"><span data-stu-id="3824c-119">To configure this policy setting for Office for the web applications, you need to use the [Office cloud policy service](../overview-office-cloud-policy-service.md).</span></span>  

<span data-ttu-id="3824c-120">Ak nenakonfigurujete toto nastavenie politiky, tieto voliteľné online funkcie budú k dispozícii pre vašich používateľov.</span><span class="sxs-lookup"><span data-stu-id="3824c-120">If you don’t configure this policy setting, the choice to use optional connected experiences will be available to your users.</span></span> <span data-ttu-id="3824c-121">Ak toto nastavenie politiky zakážete, vaši používatelia nebudú mať k dispozícii žiadne voliteľné online funkcie.</span><span class="sxs-lookup"><span data-stu-id="3824c-121">If you disable this policy setting, your users won’t be able to use any of the optional connected experiences.</span></span>

<span data-ttu-id="3824c-122">Pre aplikácie Office na webe sa nastavenie politiky vzťahuje na prípad, keď vaši používatelia pracujú na dokumentoch balíka Office, ktoré sú uložené na webovom úložisku od spoločnosti, ako je napríklad OneDrive for Business alebo SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="3824c-122">For Office for the web applications, the policy setting applies to when your users are working on Office documents that are saved to web-based storage from Microsoft, such as OneDrive for Business or SharePoint Online.</span></span>

<span data-ttu-id="3824c-123">Keďže používate službu politiky Office v cloude, toto nastavenie politiky platí, aj keď vaši používatelia používajú Office na zariadeniach s Windowsom, iOS, Androidom alebo zariadeniach Mac.</span><span class="sxs-lookup"><span data-stu-id="3824c-123">Because you’re using the Office cloud policy service, this policy setting also applies to when your users are using Office on Windows, Mac, iOS, or Android devices.</span></span> <span data-ttu-id="3824c-124">Toto nastavenie politiky nie je možné nakonfigurovať len pre používateľov, ktorí používajú aplikácie Office na webe,</span><span class="sxs-lookup"><span data-stu-id="3824c-124">You can’t configure this policy setting just for when your users are using Office for the web applications.</span></span> <span data-ttu-id="3824c-125">Môžete však vytvoriť konfiguráciu politiky, ktorá zahŕňa toto nastavenie politiky a nastaviť túto konfiguráciu politiky tak, aby platila iba pre používateľov, ktorí k dokumentom pristupujú anonymne pomocou aplikácií Office na webe.</span><span class="sxs-lookup"><span data-stu-id="3824c-125">But, you can create a policy configuration that includes this policy setting and have that policy configuration only apply to users that access documents anonymously using Office for the web applications.</span></span>

<span data-ttu-id="3824c-126">Ak sa rozhodnete používateľom sprístupniť voliteľné online funkcie, pri prvom použití aplikácie Office pre web sa im zobrazí oznámenie o ochrane osobných údajov.</span><span class="sxs-lookup"><span data-stu-id="3824c-126">If you choose to make optional connected experiences available to your users, your users will be shown a privacy notification the first time they use an Office for the web app.</span></span> <span data-ttu-id="3824c-127">Toto oznámenie oznamuje používateľom, že ste im udelili možnosť používať tieto voliteľné online funkcie.</span><span class="sxs-lookup"><span data-stu-id="3824c-127">This notification lets your users know that you’ve given them the option to use these optional connected experiences.</span></span> <span data-ttu-id="3824c-128">Oznámenie tiež informuje používateľov o tom, že voliteľné online funkcie sa poskytujú v rámci zmluvy o poskytovaní služieb spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3824c-128">The notification also informs your users that the optional connected experiences are provided under the Microsoft Services Agreement.</span></span> <span data-ttu-id="3824c-129">Keďže toto oznámenie je dôležitou informáciou pre používateľov, je potrebné ho zobraziť a nie je možné ho v mene používateľov vypnúť, skryť ani prijať.</span><span class="sxs-lookup"><span data-stu-id="3824c-129">Because this notification is important information for your users, this notification must be shown and can't be turned off, hidden, or accepted on behalf of your users.</span></span>

## <a name="users-can-choose-to-turn-off-optional-connected-experiences"></a><span data-ttu-id="3824c-130">Používatelia sa môžu rozhodnúť vypnúť voliteľné online funkcie</span><span class="sxs-lookup"><span data-stu-id="3824c-130">Users can choose to turn off optional connected experiences</span></span>

<span data-ttu-id="3824c-131">Ak sa rozhodnete používateľom sprístupniť voliteľné online funkcie, používatelia môžu prejsť na svoje [nastavenia ochrany osobných údajov konta](https://support.microsoft.com/office/3e7bc183-bf52-4fd0-8e6b-78978f7f121b#ID0EAADAAA=Online) a vypnúť tam prístup k voliteľným online funkciám.</span><span class="sxs-lookup"><span data-stu-id="3824c-131">If you choose to make optional connected experiences available to your users, your users can go to their [account privacy settings](https://support.microsoft.com/office/3e7bc183-bf52-4fd0-8e6b-78978f7f121b#ID0EAADAAA=Online) and choose to turn off their access to optional connected experiences.</span></span> <span data-ttu-id="3824c-132">Táto možnosť je v nastaveniach ochrany osobných údajov konta k dispozícii len v prípade, ak sú vaši používatelia prihlásení pomocou pracovného alebo školského konta.</span><span class="sxs-lookup"><span data-stu-id="3824c-132">This choice is available in the account privacy settings only if your users are signed in with their work or school account.</span></span> <span data-ttu-id="3824c-133">Vy ako správca nemáte možnosť zabrániť jednotlivcom vo vašej spoločnosti vypnúť svoj prístup k voliteľným online funkciám v nastaveniach ochrany osobných údajov konta, ak ste im umožnili vybrať si používanie voliteľných online funkcií.</span><span class="sxs-lookup"><span data-stu-id="3824c-133">There is no way that you, as the admin, can prevent individual users in your organization from turning off their access to optional connected experience in their account privacy settings if you've given your users the choice to use optional connected experiences.</span></span>

## <a name="related-articles"></a><span data-ttu-id="3824c-134">Súvisiace články</span><span class="sxs-lookup"><span data-stu-id="3824c-134">Related articles</span></span>

- [<span data-ttu-id="3824c-135">Prehľad ovládacích prvkov na ochranu osobných údajov pre Aplikácie Microsoft 365 pre veľké organizácie</span><span class="sxs-lookup"><span data-stu-id="3824c-135">Overview of privacy controls for Microsoft 365 Apps for enterprise</span></span>](overview-privacy-controls.md)
- [<span data-ttu-id="3824c-136">Spravovanie ovládacích prvkov na ochranu osobných údajov pre Aplikácie Microsoft 365 pre veľké organizácie</span><span class="sxs-lookup"><span data-stu-id="3824c-136">Use policy settings to manage privacy controls for Microsoft 365 Apps for enterprise</span></span>](manage-privacy-controls.md)
- [<span data-ttu-id="3824c-137">Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre Mac pomocou predvolieb</span><span class="sxs-lookup"><span data-stu-id="3824c-137">Use preferences to manage privacy controls for Office for Mac</span></span>](mac-privacy-preferences.md)
- [<span data-ttu-id="3824c-138">Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office v zariadeniach so systémom iOS pomocou predvolieb</span><span class="sxs-lookup"><span data-stu-id="3824c-138">Use preferences to manage privacy controls for Office on iOS devices</span></span>](ios-privacy-preferences.md)
- [<span data-ttu-id="3824c-139">Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre zariadenia s Androidom s nastaveniami politiky</span><span class="sxs-lookup"><span data-stu-id="3824c-139">Use policy settings to manage privacy controls for Office on Android devices</span></span>](android-privacy-controls.md)