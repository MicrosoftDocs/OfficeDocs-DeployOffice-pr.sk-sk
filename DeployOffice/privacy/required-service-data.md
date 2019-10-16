---
title: Požadované údaje služieb pre Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
audience: ITPro
ms.topic: reference
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection: Ent_O365
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
description: V tomto článku správcovia služieb Office získajú informácie o požadovaných údajoch služieb, ktoré sa zhromažďujú o pripojených funkciách v balíku Office.
hideEdit: true
ms.openlocfilehash: eaa659e375d3d5c29d5410ab53db7ae583df6e9d
ms.sourcegitcommit: 02c4120c0b10bfe378d21d60699ae49aaef97834
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/15/2019
ms.locfileid: "37510640"
---
# <a name="required-service-data-for-office"></a>Požadované údaje služieb pre Office 

> [!IMPORTANT]
> Informácie v tomto článku sa týkajú verzie 1904 alebo novšej verzie nasledujúceho klientskeho softvéru balíka Office nainštalovaného v počítači s Windowsom:
> - Office 365 ProPlus a Office 365 Business
> - Office 365 Personal, Office 365 Home alebo iné verzie balíka Office, ktoré sú súčasťou predplatného služieb Office 365.
> - Project a Visio, ktoré sú súčasťou niektorých plánov predplatného, ako sú napríklad Project Online Professional alebo Visio Online Plan 2.
>
> Informácie platia aj pre verziu 16.28 alebo novšie verzie týchto aplikácií balíka Office pre Mac: Excel, Outlook, OneNote, PowerPoint a Word.

Office pozostáva z klientskych softvérových aplikácií a online funkcií, ktoré sú navrhnuté tak, aby umožňovali efektívnejšiu tvorbu, komunikáciu a spoluprácu. Príkladom online funkcií je práca na dokumente spoločne s inými používateľmi vo OneDrive for Business alebo preklad obsahu wordového dokumentu do iného jazyka.

Požadované údaje služieb sú dôležité, pretože nám umožňujú poskytovať tieto cloudové pripojené funkcie a tiež pomáhajú zaručiť, že tieto funkcie budú zabezpečené a budú zákazníkom fungovať podľa očakávania. Tieto typy informácií predstavujú požadované údaje služieb:

- **Zákaznícky obsah**, čo je obsah, ktorý vytvárate pomocou balíka Office, ako je napríklad text napísaný vo wordovom dokumente, a ktorý sa používa v súvislosti s pripojenými službami.
- **Funkčné údaje**, ktoré zahŕňajú informácie vyžadované pripojenou funkciou na vykonávanie jej úlohy, ako sú napríklad informácie o konfigurácii aplikácie.
- **Diagnostické údaje služby**, čo sú údaje potrebné na to, aby služba bola neustále zabezpečená, aktuálna a fungovala podľa očakávania. Keďže tieto údaje sa výhradne týkajú pripojenej funkcie, sú oddelené od úrovne povinných alebo voliteľných diagnostických údajov.

## <a name="example-of-required-service-data-for-a-connected-experience"></a>Príklad požadovaných údajov služieb pre pripojenú funkciu

Na lepšie pochopenie požadovaných údajov služieb uvádzame nasledovný vzorový scenár používania nástroja PowerPoint Designer, čo je pripojená služba, ktorú môžete využívať pri vytváraní snímok pre prezentáciu. PowerPoint Designer vám pomáha vylepšovať vaše snímky tak, že automaticky generuje návrhy vzhľadu, z ktorých si môžete vybrať. Keď na snímku pridávate obsah, Designer pracuje na pozadí a spája obsah s profesionálne navrhnutými rozloženiami.

Požadované údaje služieb pre Office, ktoré sa odosielajú do spoločnosti Microsoft, aby táto pripojená funkcia mohla fungovať, zahŕňajú nasledovné:

- *Zákaznícky obsah*, ako sú napríklad text alebo obrázky, ktoré ste pridali na snímku.
- *Funkčné údaje*, ako sú napríklad údaje o tom, na ktorej snímke pracujete a aké má rozloženie.
- *Diagnostické údaje služby*, ako sú napríklad udalostí, z ktorých sa dozvieme, či sa odporúčaný návrh správne použil na snímku a či sa volania služby vykonali správne.

## <a name="view-and-manage-required-service-data"></a>Zobrazenie a spravovanie požadovaných údajov služieb

Diagnostické údaje služby môžete zobraziť pomocou zobrazovača diagnostických údajov. Ďalšie informácie sa nachádzajú v časti [Príklady udalostí pre diagnostické údaje služieb](#examples-of-events-for-service-diagnostic-data).

Poskytujeme vám možnosť rozhodnúť sa, ktoré typy pripojených funkcií chcete používať v balíku Office, čo zároveň určuje, ktoré požadované údaje služieb sa nám odosielajú. PowerPoint Designer je napríklad jednou z pripojených funkcií na analýzu obsahu. Ak sa rozhodnete vypnúť pripojené funkcie, ktoré analyzujú obsah, nebudú sa nám odosielať žiadne požadované údaje služieb o PowerPoint Designeri, pretože PowerPoint Designer nebude k dispozícii.

Požadované údaje služieb sa taktiež zhromažďujú a odosielajú spoločnosti Microsoft pre služby, ktoré sú nevyhnutné na fungovanie balíka Office, ako je napríklad licenčná služba, ktorá potvrdzuje, že máte správnu licenciu na používanie balíka Office. Tieto údaje o nevyhnutných službách sa odosielajú bez ohľadu na ďalšie nastavenia, ktoré ste nakonfigurovali.

Ďalšie informácie sa nachádzajú v nasledujúcich témach:

- [Pripojené funkcie v Office](connected-experiences.md)
- [Nevyhnutné služby pre Office](essential-services.md)
- [Používanie nástroja Diagnostic Data Viewer s balíkom Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)

Ak ste správcom v organizácii, možno vás budú zaujímať aj nasledovné témy:

- [Prehľad ovládacích prvkov na ochranu osobných údajov pre Office 365 ProPlus](overview-privacy-controls.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office 365 ProPlus s nastaveniami politiky](manage-privacy-controls.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre Mac pomocou predvolieb](mac-privacy-preferences.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office v zariadeniach so systémom iOS pomocou predvolieb](ios-privacy-preferences.md)

## <a name="examples-of-events-for-service-diagnostic-data"></a>Príklady udalostí pre diagnostické údaje služieb

Diagnostické údaje služieb sa zobrazujú v zobrazovači diagnostických údajov a sú usporiadané do rovnakých kategórií, aké používajú požadované a voliteľné diagnostické údaje. Napríklad *Používanie produktov a služieb* alebo *Výkon produktov a služieb*.

Udalosti diagnostických údajov služieb nám poskytujú potrebné informácie o tom, či pripojená funkcia funguje podľa očakávania zákazníka. Napríklad, či sa služba používaná pripojenou funkciou úspešne spustila a bola k dispozícii podľa potreby, či sa pri práci so službou vyskytli chyby alebo iné nečakané problémy (zlyhania) a aká bola odozva alebo výkon služba.

V nasledujúcej tabuľke je uvedených niekoľko príkladov udalostí pre diagnostické údaje služieb.

| **Názov**      | **Popis**    |
| ---------- | --------------------- |
| Office.Excel.Coauth.SaveXrr     | Udalosť spustená v Exceli počas používania služby spolupráce, ktorá nahlasuje podrobnosti o jednotlivých revíziách zapísaných v denníku revízií. Poskytuje monitorovanie časového oneskorenia a označuje chyby v Exceli, ktoré súvisia so spoluprácou  |
| Office.Excel.Coauth.CloseWorkbook  | Udalosť spustená v Exceli počas používania služby spolupráce, ktorá nahlasuje, kedy došlo k zavretiu zošita. Je to potrebné pri určovaní prípadných chýb s opätovným načítaním a automatickým obnovením. Poskytuje meranie úspechu pre aktivity služby spolupráce.   |
| Office.Security.OCX.NonTrustedEncounter    | Udalosť spustená v aplikáciách balíka Office (vrátane Wordu, Excelu, Outlooku, PowerPointu a Visia), keď používateľ otvorí nedôveryhodný dokument s ovládacím prvkom ActiveX. Používa sa na všeobecné posúdenie používania ovládacích prvkov ActiveX vložených v dokumentoch balíka Office a na pomoc pri riešení problémov so zabezpečením v reakcii na incidenty zabezpečenia.  |
| Office.Security.UrlReputation.GetUrlReputation | Udalosť spustená v aplikáciách balíka Office (vrátane Wordu, Excelu, PowerPointu, Visia a Publishera), ktorá sleduje úspech alebo zlyhanie volaní Safe Links. Používa sa na zabezpečenie správneho fungovania služby Safe Links a na diagnostikovanie problémov.  |
| Office.Voice.VoiceManager.StreamingAudio   | Udalosť spustená v aplikáciách balíka Office (vrátane Wordu, Outlooku a PowerPointu), ktorá poskytuje informácie o stave služby prevodu streamovania zvuku na reč. Obsahuje informácie o veľkosti streamovaného zvuku a prípadných chybách, ktoré sa vyskytli. Tieto informácie sa používajú na monitorovanie stavu služby stavu a na diagnostikovanie problémov nahlásených zákazníkmi. |
