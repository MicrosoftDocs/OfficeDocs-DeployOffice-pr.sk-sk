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
ms.openlocfilehash: 69a8880b03e63be391731f9882bcee17a81a51ab
ms.sourcegitcommit: e542473cc4fe07a98874c275846f6982a6863e35
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/05/2019
ms.locfileid: "39837729"
---
# <a name="use-policy-settings-to-manage-privacy-controls-for-office-on-android-devices"></a>Spravovanie nastavení ochrany osobných údajov pre Office v zariadeniach s Androidom pomocou nastavení politiky

K dispozícii sú nastavenia politiky pre Office v zariadeniach s Androidom, ktoré umožňujú ovládať nastavenia pre:

- ***Diagnostické údaje***, ktoré sa zhromažďujú a odosielajú spoločnosti Microsoft o používanom klientskom softvéri balíka Office.

- ***Online funkcie***, ktoré využívajú cloudové funkcie na poskytovanie rozšírených funkcií balíka Office vám a vašim používateľom.

Ďalšie informácie o diagnostických údajoch a online funkciách nájdete v téme [Prehľad ovládacích prvkov na ochranu osobných údajov](overview-privacy-controls.md).

Tieto nastavenia politiky sa týkajú nasledujúcich aplikácií:
- Word pre Android, Excel pre Android a PowerPoint pre Android verzie 16.0.12228.20260 a novšej.
- OneNote pre Android verzie 16.0.12228.20004 a novšej.

> [!NOTE]
>- Tieto nastavenia politiky sa vzťahujú aj na verziu 16.0.12130.20272 a novšiu verejného náhľadu [mobilnej aplikácie Office](https://techcommunity.microsoft.com/t5/Office-Apps-Blog/Introducing-Office-Your-new-go-to-mobile-app-for-getting-work/ba-p/977172) pre Android.
>- Pri používaní verejného náhľadu mobilnej aplikácie Office pre Android sa budú zhromažďovať denníky zlyhaní, ktoré môžu v niektorých prípadoch zahŕňať obsah.
>- Ak máte obavy v súvislosti so zhromažďovaním údajov z verejného náhľadu mobilnej aplikácie Office pre Android, mali by ste informovať používateľov, aby sa do aplikácie neprihlasovali pomocou svojich pracovných ani školských kont.

## <a name="policy-settings-available-for-office-on-android-devices"></a>Nastavenia politiky dostupné pre Office v zariadeniach s Androidom

V nasledujúcej tabuľke sú uvedené nastavenia politiky dostupné pre Office v zariadeniach s Androidom a odkazy na ďalšie informácie o jednotlivých nastaveniach politiky.

> [!NOTE]
>- Ďalšie uvedené informácie zahŕňajú nastavenia politiky pre Office v zariadeniach s Windowsom. Rovnaké informácie platia aj pre Office v zariadeniach s Androidom, pretože ide o rovnaké nastavenia politiky.
>- Nastavenie politiky *Povoliť používanie pripojených funkcií v Office*, ktoré je dostupné pre Office v zariadeniach s Windowsom, sa nevzťahuje na Office v zariadeniach s Androidom. 


|Názov nastavenia politiky  |Ďalšie informácie |
|---------|---------|
|Konfigurácia úrovne diagnostických údajov o klientskom softvéri, ktoré služby Office odosielajú spoločnosti Microsoft|[Nastavenie politiky pre diagnostické údaje](manage-privacy-controls.md#policy-setting-for-diagnostic-data)         |
|Povoliť používanie pripojených funkcií na analýzu obsahu v Office| [Nastavenie politiky pre pripojené funkcie na analýzu obsahu](manage-privacy-controls.md#policy-setting-for-connected-experiences-that-analyze-your-content)        |
|Povoliť používanie pripojených funkcií na sťahovanie online obsahu v Office |[Nastavenie politiky pre pripojené funkcie na sťahovanie online obsahu](manage-privacy-controls.md#policy-setting-for-connected-experiences-that-download-online-content)         |
|Povoliť používanie dodatočných voliteľných pripojených funkcií v Office |[Nastavenie politiky pre voliteľné pripojené funkcie](manage-privacy-controls.md#policy-setting-for-optional-connected-experiences)|



## <a name="use-office-cloud-policy-service-to-apply-policy-settings"></a>Použitie nastavení politiky pomocou cloudovej služby politiky pre Office

Ak chcete použiť niektoré z týchto štyroch nastavení politiky pre Office v zariadeniach s Androidom, musíte použiť cloudovú službu politiky pre Office. Ďalšie informácie o použití cloudovej služby politiky pre Office nájdete v téme [Prehľad cloudovej služby politiky pre Office](../overview-office-cloud-policy-service.md).

> [!NOTE]
> Ak ste v minulosti pomocou cloudovej služby politiky pre Office konfigurovali tieto nastavenia politiky pre Office v zariadeniach s Windowsom, rovnaké nastavenia sa budú vzťahovať aj na Office v zariadeniach s Androidom. Stačí sa prihlásiť do cloudovej služby politiky pre Office a služba automaticky použije nastavenia pre Office v zariadeniach s Androidom.