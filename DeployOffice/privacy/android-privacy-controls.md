---
title: Spravovanie nastavení ochrany osobných údajov pre Office v zariadeniach s Androidom pomocou nastavení politiky
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
description: V tomto článku získajú správcovia služieb Office informácie o postupoch spravovania nastavení ochrany osobných údajov pre Office v zariadeniach s Androidom.
hideEdit: true
ms.openlocfilehash: 36ae9878d03845c24e3717dfac970b2b961279dc
ms.sourcegitcommit: acb22296532bbfdfcad4dc1e7162f812997fbdd1
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/08/2019
ms.locfileid: "38068450"
---
# <a name="use-policy-settings-to-manage-privacy-controls-for-office-on-android-devices"></a><span data-ttu-id="9f83f-103">Spravovanie nastavení ochrany osobných údajov pre Office v zariadeniach s Androidom pomocou nastavení politiky</span><span class="sxs-lookup"><span data-stu-id="9f83f-103">Use policy settings to manage privacy controls for Office 365 ProPlus</span></span>

<span data-ttu-id="9f83f-104">K dispozícii sú nastavenia politiky pre Office v zariadeniach s Androidom, ktoré umožňujú ovládať nastavenia pre:</span><span class="sxs-lookup"><span data-stu-id="9f83f-104">There are new preference settings for Office on iOS devices that allow you to control settings related to the following:</span></span>

- <span data-ttu-id="9f83f-105">***Diagnostické údaje***, ktoré sa zhromažďujú a odosielajú spoločnosti Microsoft o používanom klientskom softvéri balíka Office.</span><span class="sxs-lookup"><span data-stu-id="9f83f-105">***Diagnostic data*** that is collected and sent to Microsoft about Office client software being used.</span></span>

- <span data-ttu-id="9f83f-106">***Online funkcie***, ktoré využívajú cloudové funkcie na poskytovanie rozšírených funkcií balíka Office vám a vašim používateľom.</span><span class="sxs-lookup"><span data-stu-id="9f83f-106">***Connected experiences*** that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="9f83f-107">Ďalšie informácie o diagnostických údajoch a online funkciách nájdete v téme [Prehľad ovládacích prvkov na ochranu osobných údajov](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="9f83f-107">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

<span data-ttu-id="9f83f-108">Tieto nastavenia politiky sa týkajú nasledujúcich aplikácií:</span><span class="sxs-lookup"><span data-stu-id="9f83f-108">These preference settings apply to the following applications:</span></span>
- <span data-ttu-id="9f83f-109">Word pre Android, Excel pre Android a PowerPoint pre Android verzie 16.0.12226.10000 a novšej.</span><span class="sxs-lookup"><span data-stu-id="9f83f-109">Version 16.0.12226.10000 and later of Word for Android, Excel for Android, and PowerPoint for Android.</span></span>
- <span data-ttu-id="9f83f-110">OneNote pre Android verzie 16.0.12228.20004 a novšej.</span><span class="sxs-lookup"><span data-stu-id="9f83f-110">Version 16.0.12228.20004 and later of OneNote for Android.</span></span>

> [!NOTE]
>- <span data-ttu-id="9f83f-111">Tieto nastavenia politiky sa vzťahujú aj na verziu 16.0.12130.20272 a novšiu verejného náhľadu [mobilnej aplikácie Office](https://techcommunity.microsoft.com/t5/Office-Apps-Blog/Introducing-Office-Your-new-go-to-mobile-app-for-getting-work/ba-p/977172) pre Android.</span><span class="sxs-lookup"><span data-stu-id="9f83f-111">These policy settings also apply to Version 16.0.12130.20272 and later of the public preview of the [Office Mobile app](https://techcommunity.microsoft.com/t5/Office-Apps-Blog/Introducing-Office-Your-new-go-to-mobile-app-for-getting-work/ba-p/977172) for Android.</span></span>
>- <span data-ttu-id="9f83f-112">Pri používaní verejného náhľadu mobilnej aplikácie Office pre Android sa budú zhromažďovať denníky zlyhaní, ktoré môžu v niektorých prípadoch zahŕňať obsah.</span><span class="sxs-lookup"><span data-stu-id="9f83f-112">Use of the public preview of the Office Mobile app for Android will collect crash logs which may in some circumstances contain content.</span></span>
>- <span data-ttu-id="9f83f-113">Ak máte obavy v súvislosti so zhromažďovaním údajov z verejného náhľadu mobilnej aplikácie Office pre Android, mali by ste informovať používateľov, aby sa do aplikácie neprihlasovali pomocou svojich pracovných ani školských kont.</span><span class="sxs-lookup"><span data-stu-id="9f83f-113">If you're concerned about the collection of data from the public preview of the Office Mobile app for Android, you should inform your users not to log into the application with their work or school accounts.</span></span>

## <a name="policy-settings-available-for-office-on-android-devices"></a><span data-ttu-id="9f83f-114">Nastavenia politiky dostupné pre Office v zariadeniach s Androidom</span><span class="sxs-lookup"><span data-stu-id="9f83f-114">Policy settings available for Office on Android devices</span></span>

<span data-ttu-id="9f83f-115">V nasledujúcej tabuľke sú uvedené nastavenia politiky dostupné pre Office v zariadeniach s Androidom a odkazy na ďalšie informácie o jednotlivých nastaveniach politiky.</span><span class="sxs-lookup"><span data-stu-id="9f83f-115">The following table lists which policy settings are available for Office on Android devices and a link to additional information about each policy setting.</span></span>

> [!NOTE]
>- <span data-ttu-id="9f83f-116">Ďalšie uvedené informácie zahŕňajú nastavenia politiky pre Office v zariadeniach s Windowsom.</span><span class="sxs-lookup"><span data-stu-id="9f83f-116">The additional information provided covers the policy settings for Office on devices running Windows.</span></span> <span data-ttu-id="9f83f-117">Rovnaké informácie platia aj pre Office v zariadeniach s Androidom, pretože ide o rovnaké nastavenia politiky.</span><span class="sxs-lookup"><span data-stu-id="9f83f-117">But the same information applies to Office on Android devices because they are the same policy settings.</span></span>
>- <span data-ttu-id="9f83f-118">Nastavenie politiky *Povoliť používanie pripojených funkcií v Office*, ktoré je dostupné pre Office v zariadeniach s Windowsom, sa nevzťahuje na Office v zariadeniach s Androidom.</span><span class="sxs-lookup"><span data-stu-id="9f83f-118">The *Allow the use of connected experiences in Office* policy setting that's available for Office on devices running Windows does not apply to Office on Android devices.</span></span> 


|<span data-ttu-id="9f83f-119">Názov nastavenia politiky</span><span class="sxs-lookup"><span data-stu-id="9f83f-119">Name of policy setting</span></span>  |<span data-ttu-id="9f83f-120">Ďalšie informácie</span><span class="sxs-lookup"><span data-stu-id="9f83f-120">Additional Information</span></span> |
|---------|---------|
|<span data-ttu-id="9f83f-121">Konfigurácia úrovne diagnostických údajov o klientskom softvéri, ktoré služby Office odosielajú spoločnosti Microsoft</span><span class="sxs-lookup"><span data-stu-id="9f83f-121">Configure the level of client software diagnostic data sent by Office to Microsoft</span></span>|[<span data-ttu-id="9f83f-122">Nastavenie politiky pre diagnostické údaje</span><span class="sxs-lookup"><span data-stu-id="9f83f-122">Policy setting for diagnostic data</span></span>](manage-privacy-controls.md#policy-setting-for-diagnostic-data)         |
|<span data-ttu-id="9f83f-123">Povoliť používanie pripojených funkcií na analýzu obsahu v Office</span><span class="sxs-lookup"><span data-stu-id="9f83f-123">Allow the use of connected experiences in Office that analyze content</span></span>| [<span data-ttu-id="9f83f-124">Nastavenie politiky pre pripojené funkcie na analýzu obsahu</span><span class="sxs-lookup"><span data-stu-id="9f83f-124">Policy setting for connected experiences that analyze your content</span></span>](manage-privacy-controls.md#policy-setting-for-connected-experiences-that-analyze-your-content)        |
|<span data-ttu-id="9f83f-125">Povoliť používanie pripojených funkcií na sťahovanie online obsahu v Office</span><span class="sxs-lookup"><span data-stu-id="9f83f-125">Allow the use of connected experiences in Office that download online content</span></span> |[<span data-ttu-id="9f83f-126">Nastavenie politiky pre pripojené funkcie na sťahovanie online obsahu</span><span class="sxs-lookup"><span data-stu-id="9f83f-126">Policy setting for connected experiences that download online content</span></span>](manage-privacy-controls.md#policy-setting-for-connected-experiences-that-download-online-content)         |
|<span data-ttu-id="9f83f-127">Povoliť používanie dodatočných voliteľných pripojených funkcií v Office</span><span class="sxs-lookup"><span data-stu-id="9f83f-127">Allow the use of additional optional connected experiences in Office</span></span> |[<span data-ttu-id="9f83f-128">Nastavenie politiky pre voliteľné pripojené funkcie</span><span class="sxs-lookup"><span data-stu-id="9f83f-128">Policy setting for optional connected experiences</span></span>](manage-privacy-controls.md#policy-setting-for-optional-connected-experiences)|



## <a name="use-office-cloud-policy-service-to-apply-policy-settings"></a><span data-ttu-id="9f83f-129">Použitie nastavení politiky pomocou cloudovej služby politiky pre Office</span><span class="sxs-lookup"><span data-stu-id="9f83f-129">Use Office cloud policy service to apply policy settings</span></span>

<span data-ttu-id="9f83f-130">Ak chcete použiť niektoré z týchto štyroch nastavení politiky pre Office v zariadeniach s Androidom, musíte použiť cloudovú službu politiky pre Office.</span><span class="sxs-lookup"><span data-stu-id="9f83f-130">To apply any of these 4 policy settings for Office on Android devices, you need to use the Office cloud policy service.</span></span> <span data-ttu-id="9f83f-131">Ďalšie informácie o použití cloudovej služby politiky pre Office nájdete v téme [Prehľad cloudovej služby politiky pre Office](../overview-office-cloud-policy-service.md).</span><span class="sxs-lookup"><span data-stu-id="9f83f-131">For more information on using the Office cloud policy service, see [Overview of the Office cloud policy service](../overview-office-cloud-policy-service.md).</span></span>

> [!NOTE]
> <span data-ttu-id="9f83f-132">Ak ste v minulosti pomocou cloudovej služby politiky pre Office konfigurovali tieto nastavenia politiky pre Office v zariadeniach s Windowsom, rovnaké nastavenia sa budú vzťahovať aj na Office v zariadeniach s Androidom.</span><span class="sxs-lookup"><span data-stu-id="9f83f-132">If you previously used Office cloud policy service to configure these policy settings for Office on devices running Windows, those same settings will apply to Office on Android devices.</span></span> <span data-ttu-id="9f83f-133">Stačí sa prihlásiť do cloudovej služby politiky pre Office a služba automaticky použije nastavenia pre Office v zariadeniach s Androidom.</span><span class="sxs-lookup"><span data-stu-id="9f83f-133">For that to happen, you just need to sign in to the Office cloud policy service and the service will apply the settings automatically to Office on Android devices.</span></span>
