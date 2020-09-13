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
# <a name="use-policy-settings-to-manage-privacy-controls-for-office-for-the-web-applications"></a>Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office na webe s nastaveniami politiky

> [!NOTE]
> Ak si chcete pozrieť zoznam produktov balíka Office, na ktorý sa vzťahujú tieto informácie o ochrane osobných údajov, pozrite si tému [Ovládacie prvky na ochranu osobných údajov dostupné pre produkty balíka Office](products-versions-privacy-controls.md).

Ako správca vašej organizácie môžete určiť, či majú vaši používatelia možnosť používať voliteľné online funkcie pri používaní Office na webe, ako je napríklad Word na webe alebo PowerPoint na webe. Táto možnosť je k dispozícii pre používateľov len v prípade, že keď používajú aplikácie Office na webe, sú prihlásení pomocou pracovného alebo školského konta. Pomocou nastavenia politiky *Povoliť používanie dodatočných voliteľných pripojených funkcií v Office* môžete určiť, či budú mať vaši používatelia možnosť používať voliteľné online funkcie.

## <a name="overview-of-optional-connected-experiences"></a>Prehľad voliteľných online funkcií

Voliteľne online funkcie sú cloudové služby, ktoré sú k dispozícii pre používateľov, keď používajú aplikáciu Office. Príkladmi voliteľných online funkcií je vytvorenie kartogramu v Exceli alebo vloženie obrázka online do wordového dokumentu, pretože obe využívajú možnosti poskytované technológiou Microsoft Bing. Používanie týchto cloudových služieb je voliteľné. 

Na voliteľné pripojené funkcie sa nevzťahuje komerčná zmluva vašej spoločnosti so spoločnosťou Microsoft. Voliteľné pripojené funkcie ponúka priamo spoločnosť Microsoft a riadia sa [zmluvou o poskytovaní služieb spoločnosti Microsoft](https://www.microsoft.com/servicesagreement). V niektorých prípadoch sa prostredníctvom týchto voliteľných funkcií poskytujú obsah alebo funkcie tretích strán a môžu sa na ne vzťahovať aj ďalšie podmienky.

Niektoré voliteľné online funkcie nemusia byť dostupné v aplikáciách Office na webe, ale sú dostupné pri používaní oných verzií aplikácie Office, napríklad počítačovej verzie na zariadení so systémom Windows.

Ďalšie informácie sa nachádzajú v téme [Prehľad voliteľných online funkcií v balíku Office](optional-connected-experiences.md).

## <a name="configure-the-policy-setting-by-using-the-office-cloud-policy-service"></a>Konfigurácia nastavenia politiky pomocou služby politiky Office v cloude

Pomocou nastavenia politiky *Povoliť používanie dodatočných voliteľných pripojených funkcií v Office* môžete určiť, či budú mať vaši používatelia možnosť používať voliteľné online funkcie. Ak chcete nakonfigurovať nastavenie politiky pre aplikácie Office pre web, musíte použiť [službu politiky Office v cloude](../overview-office-cloud-policy-service.md).  

Ak nenakonfigurujete toto nastavenie politiky, tieto voliteľné online funkcie budú k dispozícii pre vašich používateľov. Ak toto nastavenie politiky zakážete, vaši používatelia nebudú mať k dispozícii žiadne voliteľné online funkcie.

Pre aplikácie Office na webe sa nastavenie politiky vzťahuje na prípad, keď vaši používatelia pracujú na dokumentoch balíka Office, ktoré sú uložené na webovom úložisku od spoločnosti, ako je napríklad OneDrive for Business alebo SharePoint Online.

Keďže používate službu politiky Office v cloude, toto nastavenie politiky platí, aj keď vaši používatelia používajú Office na zariadeniach s Windowsom, iOS, Androidom alebo zariadeniach Mac. Toto nastavenie politiky nie je možné nakonfigurovať len pre používateľov, ktorí používajú aplikácie Office na webe, Môžete však vytvoriť konfiguráciu politiky, ktorá zahŕňa toto nastavenie politiky a nastaviť túto konfiguráciu politiky tak, aby platila iba pre používateľov, ktorí k dokumentom pristupujú anonymne pomocou aplikácií Office na webe.

Ak sa rozhodnete používateľom sprístupniť voliteľné online funkcie, pri prvom použití aplikácie Office pre web sa im zobrazí oznámenie o ochrane osobných údajov. Toto oznámenie oznamuje používateľom, že ste im udelili možnosť používať tieto voliteľné online funkcie. Oznámenie tiež informuje používateľov o tom, že voliteľné online funkcie sa poskytujú v rámci zmluvy o poskytovaní služieb spoločnosti Microsoft. Keďže toto oznámenie je dôležitou informáciou pre používateľov, je potrebné ho zobraziť a nie je možné ho v mene používateľov vypnúť, skryť ani prijať.

## <a name="users-can-choose-to-turn-off-optional-connected-experiences"></a>Používatelia sa môžu rozhodnúť vypnúť voliteľné online funkcie

Ak sa rozhodnete používateľom sprístupniť voliteľné online funkcie, používatelia môžu prejsť na svoje [nastavenia ochrany osobných údajov konta](https://support.microsoft.com/office/3e7bc183-bf52-4fd0-8e6b-78978f7f121b#ID0EAADAAA=Online) a vypnúť tam prístup k voliteľným online funkciám. Táto možnosť je v nastaveniach ochrany osobných údajov konta k dispozícii len v prípade, ak sú vaši používatelia prihlásení pomocou pracovného alebo školského konta. Vy ako správca nemáte možnosť zabrániť jednotlivcom vo vašej spoločnosti vypnúť svoj prístup k voliteľným online funkciám v nastaveniach ochrany osobných údajov konta, ak ste im umožnili vybrať si používanie voliteľných online funkcií.

## <a name="related-articles"></a>Súvisiace články

- [Prehľad ovládacích prvkov na ochranu osobných údajov pre Aplikácie Microsoft 365 pre veľké organizácie](overview-privacy-controls.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Aplikácie Microsoft 365 pre veľké organizácie](manage-privacy-controls.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre Mac pomocou predvolieb](mac-privacy-preferences.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office v zariadeniach so systémom iOS pomocou predvolieb](ios-privacy-preferences.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre zariadenia s Androidom s nastaveniami politiky](android-privacy-controls.md)