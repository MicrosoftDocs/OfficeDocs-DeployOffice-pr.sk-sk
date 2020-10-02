---
title: Voliteľné diagnostické údaje pre Office
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
description: V tomto článku správcovia služieb Office získajú informácie o voliteľných diagnostických údajoch v balíku Office vrátane niekoľkých príkladov udalostí.
hideEdit: true
ms.openlocfilehash: 2183863e1f7050d7d6ba838b639debf2b53ac9bd
ms.sourcegitcommit: e1e4c309d62d0708404b7838c96416ce89f1b8b7
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/01/2020
ms.locfileid: "48328334"
---
# <a name="optional-diagnostic-data-for-office"></a>Voliteľné diagnostické údaje pre Office

> [!NOTE]
> Ak si chcete pozrieť zoznam produktov balíka Office, na ktorý sa vzťahujú tieto informácie o ochrane osobných údajov, pozrite si tému [Ovládacie prvky na ochranu osobných údajov dostupné pre produkty balíka Office](products-versions-privacy-controls.md).

Diagnostické údaje sa používajú na zabezpečenie a aktualizovanie balíka Office, zisťovanie, diagnostiku a riešenie problémov, ako aj na vylepšenia produktov. Tieto údaje neobsahujú meno ani e-mailovú adresu používateľa, obsah súborov používateľa ani informácie o aplikáciách, ktoré nesúvisia s balíkom Office.

Tieto diagnostické údaje sa zhromažďujú a odosielajú spoločnosti Microsoft o klientskom softvéri balíka Office, ktorý sa používa v počítačoch s Windowsom. Niektoré diagnostické údaje sú povinné, a iné diagnostické údaje sú voliteľné. Máte možnosť si vybrať, či nám budete odosielať povinné alebo voliteľné diagnostické údaje, pomocou ovládacích prvkov ochrany osobných údajov, ako sú nastavenia politiky pre organizácie. Nám odoslané diagnostické údaje môžete zobraziť pomocou zobrazovača diagnostických údajov.

***Voliteľné diagnostické údaje*** sú dodatočné údaje, ktoré nám pomáhajú zlepšovať produkty, a obsahujú rozšírené informácie, ktoré nám pomáhajú rozpoznávať, diagnostikovať a riešiť problémy.

Ak sa rozhodnete odosielať nám voliteľné diagnostické údaje, budú obsahovať aj požadované diagnostické údaje. Môžu sa odosielať aj súbory diagnostického denníka balíka Office, ktoré obsahujú informácie veľmi podobné voliteľným diagnostickým údajom. Ďalšie informácie o týchto súboroch denníkov nájdete v téme [Prehľad súborov diagnostického denníka pre Office](https://support.microsoft.com/office/fba86aac-70dc-4858-ae1f-ec2034346cdf).

Príkladmi voliteľných diagnostických údajov sú údaje, ktoré zhromažďujeme o tvaroch, ktoré používatelia vkladajú do wordových dokumentov, aby sme mohli poskytovať lepšie možnosti, a údaje, ktoré zhromažďujeme o čase potrebnom na zobrazenie powerpointovej snímky na obrazovke, aby sme mohli zlepšiť funkčnosť, ak je zobrazenie pomalé.

Ďalšie informácie o diagnostických údajoch sa nachádzajú v článkoch:

- [Povinné diagnostické údaje pre Office](required-diagnostic-data.md)
- [Používanie nástroja Diagnostic Data Viewer s balíkom Office](https://support.microsoft.com/office/cf761ce9-d805-4c60-a339-4e07f3182855)

Ak ste správcom v organizácii, možno vás budú zaujímať aj nasledovné články:

- [Prehľad ovládacích prvkov na ochranu osobných údajov pre Aplikácie Microsoft 365 pre veľké organizácie](overview-privacy-controls.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Aplikácie Microsoft 365 pre veľké organizácie](manage-privacy-controls.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre Mac pomocou predvolieb](mac-privacy-preferences.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office v zariadeniach so systémom iOS pomocou predvolieb](ios-privacy-preferences.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre zariadenia s Androidom s nastaveniami politiky](android-privacy-controls.md)

## <a name="categories-of-optional-diagnostic-data"></a>Kategórie voliteľných diagnostických údajov

Voliteľné diagnostické údaje sú usporiadané do nasledujúcich kategórií:

- Inštalácia softvéru a inventár
- Používanie produktov a služieb
- Výkon produktov a služieb
- Pripojiteľnosť a konfigurácia zariadenia

Tieto kategórie sa zobrazujú v zobrazovači diagnostických údajov a sú to rovnaké kategórie, aké sa používajú pre povinné diagnostické údaje.

Nasledujúce časti obsahujú popis každej kategórie a príklady udalostí v každej kategórii.

## <a name="software-setup-and-inventory-events"></a>Udalosti v kategórii Inštalácia softvéru a inventár

Do tejto kategórie patria udalostí, ktoré sa môžu vzťahovať na tieto oblasti:

- Nainštalovaný produkt a verzia a stav inštalácie
- Softvérové doplnky a ich nastavenia
- Chybové stavy dokumentu, funkcie a doplnku, ktoré môže ohroziť zabezpečenie, vrátane pripravenosti na aktualizáciu produktu.

Nasledujúca tabuľka obsahuje príklady udalostí v tejto kategórii a ich popis.

| **Názov udalosti**   | **Popis udalosti**  |
| ---- | ---- |
| Office.Extensibility.AppCommands.GetRibbonUpdatesForUserId | Táto udalosť označuje, či Word úspešne aktualizuje pás s nástrojmi používateľského rozhrania Wordu, keď používateľ zmení svoju identitu. Pomocou tejto udalosti rozpoznávame nesprávne nastavenie a iné problémy, ktoré by mohli ovplyvniť používateľské rozhranie balíka Office. |
| Office.Extensibility.AppCommands.AppCmdInstall   | Táto udalosť poskytuje informácie o doplnku balíka Office, ktorý používateľ nainštaloval, vrátane ID aplikácie, zostavy a verzie operačného systému, úspešnosti inštalácie a trvaní inštalácie.  |

## <a name="product-and-service-usage-events"></a>Udalosti v kategórii Používanie produktov a služieb

Do tejto kategórie patria udalostí, ktoré sa môžu vzťahovať na tieto oblasti:

- Úspešnosť fungovania aplikácie. Obmedzené na otvorenie a zatvorenie aplikácie a dokumentov, úpravu súborov a zdieľanie súborov (spoluprácu).
- Určenie, či sa vyskytli konkrétne udalosti funkcie, napríklad spustenie alebo ukončenie a či je funkcia spustená.
- Funkcie zjednodušenia ovládania balíka Office

Nasledujúca tabuľka obsahuje príklady udalostí v tejto kategórii a ich popis.

| **Názov udalosti**   | **Popis udalosti**  |
| ------ | ------- |
| Office.Word.Commanding.Highlight  | Táto udalosť označuje, že Word vykonal príkaz na zvýraznenie textu. Táto udalosť sa používa na zistenie chýb v príkaze zvýraznenia textu.  |
| Office.Translator.AddInLoaded   | Prezenčný signál na určenie, či sa funkcia prekladača spustila úspešne načítala a vykreslila.  |
| Office.Graphics.GVizInsertShape |Sleduje používanie funkcie Vložiť tvar vo Worde a tiež nahlasuje podrobnosti o typoch vložených tvarov a o tom, z akého zdroja boli vložené.| 
| Office.PowerPoint.PPT.Desktop.SummaryZoomInsertionRule   | Táto udalosť určuje, či sa v dokumente nachádzajú nejaké sekcie, keď používateľ vkladá Náhľad obsahu, a či sa používateľ rozhodne odstrániť existujúce sekcie. |
| Office.Security.SecureReaderHost.ProtectedViewValidation | Sleduje, kedy a prečo sa súbor otvoril v chránenom zobrazení. Používa sa na diagnostikovanie stavov, kedy by sa chránené zobrazenie nemuselo správne spustiť, aby sa zaručilo, že funkcia funguje správne. |

## <a name="product-and-service-performance-events"></a>Udalosti v kategórii Výkon produktov a služieb

Do tejto kategórie patria udalostí, ktoré sa môžu vzťahovať na tieto oblasti:

- Neočakávané ukončenia (zlyhania) aplikácie a stav aplikácie, keď sa to stane.
- Dlhý čas odozvy alebo nízky výkon v prípadoch ako spustenie aplikácie alebo otvorenie súboru.
- Chyby funkčnosti funkcie alebo používateľského rozhrania.

Nasledujúca tabuľka obsahuje príklady udalostí v tejto kategórii a ich popis.

| **Názov udalosti**    | **Popis udalosti**   |
| --------------- | -------------- |
| Office.Word.Word.CoreSaveTime100ns     | V tejto udalosti sa zaznamenáva výkon aktivity ukladania dokumentu vo Worde. Táto udalosť sa používa na zistenie chýb a problémov s výkonom v aktivite ukladania súboru vo Worde.|
| Office.Identity.SignInForWamAccountAad  | Táto udalosť sa odošle, keď je používateľ prihlásený v konte služby Azure Active Directory s knižnicou Web Account Manager (WAM). Táto udalosť odosiela metaúdaje, ako sú napríklad názov aplikácie, verzia aplikácie chybový kód, ak aplikácia zlyhala. |
| Office.PowerPoint.PPT.Desktop.FileOpen.FirstSlideMasterThumbnailRenderTime | Táto udalosť zhromažďuje čas potrebný na vykreslenie miniatúry predlohy prvej snímky v PowerPointe.  |
| Office.Extensibility.Diagnostics   | Táto udalosť poskytuje všeobecné diagnostické informácie pre doplnky balíka Office, ako sú napríklad správy o zlyhaní na ladenie.|

## <a name="device-connectivity-and-configuration-events"></a>Udalosti v kategórii Pripojiteľnosť a konfigurácia zariadenia

Do tejto kategórie patria udalostí, ktoré sa môžu vzťahovať na tieto oblasti:

- Stav sieťového pripojenia a nastavenia zariadenia, napríklad pamäte.

Nasledujúca tabuľka obsahuje príklady udalostí v tejto kategórii a ich popis.

| **Názov udalosti**                    | **Popis udalosti**                                                                                                                                                     |
| ------ | ----- |
| Office.Graphics.ArtViewValidate | Táto udalosť zaznamenáva overenie výsledkov zobrazenia grafických prvkov, ktoré podporuje grafické používateľské rozhranie. Pomocou tejto udalosti zhromažďujeme údaje o používaní a chybách týkajúce sa vykresľovania grafických prvkov. |
| Office.Graphics.ARCExceptionScope | Táto udalosť sleduje zlyhania vykresľovania pochádzajúce z nástroja vykresľovania. |
| Office.Extensibility.ODPLatency   | Táto udalosť poskytuje informácie o sieťovom pripojení a rýchlosti používateľa.     |
