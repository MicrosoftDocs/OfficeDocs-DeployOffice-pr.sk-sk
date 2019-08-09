---
title: Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office 365 ProPlus pomocou nastavení politiky
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
audience: ITPro
ms.topic: article
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection:
- Ent_O365
- M365-modern-desktop
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
description: V tomto článku správcovia služieb Office získajú informácie o postupoch spravovania ovládacích prvkov ochrany osobných údajov v službách Office 365 ProPlus pomocou nastavení politiky.
hideEdit: true
ms.openlocfilehash: 55c6c6477d4c03d94048c98c961179686eb29c83
ms.sourcegitcommit: 0fd23324ba1364fa1f8dd1578adf25946adde90f
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/07/2019
ms.locfileid: "36238985"
---
# <a name="use-policy-settings-to-manage-privacy-controls-for-office-365-proplus"></a>Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office 365 ProPlus pomocou nastavení politiky

Spoločnosť Microsoft sa zaviazala poskytovať informácie a ovládacie prvky potrebné na rozhodovanie o tom, ako sa vaše údaje zhromažďujú a používajú pri používaní služieb Office 365 ProPlus.

Od verzie 1904 služieb Office 365 ProPlus sú k dispozícii nové nastavenia politiky, ktoré umožňujú ovládať nastavenia týkajúce sa:

- ***diagnostických údajov***, ktoré sa zhromažďujú a odosielajú spoločnosti Microsoft o používanom klientskom softvéri balíka Office,

- ***Pripojené funkcie***, ktoré využívajú cloudové funkcie na poskytovanie rozšírených funkcií balíka Office vám a vašim používateľom.

Päť nových nastavení politiky:

- Konfigurácia úrovne diagnostických údajov o klientskom softvéri, ktoré služby Office odosielajú spoločnosti Microsoft
- Povoliť používanie pripojených funkcií na analýzu obsahu v Office
- Povoliť používanie pripojených funkcií na sťahovanie online obsahu v Office
- Povoliť používanie dodatočných voliteľných pripojených funkcií v Office
- Povoliť používanie pripojených funkcií v Office

Tieto nastavenia politiky je možné implementovať pomocou buď skupinovej politiky, alebo [cloudovej služby politiky pre Office](https://docs.microsoft.com/DeployOffice/overview-office-client-policy-service). Ak používate skupinovú politiku, musíte si z [centra sťahovania softvéru Microsoft](https://www.microsoft.com/download/details.aspx?id=49030) stiahnuť najnovšiu verziu súborov šablón na správu (ADMX/ADML).

> [!NOTE]
> Ďalšie informácie o spravovaní ovládacích prvkov na ochranu osobných údajov pre Office pre Mac nájdete v téme [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre Mac pomocou predvolieb](mac-privacy-preferences.md).

Ak používate nástroj Group Policy Management, všetky tieto nastavenia politiky sa nachádzajú v časti User Configuration (Konfigurácia používateľa)\\Policies (Politiky)\\Administrative Templates (Nástroje na správu)\\Microsoft Office 2016\\Privacy (Ochrana osobných údajov)\\Trust Center (Centrum dôveryhodnosti).

Tieto nové nastavenia politiky sa vzťahujú aj na počítačové verzie Projectu a Visia, ktoré sú súčasťou niektorých plánov predplatného, ako sú napríklad Project Online Professional alebo Visio Online Plan 2. Vzťahujú sa aj na plán služieb Office 365 Business.

Nejaké existujúce nastavenia politiky sa na služby Office 365 ProPlus už nebudú vzťahovať a tiež by ste mali vedieť o nejakých ďalších zmenách používateľského rozhrania týkajúcich sa nastavenia ochrany osobných údajov, pretože vaši používatelia si ich môžu všimnúť a pýtať sa na ne.

Rovnako ako v prípade akýchkoľvek nových nastavení politiky by ste ich najskôr mali dôkladne otestovať v obmedzenom, kontrolovanom prostredí, aby sa zaručilo, že nastavenia, ktoré nakonfigurujete, majú požadovaný účinok, a až potom tieto nastavenia politiky implementovať v celej organizácii.

## <a name="policy-setting-for-diagnostic-data"></a>Nastavenia politiky pre diagnostické údaje

Diagnostické údaje sa používajú na zabezpečenie a aktualizovanie balíka Office, zisťovanie, diagnostiku a riešenie problémov, ako aj na vylepšenia produktov.

Pomocou nastavenia politiky *Konfigurácia úrovne diagnostických údajov o klientskom softvéri, ktoré služby Office odosielajú spoločnosti Microsoft* môžete  nastaviť úroveň diagnostických údajov odosielaných spoločnosti Microsoft.

Ak zapnete toto nastavenie politiky, musíte určiť, aká úroveň diagnostických údajov sa odosiela do spoločnosti Microsoft. Dostupné voľby sú Povinné, Voliteľné a Žiadne.

- Ak vyberiete možnosť ***Požadované***, spoločnosti Microsoft sa odosielajú minimálne údaje potrebné na očakávané zabezpečenie balíka Office, jeho aktualizáciu a výkonnosť v zariadení, v ktorom je nainštalovaný.

- Ak vyberiete možnosť ***Voliteľné***, spoločnosti Microsoft sa odosielajú dodatočné údaje, ktoré nám pomáhajú zlepšovať produkty, a obsahujú rozšírené informácie, ktoré nám pomáhajú rozpoznávať, diagnostikovať a riešiť problémy. Ak sa rozhodnete odosielať nám voliteľné diagnostické údaje, budú obsahovať aj požadované diagnostické údaje.

- Ak vyberiete možnosť ***Žiadne***, spoločnosti Microsoft sa neodosielajú žiadne diagnostické údaje o klientskom softvéri balíka Office, ktorý sa používa v zariadení používateľa. Táto možnosť však výrazne obmedzuje schopnosť spoločnosti Microsoft zisťovať, diagnostikovať a riešiť problémy, ktoré sa používateľom môžu vyskytnúť pri používaní balíka Office.

Ak vypnete alebo nenakonfigurujete toto nastavenie politiky, spoločnosti Microsoft sa odosielajú voliteľné aj požadované diagnostické údaje.

Ďalšie informácie o diagnostických údajoch sa nachádzajú v témach:

- [Prehľad ovládacích prvkov na ochranu osobných údajov pre Office 365 ProPlus](overview-privacy-controls.md)
- [Požadované diagnostické údaje pre Office](required-diagnostic-data.md)
- [Voliteľné diagnostické údaje pre Office](optional-diagnostic-data.md)
- [Používanie nástroja Diagnostic Data Viewer s balíkom Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)

## <a name="policy-settings-for-connected-experiences"></a>Nastavenia politiky pre pripojené funkcie

Office 365 ProPlus pozostáva z klientskych softvérových aplikácií a pripojených funkcií, ktoré sú navrhnuté tak, aby umožňovali efektívnejšiu tvorbu, komunikáciu a spoluprácu. Príkladom pripojených funkcií je práca na dokumente spoločne s inými používateľmi vo OneDrive for Business alebo preklad obsahu wordového dokumentu do iného jazyka.

Chápeme, že chcete mať možnosť rozhodnúť sa, ktoré typy pripojených funkcií majú vaši používatelia k dispozícii pri práci s aplikáciami balíka Office. Preto sú k dispozícii štyri nové nastavenia politiky:

- Povoliť používanie pripojených funkcií na analýzu obsahu v Office
- Povoliť používanie pripojených funkcií na sťahovanie online obsahu v Office
- Povoliť používanie dodatočných voliteľných pripojených funkcií v Office
- Povoliť používanie pripojených funkcií v Office

Ak nenakonfigurujete tieto nastavenia politiky, budú pre vašich používateľov k dispozícii všetky tieto pripojené funkcie. Vaši používatelia tak získajú všetky funkcie a možnosti, ktoré sú dostupné prostredníctvom služieb Office 365 ProPlus. Chápeme však, že na spĺňanie určitých požiadaviek vašej spoločnosti môže byť potrebné vypnúť niektoré alebo všetky tieto pripojené funkcie.

> [!IMPORTANT]
> Problém týkajúci sa vypnutia týchto 4 nastavení politiky bol nedávno opravený publikovaním nových súborov šablón na správu (ADMX/ADML) v utorok 28. mája 2019. Stiahnite a nainštalujte si aktualizované súbory skupinovej politiky z [Centra sťahovania softvéru](https://www.microsoft.com/en-us/download/details.aspx?id=49030).

Ak sa rozhodnete neposkytovať používateľom niektoré typy pripojených funkcií, príkazy pre tieto funkcie na páse s nástrojmi alebo v ponuke budú neaktívne alebo sa pri pokuse o použitie týchto pripojených funkcií používateľom zobrazí chybové hlásenie. V takom prípade sa spoločnosti Microsoft nebudú odosielať žiadne [požadované údaje služieb](required-service-data.md) pre tieto pripojené funkcie.

Vaši používatelia sa nebudú môcť rozhodnúť zapnúť alebo vypnúť tieto pripojené funkcie, ktoré sú súčasťou služieb Office 365 ProPlus, ak sú prihlásení do služieb Office pomocou poverení organizácie, ktoré sa niekedy označujú ako pracovné alebo školské konto.

### <a name="policy-setting-for-connected-experiences-that-analyze-your-content"></a>Nastavenia politiky pre pripojené funkcie na analýzu obsahu

Toto sú funkcie, ktoré používajú obsah balíka Office na poskytovanie odporúčaní pre návrh, úprav návrhov, prehľadov údajov a podobných funkcií. Príkladmi sú PowerPoint Designer alebo editor vo Worde. Zoznam týchto pripojených funkcií nájdete v téme [Pripojené funkcie v Office](connected-experiences.md).

Pomocou nastavenia politiky *Povoliť používanie pripojených funkcií na analýzu obsahu v Office* môžete určiť, či budú tieto typy pripojených funkcií k dispozícii vašim používateľom. Ak nenakonfigurujete toto nastavenie politiky, tieto pripojené funkcie budú k dispozícii pre vašich používateľov.

Majte na pamäti, že ak vypnete nastavenie politiky *Povoliť používanie pripojených funkcií v Office*, pripojené funkcie na analýzu obsahu nebudú vašim používateľom k dispozícii.

### <a name="policy-setting-for-connected-experiences-that-download-online-content"></a>Nastavenie politiky pre pripojené funkcie na sťahovanie online obsahu

Toto sú funkcie, ktoré umožňujú vyhľadať a sťahovať online obsah vrátane šablón, obrázkov, 3D modelov, videí a referenčných materiálov na vylepšenie vašich dokumentov. Napríklad šablóny balíka Office alebo funkcia Rýchly štart pre PowerPoint. Zoznam týchto pripojených funkcií nájdete v téme [Pripojené funkcie v Office](connected-experiences.md).

Pomocou nastavenia politiky *Povoliť používanie pripojených funkcií na sťahovanie online obsahu v Office* môžete určiť, či budú tieto typy pripojených funkcií k dispozícii vašim používateľom. Ak nenakonfigurujete toto nastavenie politiky, tieto pripojené funkcie budú k dispozícii pre vašich používateľov.

Majte na pamäti, že ak vypnete nastavenie politiky *Povoliť používanie pripojených funkcií v Office*, pripojené funkcie na sťahovanie online obsahu nebudú vašim používateľom k dispozícii.

### <a name="policy-setting-for-optional-connected-experiences"></a>Nastavenia politiky pre voliteľné pripojené funkcie

Okrem pripojených funkcií uvedených vyššie, ktoré sú súčasťou plánu služieb Office 365 ProPlus, existujú aj nejaké voliteľné pripojené funkcie a môžete k nim umožniť používateľom prístup so svojím kontom organizácie. Napríklad funkcie LinkedInu v asistentovi životopisu vo Worde alebo funkcia 3D máp v Exceli, ktorá využíva službu Bing. Ďalšie príklady nájdete v téme [Prehľad voliteľných pripojených funkcií v balíku Office](optional-connected-experiences.md)

Tieto pripojené funkcie sú iné, pretože sa na ne nevzťahuje komerčná zmluva vašej spoločnosti so spoločnosťou Microsoft. Voliteľné pripojené funkcie ponúka priamo spoločnosť Microsoft a riadia sa [zmluvou o poskytovaní služieb spoločnosti Microsoft](https://www.microsoft.com/servicesagreement), nie [podmienkami poskytovania online služieb](https://www.microsoft.com/licensing/product-licensing/products). V niektorých prípadoch sa prostredníctvom týchto voliteľných funkcií poskytujú obsah alebo funkcie tretích strán a môžu sa na ne vzťahovať aj ďalšie podmienky. Ďalšie informácie sa nachádzajú v téme [Prehľad voliteľných pripojených funkcií v balíku Office](optional-connected-experiences.md).

Pomocou nastavenia politiky *Povoliť používanie dodatočných voliteľných pripojených funkcií v Office* môžete určiť, či budú tieto typy pripojených funkcií k dispozícii vašim používateľom. Ak nenakonfigurujete toto nastavenie politiky, tieto voliteľné online funkcie budú k dispozícii pre vašich používateľov.

Aj keď sa rozhodnete tieto voliteľné pripojené funkcie sprístupniť používateľom, vaši používatelia ich budú môcť vypnúť ako skupinu v [dialógovom okne nastavenia ochrany osobných údajov](https://support.office.com/article/3e7bc183-bf52-4fd0-8e6b-78978f7f121b). Vaši používatelia budú mať túto možnosť, len ak sú prihlásení do služieb Office pomocou poverení organizácie (ktoré sa niekedy označujú ako pracovné alebo školské konto) a nie pomocou osobnej e-mailovej adresy.

Taktiež platí, že niektoré tieto voliteľné pripojené funkcie sa považujú aj za pripojené funkcie na analýzu obsahu alebo na sťahovanie online obsahu. Napríklad vkladanie online obrázkov je voliteľná pripojená funkcia, ktorá využíva službu Microsoft Bing, ale považuje sa aj za pripojenú funkciu na sťahovanie online obsahu. Preto ak vypnete nastavenie politiky *Povoliť používanie pripojených funkcií na sťahovanie online obsahu v Office*, funkcia vkladania online obrázkov nebude vašim používateľom k dispozícii. Nebude k dispozícii, ani ak ste zapli nastavenie politiky *Povoliť používanie dodatočných voliteľných pripojených funkcií v Office*. Ďalšie informácie o tom, ktoré pripojené analyzujú obsah alebo sťahujú online obsah, sa nachádzajú v téme [Pripojené funkcie v Office](connected-experiences.md).

Je tu však jedna výnimka. Nastavenie politiky *Povoliť používanie dodatočných voliteľných pripojených funkcií v Office* neriadi funkcie, ktoré vyžadujú pripojenie vášho konta LinkedIn k pracovnému alebo školskému kontu Microsoft. Informácie o riadení týchto typov funkcií, ako sú napríklad informácie z LinkedInu na [karte profilu](https://support.office.com/article/365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) v Outlooku, nájdete v témach [Prepojenie kont LinkedIn a Microsoft](https://support.office.com/article/dc81cc70-4d64-4755-9f1c-b9536e34d381) a [Súhlas s kontaktmi konta LinkedInu pre organizáciu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/linkedin-integration).

### <a name="policy-setting-for-most-connected-experiences"></a>Nastavenia politiky pre väčšinu pripojených funkcií

Pomocou nastavenia politiky *Povoliť používanie pripojených funkcií v Office* môžete určiť, či bude väčšina pripojených funkcií dostupných v službách Office 365 ProPlus k dispozícii vašim používateľom. Ak vypnete toto nastavenie politiky, tieto typy pripojených funkcií nebudú k dispozícii pre vašich používateľov:

- Funkcie na analýzu obsahu
- Funkcie na sťahovanie online obsahu
- Voliteľné pripojené funkcie

Okrem toho platí, že ak vypnete toto nastavenie politiky, vypne sa aj väčšina ostatných pripojených funkcií, ako sú napríklad spolutvorba dokumentov a online ukladací priestor súborov. Zoznam týchto ostatných pripojených funkcií nájdete v téme [Pripojené funkcie v Office](connected-experiences.md).

Aj keď vypnete toto nastavenie politiky, niektoré funkcie balíka Office zostanú dostupné, napríklad synchronizácia poštovej schránky v Outlooku, a aplikácie Teams a Skype for Business budú aj naďalej fungovať. [Nevyhnutné služby](essential-services.md), ako je napríklad licenčná služba, ktorá potvrdzuje, že máte správnu licenciu na používanie služieb Office, takisto zostanú k dispozícii.

## <a name="existing-policy-settings-that-are-replaced-by-new-policy-settings"></a>Existujúce nastavenia politiky, ktoré nahrádzajú nové nastavenia politiky

Od verzie 1904 sa dve existujúce nastavenia politiky už nevzťahujú na služby Office 365 ProPlus. Tieto nové nastavenia politiky sú:

- **Send personal information** (Odosielať osobné informácie), ktoré sa nachádza v časti User Configuration (Konfigurácia používateľa)\\Policies (Politiky)\\Administrative Templates (Nástroje na správu)\\Microsoft Office 2016\\Privacy (Ochrana osobných údajov)\\Trust Center (Centrum dôveryhodnosti).

- **Online Content Options** (Možnosti online obsahu), ktoré sa nachádza v časti User Configuration (Konfigurácia používateľa)\\Policies (Politiky)\\Administrative Templates (Nástroje na správu)\\Microsoft Office 2016\\Tools (Nástroje) | Options (Možnosti) | General (Všeobecné) | Service Options... (Možnosti služieb...)\\Online Content (Online obsah).

Od verzie 1904 nebude mať nakonfigurovanie týchto dvoch existujúcich nastavení politiky žiaden vplyv na služby Office 365 ProPlus. Tieto nastavenia sa už neuplatňujú, pretože ich nahrádzajú tieto nové nastavenia politiky:

- Povoliť používanie pripojených funkcií na analýzu obsahu v Office
- Povoliť používanie pripojených funkcií na sťahovanie online obsahu v Office
- Povoliť používanie dodatočných voliteľných pripojených funkcií v Office
- Povoliť používanie pripojených funkcií v Office

Tieto nové nastavenia politiky poskytujú presnejšiu úroveň kontroly než uvedené dve existujúce nastavenia politiky. Napríklad ak ste predtým použili nastavenie politiky *Odosielať osobné informácie*, funkcia Rýchly štart pre PowerPoint aj Inteligentné vyhľadávanie by bola vypnutá. Ak však teraz s novými nastaveniami politiky vypnete pomocou nastavenia politiky *Povoliť používanie pripojených funkcií na analýzu obsahu v Office* tento typ pripojených funkcií, vypne sa len funkcia Inteligentné vyhľadávanie. Funkcia Rýchly štart pre PowerPoint bude naďalej dostupná vašim používateľom.

Tieto nastavenia politiky sa aj naďalej zobrazujú v nástroji Group Policy Management, pretože sa stále vzťahujú na multilicenčné verzie balíka Office 2016 a Office 2019, ako je napríklad Office Professional Plus 2019.

## <a name="what-about-existing-policy-settings-that-control-connected-experiences"></a>Ako je to v prípade existujúcich nastavení politiky, ktorá riadia pripojené funkcie?

Ako už asi viete, k dispozícii je niekoľko existujúcich nastavené politiky, ktoré umožňujú riadiť pripojené funkcie. Tu je niekoľko príkladov existujúcich nastavení politiky:

- *PowerPoint Designer Options* (Možnosti PowerPoint Designera), ktoré sa nachádza v časti User Configuration (Konfigurácia používateľa)\\Policies (Politiky)\\Administrative Templates (Nástroje na správu)\\Microsoft Office 2016\\Tools (Nástroje) | Options (Možnosti) | General (Všeobecné) | Service Options... (Možnosti služieb...)\\PowerPoint Designer

- *Turn off QuickStarter* (Vypnúť Rýchly štart), ktoré sa nachádza v časti User Configuration (Konfigurácia používateľa)\\Policies (Politiky)\\Administrative Templates (Nástroje na správu)\\Microsoft PowerPoint 2016\\PowerPoint Options (Možnosti PowerPointu)\\General (Všeobecné)

- *Allow LinkedIn Resume Assistant feature* (Povoliť funkciu Sprievodca životopisom LinkedIn), ktoré sa nachádza v časti User Configuration (Konfigurácia používateľa)\\Policies (Politiky)\\Administrative Templates (Nástroje na správu)\\Microsoft Word 2016\\Word Options (Možnosti Wordu)\\General (Všeobecné)

 Tieto existujúce nastavenia politiky môžete naďalej používať na vypnutie jednotlivých pripojených funkcií. Majte však na pamäti, že ak použijete niektoré z nových nastavení politiky, toto nastavenie politiky môže vypnúť pripojenú funkciu, ktorú ste zapli pomocou iného nastavenia politiky. Ak ste napríklad zapli nastavenie politiky *Povoliť funkciu Sprievodca životopisom LinkedIn*, ale vypli nastavenie politiky *Povoliť používanie pripojených funkcií v Office*, Sprievodca životopisom LinkedIn nebude vašim používateľom k dispozícii.

Vo všeobecnosti platí, že ak je jedno nastavenie politiky nakonfigurované na zapnutie konkrétnej pripojenej funkcie a zároveň je iné nastavenie politiky nakonfigurované na vypnutie daného typu pripojenej funkcie, potom je daná konkrétna pripojená funkcia pre používateľov vypnutá.

## <a name="privacy-related-changes-to-the-office-ui"></a>Zmeny používateľského rozhrania balíka Office týkajúce sa ochrany osobných údajov

Došlo k niekoľkým zmenám používateľského rozhrania služieb Office 365 ProPlus týkajúcim sa ochrany osobných údajov, ktoré si vaši používatelia môžu všimnúť a pýtať sa na ne. Tieto zmeny sú priamym dôsledkom nových ovládacích prvkov na ochranu osobných údajov a nastavení politiky dostupných od verzie 1904.

### <a name="dialog-about-optional-connected-experiences"></a>Dialógové okno o voliteľných online funkciách

Ak ste sa rozhodli poskytnúť používateľom [voliteľné online funkcie](optional-connected-experiences.md), pri prvom otvorení aplikácie balíka Office po aktualizácii na verziu 1904 alebo novšiu sa používateľom zobrazí informačné dialógové okno. Toto dialógové okno informuje používateľov, že ste im poskytli možnosť používať tieto voliteľné pripojené funkcie a informuje ich, že môžu prejsť na položku **Súbor** > **Konto**  >  **Ochrana osobných údajov konta** a zmeniť toto nastavenie.

### <a name="privacy-settings-removed-from-the-office-ui"></a>Nastavenia ochrany osobných údajov odstránené z používateľského rozhrania balíka Office

Nasledujúce nastavenia sú odstránené z okna **Súbor** > **Možnosti** > **Centrum dôveryhodnosti** > **Nastavenie centra dôveryhodnosti...** > **Možnosti ochrany osobných údajov**:

- Získajte návrhy, informácie, odporúčania a služby tým, že povolíte balíku Office, aby mal prístup k vylepšeniam produktov a aby ich mohol aj vykonávať na základe obsahu Office na svojom zariadení.

- Povoliť, aby sa Office pripájal k online službám spoločnosti Microsoft a mohol poskytovať relevantné funkcie podľa vášho používania a predvolieb.

Takisto v okne **Súbor** > **Možnosti** > **Všeobecné** je odstránená možnosť zapnutia inteligentných služieb Office.

Ako správca pre vašu organizáciu teraz môžete ovládate príslušné nastavenia týchto funkcií prostredníctvom nových nastavení politiky opísaných vyššie.

### <a name="privacy-settings-added-to-the-office-ui"></a>Nastavenia ochrany osobných údajov pridané do používateľského rozhrania balíka Office

Tieto prvky boli pridané do používateľského rozhrania balíka Office:

- V okne **Súbor** > **Konto** sa používateľom bude zobrazovať nová voľba **Ochrana osobných údajov konta** > **Spravovať nastavenia**. V časti **Spravovať nastavenia**môžu používatelia vypnúť voliteľné pripojené funkcie, ak ste im dali túto možnosť.

- V okne **Súbor** > **Možnosti** > **Centrum dôveryhodnosti** > **Nastavenie centra dôveryhodnosti...** > **Možnosti ochrany osobných údajov** je možnosť povoliť používanie nástroja [Diagnostic Data Viewer](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855) v zariadení.

 
## <a name="control-privacy-settings-by-editing-the-registry"></a>Ovládanie nastavení ochrany osobných údajov úpravou databázy Registry

Niektorí správcovia uprednostňujú zmenu nastavení priamo v databáze Registry, napríklad pomocou skriptu, namiesto použitia skupinovej politiky alebo cloudovej služby politiky pre Office. Pri konfigurácii nastavení ochrany osobných údajov priamo v databáze Registry môžete použiť nasledujúce informácie.


|**Nastavenie politiky** |**Nastavenie databázy Registry**  |**Hodnoty**  |
|---------|---------|---------|---------|
|Konfigurácia úrovne diagnostických údajov o klientskom softvéri, ktoré služby Office odosielajú spoločnosti Microsoft  | SendTelemetry |1 = Povinné <br/> 2 = Voliteľné <br/> 3 = Žiadne|
|Povoliť používanie pripojených funkcií na analýzu obsahu v Office  | UserContentDisabled | 1 = Povolené <br/> 2 = Zakázané|
|Povoliť používanie pripojených funkcií na sťahovanie online obsahu v Office  | DownloadContentDisabled | 1 = Povolené <br/> 2 = Zakázané|
|Povoliť používanie dodatočných voliteľných pripojených funkcií v Office   | ControllerConnectedServicesEnabled  |1 = Povolené <br/> 2 = Zakázané|
|Povoliť používanie pripojených funkcií v Office | DisconnectedState  | 1 = Povolené <br/> 2 = Zakázané|

Ak chcete vytvoriť súbor .reg pre nastavenia ochrany osobných údajov, otvorte Poznámkový blok a skopírujte doň nasledujúce riadky. Upravte hodnoty podľa svojich potrieb a potom súbor uložte. Uistite sa, že názov súboru obsahuje príponu .reg

```
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\Policies\Microsoft\office\16.0\common\privacy]
"disconnectedstate"=dword:00000001
"usercontentdisabled"=dword:00000001
"downloadcontentdisabled"=dword:00000001
"controllerconnectedservicesenabled"=dword:00000001

[HKEY_CURRENT_USER\Software\Policies\Microsoft\office\common\clienttelemetry]
"sendtelemetry"=dword:00000002
```

Tento súbor .reg môžete napríklad použiť pomocou príkazu regedit.exe v skripte na konfigurovanie nastavení ochrany osobných údajov pre používateľa.