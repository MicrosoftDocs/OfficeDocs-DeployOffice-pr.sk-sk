---
title: Povinné diagnostické údaje pre Office
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
description: Správcom balíka Office sú poskytované informácie o požadovaných diagnostických údajoch v Office a zoznam udalostí a údajových polí.
hideEdit: true
ms.openlocfilehash: e6078bf96c60d0f01aeaea0cabe32f135a8fa1a3
ms.sourcegitcommit: 0fd23324ba1364fa1f8dd1578adf25946adde90f
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/07/2019
ms.locfileid: "36238915"
---
# <a name="required-diagnostic-data-for-office"></a>Povinné diagnostické údaje pre Office

> [!IMPORTANT]
> Informácie v tomto článku sa týkajú verzie 1904 alebo novšej verzie nasledujúceho klientskeho softvéru balíka Office nainštalovaného v počítači s Windowsom:
> - Office 365 ProPlus a Office 365 Business
> - Office 365 Personal, Office 365 Home alebo iné verzie balíka Office, ktoré sú súčasťou predplatného služieb Office 365.
> - Project a Visio, ktoré sú súčasťou niektorých plánov predplatného, ako sú napríklad Project Online Professional alebo Visio Online Plan 2.
>
> Informácie platia aj pre verziu 16.28 alebo novšie verzie týchto aplikácií balíka Office pre Mac: Excel, Outlook, OneNote, PowerPoint a Word.

Diagnostické údaje sa používajú na zabezpečenie a aktualizovanie balíka Office, zisťovanie, diagnostiku a riešenie problémov, ako aj na vylepšenia produktov. Tieto údaje neobsahujú meno ani e-mailovú adresu používateľa, obsah súborov používateľa ani informácie o aplikáciách, ktoré nesúvisia s balíkom Office.

Tieto diagnostické údaje sa zhromažďujú a odosielajú spoločnosti Microsoft o klientskom softvéri balíka Office, ktorý sa používa v počítačoch s Windowsom. Niektoré diagnostické údaje sú povinné, a iné diagnostické údaje sú voliteľné. Máte možnosť si vybrať, či nám budete odosielať povinné alebo voliteľné diagnostické údaje, pomocou ovládacích prvkov ochrany osobných údajov, ako sú nastavenia politiky pre organizácie. Nám odoslané diagnostické údaje môžete zobraziť pomocou Zobrazovača diagnostických údajov.

***Povinné diagnostické údaje*** sú minimom potrebným na očakávané zabezpečenie balíka Office, jeho aktualizáciu a výkonnosť v zariadení, v ktorom je nainštalovaný.

Povinné diagnostické údaje pomáhajú identifikovať problémy s balíkom Office, ktoré môžu súvisieť s konfiguráciou zariadenia alebo softvéru. Pomáhajú napríklad určiť, či funkcia balíka Office zlyháva častejšie pri konkrétnej verzii operačného systému, či ide o novo zavedené funkcie alebo či sa to stáva, ak sú niektoré funkcie balíka Office vypnuté. Povinné diagnostické údaje pomáhajú zistiť, diagnostikovať a riešiť tieto problémy rýchlejšie, čím sa znižuje ich vplyv na používateľov alebo organizácie.

Ďalšie informácie o diagnostických údajoch sa nachádzajú v témach:

- [Voliteľné diagnostické údaje pre Office](optional-diagnostic-data.md)
- [Používanie Zobrazovača diagnostických údajov s balíkom Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)

Ak ste správcom v organizácii, možno vás budú zaujímať aj nasledovné témy:

- [Prehľad ovládacích prvkov na ochranu osobných údajov pre Office 365 ProPlus](overview-privacy-controls.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office 365 ProPlus s nastaveniami politiky](manage-privacy-controls.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre Mac pomocou preferencií](mac-privacy-preferences.md)

## <a name="categories-data-subtypes-events-and-data-fields-for-required-diagnostic-data"></a>Kategórie, podtypy údajov, udalosti a údajové polia povinných diagnostických údajov

Povinné diagnostické údaje sú usporiadané do kategórií a podtypov údajov. Každý podtyp údajov obsahuje udalosti, ktoré obsahujú údajové polia, ktoré sú špecifické pre danú udalosť.

Nasledujúca tabuľka obsahuje zoznam kategórií povinných diagnostických údajov. Podtypy údajov v každej kategórii sú uvedené aj s popisom zamerania daného podtypu údajov. Tu sú prepojenia na každú sekciu podtypu údajov, kde nájdete tieto informácie:

- Zoznam udalostí v danom podtype údajov
- Popis každej udalosti
- Zoznam údajových polí v každej udalosti
- Popis každého údajového poľa

| **Kategória**       | **Podtyp údajov**| **Popis**    |
| ---------- | ------------- | ---- |
| **Inštalácia softvéru a inventár** | [Inštalácia balíka Office a inventár](#office-setup-and-inventory-subtype)   | Nainštalovaný produkt a verzia a stav inštalácie.  |
| | [Konfigurácia doplnkov balíka Office](#office-add-in-configuration-subtype)  | Softvérové doplnky a ich nastavenia     |
| | [Zabezpečenie](#security-subtype)  | Chybové stavy dokumentu, funkcie a doplnku, ktoré môže ohroziť zabezpečenie, vrátane pripravenosti na aktualizáciu produktu.  |
| **Používanie produktov a služieb**    | [Úspešnosť funkcie aplikácie](#application-feature-success-subtype)   | Úspešnosť fungovania aplikácie. Obmedzené na otvorenie a zatvorenie aplikácie a dokumentov, úpravu súborov a zdieľanie súborov (spoluprácu). |
| | [Stav a spustenie aplikácie](#application-status-and-boot-subtype)    | Určenie, či sa vyskytli konkrétne udalosti funkcie, napríklad spustenie alebo ukončenie a či je funkcia spustená.   |
| | [Konfigurácia zjednodušenia ovládania balíka Office](#office-accessibility-configuration-subtype)  | Funkcie zjednodušenia ovládania balíka Office       |
| | [Ochrana osobných údajov](#privacy-subtype)| Nastavenia ochrany osobných údajov v Office|
| **Výkon produktov a služieb**       | [Neočakávané ukončenie (zlyhanie) aplikácie](#unexpected-application-exit-crash-subtype)  | Neočakávané ukončenia aplikácie a stav aplikácie, keď sa to stane.    |
|  | [Výkon funkcie aplikácie](#application-feature-performance-subtype)  | Dlhý čas odozvy alebo nízky výkon v prípadoch ako spustenie aplikácie alebo otvorenie súboru. |
|  | [Chyba aktivity aplikácie](#application-activity-error-subtype)   | Chyby funkčnosti funkcie alebo používateľského rozhrania.  |
| **Pripojiteľnosť a konfigurácia zariadenia** | [Pripojiteľnosť a konfigurácia zariadenia](#device-connectivity-and-configuration-subtype) | Stav sieťového pripojenia a nastavenia zariadenia, napríklad pamäte. |


> [!NOTE]
> - Zobrazovač diagnostických údajov zobrazuje kategórie, ale nezobrazuje podtypy údajov.
> - Údajové pole označené ako *zastarané* je alebo čoskoro bude odstránené z povinných diagnostických údajov. Niektoré z týchto údajových polí sú duplicitné položky, ktoré vznikli pri modernizácii diagnostických údajov a používali sa na zabezpečenie toho, aby nedošlo k žiadnemu prerušeniu služby pri zostavách živého diagnostického monitorovania.

## <a name="categories-and-data-fields-that-are-common-for-all-events"></a>Kategórie a údajové polia, ktoré sú spoločné pre všetky udalosti

Existuje niekoľko informácií o udalostiach, ktoré sú spoločné pre všetky udalosti bez ohľadu na kategóriu alebo podtyp údajov. Tieto spoločné informácie, ktoré sa niekedy označujú ako *údajové zmluvy*, sú usporiadané do kategórií. Každá kategória obsahuje polia. Tieto polia sú metaúdaje a vlastnosti jednotlivých udalostí. Tieto informácie môžete zobraziť pomocou Zobrazovača diagnostických údajov.

Kategórie informácií, ktoré sa o udalostiach zhromažďujú, možno rozdeliť do dvoch skupín:

  - [Informácie spoločné pre všetky udalosti](#information-common-to-all-events)
  - [Informácie, ktoré konkrétne podporujú zber diagnostických údajov](#information-that-specifically-supports-diagnostic-data-collection)

### <a name="information-common-to-all-events"></a>*Informácie spoločné pre všetky udalosti*

Informácie, ktoré sú spoločné pre všetky udalosti, sa zhromažďujú v nasledujúcich kategóriách.

#### <a name="app"></a>Aplikácia 

Informácie o aplikácii. Všetky polia sú konštantné pre všetky relácie danej verzie aplikácie.

Táto kategória obsahuje tieto polia:

  - **Branch** – vetva, z ktorej pochádza daná zostava. Umožňuje určiť, z akého typu vetvy daná zostava pochádza, aby sme mohli správne zacieliť opravy.
  - **InstallType** – enumerátor, ktorý identifikuje spôsob, akým používateľ nainštaloval aplikácie. Umožňuje určiť, či konkrétne inštalačné mechanizmy vytvárajú problémy, ktoré nie sa nezobrazia v iných inštalačných mechanizmoch.
  - **Name** – názov aplikácie, ktorá poskytuje údaje. Umožňuje identifikovať, ktorá aplikácia zobrazuje chybu, aby sme vedeli, ako problém riešiť.
  - **Platform** – široká klasifikácia platformy, na ktorej je aplikácia spustená. Umožňuje identifikovať, na ktorých platformách sa môže vyskytnúť chyba, aby sme správne určili prioritu problému.
  - **Version** – verzia aplikácie. Umožňuje identifikovať, ktoré verzie produktu zobrazujú problém, aby správne určili jeho prioritu.

#### <a name="client"></a>Klient 

Identifikátor týkajúci sa inštancie balíka Office v zariadení. Konštanta pre všetky relácie všetkých aplikácií danej verzie inštalácie pre balíky viacerých aplikácií alebo konštantu pre všetky relácie danej verzie aplikácie.

Táto kategória obsahuje tieto polia:

  - **Id** – jedinečný identifikátor priradený klientovi v čase inštalácie balíka Office. Umožňuje identifikovať, či problémy majú vplyv na konkrétnu množinu inštalácií a koľko používateľov je ovplyvnených.

#### <a name="consent"></a>Súhlas

Informácie o súhlase používateľov týkajúcom sa diagnostických údajov a online funkcií.

Táto kategória obsahuje tieto polia:

  - **UserCategory** – identifikuje typ používateľa, od ktorého pochádza súhlas. Môže to byť MSAUser, AADUser alebo LocalDeviceUser.

  - **DiagnosticConsentLevel** – označuje úroveň súhlasu ohľadom diagnostických údajov, ktorý používateľ udelil.

  - **DiagnosticConsentSourceLocation** – označuje, ako používateľ poskytol súhlas ohľadom diagnostických údajov.

  - **DiagnosticConsentConsentTime** – označuje, kedy používateľ poskytol súhlas ohľadom diagnostických údajov.

  - **ServiceConnectionState** – označuje, či sa používateľ rozhodol použiť alebo nepoužiť všetky online funkcie.

  - **ServiceConnectionStateSourceLocation** – označuje, ako sa používateľ rozhodol, či použiť všetky online funkcie.

  - **ServiceConnectionStateConsentTime** – označuje, kedy sa používateľ rozhodol, či použiť všetky online funkcie.

  - **ControllerConnectedServicesState** – označuje, či má používateľ prístup k voliteľným online funkciám.

  - **ControllerConnectedServicesStateSourceLocation** – označuje, ako používateľ uskutočnil výber voliteľných online funkcií.

  - **ControllerConnectedServicesStateConsentTime** – označuje, kedy používateľ zvolil stav voliteľných online funkcií.

  - **UserContentDependentState** – označuje, či sa používateľ rozhodol zapnúť alebo vypnúť online funkcie na analýzu obsahu.

  - **UserContentDependentStateSourceLocation** – označuje, ako používateľ uskutočnil rozhodnutie zapnúť alebo vypnúť online funkcie, ktoré analyzujú obsah.

  - **UserContentDependentStateConsentTime** – označuje, kedy sa používateľ rozhodol zapnúť alebo vypnúť online funkcie, ktoré analyzujú obsah.

  - **DownloadContentState** – označuje, či sa používateľ rozhodol zapnúť alebo vypnúť online funkcie, ktoré sťahujú online obsah.

  - **DownloadContentStateSourceLocation** – označuje, ako používateľ uskutočnil rozhodnutie zapnúť alebo vypnúť online funkcie, ktoré sťahujú online obsah.

  - **DownloadContentStateConsentTime** – označuje, kedy používateľ uskutočnil rozhodnutie zapnúť alebo vypnúť online funkcie, ktoré sťahujú online obsah.

#### <a name="device"></a>Zariadenie 

Informácie o operačnom systéme a zostave.

Táto kategória obsahuje tieto polia:

  - **OsBuild** – číslo zostavy operačného systému v zariadení. Umožňuje určiť, či problémy majú na jednotlivé balíky Service Pack alebo verzie daného operačného systému iný vplyv ako na ostatné, aby sme mohli určiť prioritu problémov.

  - **OsVersion** – hlavná verzia operačného systému nainštalovaného v zariadení. Umožňuje určiť, či problémy majú na konkrétnu verziu operačného systému väčší vplyv ako na ostatné, aby sme mohli určiť prioritu problémov.

#### <a name="legacy"></a>Staršia verzia 

Poskytuje ID aplikácie a verziu operačného systému z dôvodu kompatibility s existujúcimi staršími postupmi zhromažďovania údajov.

Táto kategória obsahuje tieto polia:

  - **AppId** – hodnota enumerátora predstavujúca aplikáciu, ktorá odosiela údaje. Umožňuje identifikovať, ktorá aplikácia zobrazuje chybu, aby sme vedeli, ako problém riešiť.

  - **OsEnv** – enumerátor označujúci operačný systém, v ktorom je relácia spustená. Umožňuje identifikovať, v ktorom operačnom systéme sa problém vyskytuje, aby sme mohli určiť prioritu problémov.

#### <a name="release"></a>Vydanie 

Informácie týkajúce sa kanála vydania. Všetky polia sú konštantné pre všetky relácie všetkých aplikácií danej verzie inštalácie. Určuje skupinu zariadení v jednej fáze cyklu vydania produktu.

Táto kategória obsahuje tieto polia:

  - **Audience** – identifikuje cieľovú podskupinu danej cieľovej skupiny. Umožňuje vysledovať podmnožiny cieľových skupín na vyhodnotenie výskytu a priority problémov.

  - **AudienceGroup** – identifikuje okruh, odkiaľ údaje pochádzajú. Umožňuje distribuovať funkcie vo fázach a identifikovať potenciálne problémy skôr, než sa dostanú k väčšine používateľov.

  - **Channel** – kanál, prostredníctvom ktorého sa produkt vydáva. Umožňuje identifikovať, či má problém na niektorý z našich distribučných kanálov iný vplyv ako na ostatné.

  - **Fork**  – identifikuje rozvetvenie produktu. Umožňuje mechanizmu zhrnúť údaje v rámci množiny čísel zostáv na identifikáciu problémov týkajúcich sa daného vydania.

#### <a name="session"></a>Relácia 

Informácie o relácii procesu. Všetky polia sú konštantné pre túto reláciu.

Táto kategória obsahuje tieto polia:

  - **ABConfigs** – identifikuje množinu skupiny funkcií, ktoré sú spustené v danej relácii. Umožňuje identifikovať, ktoré jednotlivé skupiny funkcií sú spustené v relácii, aby sme mohli určiť, či skupina funkcií je zdrojom problému, ktoré má vplyv na používateľov.

  - **EcsETag** – indikátor systému testovania funkcií, ktorý predstavuje skupiny funkcií odoslané do zariadenia. Umožňuje identifikovať, ktoré skupiny funkcií majú nepriaznivý vplyv na danú reláciu.

  - **Flags** – príznaky sledovania bitovej masky vzťahujúce sa na celú reláciu, aktuálne s primárnym zameraním na možnosti vzoriek a diagnostických údajov. Umožňuje ovládať spôsob správania danej relácie vo vzťahu k diagnostickým údajom, ktoré relácia vytvára.

  - **Id** – jedinečne identifikuje danú reláciu údajov. Umožňuje identifikovať vplyv problémov vyhodnotením počtu ovplyvnených relácií a toho, či existujú spoločné prvky týchto relácií.

  - **ImpressionId** – identifikuje množinu skupiny funkcií, ktoré sú spustené v danej relácii. Umožňuje identifikovať, ktoré jednotlivé skupiny funkcií sú spustené v relácii, aby sme mohli určiť, či skupina funkcií je zdrojom problému, ktoré má vplyv na používateľov.

  - **MeasuresEnabled** – príznak, ktorý označuje, či sú údaje aktuálnych relácií vzorkované alebo nie. Umožňuje určiť, ako sa štatisticky vyhodnotia údaje, ktoré zhromažďujú z danej relácie.

  - **SamplingClientId** – ID klienta na určenie, či je súčasťou vzorkovania. Umožňuje určiť, prečo jednotlivé relácie boli alebo neboli súčasťou vzorkovania.

#### <a name="user"></a>Používateľ

Poskytuje informácie o nájomníkovi pre komerčné jednotky SKU softvéru.

Táto kategória obsahuje tieto polia:

  - **PrimaryIdentityHash** – pseudoidentifikátor, ktorý predstavuje aktuálneho používateľa.

  - **PrimaryIdentitySpace** – typ identity v pseudoidentifikátore PrimaryIdentityHash. Môže to byť MASCID, OrgIdCID alebo UserObjectId.

  - **TenantGroup** – typ nájomníka, ktorému patrí predplatné. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov.

  - **TenantId** – nájomník, s ktorým je predplatné používateľa spojené. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

### <a name="information-that-specifically-supports-diagnostic-data-collection"></a>*Informácie, ktoré konkrétne podporujú zber diagnostických údajov*

Informácie, ktoré konkrétne podporujú zber diagnostických údajov, sa zbierajú v nasledujúcich kategóriách.

#### <a name="activity"></a>Aktivita

Informácie na pochopenie úspešnosti samotnej udalosti zberu údajov.

Táto kategória obsahuje tieto polia:

  - **AggMode** – určuje, ako má systém agregovať výsledky aktivity. Umožňuje obmedziť množstvo informácií nahratých zo zariadenia používateľa agregáciou výsledkov aktivity do jednej udalosti, ktorá sa odosiela pravidelne.

  - **Count** – označuje, koľkokrát sa aktivita vyskytla, ak počet pochádza z agregovanej udalosti. Umožňuje určiť, ako často bola aktivita úspešná alebo neúspešná na základe agregačného režimu aktivity.

  - **CV** – hodnota, ktorá identifikuje vzťah medzi aktivitami a podradenými aktivitami. Umožňuje znova vytvoriť vzťah medzi vnorenými aktivitami.

  - **Duration** – časový úsek, ktorý bol potrebný na vykonanie aktivity. Umožňuje identifikovať problémy s výkonom, ktoré majú negatívny vplyv na prostredie používateľa.

  - **Result**.**Code** – aplikáciou definovaný kód na identifikáciu daných výsledkov. Umožňuje určiť konkrétnejšie podrobností o danom zlyhaní, ako je napríklad kód zlyhania, pomocou ktorého je možné klasifikovať a riešiť problémy.

  - **Result.Tag** – značka celého čísla, ktorá identifikuje miesto v kóde, kde bol výsledok vytvorený. Umožňuje jednoznačne určiť miesto v kóde, kde bol výsledok vytvorený, vďaka čomu je možné klasifikovať zlyhania.

  - **Result**.**Type** – typ kódu výsledku. Identifikuje, aký typ kódu výsledku bol odoslaný, aby bolo možné hodnotu správne interpretovať.

  - **Success** – príznak označujúci úspešnosť alebo zlyhanie aktivity. Umožňuje určiť, či akcie, ktoré používateľ v produktoch vykoná, sú úspešné alebo neúspešné. Umožňuje to identifikovať problémy, ktoré majú vplyv na používateľa.

#### <a name="application"></a>Aplikácia 

Informácie o inštalácii aplikácie, z ktorej sa zhromažďujú udalosti.

Táto kategória obsahuje tieto polia:

  - **Architecture** – architektúra aplikácie. Umožňuje klasifikovať chyby, ktoré môžu byť špecifické pre architektúru aplikácie.

  - **Click2RunPackageVersion** – číslo verzie balíka Klikni a spusti, z ktorého bola aplikácia nainštalovaná. Umožňuje identifikovať, ktorá verzia programu sa použila na inštaláciu balíka Office, aby sme mohli identifikovať problémy súvisiace s inštaláciou.

  - **DistributionChannel** – kanál, v ktorom bola aplikácia nasadená. Umožňuje rozdeliť prichádzajúce údaje, aby sme mohli určiť, či majú problémy vplyv na cieľové skupiny.

  - **InstallMethod** – označuje, či bola aktuálna zostava balíka Office inovovaná zo staršej zostavy, vrátená na staršiu zostavu alebo nanovo nainštalovaná.

  - **IsClickToRunInstall** – príznak, ktorý označuje, či išlo o inštaláciu Klikni a spusti. Umožňuje identifikovať problémy, ktoré môžu byť špecifické pre mechanizmus inštalácie Klikni a spusti.

  - **IsDebug** – príznak označujúci, či je zostava balíka Office zostavou ladenia. Umožňuje identifikovať, či problémy pochádzajú zo zostáv ladenia, ktoré sa môžu správať odlišne.

  - **IsInstalledOnExternalStorage** – príznak, ktorý označuje, či bol balík Office nainštalovaný v externom úložnom zariadení. Umožňuje určiť, či problémy možno vysledovať do externého umiestnenia ukladacieho priestoru.

  - **IsOEMInstalled** – príznak, ktorý označuje, či bol balík Office nainštalovaný výrobcom OEM. Umožňuje určiť, či bola aplikácia nainštalovaná výrobcom OEM, čo nám pomáha klasifikovať a identifikovať problémy.

  - **PreviousVersion** – verzia balíka Office, ktorý bol predtým nainštalovaný v počítači. Umožňuje vrátiť sa späť na predchádzajúcu verziu, ak je aktuálna verzia problematická.

  - **ProcessFileName** – názov súboru aplikácie. Umožňuje identifikovať názov spustiteľného súboru, ktorý generuje údaje, pretože viaceré rôzne názvy súborov procesov môžu byť uvádzané ako názov rovnakej aplikácie.

#### <a name="client"></a>Klient

Informácie o klientovi balíka Office.

Táto kategória obsahuje tieto polia:

  - **FirstRunTime** – čas prvého spustenia klienta. Umožňuje pochopiť, ako dlho má klient nainštalovaný balík Office.

#### <a name="device"></a>Zariadenie

Informácie o konfigurácii a možnostiach zariadenia.

Táto kategória obsahuje tieto polia:

  - **DigitizerInfo** – informácie o digitalizátore používanom zariadením. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **FormFactor** – identifikuje, aký je činiteľ tvaru zariadenia, ktoré odosiela informácie. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **FormFactorFamily** – identifikuje, aký je činiteľ tvaru zariadenia, ktoré odosiela informácie. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **HorizontalResolution** – vodorovné rozlíšenie obrazovky zariadenia. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **Id** – jedinečný identifikátor zariadenia. Umožňuje identifikovať rozšírenie problémov v množine zariadení.

  - **IsEDPPolicyEnabled** – príznak, ktorý označuje, či je v počítači zapnutá rozšírená ochrana údajov. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **IsTerminalServer** – príznak určujúci, či je počítač terminálový server. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **Manufacturer** – výrobca zariadenia. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **Model** – model zariadenia. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **MotherboardUUIDHash** – hodnota hash jedinečného identifikátora základnej dosky. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **Name** – názov zariadenia. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **NumProcPhysCores** – počet fyzických jadier v počítači. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **OsLocale** – miestne nastavenie operačného systému, ktorý je spustený. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **ProcessorArchitecture** – architektúra procesora. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **ProcessorCount** – počet procesorov v počítači. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **ProcSpeedMHz** – rýchlosť procesora. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **RamMB** – množstvo pamäte v zariadení. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **ScreenDepth** – umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **ScreenDPI** – hodnota DPI obrazovky. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **SusClientId** – ID služby Windows Update zariadenia, v ktorom je balík Office spustený.

  - **SystemVolumeFreeSpaceMB** – množstvo voľného miesta v systémovom zväzku. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **SystemVolumeSizeMB** – veľkosť systémového zväzku v počítači. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **VerticalResolution** – zvislé rozlíšenie obrazovky zariadenia. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **WindowErrorReportingMachineId** – jedinečný identifikátor počítača poskytnutý technológiou hlásenia chýb systému Windows. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **WindowSqmMachineId** – jedinečný identifikátor počítača poskytnutý technológiou SQM systému Windows. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

#### <a name="event"></a>Udalosť 

Informácie špecifické pre udalosť vrátane jedinečného identifikátora v relácii.

Táto kategória obsahuje tieto polia:

  - **Contract** – zoznam všetkých zmlúv, ktoré udalosť implementuje. Umožňuje vyhodnotiť, aké údaje sú súčasťou jednotlivých udalostí, aby sme ich mohli efektívne spracovať.

  - **CV** – hodnota, ktorá umožňuje identifikovať udalosti, ktoré navzájom súvisia. Slúži na diagnostiku, ktorá umožňuje identifikovať vzory súvisiaceho správania alebo súvisiacich udalostí.

  - **Flags** – informácia používaná na zmenu spôsobu, akým daná udalosť odpovedá. Slúži na spravovanie toho, ako sa s danou udalosťou zaobchádza na účely nahratia údajov pre spoločnosť Microsoft.

  - **Id** – jedinečný identifikátor udalosti. Umožňuje jedinečnú identifikáciu prijatých udalostí.

  - **Name** – názov udalosti. Umožňuje identifikovať udalosť, ktorá bola odoslaná z klienta.

  - **Rule** – identifikátor pravidla, ktoré vygenerovalo údaje, ak boli vygenerované podľa pravidla. Umožňuje identifikovať zdroj údajov, aby sme mohli overiť a spravovať parametre daných udalostí.

  - **RuleId** – identifikátor pravidla, ktoré vygenerovalo údaje, ak boli vygenerované podľa pravidla. Umožňuje identifikovať zdroj údajov, aby sme mohli overiť a spravovať parametre daných udalostí.

  - **RuleInterfaces** – všetky rozhrania, ktoré sú implementované podľa konkrétneho pravidla. Umožňuje klasifikovať a importovať údaje na základe štruktúry, čo zjednodušuje spracovanie údajov.

  - **RuleVersion** – identifikátor pravidla, ktoré vygenerovalo údaje, ak boli vygenerované podľa pravidla. Umožňuje identifikovať zdroj údajov, aby sme mohli overiť a spravovať parametre daných udalostí.

  - **SampleRate** – indikácia percentuálnej hodnoty používateľov, ktorí odosielajú tento údaj. Umožňuje to vykonať štatistickú analýzu údajov a pri veľmi bežných údajových bodoch nevyžaduje, aby ho odosielali všetci používatelia.

  - **SchemaVersion** – verzia schémy použitá na generovanie diagnostických údajov. Vyžaduje sa na spravovanie údajov odoslaných z klienta. Umožňuje to neskôr zmeniť, aké údaje sú odosielané z každého klienta.

  - **Sequence** – počítadlo, ktoré označuje poradie, v akom bola udalosť vytvorená na strane klienta. Umožňuje zoradiť prijaté údaje, aby sme mohli identifikovať, aké kroky mohli viesť k problému, ktorý má vplyv na klientov.

  - **Source** – zdrojový kanál, ktorý sa použil na nahratie údajov. Vyžaduje sa na monitorovanie všetkých našich kanálov nahrávania a ich celkového stavu a pomáha identifikovať problémy s kanálom nahrávania. Umožňuje monitorovať jednotlivé kanály nahrávania, aby sa zaistila ich kompatibilita.

  - **Time** – čas vygenerovania udalosti na strane klienta. Umožňuje synchronizovať a overiť poradie udalostí vygenerovaných na strane klienta, ako aj vytvoriť metriky výkonu pre používateľské pokyny. 

#### <a name="host"></a>Hostiteľ

Informácie o aplikácii, ktorá hosťuje vstavanú aplikáciu.

Táto kategória obsahuje tieto polia:

  - **Id** – jedinečný identifikátor priradený hostiteľskej aplikácii vstavanou aplikáciou.

  - **SessionId** – globálne jedinečný identifikátor relácie hostiteľa.

  - **Version** – identifikátor verzie primárneho spustiteľného súboru hostiteľa.

#### <a name="legacy"></a>Staršia verzia

Informácie potrebné na kompatibilitu starších systémov.

Táto kategória obsahuje tieto polia:

  - **OsBuild** – špecifické číslo zostavy operačného systému. Umožňuje zistiť, z ktorej verzie operačného systému diagnostické údaje pochádzajú, aby sa určila priorita problémov.

  - **OsBuildRevision** – číslo revízie zostavy operačného systému. Umožňuje zistiť, z ktorej verzie operačného systému diagnostické údaje pochádzajú, aby sa určila priorita problémov.

  - **OsMinorVersion** – vedľajšia verzia operačného systému. Umožňuje zistiť, z ktorej verzie operačného systému diagnostické údaje pochádzajú, aby sa určila priorita problémov.

  - **OsVersionString** – zjednotený reťazec predstavujúci číslo zostavy operačného systému. Umožňuje zistiť, z ktorej verzie operačného systému diagnostické údaje pochádzajú, aby sa určila priorita problémov.

#### <a name="session"></a>Relácia

Informácie o relácii procesu.

Táto kategória obsahuje tieto polia:

  - **ABConfigsDelta** – sleduje rozdiel medzi aktuálnymi údajmi ABConfigs a predchádzajúcu hodnotu. Umožňuje sledovať, aké nové skupiny funkcií sú v počítači, čo pomáha určiť, či je za problém zodpovedná nová skupina funkcií.

  - **CollectibleClassification** – triedy informácií, ktoré môže relácia zhromaždiť. Umožňuje filtrovať relácie na základe údajov, ktoré obsahujú.

  - **DisableTelemetry** – príznak, ktorý označuje či je nastavený kľúč DisableTelemetry. Umožňuje zistiť, či relácia nehlásila diagnostické údaje iné ako EssentialServiceMetadata.

  - **SamplingKey** – kľúč používaný na určenie, či relácia je alebo nie je vzorkovaná. Umožňuje pochopiť, ako pri jednotlivých reláciách prebieha voľba toho, či budú alebo nebudú vzorkované.

  - **SamplingMethod** – metóda použitá na určenie politiky vzorkovania. Umožňuje pochopiť, aké údaje pochádzajú z relácie.

  - **Sequence** – jedinečný číselný identifikátor relácie. Umožňuje vytvoriť poradie relácií na analýzu problémov, ktoré sa mohli vyskytnúť.

  - **Start** – čas spustenia relácie procesu. Umožňuje stanoviť, kedy relácia začala.

  - **TimeZoneBiasInMinutes** -rozdiel v minútach medzi časom UTC a miestnym časom. Umožňuje normalizáciu času UTC späť na miestny čas.

  - **SamplingClientIdValue** – hodnota kľúča použitého na určenie vzorkovania. Umožňuje určiť, prečo relácia bola alebo nebola vzorkovaná.

  - **SamplingDeviceIdValue** – hodnota kľúča použitého na určenie vzorkovania. Umožňuje určiť, prečo relácia bola alebo nebola vzorkovaná.

  - **SamplingSessionKValue** – rozšírené metaúdaje vzorkovania. Pomáhajú vyhodnotiť štatistický význam prijatých údajov.

  - **SamplingSessionNValue** – rozšírené metaúdaje vzorkovania. Pomáhajú vyhodnotiť štatistický význam prijatých údajov.

  - **TelemetryPermissionLevel** – hodnota označujúca úroveň diagnostických údajov, s ktorými používateľ explicitne súhlasil. Umožňuje pochopiť, akú úroveň diagnostických údajov môžete od relácie očakávať.

## <a name="data-fields-that-are-common-for-onenote-events"></a>Údajové polia, ktoré sú spoločné pre udalosti OneNotu

Nasledujúce údajové polia sú spoločné pre všetky udalosti OneNotu v systémoch Mac, iOS a Android.

> [!NOTE]
> Pri používaní Zobrazovača diagnostických údajov zobrazujú udalosti OneNotu v systémoch Mac, iOS a Android názov Aktivita, Údaje zostavy alebo Neočakávané. Ak chcete nájsť skutočný názov udalosti, vyberte udalosť a potom sa pozrite na pole EventName.

- **Activity_ActivityType** – označuje typ tejto udalosti aktivity. Aktivita môže byť bežná aktivita alebo aktivita s vysokou hodnotou.

- **Activity_AggMode** – určuje, ako má systém agregovať výsledky aktivity. Umožňuje obmedziť množstvo informácií nahratých zo zariadenia používateľa agregáciou výsledkov aktivity do jednej udalosti, ktorá sa odosiela pravidelne.

- **Activity_Count** – označuje, koľkokrát sa aktivita vyskytla, ak počet pochádza z agregovanej udalosti. Umožňuje určiť, ako často bola aktivita úspešná alebo neúspešná na základe agregačného režimu aktivity.

- **Activity_CV** – hodnota, ktorá identifikuje vzťah medzi aktivitami a podradenými aktivitami. Umožňuje znova vytvoriť vzťah medzi vnorenými aktivitami.

- **Activity_DetachedDurationInMicroseconds** – čas, keď aktivita je nečinná a v skutočnosti nerobí nič, ale čas sa stále započítava do celkového času trvania aktivity.

- **Activity_DurationInMicroseconds** – časový úsek, ktorý bol potrebný na vykonanie aktivity. Umožňuje identifikovať problémy s výkonom, ktoré majú negatívny vplyv na prostredie používateľa.

- **Activity_Expiration** – dátum v číselnom formáte označuje, kedy sa táto udalosť prestane odosielať z klientov.

- **Activity_FailCount** – počet zlyhaní tejto aktivity

- **Activity_Name** – krátky názov udalosti. Umožňuje identifikovať udalosť, ktorá bola odoslaná z klienta.

- **Activity_Namespace** – priestor názvov udalosti. Umožňuje zoskupovať udalosť do skupín.

- **Activity_Reason** – reťazec označujúci dôvod skončenia aktivity s určitým výsledkom.

- **Activity_Result** – príznak označujúci úspešnosť, zlyhanie alebo neočakávané zlyhanie aktivity. Umožňuje určiť, či akcie, ktoré používateľ v produktoch vykoná, sú úspešné alebo neúspešné. Umožňuje to identifikovať problémy, ktoré majú vplyv na používateľa.

- **Activity_State** – príznak označujúci, či udalosť predstavuje začiatok aktivity používateľa alebo koniec aktivity používateľa.

- **Activity_FailCount** – počet úspešností tejto aktivity.

- **ErrorCode** – označuje kód chyby, ak je k dispozícii.

- **ErrorCode2** – označuje druhý kód chyby, ak je k dispozícii.

- **ErrorCode3** – označuje tretí kód chyby, ak je k dispozícii.

- **ErrorTag** – označuje značku priradenú v kóde chyby, ak je k dispozícii.

- **ErrorType** – označuje typ chyby, ak je k dispozícii.

- **EventName** – jedinečný názov udalosti OneNotu. Udalosti OneNotu používajú toto vlastné pole na zadanie jedinečného názvu z dôvodu technického obmedzenia v minulosti.

- **ExpFeatures** – označuje, či má používateľ v aplikácii OneNote zapnutý prepínač experimentálnych funkcií alebo nie.

- **ExpirationDate** – dátum v číselnom formáte označuje, kedy sa táto udalosť prestane odosielať z klientov.

- **IsConsumer** – označuje, či ide o používateľa v programe Consumer alebo nie.

- **IsEdu** – označuje, či ide o používateľa v nájomníkovi programu Education alebo nie.

- **IsIW** – označuje, či ide o používateľa v programe Enterprise alebo nie.

- **IsMsftInternal** – označuje, či je používateľ zamestnancom spoločnosti Microsoft alebo nie.

- **IsPremiumUser** – označuje, či má používateľ prémiovú licenciu alebo nie.

- **Namespace** – priestor názvov udalosti. Umožňuje zoskupovať udalosť do skupín.

- **Release_AppStore** – príznak označujúci, či zostava pochádza z obchodu s aplikáciami alebo nie.

- **Release_Audience** – identifikuje cieľovú podskupinu danej cieľovej skupiny. Umožňuje vysledovať podmnožiny cieľových skupín na vyhodnotenie výskytu a priority problémov.

- **Release_AudienceGroup** – identifikuje okruh, odkiaľ údaje pochádzajú. Umožňuje distribuovať funkcie vo fázach a identifikovať potenciálne problémy skôr, než sa dostanú k väčšine používateľov.

- **Release_Channel** – kanál, prostredníctvom ktorého sa produkt vydáva. Umožňuje identifikovať, či má problém na niektorý z našich distribučných kanálov iný vplyv ako na ostatné.

- **RunningMode** – označuje spôsob spustenia aplikácie používateľom alebo procesom systému.

- **SchemaVersion** – označuje aktuálnu verziu schémy telemetrie v kanáli telemetrie vo OneNote.

- **Session_EcsETag** – indikátor systému testovania funkcií, ktorý predstavuje skupiny funkcií odoslané do zariadenia. Umožňuje identifikovať, ktoré skupiny funkcií majú nepriaznivý vplyv na danú reláciu.

- **Session_ImpressionId** – identifikuje množinu skupiny funkcií, ktoré sú spustené v danej relácii. Umožňuje identifikovať, ktoré jednotlivé skupiny funkcií sú spustené v relácii, aby sme mohli určiť, či skupina funkcií je zdrojom problému, ktoré má vplyv na používateľov.

- **SessionCorrelationId** – globálne jedinečný identifikátor relácie hostiteľa.

- **SH_ErrorCode** – označuje kód chyby, ak je k dispozícii, keď aktivita zlyhá.

- **Tag** – značka celého čísla, ktorá identifikuje miesto v kóde, kde bola udalosť telemetrie vytvorená.

- **UserInfo_IdType** – reťazec označujúci typ konta používateľa.

- **UserInfo_OMSTenantId** – nájomník, s ktorým je predplatné používateľa spojené. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

- **UserInfo_OtherId** – zoznam neprimárnych pseudonymných identifikátorov, ktoré predstavujú kontá používateľa.

- **UserInfo_OtherIdType** – zoznam neprimárnych typov kont.

## <a name="software-setup-and-inventory-data-events"></a>Údajové udalosti v kategórii Inštalácia softvéru a inventár

Toto sú podtypy údajov v tejto kategórii:
- [Inštalácia balíka Office a inventár](#office-setup-and-inventory-subtype)
- [Konfigurácia doplnkov balíka Office](#office-add-in-configuration-subtype)
- [Zabezpečenie](#security-subtype)  

### <a name="office-setup-and-inventory-subtype"></a>*Podtyp Inštalácia balíka Office a inventár*

Nainštalovaný produkt a verzia a stav inštalácie.

#### <a name="officeclicktorunupdatestatus"></a>Office.ClickToRun.UpdateStatus

Platí pre všetky aplikácie win32. Pomáha pochopiť stav procesu aktualizácie balíka Office (úspešná alebo neúspešná s podrobnosťami chyby).

Zhromažďujú sa tieto polia:

- **build** – aktuálne nainštalovaná verzia balíka Office

- **channel** – kanál, cez ktorý bol distribuovaný balík Office

- **errorCode** – kód chyby s informáciou o zlyhaní

- **errorMessage** – ďalšie informácie o chybe

- **status** – aktuálny stav aktualizácie

- **targetBuild** – verzia, na ktorú sa balík Office aktualizuje

#### <a name="officecompliancefileformatballotdisplayedonfirstboot"></a>Office.Compliance.FileFormatBallotDisplayedOnFirstBoot

Označuje, či sa používateľovi zobrazilo dialógové okno výberu formátu súboru balíka Office pri prvom alebo druhom štarte Wordu, Excelu, PowerPointu vo Win32.  Sleduje, či sa zobrazí dialógové okno voľby formátu súboru – udalosť sa odošle pri prvom alebo druhom štarte Wordu, Excelu alebo PPT Win32.

Zhromažďujú sa tieto polia:

- **CountryRegion** – nastavenie oblasti krajiny používateľov v systéme Windows

- **FileFormatBallotBoxAppIDBootedOnce** – v ktorej aplikácii (Word, Excel, PPT) sa spracovala logika zobrazenia voľby formátu súboru.

- **FileFormatBallotBoxDisplayedOnFirstBoot** – aký je výsledok zobrazenia voľby formátu súboru (zobrazuje sa/nezobrazuje sa ako neočakávaný/nezobrazený z dôvodu licencie/nezobrazený z dôvodu polohy).

#### <a name="officecompliancefileformatballotoption"></a>Office.Compliance.FileFormatBallotOption

Sleduje, či sa zobrazí dialógové okno voľby formátu súboru – udalosť sa odošle pri prvom alebo druhom štarte Wordu, Excelu alebo PPT Win32.  Označuje, či sa zobrazuje dialógové okno výberu formátu súboru balíka Office pri prvom alebo druhom štarte Wordu, Excelu, PowerPointu vo Win32.

Zhromažďujú sa tieto polia:

- **FileFormatBallotSelectedOption** – identifikuje možnosť formátu súboru (OOXML/ODF), ktorú používateľ vybral prostredníctvom dialógového okna voľby formátu súboru.


#### <a name="officecorrelationmetadatautccorrelationmetadata"></a>Office.CorrelationMetadata.UTCCorrelationMetadata

Zhromažďuje metaúdaje balíka Office prostredníctvom UTC na porovnanie s ekvivalentnými údajmi zhromaždenými prostredníctvom kanála telemetrie balíka Office a kontrolu správnosti a úplnosti údajov.

Zhromažďujú sa tieto polia:

- **abConfigs** – zoznam ID funkcií na určenie, ktoré funkcie sú zapnuté v klientovi alebo prázdne, keď tieto údaje nie sú zhromažďované.

- **abFlights** – hodnota „NoNL:NoFlights“, keď skupiny funkcií nie sú nastavené. V opačnom prípade hodnota „holdoutinfo=unknown“.

- **AppSessionGuid** – identifikátor konkrétnej relácie aplikácie, ktorá začína v čase vytvorenia procesu a pretrváva až do konca procesu. Je formátovaný ako štandardný 128-bitový identifikátor GUID, ale skladá sa zo 4 častí. Tieto štyri časti sú v poradí 1. ID procesu 32-bitovej verzie, 2. ID relácie 16-bitovej verzie, 3. ID spustenia 16-bitovej verzie, 4. čas vytvorenia procesu 64-bitovej verzie v UTC 100ns.

- **appVersionBuild** – číslo verzie zostavy aplikácie.

- **appVersionMajor** – číslo hlavnej verzie aplikácie.

- **appVersionMinor** – číslo vedľajšej verzie aplikácie.

- **appVersionRevision** – číslo verzie revízie aplikácie.

- **audienceGroup** – názov cieľovej skupiny používateľov vydania

- **audienceId** – názov cieľovej skupiny vydania

- **channel** – kanál, cez ktorý bol distribuovaný balík Office

- **deviceClass** – činiteľ tvaru zariadenia z operačného systému

- **ecsETag** – identifikátor experimentu procesu

- **impressionId** – identifikátor GUID označujúci aktuálnu množinu funkcií.

- **languageTag** -aktuálna značka jazyka skupiny IETF používateľského rozhrania balíka Office

- **officeUserID** – náhodne vytvorený identifikátor GUID pre túto inštaláciu balíka Office

- **osArchitecture** – architektúra operačného systému

- **osEnvironment** – celé číslo označujúce operačný systém (Windows, Android, iOS, Mac atď.).

- **osVersionString** – verzia operačného systému

- **sessionID** – náhodne vytvorený identifikátor GUID na identifikáciu relácie aplikácie

- **UTCReplace_AppSessionGuid** – konštantná boolovská hodnota. Vždy hodnota True.

#### <a name="officetargetedmessagingensurecached"></a>Office.TargetedMessaging.EnsureCached 

Sleduje, či bol stiahnutý balík pre dynamické plátno. Berie do úvahy konfiguráciu softvéru, pretože balík musí byť úspešne stiahnutý, aby umožnil klientovi vykresliť správne prostredie. Veľmi dôležité najmä v rámci spotrebiteľských predplatných, kde pomocou plátna informujeme používateľa, že platnosť licencie uplynula. Slúži na sledovanie metaúdajov balíka dynamického obsahu, ktorý bol stiahnutý a uložený do vyrovnávacej pamäte produktom, ako aj výsledky operácií vykonaných s balíkom: zlyhania stiahnutia, zlyhania rozbalenia, zlyhania kontrol konzistentnosti, počet výskytov vo vyrovnávacej pamäti, využitia balíka, zdroje sťahovania.

Zhromažďujú sa tieto polia:

  - **Data\_CacheFolderNotCreated** – boolovský príznak, ktorý označuje, či bolo vytvorenie priečinka vyrovnávacej pamäte úspešné

  - **Data\_CdnPath – zdrojová adresa balíka**

  - **Data\_EnsureCached** – boolovský príznak, ktorý označuje, či bol balík obsahu uložený do vyrovnávacej pamäte

  - **Data\_ExistsAlready** boolovský príznak, ktorý označuje, že balík bol stiahnutý už predtým a bol vykonaný ďalší pokus

  - **Data\_GetFileStreamFailed** – zdrojový balík nie je k dispozícii v zdroji

  - **Data\_GetFileStreamFailedToCreateLocalFolder** – problémy s lokálnym diskom, ktoré spôsobujú zlyhanie vytvorenia adresára

  - **Data\_GetFileStreamFromPackageFailed** – príznak, ktorý označuje, ak bol balík stiahnutý, ale klient ho nedokáže prečítať

  - **Data\_GetFileStreamFromPackageSuccess** – úspešné pokusy čítania balíka

  - **Data\_GetFileStreamSuccess** – bez problémov s diskom či konfiguráciou, ktoré by nedovolili čítať prúd súborov

  - **Data\_GetRelativePathsFailed** – relatívna cesta nesmeruje na dostupné umiestnenie

  - **Data\_HashActualValue** – hodnota hash získaná z názvu súboru pri použití balíka

  - **Data\_HashCalculationFailed** – chyba výpočtu hodnoty hash

  - **Data\_HashMatchFailed** – nesúlad hodnoty hash medzi názvom balíka a hodnotami databázy Registry vo vyrovnávacej pamäti

  - **Data\_HashMatchSuccess** – úspešná kontrola konzistentnosti hodnoty hash

  - **Data\_PackageDownloadRequestFailed** – balík nie je možné stiahnuť

  - **Data\_PackageDownloadRequestNoData** – stiahnutý balík neobsahuje žiadne údaje

  - **Data\_PackageDownloadRequestSuccess** – úspešné stiahnutie balíka

  - **Data\_PackageExplodedSuccess** – stavy pokusov o rozbalenie

  - **Data\_PackageOpenFailed** – neúspešné pokusy otvorenia súboru balíka

  - **Data\_PackageOpenSuccess** – úspešné pokusy otvorenia súboru balíka

  - **Data\_SuccessHashValue** – hodnota hash získaná z názvu súboru pri stiahnutí balíka

  - **Data\_SuccessSource** – povrch, pre ktorý sa balík stiahol

#### <a name="officevisiovisiosku"></a>Office.Visio.VisioSKU

Zaznamenáva jednotky SKU Visia, či ide o Standard alebo Professional. Potrebné pri kategorizácii problémov podľa jednotiek SKU.

Zhromažďujú sa tieto polia:

  - **Data\_VisioSKU**:**integer** – 0 pre jednotky SKU Standard a 1 pre jednotky SKU Professional

### <a name="office-add-in-configuration-subtype"></a>*Podtyp Konfigurácia doplnkov balíka Office*

Softvérové doplnky a ich nastavenia

#### <a name="exceladdindefinedfunctioncustomfunctionsallinone"></a>Excel.AddinDefinedFunction.CustomFunctionsAllInOne

Zhromažďuje informácie o tom, ako sa v režime runtime správajú funkcie vlastných doplnkov. Udržiava počítadlá pokusov spustenia, úspešných dokončení, chýb infraštruktúry a chýb používateľských kódov. Táto možnosť sa používa na identifikovanie problémov so spoľahlivosťou v produkte a riešenie problémov, ktoré majú vplyv na používateľov.
 
Zhromažďujú sa tieto polia:

- **AsyncBegin** – počet asynchrónnych funkcií, ktoré začínajú

- **AsyncEndAddinError** – počet asynchrónnych funkcií, ktoré končia chybou

- **AsyncEndInfraFailure** – počet asynchrónnych funkcií, ktoré končia zlyhaním infraštruktúry

- **AsyncEndSuccess** – počet asynchrónnych funkcií, ktoré končia úspešne

- **AsyncRemoveCancel** – počet zrušených asynchrónnych funkcií 

- **AsyncRemoveRecycle** – počet asynchrónnych funkcií, ktoré boli odstránené z dôvodu recyklácie 

- **StreamingCycles1** – počítadlo streamovania cyklov

#### <a name="officeextensibilityappcommandsappcmdprojectionstatus"></a>Office.Extensibility.AppCommands.AppCmdProjectionStatus

Zhromažďuje informácie na sledovanie, ktoré inštalácie doplnku balíka Office aktualizovali pás s nástrojmi úspešne a neúspešne.

Slúži na riešenie bežných problémov registrácie, keď doplnky nie sú nainštalované správne a z toho dôvodu sú nepoužiteľné.

Zhromažďujú sa tieto polia:

  - Žiadne

#### <a name="officeextensibilityappcommandsaddsolution"></a>Office.Extensibility.AppCommands.AddSolution

Zhromažďuje informácie o inštalácii pre doplnky balíka Office, ktorými sa prispôsobuje pás s nástrojmi.  Používa sa na zisťovanie problémov s tým, ako vlastné doplnky upravujú pás s nástrojmi balíka Office.
 
Zhromažďujú sa tieto polia:

- **AppVersion** – verzia aplikácie

- **SolutionId** – ID riešenia

- **StoreType** – označuje pôvod aplikácie

- **TelemetryId** – ID telemetrie na základe prihlásenej identity


#### <a name="officeextensibilitycatalogexchangegetentitlements"></a>Office.Extensibility.Catalog.ExchangeGetEntitlements

Údaje o úspešnom a neúspešnom načítaní údajov nároku na doplnok pre doplnky priradené správcom nájomníka služieb Office 365. Slúžia na metriku stavu, grafy a analýzu problémov zákazníkov.

Zhromažďujú sa tieto polia:

  - **CachingResult** – výsledok pokusu o uloženie vrátenej hodnoty volania služby

  - **ClientParameter** – identifikátor klienta odoslaný počas volania služby

  - **EntitlementsCount** – počet nárokov očakávaných v odpovedi na volanie

  - **EntitlementsParsed** – počet nárokov analyzovaných z odpovede

  - **IsAllEntitlementsParsed** – označuje, či sa počet očakávaných nárokov zhoduje s analyzovaným počtom nárokov

  - **ServiceCallHResult** – výsledok vrátený rozhraním API volania služby

  - **TelemetryId** – identifikátor GUID predstavujúci jedinečného používateľa

  - **UsedCache** – označuje, či bol použitá odpoveď z vyrovnávacej pamäte namiesto volania služby

  - **VersionParameter** – číslo verzie balíka Office odoslané v rámci volania služby

#### <a name="officeextensibilitycatalogexchangegetlastupdate"></a>Office.Extensibility.Catalog.ExchangeGetLastUpdate

Údaje o úspešnom a neúspešnom načítaní potrebných aktualizovaných údajov o doplnkoch priradených správcom nájomníka služieb Office 365. Slúžia na metriku stavu, grafy a analýzu problémov zákazníkov. ExchangeGetLastUpdate sa spustí vždy pri štarte v rámci kódu hostiteľa a určí, či sa zmenili priradenia doplnku pre používateľa.  Ak áno, potom sa načíta osf.DLL, aby sme mohli volať ExchangeGetEntitlements a získať konkrétne priradenia (a ExchangeGetManifests sa zavolá, aby sa načítal každý nový manifest, ktorý bude potrebný).  ExchangeGetEntitlements (a ExchangeGetManifests) je možné tiež volať na požiadanie po spustení hostiteľskej aplikácie.  Cieľom je nenačítať veľkú knižnicu DLL, ak to nie je potrebné.  Bez toho, aby táto udalosť bola medzi povinnými údajmi, by nebolo možné zistiť, či sa používateľom nedarí získať im priradené doplnky, ak prvé volanie služby nie je úspešné.  Ide tiež o hlavný signál pre všetky problémy s overovaním, s ktorými sa stretávame, keď hovoríme so službou.

Zhromažďujú sa tieto polia:

  - **Abort** – označuje, či bol hostiteľ vypnutý počas volania služby

  - **AllowPrompt** – označuje, či bolo zapnuté zobrazovanie výziev na overenie

  - **AuthScheme** – schému overenia požadovaná serverom Exchange

  - **BackEndHttpStatus** – kód protokolu HTTP oznámený pri komunikácii so serverom Exchange

  - **BackupUrl** – sekundárna URL adresu servera Exchange na volanie

  - **BEServer** – názov servera Exchange

  - **CalculatedBETarget** – úplný názov počítača servera Exchange

  - **Call(n)\_TokenAuthError** – chyba overenia n-tého pokusu o volanie služby

  - **Call(n)\_TokenIsValid** – označuje, či bol overovací token platný pri n-tom pokuse o volanie služby

  - **CallMethod** – reťazec označujúci cestu, ktorou išiel kód

  - **ConfigSvcReady** – označuje, či služba konfigurácie už bola inicializovaná

  - **Date** – hodnota vrátená zo servera Exchange

  - **DiagInfo** – informácie vrátené zo servera Exchange

  - **End\_TicketAuthError** – každá chyba pri získavaní overovacieho lístka po volaní služby

  - **End\_TokenIsValid** – označuje, či je overovací lístok platný po volaní služby

  - **EndingIdentityState** – nahlásený stav objektov identity po uskutočnení volania služby

  - **EwsHandler** – hodnota vrátená zo servera Exchange

  - **FEServer** – klientske rozhranie servera Exchange, ktoré rieši žiadosť

  - **HResult** – kód výsledku

  - **HttpStatus** – kód stavu protokolu HTTP vrátený zo servera Exchange

  - **IsSupportedAuthResponse** – označuje, či typ overenia patrí medzi použiteľné

  - **LastUpdateValueRegistry** – hodnota hash načítaná z databázy Registry

  - **LastUpdateValueRetrieved** – hodnota hash vrátená z volania služby

  - **MSDiagnostics** – hodnota vrátená zo servera Exchange

  - **MsoHttpResult** – hodnota enumerátora vrátená z rozhrania API protokolu HTTP

  - **NeedRefresh** – pole s hodnotou true alebo false, ktoré označuje, či je údaj o doplnku zastaraný a je potrebné ho aktualizovať.

  - **PrimaryUrl** – hlavná URL adresa, na ktorú sa uskutočňuje volanie služby

  - **RequestId** – hodnota vrátená zo servera Exchange

  - **RequestTryCount** – počet našich pokusov o uskutočnenie volania služby

  - **RequestTryCount** – počet našich pokusov o komunikáciu so serverom Exchange

  - **ResultChain** – rad kódu výsledku z každého pokusu o volanie služby

  - **StartingIdentityState** – nahlásený stav objektov identity pred uskutočnením volania služby

  - **TelemetryId** – identifikátor GUID predstavujúci jedinečného používateľa, či je potrebné vykonať ďalšie volania služby

#### <a name="officeextensibilitycatalogexchangegetmanifests"></a>Office.Extensibility.Catalog.ExchangeGetManifests

Údaje o úspešnom a neúspešnom načítaní údajov manifestov doplnkov pre doplnky priradené správcom nájomníka služieb Office 365. Slúžia na metriku stavu, grafy a analýzu problémov zákazníkov.

Zhromažďujú sa tieto polia:

  - **CachedManifestsParsed** – počet manifestov nachádzajúcich sa vo vyrovnávacej pamäti

  - **IsAllReturnedManifestsParsed** – označuje, či bolo možné analyzovať všetky vrátené manifesty

  - **ManifestsRequested** – počet potrebných manifestov

  - **ManifestsReturned** – počet manifestov vrátených zo servera

  - **ManifestsToRetrieve** – počet manifestov, ktoré sa majú získať zo servera

  - **ReturnedManifestsParsed** – počet manifestov vrátených zo servera, ktoré boli úspešne analyzované

  - **TelemetryId** – identifikátor GUID predstavujúci jedinečného používateľa

#### <a name="officeextensibilityuxfensureloadosfdll"></a>Office.Extensibility.UX.FEnsureLoadOsfDLL 

Sleduje zlyhanie načítania Osf.DLL. Zisťuje neúspešne načítanú knižnicu DLL, ktorá bráni spusteniu funkcie.

Zhromažďujú sa tieto polia:

  - Žiadne

#### <a name="officeextensibilityuxfensureloadosfuidll"></a>Office.Extensibility.UX.FEnsureLoadOsfUIDLL 

Sleduje zlyhanie načítania OsfUI.DLL. Zisťuje neúspešne načítanú knižnicu DLL, ktorá bráni spusteniu funkcie.

Zhromažďujú sa tieto polia:

  - Žiadne

#### <a name="officeextensibilityuxfensureosfshareddllload"></a>Office.Extensibility.UX.FEnsureOsfSharedDLLLoad 

Sleduje zlyhanie načítania OsfShared.DLL. Zisťuje neúspešne načítanú knižnicu DLL, ktorá bráni spusteniu funkcie.

Zhromažďujú sa tieto polia:

  - Žiadne

#### <a name="officeextensibilityvbatelemetrycomobjectinstantiated"></a>Office.Extensibility.VBATelemetryComObjectInstantiated

Zhromažďuje informácie o vyvolaní automatizačného servera alebo klienta v riešeniach VBA. Umožňuje pochopiť interakciu medzi VBA a objektami COM

Zhromažďujú sa tieto polia:

  - **ComObjectInstantiatedCount** – počet inštancií objektov COM

  - **HashComObjectInstantiatedClsid** – hodnota hash identifikátora triedy objektu COM

  - **HashProjectName** – hodnota hash názvu projektu VBA

  - **TagId** – jedinečná značka

#### <a name="officeextensibilityvbatelemetrydeclare"></a>Office.Extensibility.VBATelemetryDeclare 

Zhromažďuje informácie o vyvolaní rozhraní API Win32 v riešeniach VBA. Umožňuje pochopiť interakciu medzi VBA a používaním a doplniť vyšetrovania zabezpečenia.

Zhromažďujú sa tieto polia:

  - **DeclareCount** – počet deklarácií

  - **HashDeclare** – hodnota hash názvu knižnice DLL

  - **HashEntryPoint** – hodnota hash názvu rozhrania API

  - **HashProjectName** – hodnota hash názvu projektu VBA

  - **IsPtrSafe** – označuje, či je vyhlásenie deklarácie kompatibilné s inou architektúrou

  - **TagId** – jedinečná značka

#### <a name="officeoutlookdesktopadd-insadd-inloaded"></a>Office.Outlook.Desktop.Add-ins.Add-inLoaded

Zhromažďuje informácie o úspešnom a neúspešnom načítaní doplnku v Outlooku. Tieto údaje sú aktívne monitorované, aby Outlook správne fungoval s doplnkami zákazníkov. Tieto údaje sa používajú na zistenie a vyšetrovanie problémov.

Zhromažďujú sa tieto polia:

  - **Štandardná aktivita HVA** bez vlastnej údajovej časti

#### <a name="officeoutlookmacaddinapiusage"></a>Office.Outlook.Mac.AddinAPIUsage

Zhromažďuje informácie o úspešných a neúspešných spusteniach doplnku v Outlooku. Tieto údaje sú aktívne monitorované, aby Outlook fungoval s doplnkami správne. Tieto údaje sa používajú na zistenie a vyšetrovanie problémov.

Zhromažďujú sa tieto polia:

- **AccountType** – typ konta priradeného k doplnku 

- **Cookie** – súbor cookie, ktorý je používaný doplnkom

- **DispId** – identifikátor odoslania 

- **EndTime** – čas skončenia doplnku 

- **ExecutionTime** – čas uplynutý počas spustenia doplnku 

- **Výsledok** – výsledok použitia doplnku v Outlooku 

- **StartTime** – čas spustenia doplnku


#### <a name="officeoutlookmacaddineventapisusage"></a>Office.Outlook.Mac.AddinEventAPIsUsage

Zhromažďuje informácie o úspešných alebo neúspešných spusteniach doplnku v Outlooku. Tieto údaje sú aktívne monitorované, aby Outlook fungoval s doplnkami správne. Tieto údaje sa používajú na zistenie a vyšetrovanie problémov.

Zhromažďujú sa tieto polia:

- **AddinType** – typ doplnku 

- **EventAction** – akcia vykonaná doplnkom 

- **EventDispid** – identifikátor odoslania

- **EventResult** – výsledok akcie vykonanej doplnkom 

#### <a name="officeoutlookmacaddininstallationfrominclientstore"></a>Office.Outlook.Mac.AddInInstallationFromInClientStore

Zhromažďuje informácie o úspešných alebo neúspešných inštaláciách doplnku v Outlooku. Tieto údaje sú aktívne monitorované, aby Outlook fungoval s doplnkami správne. Tieto údaje sa používajú na zistenie a vyšetrovanie problémov.

Zhromažďujú sa tieto polia:

- **AccountType** – typ konta priradeného k doplnku 

- **FailureReason** – dôvod zlyhania inštalácie doplnku 

- **MarketplaceAssetId** – identifikátor obchodu s doplnkami 

- **Status** – stav inštalácie doplnku


#### <a name="officeprogrammabilityadd-insinternalsetconnectenterprise"></a>Office.Programmability.Add-ins.InternalSetConnectEnterprise

Udalosť vygenerovaná pri načítaní doplnku COM v zariadení Enterprise. Desktop Analytics: načítania v počte \# sa použijú ako menovateľ na výpočet stavu (zlyhania \#/načítania \#) pri výpočte metriky stavu pre okruhy Pilot a Production v podnikových scenároch. Vyžaduje si to, aby údaje boli presné, nie vzorkované, keďže počet zariadení je nižší (100 až 1000).

Zhromažďujú sa tieto polia:

  - **Add-inconnectFlag** – aktuálne správanie pri načítaní

  - **Add-inDescription** – popis doplnku

  - **Add-inFileName** – názov súboru doplnku bez cesty k súboru

  - **Add-inFriendlyName** – popisný názov doplnku

  - **Add-inId** – ID triedy doplnku

  - **Add-inProgId** – ID programu doplnku

  - **Add-inProvider** – poskytovateľ doplnku

  - **Add-inTimeDateStamp** – časová pečiatka doplnku z metaúdajov knižnice DLL

  - **Add-inVersion** – verzia doplnku

#### <a name="officevisiovisioaddonload"></a>Office.Visio.Visio.AddonLoad

Zaznamenáva chyby, keď riešenie zlyhá pri načítavaní. Potrebné pri ladení chýb načítania doplnku vo Visiu.

Zhromažďujú sa tieto polia:

  - **Data\_Load1Error:integer** – hodnotu chyby počas načítania doplnku Visia

#### <a name="officevisiovisioaddonusage"></a>Office.Visio.Visio.AddonUsage

Zaznamenáva chyby v prípade chyby vo funkčnosti riešenia. Potrebné pri ladení chýb načítania doplnku v doplnkoch.

Zhromažďujú sa tieto polia:

  - **Data\_DocumentSessionLogID:string** – identifikátor relácie dokumentu

  - **Data\_IsEnabled**:**bool** – hodnota true, ak je riešenie povolené

  - **Data\_TemplateID:string** – identifikátor GUID šablóny, v ktorej sa načítalo riešenie. Záznam 0 pre vlastné riešenie

  - **Data\_AddOnID**:**string** – identifikátor GUID na identifikáciu načítaného doplnku

  - **Data\_Error**:**integer** – ID chyby

### <a name="security-subtype"></a>*Podtyp zabezpečenia*

Chybové stavy dokumentu, funkcie a doplnku, ktoré môže ohroziť zabezpečenie, vrátane pripravenosti na aktualizáciu produktu.

#### <a name="officesecurityactivationfilterclsidactivated"></a>Office.Security.ActivationFilter.CLSIDActivated

Sleduje, kedy sa konkrétny identifikátor triedy (Flash, Silverlight atď.) aktivuje v Office. Umožňuje sledovať vplyv blokovania ovládacích prvkov Flash, Silverlight a Shockwave na koncových používateľov.

Zhromažďujú sa tieto polia:

  - **ActivationType** – typ aktivácie ovládacieho prvku

  - **Blocked** – označuje, či bol ovládací prvok zablokovaný balíkom Office

  - **CLSID** – identifikátor triedy ovládacieho prvku

  - **Count** – označuje, koľkokrát bol ovládací prvok aktivovaný

#### <a name="officesecurityactivationfilterfailedtoregister"></a>Office.Security.ActivationFilter.FailedToRegister

Sleduje chyby v obmedzení rizík zabezpečenia, ktoré blokuje aktiváciu nebezpečných ovládacích prvkov v Office.

Umožňuje diagnostiku chýb v obmedzení rizík zabezpečenia, ktoré môžu mať vplyv na zabezpečenie koncových používateľov.

Zhromažďujú sa tieto polia:

  - Žiadne

#### <a name="officesecuritycomsecurityfileextensionlistfromservice"></a>Office.Security.ComSecurity.FileExtensionListFromService

Sleduje, či boli prečítané prípony blokovania balíčkovača v službe konfigurácie alebo bol použitý predvolený zoznam klienta. Umožňuje zabezpečiť efektivitu obmedzenia rizík zabezpečenia, ktoré chráni koncových používateľov balíka Office.

Zhromažďujú sa tieto polia:

  - **RetrievedFromServiceStatus** – označuje, či sa načítal zoznam prípon súborov, ktoré sa majú blokovať, a ak nie, čo bolo dôvodom chyby

#### <a name="officesecuritycomsecurityload"></a>Office.Security.ComSecurity.Load

Sleduje, keď sa načíta objekt OLE v dokumente. Umožňuje zabezpečiť efektivitu obmedzenia rizík zabezpečenia, ktoré chráni koncových používateľov balíka Office.

Zhromažďujú sa tieto polia:

  - **Clsid** – identifikátor triedy ovládacieho prvku OLE

  - **Count** – označuje, koľkokrát bol načítaný ovládací prvok OLE

  - **DocUrlHash** – hodnota hash predstavujúca dokument jednoznačne. (Poznámka: Skutočné podrobnosti o dokumente sa z tohto nedajú zistiť žiadnym spôsobom. Ide len o jedinečné označenie dokumentu.)

  - **IsCategorized** – označuje, či bol ovládací prvok OLE kategorizovaný na načítanie v Office

  - **IsInsertable** – označuje, či je ovládací prvok OLE vložiteľný alebo nie

#### <a name="officesecuritycomsecurityobjdetected"></a>Office.Security.ComSecurity.ObjDetected

Sleduje, keď sa zistí objekt OLE v dokumente. Umožňuje zabezpečiť efektivitu obmedzenia rizík zabezpečenia, ktoré chráni koncových používateľov balíka Office.

Zhromažďujú sa tieto polia:

  - **Clsid** – identifikátor triedy ovládacieho prvku OLE

  - **Count** – koľkokrát bol tento objekt OLE zistený

  - **DocUrlHash** – hodnota hash predstavujúca dokument jednoznačne. (Poznámka: Skutočné podrobnosti o dokumente sa z tohto nedajú zistiť žiadnym spôsobom. Ide len o jedinečné označenie dokumentu.)

  - **IsCategorized** – označuje, či je ovládací prvok OLE kategorizovaný na načítanie v Office

  - **IsInsertable** – označuje, či je ovládací prvok OLE vložiteľný alebo nie

#### <a name="officesecuritycomsecuritypackageractivation"></a>Office.Security.ComSecurity.PackagerActivation

Sleduje výsledok obmedzenia rizík zabezpečenia, ktoré blokuje nebezpečné prípony vložené v dokumentoch balíka Office. Umožňuje zabezpečiť efektivitu obmedzenia rizík zabezpečenia, ktoré chráni koncových používateľov balíka Office.

Zhromažďujú sa tieto polia:

  - **FromInternet** – označuje, či bol dokument z internetu

  - **PackagerSetting** – označuje, aké bolo aktuálne nastavenie balíčkovača

  - **TrustedDocument** – označuje, či bol dokument dôveryhodným dokumentom

#### <a name="officesecuritycomsecuritypackageractivationerrors"></a>Office.Security.ComSecurity.PackagerActivationErrors

Sleduje chyby v obmedzení rizík zabezpečenia, ktoré blokuje nebezpečné prípony vložené v dokumentoch balíka Office. Umožňuje zabezpečiť efektivitu obmedzenia rizík zabezpečenia, ktoré chráni koncových používateľov balíka Office.

Zhromažďujú sa tieto polia:

  - **Error** – kód chyby

  - **Extension** – označuje, aká bola prípona súboru

  - **FromInternet** – označuje, či bol dokument z internetu

  - **LinkedDocument** – označuje, či to bol alebo nebol prepojený dokument

  - **PackagerSetting** – označuje, aké bolo aktuálne nastavenie balíčkovača

  - **TrustedDocument** – označuje, či bol dokument dôveryhodný


#### <a name="officesecuritymacrointernetvbablockenabled"></a>Office.Security.Macro.InternetVBABlockEnabled

Sleduje, či je v klientovi zapnuté nastavenia blokovania makra z internetu. Slúži na vyhodnotenie použitia obmedzenia rizík zabezpečenia na ochranu pred škodlivými makrami.

Zhromažďujú sa tieto polia:

  - Žiadne

#### <a name="officesecuritymacropolicydigsigtrustedpublishers"></a>Office.Security.Macro.PolicyDigSigTrustedPublishers

Sleduje, či bolo makro overené a pochádza od dôveryhodného vydavateľa. Umožňuje zabezpečiť efektivitu obmedzenia rizík zabezpečenia, ktoré chráni koncových používateľov balíka Office.

Zhromažďujú sa tieto polia:

  - **Policy** – označuje, či politika je alebo nie je nastavená, alebo nie je k dispozícii

#### <a name="officesecuritymacroprompted"></a>Office.Security.Macro.Prompted

Sleduje, keď sa používateľovi zobrazí výzva na povolenie makier VBA. Umožňuje vyhodnotiť výskyt makier VBA a zavádzať budúce obmedzenia rizík zabezpečenia, ktoré obmedzia spustenia makier v rámci odozvy na incidenty zabezpečenia.

Zhromažďujú sa tieto polia:

  - **PromptType** – označuje, aký typ výzvy sa zobrazil

  - **VBAMacroAntiVirusHash** – antivírusová hodnota hash makra

  - **VBAMacroAntiVirusHRESULT** – výsledok antivírusového hodnotenia

#### <a name="officesecuritymacrovbasecureruntimesessionenablestate"></a>Office.Security.Macro.VBASecureRuntimeSessionEnableState

Sleduje každé overenie režimu Runtime AMSI, ktoré sa uskutoční pri spustení makra. Sleduje efektivitu overenia režimu Runtime AMSI pri spustení makra a identifikuje chyby, ktoré môžu mať vplyv na zabezpečenie koncových používateľov.

Zhromažďujú sa tieto polia:

  - **IsRegistry** – označuje, či správca nastavil nejaké prepisovanie v databáze Registry

  - **State** – označuje, aký je stav zabezpečenia režimu Runtime

#### <a name="officesecuritymacroxl4prompted"></a>Office.Security.Macro.XL4Prompted

Sleduje, keď sa používateľovi zobrazí výzva na povolenie makier XL4. Umožňuje vyhodnotiť výskyt makier XL4 v Exceli a zavádzať budúce obmedzenia rizík zabezpečenia, ktoré predvolene blokujú XL4 v rámci odozvy na incidenty zabezpečenia, ktoré sa týkajú zneužitia makier XL4.

Zhromažďujú sa tieto polia:

  - **PromptType** – označuje, aký typ výzvy sa zobrazil


#### <a name="officesecurityocxufiprompt"></a>Office.Security.OCX.UFIPrompt

Sleduje, keď sa používateľovi zobrazí upozornenie zabezpečenia pri načítaní ovládacieho prvku ActiveX, ktorý je označený ako nebezpečný na inicializáciu. Umožňuje sledovať výskyt ovládacích prvkov UFI ActiveX v dokumentoch balíka Office a zavádzať obmedzenia rizík (napr. ovládacie prvky Killbitting) v rámci odozvy na incidenty zabezpečenia.

Zhromažďujú sa tieto polia:

  - **IsFromInternet** – označuje, či je dokument otvorený z internetu

  - **IsSecureReaderMode** – označuje, či je dokument otvorený v zabezpečenej čítačke

  - **OcxTrustCenterSettings** – označuje, aké je aktuálne nastavenie technológie ActiveX


#### <a name="officesecuritysecurereaderhostopeninosr"></a>Office.Security.SecureReaderHost.OpenInOSR

Sleduje dokončenie otvorenia súboru v chránenom zobrazení. Umožňuje diagnostiku podmienok, ktoré vedú k zlyhaniu pri otváraní súborov v chránenom zobrazení, čo má vplyv na zabezpečenie a produktivitu zákazníkov.

Zhromažďujú sa tieto polia:

  - Žiadne

## <a name="product-and-service-usage-data-events"></a>Udalosti v kategórii Údaje o používaní produktov a služieb

Toto sú podtypy údajov v tejto kategórii:

- [Úspešnosť funkcie aplikácie](#application-feature-success-subtype)
- [Stav a spustenie aplikácie](#application-status-and-boot-subtype)
- [Konfigurácia zjednodušenia ovládania balíka Office](#office-accessibility-configuration-subtype)
- [Ochrana osobných údajov](#privacy-subtype)


### <a name="application-feature-success-subtype"></a>*Podtyp Úspešnosť funkcie aplikácie*

Úspešnosť fungovania aplikácie. Obmedzené na otvorenie a zatvorenie aplikácie a dokumentov, úpravu súborov a zdieľanie súborov (spoluprácu).

#### <a name="officeappcompatappcompatagentupload"></a>Office.AppCompat.AppCompat.AgentUpload

Generuje sa pri spustení klienta, ak koncový používateľ povolil tabuľu telemetrie balíka Office.  Zhromažďuje informácie o tom, kedy agent telemetrie balíka Office nahral údaje do priečinka na zdieľanie. Primárnym využítím tejto udalosti je monitorovanie stavu agenta telemetrie balíka Office a jej druhotným využitím je odhad používania tabule telemetrie balíka Office.

Zhromažďujú sa tieto polia:

- **UploadTime** – časová pečiatka posledného úspešného nahrávania vykonaného agentom telemetrie.


#### <a name="officeappcompatappcompatagentscanandupload"></a>Office.AppCompat.AppCompat.AgentScanAndUpload

Zhromažďuje sa len vtedy, ak koncový používateľ povolil tabuľu telemetrie balíka Office. Zhromažďuje informácie o tom, kedy sa spustil agent telemetrie balíka Office.  Tieto údaje sa zhromažďujú len vtedy, ak je tabuľa telemetrie balíka Office povolená a používa sa na určenie stavu agenta telemetrie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data.AgentExit** – časová pečiatka toho, keď je agent telemetrie úspešne ukončený

  - **Data.AgentScan** – časová pečiatka toho, keď agent telemetrie úspešne dokončil sken

  - **Data.AgentUpload** – časová pečiatka toho, keď agent telemetrie úspešne dokončil nahratie

#### <a name="officeappcompatappcompattelemetrydashboardresiliencycrashlog"></a>Office.AppCompat.AppCompat.TelemetryDashboardResiliencyCrashLog

Zhromažďuje sa len vtedy, ak koncový používateľ (s najväčšou pravdepodobnosťou správca) povolil tabuľu telemetrie balíka Office. Zhromažďuje informácie o výskyte zlyhaní doplnkov a dokumentov balíka Office. Tieto údaje sa zhromažďujú len vtedy, ak používateľ povolil tabuľu telemetrie balíka Office a používa sa na určenie toho, či dochádza k zvýšenému výskytu zlyhaní doplnkov alebo dokumentov.

Zhromažďujú sa tieto polia:

  - **Data.CollectionTime** – časová pečiatka toho, kedy sa zaznamenala udalosť zlyhania

#### <a name="officeconnectdeviceactivitystart"></a>Office.ConnectDevice.Activity.Start

Umožňuje zistiť, či pripojenie k zariadeniu alebo aplikácii bolo úspešné.  Umožňuje sledovanie stavu funkcie a monitorovanie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Datasource_Type** -informácia o sériovom zariadení alebo službe aplikácie

- **DataSource_Name** – názov pripojeného zdroja údajov

- **Activity_Name** – názov aktivity „ConnectDevice“

- **Activity_CV** – ID na koreláciu udalostí počas relácie pripojenia

- **Activity_StartStopType** – spustenie

- **Activity_DateTimeTicks** – dátum a čas aktivity
 
#### <a name="officeconnectdeviceactivitystop"></a>Office.ConnectDevice.Activity.Stop

Umožňuje zistiť, či pripojenie k zariadeniu alebo aplikácii bolo úspešné. Umožňuje sledovanie stavu a monitorovanie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Datasource_Type** -informácia o sériovom zariadení alebo službe aplikácie

- **DataSource_Name** – názov pripojeného zdroja údajov

- **Activity_Name** – názov aktivity „ConnectDevice“

- **Activity_CV** – ID na koreláciu udalostí počas relácie pripojenia

- **Activity_StartStopType** – zastavenie

- **Activity_DateTimeTicks** – dátum a čas aktivity

#### <a name="officeextensibilitycatalogexchangeprocessentitlement"></a>Office.Extensibility.Catalog.ExchangeProcessEntitlement

Údaje o spracovaní individuálneho nároku na doplnok priradený správcom nájomníka služieb Office 365.

Používajú sa pri vytváraní grafov (požadovaných manažmentom tímu) úspešnosti zákazníkov a analýzy problémov zákazníkov.

Zhromažďujú sa tieto polia:

  - **AppVersion** – verzia hosťujúcej aplikácie doplnku.

  - **SolutionId** – identifikátor GUID predstavujúci jedinečný doplnok

  - **TelemetryId** – identifikátor GUID predstavujúci jedinečného používateľa

#### <a name="officeextensibilitycatalogexchangeprocessmanifest"></a>Office.Extensibility.Catalog.ExchangeProcessManifest

Údaje o spracovaní individuálneho manifestu doplnku priradeného správcom nájomníka služieb O365. Používa sa na analýzu problémov zákazníkov a vytváranie grafov úspešnosti zákazníka.
 
Zhromažďujú sa tieto polia:

- **AppVersion** – verzia aplikácie

- **IsAllReturnedManifestsParsed** – logická hodnota označujúca, že sme analyzovali všetky vrátené manifesty

- **IsAppCommand** – logická hodnota označujúca, či ide o príkaz aplikácie 

- **ReturnedManifestsParsed** – počet analyzovaných manifestov

- **SolutionId** – ID riešenia

- **TelemetryId** – ID telemetrie na základe prihlásenej identity

#### <a name="officeextensibilityodpappcommandsribbonclick"></a>Office.Extensibility.ODPAppCommandsRibbonClick

Zhromažďuje informácie o tom, či kliknutie na vlastný ovládacví prvok doplnku bolo úspešné alebo nie. Používa sa na zisťovanie problémov v interakcii používateľa s ovládacími prvkami doplnku.
 
Zhromažďujú sa tieto polia:

- **CommandActionType** – typ príkazu doplnku

- **CommandLabel** – označenie príkazu, na ktorý sa kliklo

- **SolutionId** – ID riešenia

#### <a name="officefileiocsiccachedfilecsiloadfilebasic"></a>Office.FileIO.CSI.CCachedFileCsiLoadFileBasic

Umožňuje zistiť, či sa súbor úspešne otvoril z vrstvy FIO. Umožňuje sledovanie stavu funkcie a monitorovanie.

Zhromažďujú sa tieto polia:

  - **Activity.Group** – značka, ktorá umožňuje zoskupiť množinu udalostí monitorovania a spravovať celkovú úspešnosť

  - **Activity.IsHVA** – príznak, ktorý označuje, že udalosť je kritická pre úspešnosť používateľa

  - **Data.AsyncOpen** – príznak, ktorý označuje otvorený obsah, ktorý prišiel po otvorení hlavnej časti

  - **Data.CacheFileId** – pripája sa k telemetrii vyrovnávacej pamäte dokumentov balíka Office a umožňuje analýzu vplyvu problémov s vyrovnávacou pamäťou na prostredie používateľa

  - **Data.CoauthStatus** – hlási stav spolupráce v rámci dokumentu pri otvorení

  - **Data.CountOfMultiRoundTripsDownload** – počet výmen údajov na serveri, ktoré sa používajú na riešenie problémov s výkonom a sieťou

  - **Data.CountOfMultiRoundTripsUpload** – počet výmen údajov na serveri, ktoré sa používajú na riešenie problémov s výkonom a sieťou

  - **Data.DialogId** – nastaví sa, ak sa zobrazí dialógové okno používateľského rozhrania počas otvorenia s informáciou, že používateľovi sa zobrazila správa s upozornením

  - **Data.DidFallbackToDAV** – nastaví sa, ak bol dokument otvorený pomocou staršieho protokolu prenosu súborov

  - **Data.Doc.AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť

  - **Data.Doc.AssistedReadingReasons** – nastaví sa, ak je v dokumente zavedená ochrana elektronických údajov

  - **Data.Doc.ChunkingType** – jednotky slúžiace na prírastkové otvorenie dokumentu

  - **Data.Doc.EdpState** – nastavenie ochrany elektronických údajov dokumentu

  - **Data.Doc.Ext** prípona dokumentu (docx, xlsb, pptx atď.)

  - **Data.Doc.Extension** – zastarané

  - **Data.Doc.FileFormat** – verzia protokolu formátu súboru

  - **Data.Doc.Fqdn** – názov domény OneDrivu alebo SharePointu Online

  - **Data.Doc.FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény

  - **Data.Doc.IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia

  - **Data.Doc.IdentityUniqueId** – zastarané

  - **Data.Doc.InitializationScenario** – zaznamenáva, ako bol dokument otvorený

  - **Data.Doc.IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky

  - **Data.Doc.IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa

  - **Data.Doc.IsCloudCollabEnabled** – príznak, ktorý označuje, že služba podporuje spoluprácu v cloude

  - **Data.Doc.IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo

  - **Data.Doc.IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce

  - **Data.Doc.IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline

  - **Data.Doc.IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu

  - **Data.Doc.Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.)

  - **Data.Doc.LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument

  - **Data.Doc.NumberCoAuthors** – počet používateľov v relácii spoločných úprav

  - **Data.Doc.PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie

  - **Data.Doc.ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie

  - **Data.Doc.ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov

  - **Data.Doc.ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov

  - **Data.Doc.ServerProtocol** – verzia protokolu použitá na komunikáciu so službou

  - **Data.Doc.ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.)

  - **Data.Doc.ServerVersion** – verzia servera, ktorý ponúka službu

  - **Data.Doc.SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie

  - **Data.Doc.SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online

  - **Data.Doc.SizeInBytes** – indikátor veľkosti dokumentu

  - **Data.Doc.SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu

  - **Data.Doc.StorageProviderId** – zastarané

  - **Data.Doc.StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý

  - **Data.Doc.SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby)

  - **Data.Doc.UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu

  - **Data.Doc.UsedWrsDataOnOpen** – diagnostický indikátor prírastkového otvorenia dokumentu

  - **Data.Doc.WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI

  - **Data.DocumentLoadEndpoint** – zastaraný/redundantný duplikát (Data.Doc.Location a Data.Doc.IsSyncbacked)

  - **Data.DocumentSizeInBytes** – zastarané/redundantné, náhrada je Data.Doc. SizeInBytes

  - **Data.DocumentSizeOnDisk** – zastarané

  - **Data.DoesBaseHaveContentOnOpen** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.DoesWorkingBranchHaveExcludedDataOnOpen** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.DownloadFragmentSize** – veľkosť údajov odoslaných v podradenej požiadavke na diagnostiku problémov so sieťou

  - **Data.DsmcStartedTooEarly** – označuje chybu pri začatí relácie spoločných úprav

  - **Data.EditorsCount** – počet ostatných spolupracovníkov upravujúcich dokument

  - **Data.ExcludedDataThresholdInBytes** – veľkosť súboru potrebná na použitie asynchrónneho otvorenia

  - **Data.FileIOResult.Code** – vyrovnávacia pamäť vráteného kódu posledného otvorenia z vrstvy protokolu

  - **Data.FileIOResult.Success** – vyrovnávacia pamäť indikátora úspešnosti posledného otvorenia z vrstvy protokolu

  - **Data.FileIOResult.Tag** – vyrovnávacia pamäť značky chyby posledného otvorenia z vrstvy protokolu

  - **Data.FileIOResult.Type** – vyrovnávacia pamäť typu chyby posledného otvorenia z vrstvy protokolu

  - **Data.FqdnHash** – zastarané, náhrada je Data\_Doc\_FqdnHash

  - **Data.FullIError** – vyrovnávacia pamäť kódov všetkých chýb otvorení z vrstvy protokolu

  - **Data.FullyQualifiedDomainName** – zastarané, náhrada je Data\_Doc\_Fqdn

  - **Data.Input.FileOpenState** – stav požadovaný aplikáciou (Na čítanie alebo Na čítanie a zapisovanie atď.) **-**

  - **Data.Input.OpenAsync** – asynchrónne otvorenie požadované aplikáciou

  - **Data.Input.OpenOfflineCopy** – otvorenie z kópie v režime offline požadované doplnkom

  - **Data.IOFlags** – zastarané

  - **Data.IsBaseBranchEmptyOnOpen** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.IsCachedHistoricalVersion** – vyrovnávacia pamäť obsahuje staršiu verziu dokumentu

  - **Data.IsDocEnterpriseProtected** – dokument je chránený pomocou šifrovania (ochrana elektronických dokumentov/EDP)

  - **Data.IsDocInODC** – dokument bol otvorený ešte predtým a už je vo vyrovnávacej pamäti

  - **Data.IsMapUnMapCase** – súčasť stavu súboru vo vyrovnávacej pamäti

  - **Data.IsMapUnMapCase.End** – súčasť stavu súboru vo vyrovnávacej pamäti

  - **Data.IsOfficeHydrationInProgress** – dokument je obnovený z offline ukladacieho priestoru v systéme Windows

  - **Data.isOfficeHydrationRequired** – dokument je momentálne v offline ukladacom priestore

  - **Data.isOpenFromCollab** – najnovšia kópia dokumentu sa načítala zo zdieľanej služby spolupráce

  - **Data.isPendingNameExist** – prebieha premenovanie dokumentu

  - **Data.IsStubFile** – dokument ešte nebol uložený v cloudovej službe

  - **Data.IsSyncBackedStateDifferentThanOnLastOpen** – zmenil sa stav dokumentu a zmeny možno nastali, kým dokument nebol otvorený

  - **Data.isTaskCanceledAfterOpenComplete** – zastarané

  - **Data.IsWorkingBranchAvailableOnOpen** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.LicenseStatus** – stav licencie na diagnostický produkt, používa sa na overenie, že príslušné funkcie produktu sú povolené pre typ licencie používateľa 

  - **Data.LicenseType** – označuje stav licencie (bezplatná, platená, skúšobná atď.)

  - **Data.Location** – označuje typ úložného média (USB, Cloud atď.)

  - **Data.LockRequestDocMode** – označuje, či je dokument k dispozícii ostatným používateľom

  - **Data.MyDeferredValue** – zastarané

  - **Data.Network.BytesReceived** – zastarané

  - **Data.Network.BytesSent** – zastarané

  - **Data.Network.ConnectionsCreated** – zastarané

  - **Data.Network.ConnectionsEnded** – zastarané

  - **Data.OcsDisableReasons** – dôvod, prečo nebola pre dokument k dispozícii zdieľaná služba spolupráce

  - **Data.OcsHostOnOpen** – príznak, ktorý označuje, že ovládací prvok sa prepne na zdieľanú službu spolupráce počas otvorenia

  - **Data.OpeningOfflineCopy** – príznak, ktorý označuje, že sa otvorí lokálna kópia dokumentu

  - **Data.Partition** – zastarané

  - **Data.RequestTime** – zastarané

  - **Data.ResourceIdHash** – zastarané

  - **Data.ResumedIncrementalOpen** – zastarané

  - **Data.RTCEnabled** – spustil sa protokol rýchlej distribúcie zmien

  - **Data.SaveOnOpen** – neuložené zmeny v lokálnom dokumente sa uložili v službe počas otvorenia

  - **Data.ServerProtocol** – zastarané, náhrada je Data\_Doc\_ServerProtocol

  - **Data.ServerType** – zastarané, náhrada je Data\_Doc\_ServerType

  - **Data.ServerVersion** – zastarané, náhrada je Data\_Doc\_ServerVersion

  - **Data.ServiceId** – zastarané, náhrada je Data\_Doc\_WopiServiceId

  - **Data.SessionId** – zastarané

  - **Data.ShouldSwitchToServerOnly** – lokálnu kópiu dokumentu nie je možné použiť, je nutné použiť serverovú verziu

  - **Data.SpecialChars** – zastarané

  - **Data.StopwatchDuration** – zastarané

  - **Data.SyncBackedFileTelemetrySessionId** – zastarané

  - **Data.SyncElapsedTime** – zastarané

  - **Data.SyncRequestId** – zastarané

  - **Data.TestProperty** – zastarané

  - **Data.TransitionToHostOnOpen** – príznak, ktorý označuje, že relácia sa pripojí k službe, ktorá je hostiteľom dokumentu

  - **Data.TransitionToHostOnOpenResult** – stav prechodu na hostiteľskú službu

  - **Data.UseCachedNetworkConnection** – príznak, ktorý označuje, či sa pripojenie použilo opakovane alebo sa vytvorilo nové pripojenie

  - **Data.UseClientIdAsSchemaLockId** – príznak na kontrolu, ako sú dokumenty v službe uzamknuté

  - **Data.WopiServiceId** – zastarané, náhrada je Data\_Doc\_WopiServiceId

#### <a name="officefileiocsiccachedfilecsisavefilebasic"></a>Office.FileIO.CSI.CCachedFileCsiSaveFileBasic

Umožňuje zistiť, či sa súbor úspešne uložil z vrstvy FIO. Umožňuje sledovanie stavu funkcie a monitorovanie.

Zhromažďujú sa tieto polia:

  - **Activity.Group** – značka, ktorá umožňuje zoskupiť množinu udalostí monitorovania a spravovať celkovú úspešnosť

  - **Activity.IsHVA** – príznak, ktorý označuje, že udalosť je kritická pre úspešnosť používateľa

  - **Data.AsyncOpen** – príznak, ktorý označuje, že dokument bol otvorený s obsahom, ktorý prišiel po otvorení hlavnej časti

  - **Data.BaseDownloadTriggered** – diagnostické sledovanie zmien, ktoré označuje, že bola požadovaná základná verzia dokumentu

  - **Data.BlockAutoUploadReasons** – kódy príčin stavu blokovania nahrávania (napr. je vypnuté automatické ukladanie, dokument je v prechode)

  - **Data.BlockUploadDueToFailedSaveAsOverExisting** – nahrávanie sa zablokuje, keď zlyhalo pri opakovanom pokuse

  - **Data.CacheFileId** – pripája sa k telemetrii vyrovnávacej pamäte dokumentov balíka Office a umožňuje analýzu vplyvu problémov s vyrovnávacou pamäťou na prostredie používateľa

  - **Data.ChartType** – zastarané

  - **Data.CoAuthStatus** – hlási stav spolupráce v rámci dokumentu pri uložení

  - **Data.CoauthUpdatesContext** – hlási kontext (zlúčenie/prírastkové otvorenie)

  - **Data.CountOfMultiRoundTripsDownload** – počet výmen údajov na serveri, ktoré sa používajú na riešenie problémov s výkonom a sieťou

  - **Data.CountOfMultiRoundTripsUpload** – počet výmen údajov na serveri, ktoré sa používajú na riešenie problémov s výkonom a sieťou

  - **Data.DialogChoice** – zaznamenáva výber v každom dialógovom okne chyby

  - **Data.DialogId** – zaznamenáva ID dialógového okna každého dialógového okna chyby, ktoré sa zobrazí počas ukladania

  - **Data.Dmc.IsOcsSupported** – zastarané

  - **Data.Doc.AccessMode** – dokument je iba na čítanie

  - **Data.Doc.AssistedReadingReasons** – nastaví sa, ak je v dokumente zavedená ochrana elektronických údajov

  - **Data.Doc.ChunkingType** – jednotky slúžiace na prírastkové otvorenie dokumentu

  - **Data.Doc.EdpState** – nastavenie ochrany elektronických údajov dokumentu

  - **Data.Doc.Ext** – prípona dokumentu (docx, xlsm, pptx atď.)

  - **Data.Doc.Extension** – zastarané

  - **Data.Doc.FileFormat** – verzia protokolu formátu súboru

  - **Data.Doc.Fqdn** – názov domény OneDrivu alebo SharePointu Online

  - **Data.Doc.FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény

  - **Data.Doc.FqdnHasi** – zastarané

  - **Data.Doc.IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie uloženia

  - **Data.Doc.IdentityUniqueId** – zastarané

  - **Data.Doc.IKFlags** – zastarané

  - **Data.Doc.InitializationScenario** – zaznamenáva, ako bol dokument otvorený

  - **Data.Doc.IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky

  - **Data.Doc.IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa

  - **Data.Doc.IsCloudCollabEnabled** – príznak, ktorý označuje, že aplikácia podporuje spoluprácu v cloude

  - **Data.Doc.IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo

  - **Data.Doc.IsOcsSupported** – príznak, ktorý označuje, že dokument podporuje spoluprácu v cloude

  - **Data.Doc.IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline

  - **Data.Doc.IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu

  - **Data.Doc.Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.)

  - **Data.Doc.LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument

  - **Data.Doc.NumberCoAuthors** – počet používateľov v relácii spoločných úprav

  - **Data.Doc.PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie

  - **Data.Doc.ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie

  - **Data.Doc.ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov

  - **Data.Doc.ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov

  - **Data.Doc.ServerProtocol** – verzia protokolu použitá na komunikáciu so službou

  - **Data.Doc.ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.)

  - **Data.Doc.ServerVersion** – verzia servera, ktorý ponúka službu

  - **Data.Doc.SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie

  - **Data.Doc.SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online

  - **Data.Doc.SizeInBytes** – indikátor veľkosti dokumentu

  - **Data.Doc.SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu

  - **Data.Doc.StorageProviderId** – zastarané

  - **Data.Doc.StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý

  - **Data.Doc.SussionId** – zastarané

  - **Data.Doc.SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby)

  - **Data.Doc.UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu

  - **Data.Doc.UsedWrsDataOnOpen** – diagnostický indikátor prírastkového otvorenia dokumentu

  - **Data.Doc.WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI

  - **Data.DocnReadOnlyReasons** – zastarané

  - **Data.DocumentSaveEndpoint** – zastaraný, náhrada je Data\_Doc\_Location

  - **Data.DocumentSaveType** – typ uloženia (Normálne, Vytvoriť, Uložiť ako)

  - **Data.DocumentSizeOnDisk** – zastarané, náhrada je Data\_Doc\_SizeInBytes

  - **Data.DoesBaseHaveContentOnOpen** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.DoesWorkingBranchHaveExcludedDataOnOpen** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.DstDoc.AccessMode** – označuje, či je nový dokument iba na čítanie alebo sa dá upraviť

  - **Data.DstDoc.EdpState** – nastavenie ochrany elektronických údajov nového dokumentu

  - **Data.DstDoc.Extension** – prípona nového dokumentu (docx, xlsm, pptx atď.)

  - **Data.DstDoc.FileFormat** – protokol formátu súboru nového dokumentu

  - **Data.DstDoc.Fqdn** – názov domény nového dokumentu OneDrivu alebo SharePointu Online

  - **Data.DstDoc.FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény nového dokumentu

  - **Data.DstDoc.IdentityUniqueId** – zastarané

  - **Data.DstDoc.IOFlags** – príznaky možností vo vyrovnávacej pamäti nového dokumentu použité pri otvorení

  - **Data.DstDoc.IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia nového dokumentu v režime offline

  - **Data.DstDoc.IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu

  - **Data.DstDoc.Location** – označuje, ktorá služba poskytla nový dokument (OneDrive, súborový server, SharePoint atď.)

  - **Data.DstDoc.NumberCoAuthors** – počet používateľov v relácii spoločných úprav v novom dokumente

  - **Data.DstDoc.ReadOnlyReasons** – dôvody, prečo bol nový dokument otvorený iba na čítanie

  - **Data.DstDoc.ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov s novým dokumentom

  - **Data.DstDoc.ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov s novým dokumentom

  - **Data.DstDoc.ServerProtocol** – verzia protokolu použitá na komunikáciu so službou pri tvorbe nového dokumentu

  - **Data.DstDoc.ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.) pre nový dokument

  - **Data.DstDoc.ServerVersion** – verzia servera, ktorý ponúka službu pre nový dokument

  - **Data.DstDoc.SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie pre nový dokument

  - **Data.DstDoc.SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online pre nový dokument

  - **Data.DstDoc.SizeInBytes** – indikátor veľkosti nového dokumentu

  - **Data.DstDoc.UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu pre nový dokument

  - **Data.EditorsCount** – počet ostatných spolupracovníkov upravujúcich dokument

  - **Data.FullIError** – vyrovnávacia pamäť kódov všetkých chýb z vrstvy protokolu

  - **Data.HasFilteredCategories** – zastarané

  - **Data.HasFilteredCategoryNames** – zastarané

  - **Data.HasFilteredSeries** – zastarané

  - **Data.HasFilteredSeriesNames** – zastarané

  - **Data.HasPendingSaveAs** – označuje, že prebieha požiadavka Uložiť ako/Uložiť kópiu

  - **Data.Input.FileOpenState** – stav požadovaný aplikáciou (Na čítanie alebo Na čítanie a zapisovanie atď.)

  - **Data.Input.FileSaveState** – stav požadovaný aplikáciou (uloženie pri otvorení, uloženie pod iným názvom atď.)

  - **Data.Input.NetworkCost** – označuje typ nákladov na sieť (účtované podľa objemu údajov, účtované podľa objemu údajov nad limit atď.)

  - **Data.Input.OpenAsync** – príznak, ktorý označuje, že aplikácia požadovala asynchrónne otvorenie

  - **Data.Input.OpenOfflineCopy** – príznak, ktorý označuje, že aplikácia požadovala otvorenie offline

  - **Data.IsCachedHistoricalVersion** – označuje, že tento súbor vo vyrovnávacej pamäti nie je najnovšia verzia

  - **Data.IsHtml** – označuje, že bol vložený text vo formáte HTML

  - **Data.IsLegacyCode** – označuje, že bol vložený text vo formáte so starším kódom

  - **Data.IsLocalOnlyFile** – označuje, že súbor bol otvorený iba z lokálneho ukladacieho priestoru

  - **Data.IsLocalOrSyncBackedFile** – označuje, že súbor bol otvorený lokálne a priradený k službe

  - **Data.IsMapUnMapCase** – súčasť stavu súboru vo vyrovnávacej pamäti

  - **Data.isOpenFromCollab** – označuje, že súbor bol otvorený zo zdieľanej služby spolupráce

  - **Data.IsStubFile** – dokument ešte nebol zdieľaný v cloudovej službe

  - **Data.IsSyncBackedFile** – dokument sa nachádza v priečinku, ktorý je automaticky synchronizovane aktualizovaný

  - **Data.IsSyncBackedStateDifferentThanOnLastOpen** – zmenil sa stav dokumentu a zmeny možno nastali, kým dokument nebol otvorený

  - **Data.IsWorkingBranchAvailableOnOpen** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.Location** – označuje typ úložného média (USB, Cloud atď.)

  - **Data.LockRequestDocMode** – označuje, či je dokument k dispozícii ostatným používateľom

  - **Data.MruRequestResult** – zastarané

  - **Data.NewDataNotAvailableReason** – zastarané

  - **Data.OcsDisableReasons** – nepoužíva sa uložením

  - **Data.OcsHostOnOpen** – nepoužíva sa uložením

  - **Data.Output.FileSaveState** – stav pri dokončení uloženia

  - **Data.PivotChart** – zastarané

  - **Data.resolveConflictState** – kódy príčin požiadavky na vyriešenie konfliktov zlúčenia

  - **Data.RTCEnabled** – spustil sa protokol rýchlej distribúcie zmien

  - **Data.SaveAsToCurrent** – označuje, že aktívny dokument prepíše uložený súbor

  - **Data.ServiceId** – zastarané, náhrada je Data\_Doc\_WopiServiceId

  - **Data.SessionId** – zastarané

  - **Data.SizeInBytes** – zastarané, náhrada je Data\_Doc\_SizeInBytes

  - **Data.StopwatchDuration** – zastarané

  - **Data.SyncBackedFileRequiresOnlineTransition** – príznak, ktorý označuje, že akcia uloženia je dočasne blokovaná online prechodom

  - **Data.SyncBackedFileSaveOnOpen** – príznak, ktorý označuje, že zmeny vykonané automatickou synchronizáciou vyžadujú uloženie pri otvorení

  - **Data.TelemetryId** – zastarané

  - **Data.TriggerSaveAfterBaseDownload** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.UploadBlockedDueToCoherencyFailure** – uloženie do služby blokované, čaká sa na vyriešenie konfliktných zmien používateľom

  - **Data.UploadBlockedDueToFailedSaveAsOverExisting** – uloženie do služby blokované v dôsledku neúspešného pokusu o prepísanie existujúceho súboru

  - **Data.UploadPreemptedForCoherency** – uloženie do služby bolo zrušené, pretože používateľ vykonáva ďalšie zmeny

  - **Data.UploadPreemptedForSaveAsOverExistingFailure** – uloženie do služby bolo zrušené v dôsledku skoršieho zlyhania SaveAsOverExisting

  - **Data.UploadScheduled** – súbor je pripravený na asynchrónne nahratie do služby

  - **Data.UseClientIdAsSchemaLockId** – príznak na kontrolu, ako sú dokumenty v službe uzamknuté

  - **Data.WorkingCopySaved** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.ZrtSaveAsforSyncBackedBusinessEnabled** – príznak, ktorý označuje rýchle ukladanie povolené pre SharePoint Online

  - **Data.ZrtSaveAsforSyncBackedConsumerEnabled** – príznak, ktorý označuje rýchle ukladanie povolené pre OneDrive Consumer

  - **Data.ZrtSaveAsforSyncBackedCTBusinessEnabled** – príznak, ktorý označuje typy obsahu na rýchle ukladanie povolené pre SharePoint Online

  - **Data.ZrtSaveAsforSyncBackedCTConsumerEnabled** – príznak, ktorý označuje typy obsahu na rýchle ukladanie povolené pre OneDrive Consumer

  - **Data.ZrtSaveAsforSyncBackedMetaDataBusinessEnabled** – príznak, ktorý označuje rýchle ukladanie metaúdajov súborov povolené pre SharePoint Online

  - **Data.ZrtSaveAsforSyncBackedMetaDataConsumerEnabled** – príznak, ktorý označuje rýchle ukladanie metaúdajov súborov povolené pre OneDrive Consumer

#### <a name="officefindtimeappfailedtostart"></a>Office.FindTime.AppFailedToStart

Zhromažďuje sa, ak spustenie aplikácie zlyhá z dôvodu výskytu neočakávanej chyby počas spúšťania. Používa na sledovanie výnimiek a zlyhaní. Pomáha monitorovať a ladiť stav aplikácie.

Zhromažďujú sa tieto polia:
- **DateTime** – časová pečiatka zaznamenania udalosti

- **EventName** – názov udalosti, ktorá sa práve zaznamenáva


#### <a name="officemanageabilityclient-fetchpolicyprechecks"></a>Office.Manageability.Client Fetch.PolicyPreChecks

Veľmi dôležitá telemetria na sledovanie zlyhania\\úspešnosti predbežného kontrolného overenia načítania politiky cloudu. ExitReason obsahuje mapu enumerátora k stavu predbežnej kontroly, kde došlo k zlyhaniu.

Zhromažďujú sa tieto polia:

  - **Data.ExitReason** – hodnota enumerátora s informáciou o dôvode ukončenia, ak predbežná kontrola zlyhala

  - **Data.Log** – hlásenie vlastného denníka s informáciou o úspešnosti alebo neúspešnosti predbežnej kontroly

#### <a name="officemanageabilityclientfetchandapplypolicy"></a>Office.Manageability.Client.Fetch.AndApplyPolicy

Veľmi dôležitá telemetria na sledovanie zlyhania\\úspešnosti spustenia načítania politiky cloudu z aplikácie. ExitReason obsahuje mapu enumerátora k dôvodu zlyhania.

Zhromažďujú sa tieto polia:

  - **Data.ExitReason** – hodnota enumerátora s informáciou o dôvode ukončenia, ak predbežná kontrola zlyhala

  - **Data.Log** – hlásenie vlastného denníka s informáciou o úspešnosti alebo neúspešnosti predbežnej kontroly


#### <a name="officeonenotenavigationcreatepage"></a>Office.OneNote.Navigation.CreatePage

Kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov OneNotu vytvárať strany vo OneNote.  Telemetria používaná na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia stranu nemôžu vytvoriť, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **IsAtSectionEnd** – označuje, či sa na konci sekcie vytvorí nová strana alebo nie.

- **IsBlank** – označuje, či je nová strana prázdna alebo vytvorená pomocou šablóny.

- **IsRecentsView** – označuje, či je strana vytvorená z posledných položiek alebo nie.

- **NavView** – označuje, či je strana vytvorená z navigačného zobrazenia alebo nie.

- **NoteType** – označuje typ strany (rýchla poznámka, zoznam alebo fotografia).

- **QuickNoteType** – označuje typ strany (rýchla poznámka, zoznam alebo fotografia).

- **RailState** – označuje stav navigačnej časti OneNotu pri vytváraní strany.

- **Trigger** – označuje vstupný bod, v ktorom sa spustí akcia vytvorenia strany.

- **TriggerInfo** – označuje ďalšie informácie týkajúce sa spúšťača.


#### <a name="officeonenotenavigationcreatesection"></a>Office.OneNote.Navigation.CreateSection

Kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov OneNotu vytvárať sekcie vo OneNote.  Telemetria používaná na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia stranu nemôžu vytvoriť, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **NotebookID** – jedinečný identifikátor poznámkového bloku.

- **SectionID** – jedinečný identifikátor vytvorenej sekcie.

- **Trigger** – označuje vstupný bod, v ktorom sa spustí akcia vytvorenia sekcie.

- **TriggerInfo** – označuje ďalšie informácie týkajúce sa spúšťača.


#### <a name="officeonenotenavigationnavigate"></a>Office.OneNote.Navigation.Navigate

Kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov OneNotu prechádzať medzi stranami vo OneNote.  Telemetria používaná na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia nemôžu prechádzať medzi stranami, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **FromNotebook** – jedinečný identifikátor poznámkového bloku.

- **FromPage** – jedinečný identifikátor strany.

- **FromSection** – jedinečný identifikátor sekcie.

- **FromSectionGroup** – jedinečný identifikátor skupiny sekcií.

- **IsCurrentUserEduStudent** – označuje, či má aktuálny používateľ rolu študenta vo vzdelávacom poznámkovom bloku alebo nie.

- **IsEduNotebook** – označuje, či sa aktuálna strana nachádza vo vzdelávacom poznámkovom bloku alebo nie.

- **IsEduNotebookReadOnlyPage** – označuje, či aktuálna strana je stranou iba na čítanie vo vzdelávacom poznámkovom bloku alebo nie.

- **ToNotebook** – jedinečný identifikátor poznámkového bloku.

- **ToPage** – jedinečný identifikátor strany.

- **ToSection** – jedinečný identifikátor sekcie.

- **ToSectionGroup** – jedinečný identifikátor skupiny sekcií.


#### <a name="officeonenotenotebookmanagementcreatenotebook"></a>Office.OneNote.NotebookManagement.CreateNotebook

Kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov OneNotu vytvárať poznámkové bloky vo OneNote.  Telemetria používaná na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia poznámkové bloky nemôžu vytvoriť, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:
    
- **NotebookID** – jedinečný identifikátor poznámkového bloku.


#### <a name="officeonenotenotebookmanagementopennotebook"></a>Office.OneNote.NotebookManagement.OpenNotebook

Kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov OneNotu otvárať poznámkové bloky vo OneNote.  Telemetria používaná na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia poznámkové bloky nemôžu otvoriť, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

-  **NotebookID** – jedinečný identifikátor poznámkového bloku.

    
#### <a name="officeonenotesearchsearch"></a>Office.OneNote.Search.Search

Kritický signálny identifikátor, ktorý sa používa na sledovanie schopnosti používateľov OneNotu vyhľadať informácie v rámci tisícok strán a poznámkových blokov.   Telemetria používaná na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia informácie v poznámkových blokoch nemôžu vyhľadať, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **PageSearchResultCount** – označuje počet výsledkov vyhľadávania, ktoré sa našli v režime vyhľadávania strán.

-  **PageTimeToFirstResultInMs** – označuje čas OneNotu potrebný na vyhľadanie prvej zhody v režime vyhľadávania strán.
    
-  **PageTimeToLastResultInMs** – označuje čas OneNotu potrebný na vyhľadanie poslednej zhody v režime vyhľadávania strán.

-  **PageTimeToMedianResultInMs** – označuje medián času OneNotu potrebného na vyhľadanie všetkých zhôd v režime vyhľadávania strán.

-  **SearchResultCount** – označuje počet nájdených výsledkov vyhľadávania.

-  **TagSearchResultCount** – označuje počet výsledkov vyhľadávania, ktoré sa našli v režime vyhľadávania značiek.

-  **TagTimeToFirstResultInMs** – označuje čas OneNotu potrebný na vyhľadanie prvej zhody v režime vyhľadávania značiek.

-  **TagTimeToLastResultInMs** – označuje čas OneNotu potrebný na vyhľadanie poslednej zhody v režime vyhľadávania značiek.

-  **TagTimeToMedianResultInMs** – označuje medián času OneNotu potrebného na vyhľadanie všetkých zhôd v režime vyhľadávania značiek.

-  **TimeToFirstResultInMs** – označuje čas OneNotu potrebný na vyhľadanie prvej zhody.

-  **TimeToLastResultInMs** – označuje čas OneNotu potrebný na vyhľadanie poslednej zhody.

-  **TimeToMedianResultInMs** – označuje medián času OneNotu potrebného na vyhľadanie všetkých zhôd.


#### <a name="officeonenotestoragenotebooksyncresult"></a>Office.OneNote.Storage.NotebookSyncResult
 
Táto udalosť zaznamenáva výsledok synchronizácie poznámkového bloku. Používa sa na zistenie počtu jedinečných cieľov synchronizácie vo výpočte skóre synchronizácie OneNotu.
 
Zhromažďujú sa tieto polia:

- **CachedError_Code** – číselný alebo alfanumerický kód, ktorý sa používa na určenie povahy chyby vo vyrovnávacej pamäti a/alebo dôvodu, prečo sa vyskytla.
    
- **CachedError_Description** – popis chyby vo vyrovnávacej pamäti.

- **CachedError_Tag** – označuje, ktoré miesto v kóde vyhodí chybu vo vyrovnávacej pamäti.

- **CachedError_Type** – typ chyby vo vyrovnávacej pamäti, napríklad Win32Error atď.

- **ExecutionTime** – čas v milisekundách, ktorý bol potrebný na replikovanie poznámkového bloku.

- **Gosid** – ID miesta globálneho objektu.

- **IdentityType** – typ identity, napríklad Windows Live, Org ID atď.

- **InitialReplicationInSession** – označuje, či je táto replikácia prvou replikáciou poznámkového bloku po otvorení alebo nie.

- **IsBackgroundSync** – označuje, či ide o synchronizáciu na pozadí alebo nie.

- **IsCachedErrorSuppressed** – označuje, či je chyba vo vyrovnávacej pamäti potlačená alebo nie.

- **IsCachedErrorUnexpected** – označuje, či je chyba vo vyrovnávacej pamäti neočakávaná alebo nie.

- **IsNotebookErrorSuppressed** – označuje, či je chyba synchronizácie úrovne poznámkového bloku potlačená alebo nie.

- **IsNotebookErrorUnexpected** – označuje, či je chyba synchronizácie úrovne poznámkového bloku neočakávaná alebo nie.

- **IsSectionErrorSuppressed** – označuje, či je chyba synchronizácie sekcie potlačená alebo nie.

- **IsSectionErrorUnexpected** – označuje, či je chyba synchronizácie sekcie neočakávaná alebo nie.

- **IsUsingRealtimeSync** – označuje, či synchronizácia poznámkového bloku používa modernú synchronizáciu obsahu strany alebo nie.

- **LastAttemptedSync** – časová pečiatka pri poslednom pokuse o synchronizáciu poznámkového bloku.

- **LastBackgroundSync** – časová pečiatka pri pokuse o najnovšiu synchronizáciu na pozadí.

- **LastNotebookViewedDate** – dátum posledného zobrazenia poznámkového bloku.

- **LastSuccessfulSync** – časová pečiatka poslednej úspešnej synchronizácie poznámkového bloku.

- **NeedToRestartBecauseOfInconsistencies** – označuje, či je potrebné reštartovať synchronizáciu z dôvodu nezrovnalostí alebo nie.

- **NotebookErrorCode** – kód chyby synchronizácie úrovne poznámkového bloku uložený v mieste grafu v poznámkovom bloku.

- **NotebookId** – ID poznámkového bloku.

- **NotebookType** – typ poznámkového bloku.

- **ReplicatingAgainBecauseOfInconsistencies** – označuje, či sa synchronizácia reštartuje z dôvodu nezrovnalostí alebo nie.

- **SectionError_Code** – číselný alebo alfanumerický kód, ktorý sa používa na určenie povahy chyby synchronizácie sekcie a/alebo dôvodu, prečo sa vyskytla.

- **SectionError_Description** – popis chyby synchronizácie sekcie.

- **SectionError_Tag** – označuje, ktoré miesto v kóde vyhodí chybu synchronizácie sekcie.

- **SectionError_Type** – typ chyby synchronizácie sekcie, napríklad Win32Error atď.

- **Success** – označuje, či je synchronizácia poznámkového bloku úspešná alebo nie.

- **SyncDestinationType** – typ cieľa synchronizácie, ako je OneDrive alebo SharePoint Online.

- **SyncId** – číslo jedinečné pre každú synchronizáciu poznámkového bloku.

- **SyncWasFirstInSession** – označuje, či je táto synchronizácia prvou synchronizáciou v aktuálnej relácii.

- **SyncWasUserInitiated** – označuje, či je táto synchronizácia iniciovaná používateľom alebo nie.

- **TenantId** – ID nájomníka SharePointu.

- **TimeSinceLastAttemptedSync** – čas od posledného pokusu o synchronizáciu poznámkového bloku.

- **TimeSinceLastSuccessfulSync** – čas od poslednej úspešnej synchronizácie poznámkového bloku.


#### <a name="officeonenotesystemapplifecycleapplaunch"></a>Office.OneNote.System.AppLifeCycle.AppLaunch

Kritický signál sa používa na zaistenie, aby používatelia OneNotu mohli úspešne spustiť aplikáciu.
Telemetria sa používa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia nemôžu spustiť aplikáciu v okne výkonu, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:     Žiadne

#### <a name="officeoutlookdesktopaccountconfigurationcreateaccountresult"></a>Office.Outlook.Desktop.AccountConfiguration.CreateAccountResult

Výsledok pridania konta do Outlooku v novom profile v zobrazení Office Backstage alebo v dialógovom okne nastavenia konta. Údaje sú aktívne monitorované, aby sa nezobrazovali žiadne výkyvy v zlyhaniach. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie. Naším cieľom je zvyšovať podiel úspešnosti každým vydaním.

Zhromažďujú sa tieto polia:

  - **AccountCreationResult** – výsledok (úspešnosť, zlyhanie, zrušenie atď.) pridania konta do Outlooku.

  - **AccountCreationTime** – čas trvania pokusu o vytvorenie konta

  - **AccountInfoSource** – zdroj nastavenia konta (napr. automatická konfigurácia, GuessSmart, automatické zisťovanie atď.)

  - **AccountType** – typ konta, ktoré sa konfiguruje.

  - **HashedEmailAddress** – hashovaná e-mailová adresa

  - **ShowPasswordPageFlightEnabled** – indikátor povolenia skupiny funkcií ShowPopImapPasswordPage

#### <a name="officeoutlookdesktopaccountconfigurationrepairaccountresult"></a>Office.Outlook.Desktop.AccountConfiguration.RepairAccountResult

Výsledok opravy konta alebo zmeny rozšíreného nastavenia konta. Údaje sú aktívne monitorované, aby sa nezobrazovali žiadne výkyvy v zlyhaniach. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie. Keďže ide o nové (refaktorované) prostredie, chceme si byť istí, že je to dobré.

Zhromažďujú sa tieto polia:

  - **AccountInfoSource** – zdroj informácií o konte pre konto použité pri pokuse o opravu

  - **AccountType** – typ konta, pre ktoré sa vykonal pokus o opravu konta

  - **HashedEmailAddress** – hashovaná e-mailová adresa

  - **ManualRepairRequested** – indikátor požadovanej opravy

  - **Result** – výsledok pokusu o opravu konta. Príklad: „Success“ (úspešný pokus) alebo „Fail\_SaveChangesToAccount“ (neúspešný pokus)

#### <a name="officeoutlookdesktopaccountconfigurationupdatepasswordresult"></a>Office.Outlook.Desktop.AccountConfiguration.UpdatePasswordResult

Výsledok aktualizácie hesla konta v rozbaľovacej ponuke nastavenia konta. Údaje sú aktívne monitorované, aby sa nezobrazovali žiadne výkyvy v zlyhaniach. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie. Keďže ide o nové (refaktorované) prostredie, chceme si byť istí, že je to dobré.

Zhromažďujú sa tieto polia:

  - **AccountType** – typ konta, pre ktoré sa vykonal pokus o aktualizáciu hesla

  - **HashedEmailAddress** – hashovaná e-mailová adresa

  - **Result** – výsledok pokusu o aktualizáciu hesla. Príklad: „Success“ (úspešný pokus) alebo „Fail\_AllowLessSecureAppsDisabled“ (neúspešný pokus)

#### <a name="officeoutlookdesktopprovidersloadproviderlibrary"></a>Office.Outlook.Desktop.Providers.LoadProviderLibrary

Táto udalosť sleduje úspešnosť alebo zlyhanie rozhrania MAPI pri pokuse načítať knižnicu DLL poskytovateľa (napr. contab32.dll, emsmdb32.dll, knižnicu DLL používanú doplnkom). Operácia rozhrania MAPI zodpovedná za načítanie knižníc DLL poskytovateľa je pre základom pre povinné operácie Outlooku ako aj rozšíriteľnosť (cez doplnky alebo vlastných poskytovateľov ukladacieho priestoru/prenosu/adresára). Aktívne monitorujeme úspešné alebo neúspešné výsledky tejto operácie s cieľom zabezpečiť, aby tieto základné funkcie rozhrania MAPI fungovali podľa očakávaní.

Zhromažďujú sa tieto polia:

  - **Štandardná aktivita HVA** bez vlastnej údajovej časti

#### <a name="officeoutlookdesktopstorescreatenewstore"></a>Office.Outlook.Desktop.Stores.CreateNewStore

Zhromažďuje výsledok vytvorenie nového ukladacieho priestoru (vrátane typu a verzie), ako aj kód výsledku. Aktívne monitorujeme túto udalosť, aby sme mohli sledovať stav schopnosti používateľa synchronizovať a ukladať poštu lokálne, archivovať e-maily (vo formáte súboru PST) alebo používať skupiny.

Zhromažďujú sa tieto polia:

  - **Štandardná aktivita HVA** s vlastnou údajovou časťou

  - **StoreType** – typ vytvoreného ukladacieho priestoru, OST/PST/NST

  - **StoreVersion** – verzia vytvoreného ukladacieho priestoru, Small/Large/Tardis

#### <a name="officeoutlookmacaccountaddworkflow"></a>Office.Outlook.Mac.AccountAddWorkflow

Výsledok pridania konta v Outlooku. Údaje sú monitorované, aby sa nezobrazovali žiadne výkyvy v zlyhaniach. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie. Naším cieľom je zvyšovať podiel úspešnosti každým vydaním. 

Zhromažďujú sa tieto polia:

- **AccountConfigMethod** – metóda konfigurácie konta.

- **AccountType** – typ konta, ktoré sa konfiguruje.

- **AccountWorkflowSession** – relácia s pokusom o vykonanie pracovného postupu konta.

- **SessionDuration** – trvanie relácie. 

- **ThreadId** – identifikátor vlákna.


#### <a name="officeoutlookmacaccountonboardingflow"></a>Office.Outlook.Mac.AccountOnboardingFlow

Výsledok pridania konta v Outlooku pomocou prostredia konfigurácie nového konta. Údaje sú monitorované, aby sa nezobrazovali žiadne výkyvy v zlyhaniach. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie. Naším cieľom je zvyšovať podiel úspešnosti každým vydaním. 

Zhromažďujú sa tieto polia:

- **AccountConfigAutoSignIn** – automatická konfigurácia konta nastavená správcom.

- **AccountConfigDomain** – doména špecifikovaná počas konfigurácie konta. 

- **AccountConfigEntryPoint** – vstupný bod, v ktorom používateľ zadal konfiguráciu konta. 

- **AccountConfigErrorCode** – kód chyby, ktorá sa vyskytla počas konfigurácie konta. 

- **AccountConfigErrorString** – chyba, ktorá sa vyskytla počas konfigurácie konta.

- **AccountConfigMethod** – metóda konfigurácie konta.

- **AccountConfigPhase** – aktuálny krok pracovného postupu konfigurácie konta.

- **AccountConfigPhaseFrom** – začiatočný krok pracovného postupu konfigurácie konta. 

- **AccountConfigPhaseTo** – posledný krok pracovného postupu konfigurácie konta. 

- **AccountType** – typ konta, ktoré sa konfiguruje.

- **AccountWorkflowSession** – relácia s pokusom o vykonanie pracovného postupu konta.

- **SessionDuration** – trvanie relácie.


#### <a name="officeoutlookmacdeleteaccountusage"></a>Office.Outlook.Mac.DeleteAccountUsage

Výsledok odstránenia konta v Outlooku. Údaje sú monitorované, aby sa nezobrazovali žiadne výkyvy v zlyhaniach. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie. Naším cieľom je zvyšovať podiel úspešnosti každým vydaním. 

Zhromažďujú sa tieto polia:

- **AccountType** – typ konta, ktoré sa konfiguruje.

- **AccountID** – identifikátor konta.

- **DeprovisionAccount** – označuje, či sa konto odstráni zo servera.

- **IsFastDelete** – označuje, či sa konto odstráni vo vlákne na pozadí.

#### <a name="officepowerpointdocoperationclose"></a>Office.PowerPoint.DocOperation.Close

Zhromažďuje sa pri zatvorení powerpointových prezentácií. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú počas procesu zatvárania, ktorý zahŕňa zachovanie a synchronizáciu údajov používateľa. Spoločnosť Microsoft používa tieto údaje, aby sa zabezpečilo fungovanie zatvárania podľa očakávaní a obsah používateľa sa úspešne zachoval.

Zhromažďujú sa tieto polia:

  - **Data\_AddDocTelemetryResult:long** – obsahuje tento záznam denníka celú potrebnú telemetriu dokumentu (polia Data\_Doc\_\*)? Ak nie, prečo?

  - **Data\_AutoSaveDisabledReasons:string** – preddefinovaná množina hodnôt toho, prečo bolo automatické ukladanie vypnuté pre tento dokument? (Chyba zlúčenia, chyba uloženia, skupinová politika atď.)

  - **Data\_CloseReason:long** – Ako sa zatvorenie uskutočnilo? Zatvorením dokumentu? Zatvorením aplikácie?

  - **Data\_CppUncaughtExceptionCount:long** – počet nespracovaných výnimiek

  - **Data\_DetachedDuration:long** – časový úsek, počas ktorého bola aktivita odpojená/nespustená

  - **Data\_Doc\_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie)

  - **Data\_Doc\_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou

  - **Data\_Doc\_ChunkingType:long** – ako je dokument uložený v SharePointe

  - **Data\_Doc\_EdpState:long** – stav ochrany podnikových údajov v dokumente

  - **Data\_Doc\_Ext:string** – prípona dokumentu

  - **Data\_Doc\_Extension:string** – prípona dokumentu

  - **Data\_Doc\_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona)

  - **Data\_Doc\_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365

  - **Data\_Doc\_FqdnHash:string** – hodnota hash miesta uloženia dokumentu

  - **Data\_Doc\_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa

  - **Data\_Doc\_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov

  - **Data\_Doc\_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument

  - **Data\_Doc\_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

  - **Data\_Doc\_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument)

  - **Data\_Doc\_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäte

  - **Data_Doc_IsRtcAlwaysOn** – má hodnotu true, ak je kanál v reálnom čase (RTC) pre tento súbor vždy zapnutý.

  - **Data\_Doc\_IsSyncBacked:bool** – overuje, či sa dokument otvára z priečinka, ktorý používa aplikáciu OneDrivu na synchronizáciu a zálohovanie

  - **Data\_Doc\_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.)

  - **Data\_Doc\_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.)

  - **Data\_Doc\_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu

  - **Data\_Doc\_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu)

  - **Data\_Doc\_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.)

  - **Data\_Doc\_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude

  - **Data\_Doc\_ServerDocId:string** – nezmeniteľný identifikátor pre dokumenty uložené v cloude

  - **Data\_Doc\_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.)

  - **Data\_Doc\_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16

  - **Data\_Doc\_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu

  - **Data\_Doc\_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníka na strane klienta a na strane servera

  - **Data\_Doc\_SizeInBytes:long** – veľkosť dokumentu v bajtoch

  - **Data\_Doc\_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu

  - **Data\_Doc\_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“

  - **Data\_Doc\_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný)

  - **Data\_Doc\_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude

  - **Data\_Doc\_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa

  - **Data\_Doc\_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“

  - **Data\_DocHasStorage:bool** – má tento dokument lokálny ukladací priestor?

  - **Data\_fLifeguarded:bool** – mal dokument niekedy chránenú životnosť (funkciou na riešenie chýb dokumentov bez zobrazenia výzvy používateľovi)?

  - **Data\_IsDocAutoSaveable:bool** – ukladá sa prezentácia automaticky?

  - **Data\_IsDocDirty:bool** – obsahuje prezentácia zmeny, ktoré ešte nie sú uložené?

  - **Data\_IsNewDoc:bool** – či ide o nový alebo existujúci dokument

  - **Data\_IsRecoveredDoc:bool** – je to obnovený dokument? (Ak predchádzajúca relácia zlyhala, tabla Obnovenie dokumentu bude zobrazená v ďalšej relácii.)

  - **Data\_NewDocDiscarded:bool** – či bola nová prezentácia zahodená bez uloženia

  - **Data\_OCSClosingDlgCanceled:bool** – ak nahratie čaká na OCS, keď používateľ zatvára dokument, používateľovi sa zobrazí dialógové okno s informáciou, aby čakal. Ktorú možnosť používateľ vybral?

  - **Data\_OCSClosingDlgExpired:bool** – zmizlo dialógové okno (po 1 minúte) automaticky?

  - **Data\_OCSClosingStatus:long** – označuje, aký je konečný stav OCS (In CSI (V CSI), Closable (Zatvoriteľný), In OCS Transition (V prechode OCS), In CSI transition (V prechode CSI) atď.)

  - **Data\_OCSClosingWaitDurationMS:long** – koľko času musel používateľ čakať na nahratie OCS

  - **Data\_OCSHandleTransitionResult:long** – preddefinovaná množina hodnôt výsledku prechodu vykonaného počas zavretia (pokus už prebehol, pokračovať v zatváraní atď.)

  - **Data\_ServerDocId:string** – identifikátor GUID na jedinečnú identifikáciu dokumentu

  - **Data\_StopwatchDuration:long** – celkový čas aktivity

  - **Data\_UserContinuedZRTClose:bool** – keď sa zobrazilo dialógové okno pri zatváraní, vybral používateľ možnosť „Continue“ (Pokračovať) na zatvorenie?

#### <a name="officepowerpointdocoperationnewdocument"></a>Office.PowerPoint.DocOperation.NewDocument

Zhromažďuje sa, keď PowerPoint vytvorí novú prezentáciu. Obsahuje metriky úspešnosti, zlyhania a výkonu.

Tieto informácie sa používajú na zabezpečenie úspešného vytvorenia súboru bez zníženie výkonu.

Zhromažďujú sa tieto polia:

  - **NewDocumentType** – vytvoril sa nový dokument pomocou šablóny alebo otvorením prázdneho dokumentu?

  - **FLifeguarded** – či má dokument chránenú životnosť (funkciou, ktorá obnoví poškodený dokument bez zobrazenia upozornenia používateľovi)

#### <a name="officepowerpointdocoperationopencompleteprotocol"></a>Office.PowerPoint.DocOperation.OpenCompleteProtocol

Zhromažďuje sa pri otvorení powerpointových prezentácií. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú počas konečných fáz procesu otvárania.

Spoločnosť Microsoft používa tieto údaje na zabezpečenie fungovania funkcie podľa očakávaní bez toho, aby sa zhoršilo otváranie prezentácií.

Zhromažďujú sa tieto polia:

  - **Data\_AntiVirusScanMethod:long** – preddefinovaná množina hodnôt typu skenovania antivírusu (IOAV, AMSI, žiadny atď.)

  - **Data\_AntiVirusScanStatus:long** – preddefinovaná množina hodnôt skenovania antivírusu, ktoré prebieha pre každý otvorený dokument (NoThreatsDetected (Žiadne zistené hrozby), Failed (Zlyhanie), MalwareDetected (Zistil sa malvér) atď.)

  - **Data\_CloseAndReopen:bool** – bol tento dokument zatvorený a znova otvorený?

  - **Data\_DetachedDuration:long** – časový úsek, počas ktorého bola aktivita odpojená/nespustená

  - **Data\_Doc\_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie)

  - **Data\_Doc\_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou

  - **Data\_Doc\_ChunkingType:long** – ako je dokument uložený v SharePointe

  - **Data\_Doc\_EdpState:long** – stav ochrany podnikových údajov v dokumente

  - **Data\_Doc\_Ext:string** – prípona dokumentu

  - **Data\_Doc\_Extension:string** – prípona dokumentu

  - **Data\_Doc\_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona)

  - **Data\_Doc\_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365

  - **Data\_Doc\_FqdnHash:string** – hodnota hash miesta uloženia dokumentu

  - **Data\_Doc\_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa

  - **Data\_Doc\_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov

  - **Data\_Doc\_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument

  - **Data\_Doc\_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

  - **Data\_Doc\_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument)

  - **Data\_Doc\_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäte

  - **Data_Doc_IsRtcAlwaysOn** – má hodnotu true, ak je kanál v reálnom čase (RTC) pre tento súbor vždy zapnutý.

  - **Data\_Doc\_IsSyncBacked:bool** – zobrazuje, či sa dokument otvára z priečinka, ktorý používa aplikáciu OneDrivu na synchronizáciu a zálohovanie

  - **Data\_Doc\_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.)

  - **Data\_Doc\_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.)

  - **Data\_Doc\_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu

  - **Data\_Doc\_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu)

  - **Data\_Doc\_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.)

  - **Data\_Doc\_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude

  - **Data\_Doc\_ServerDocId:string** – nezmeniteľný identifikátor pre dokumenty uložené v cloude

  - **Data\_Doc\_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.)

  - **Data\_Doc\_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16

  - **Data\_Doc\_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu

  - **Data\_Doc\_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

  - **Data\_Doc\_SizeInBytes:long** – veľkosť dokumentu v bajtoch

  - **Data\_Doc\_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu

  - **Data\_Doc\_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“

  - **Data\_Doc\_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný)

  - **Data\_Doc\_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude

  - **Data\_Doc\_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa

  - **Data\_Doc\_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“

  - **Data\_ExecutionCount:long** – koľkokrát sme vykonali protokol IncOpen pred spustením tohto protokolu (OpenComplete)

  - **Data\_FailureComponent:long** – preddefinovaná množina hodnôt toho, ktorá súčasť spôsobila zlyhanie protokolu (Conflict (Konflikt), CSI, Internal (Interné) atď.)

  - **Data\_FailureReason:long** – preddefinovaná množina hodnôt dôvodu zlyhania (FileIsCorrupt, BlockedByAntivirus atď.)

  - **Data_FullDownloadRoundTripCount:long** – počet návštev servera potrebných na stiahnutie celého dokumentu.
  
  - **Data_IsProtocolRunInIncOpenMode:bool** – či sa spustil protokol pre prírastkové sťahovanie, čo je sťahovanie, pri ktorom sa časti dokumentu stiahnu po jeho počiatočnom zobrazení používateľovi.

  - **Data\_MethodId:long** – zobrazuje, ktorý riadok kódu sa interne vykonal ako posledný

  - **Data\_StopwatchDuration:long** – celkový čas aktivity

  - **Data\_TimeToEdit:long** – čas, po ktorom bolo možné dokument upravovať

  - **Data\_TimeToView:long** – čas potrebný na vykreslenie prvej snímky dokumentu

  - **Data\_UnhandledException:bool** – existuje nejaká nespracovaná natívna výnimka?

#### <a name="officepowerpointdocoperationsave"></a>Office.PowerPoint.DocOperation.Save

Zhromažďuje sa vždy, keď PowerPoint vykoná uloženie pomocou cesty moderného kódu. Zahŕňa typ výsledku úspešnosti alebo zlyhania pre metriku výkonu pri ukladaní a metaúdaje relevantného dokumentu.  Zlyhania uloženia môžu mať za následok stratu údajov. Spoločnosť Microsoft používa tieto údaje, aby sa zabezpečilo fungovanie funkcie podľa očakávaní a obsah používateľa sa úspešne zachoval.

Zhromažďujú sa tieto polia:

  - **Data\_AddDocTelemetryResult:long** – obsahuje tento záznam denníka celú potrebnú telemetriu dokumentu (polia Data\_Doc\_\*)? Ak nie, prečo?

  - **Data\_BeforeSaveEvent:long** – časový úsek, po ktorom nastala udalosť dokumentu pred uložením

  - **Data\_CheckDownRevSaveTimeMS:long** – čas potrebný na kontrolu revízie

  - **Data\_CheckMacroSaveTimeMS:long** – čas potrebný na uloženie makier

  - **Data\_ClearAutoSaveTimeMS:long** – čas potrebný na vymazanie príznaku automatického ukladania

  - **Data\_ClearDirtyFlagTimeMS:long** – čas potrebný na vymazanie príznaku zmeneného dokumentu

  - **Data\_CloneDocumentTimeMS:long** – čas potrebný na klonovanie dokumentu pred spustením ukladania

  - **Data\_CommitTransactionTimeMS:long** – čas potrebný na potvrdenie transakcie uloženia

  - **Data\_CppUncaughtExceptionCount:long** – nezachytené natívne výnimky počas spustenej aktivity

  - **Data\_DetachedDuration:long** – časový úsek, počas ktorého bola aktivita odpojená/nespustená

  - **Data\_Doc\_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie)

  - **Data\_Doc\_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou

  - **Data\_Doc\_ChunkingType:long** – ako je dokument uložený v SharePointe

  - **Data\_Doc\_EdpState:long** – stav ochrany podnikových údajov v dokumente

  - **Data\_Doc\_Ext:string** – prípona dokumentu

  - **Data\_Doc\_Extension:string** – prípona dokumentu

  - **Data\_Doc\_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona)

  - **Data\_Doc\_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365

  - **Data\_Doc\_FqdnHash:string** – hodnota hash miesta uloženia dokumentu

  - **Data\_Doc\_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa

  - **Data\_Doc\_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov

  - **Data\_Doc\_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument

  - **Data\_Doc\_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

  - **Data\_Doc\_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument)

  - **Data\_Doc\_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäte

  - **Data_Doc_IsRtcAlwaysOn** – má hodnotu true, ak je kanál v reálnom čase (RTC) pre tento súbor vždy zapnutý.

  - **Data\_Doc\_IsSyncBacked:bool** – zobrazuje, či sa dokument otvára z priečinka, ktorý používa aplikáciu OneDrivu na synchronizáciu a zálohovanie

  - **Data\_Doc\_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.)

  - **Data\_Doc\_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.)

  - **Data\_Doc\_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu

  - **Data\_Doc\_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu)

  - **Data\_Doc\_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.)

  - **Data\_Doc\_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude

  - **Data\_Doc\_ServerDocId:string** – nezmeniteľný identifikátor pre dokumenty uložené v cloude

  - **Data\_Doc\_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.)

  - **Data\_Doc\_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16

  - **Data\_Doc\_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu

  - **Data\_Doc\_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

  - **Data\_Doc\_SizeInBytes:long** – veľkosť dokumentu v bajtoch

  - **Data\_Doc\_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu

  - **Data\_Doc\_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“

  - **Data\_Doc\_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný)

  - **Data\_Doc\_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude

  - **Data\_Doc\_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa

  - **Data\_Doc\_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“

  - **Data\_DurationUAEOnSaveStartedMs:long** – čas potrebný na ukončenie neznámej aplikácie počas ukladania

  - **Data\_EnsureSaveTransactionTimeMS:long** – čas potrebný na zabezpečenie vytvorenia transakcie uloženia, ak už neexistuje

  - **Data\_FailureComponent:long** – preddefinovaná množina hodnôt toho, ktorá súčasť spôsobila zlyhanie protokolu (Conflict (Konflikt), CSI, Internal (Interné) atď.)

  - **Data\_FailureReason:long** – preddefinovaná množina hodnôt dôvodu zlyhania (FileIsCorrupt (Poškodený súbor), BlockedByAntivirus (Blokované antivírusom) atď.)

  - **Data\_fLifeguarded:bool** – mal dokument niekedy chránenú životnosť (funkciou na riešenie chýb dokumentov bez zobrazenia výzvy používateľovi)?

  - **Data\_HandleEnsureContentType:long** – čas potrebný na zabezpečenie toho, že všetky typy obsahu sú správne

  - **Data\_HandleEnsureContentTypeTimeMS:long** – čas potrebný na zabezpečenie toho, že všetky typy obsahu sú správne

  - **Data\_HasEmbeddedFont:bool** – obsahuje tento dokument vložené písma?

  - **Data\_InitializeSaveTimeMS:long** – čas potrebný na inicializáciu obsahu dokumentu a spustenie ukladania

  - **Data\_InOCSTransition:bool** – či je toto uloženie vykonané na prechod na OCS

  - **Data\_IsSavingWithEmbeddedFont:bool** – obsahuje tento dokument vložené písma?

  - **Data\_MethodId:long** – ktorý riadok kódu sa interne vykonal ako posledný

  - **Data\_PerformEmbedFontsTimeMS:long** – čas potrebný na serializovanie vložených písiem

  - **Data\_PerformModernSaveTimeMS:long** – čas potrebný na vykonanie moderného uloženia (s novým kódom)

  - **Data\_PerformPostSaveTimeMS:long** – čas potrebný na vykonanie funkcií po uložení (oznámenia, položky vrátenia akcií)

  - **Data\_PrepareForSaveTimeMS:long** – čas potrebný na spustenie ukladania

  - **Data\_RaiseDocumentBeforeSaveEventTimeMS:long** – časový úsek, po ktorom nastala udalosť BeforeSave (Pred uložením)

  - **Data\_ReflectDocumentChangeTimeMS:long** – čas potrebný na prejavenie uložených zmien v používateľskom rozhraní (opakované vyplnenie miniatúr atď.)

  - **Data\_ReportStartTimeMS:long** – čas potrebný na dokončenie inicializácie telemetrie na ukladanie

  - **Data\_ReportSuccessTimeMS:long** – čas potrebný na dokončenie hlásenia o úspešnom uložení

  - **Data\_ResetDirtyFlagOnErrorTimeMS:long** – čas potrebný na vynulovanie príznaku zmeneného dokumentu pri chybe

  - **Data\_SaveReason:long** – preddefinovaná množina hodnôt dôvodu vykonania tohto uloženia (automatické ukladanie, ToOCSTransitionSave, ToCSITransitionSave atď.)

  - **Data\_SaveType:long** – preddefinovaná množina hodnôt typu uloženia (Uložiť ako, Publikovať, manuálne, OMSave atď.)

  - **Data\_SavingWithFont:bool** – ukladáme dokument s novými vloženými písmami?

  - **Data\_ScrubClonedDocumentTimeMS:long** – čas potrebný na odstránenie osobných informácií v klonovanej kópii dokumentu

  - **Data\_StopwatchDuration:long** – celkový čas aktivity

  - **Data\_TransactionType:long** – ide o transakciu uloženia alebo zlúčenia a uloženia?

#### <a name="officepowerpointdocoperationsaveas"></a>Office.PowerPoint.DocOperation.SaveAs

Zhromažďuje sa vždy, keď PowerPoint vykoná akciu Uložiť ako. Zahŕňa typ výsledku úspešnosti alebo zlyhania pre metriku výkonu pri ukladaní a metaúdaje relevantného dokumentu. Zlyhania uloženia môžu mať za následok stratu údajov.  Spoločnosť Microsoft používa tieto údaje, aby sa zabezpečilo fungovanie funkcie podľa očakávaní a obsah používateľa sa úspešne zachoval.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemetryResult:long** – obsahuje tento záznam denníka celú potrebnú telemetriu dokumentu (polia Data_Doc_*)? Ak nie, prečo?

- **Data_CppUncaughtExceptionCount:long** – nezachytené natívne výnimky počas spustenej aktivity.

- **Data_DetachedDuration:long** – časový úsek, počas ktorého bola aktivita odpojená/nespustená.

- **Data_DstDoc_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie).

- **Data_DstDoc_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_DstDoc_ChunkingType:long** – ako je dokument uložený v SharePointe.

- **Data_DstDoc_EdpState:long** – stav ochrany podnikových údajov v dokumente.

- **Data_DstDoc_Ext:string** – prípona dokumentu.

- **Data_DstDoc_Extension:string** – prípona dokumentu.

- **Data_DstDoc_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona).

- **Data_DstDoc_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365.
    
- **Data_DstDoc_FqdnHash:string** – hodnota hash miesta uloženia dokumentu.

- **Data_DstDoc_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa.

- **Data_DstDoc_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov.

- **Data_DstDoc_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument.

- **Data_DstDoc_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.).
    
- **Data_DstDoc_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

- **Data_DstDoc_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument).

- **Data_DstDoc_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS.

- **Data_DstDoc_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäti.

- **Data_DstDoc_IsSyncBacked:bool** – otvára sa dokument z priečinka, ktorý používa aplikáciu synchronizácie zálohovania OneDrivu?
    
- **Data_DstDoc_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.).

- **Data_DstDoc_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.).

- **Data_DstDoc_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu.

- **Data_DstDoc_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu).

- **Data_DstDoc_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.).

- **Data_DstDoc_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude.

- **Data_DstDoc_ServerDocId:string** – nezmeniteľný identifikátor pre dokumenty uložené v cloude.

- **Data_DstDoc_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.).

- **Data_DstDoc_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI).

- **Data_DstDoc_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16.

- **Data_DstDoc_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu.

- **Data_DstDoc_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

- **Data_DstDoc_SizeInBytes:long** – veľkosť dokumentu v bajtoch.

- **Data_DstDoc_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu.

- **Data_DstDoc_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“.

- **Data_DstDoc_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný).

- **Data_DstDoc_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude.

- **Data_DstDoc_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa.

- **Data_DstDoc_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“.

- **Data_FileType:long** – preddefinovaná množina hodnôt interného typu súboru.

- **Data_fLifeguarded:bool** – či mal dokument niekedy chránenú životnosť (funkciou na riešenie chýb dokumentov bez zobrazenia výzvy používateľovi).

- **Data_FWebCreated:bool** – má tento dokument príznak WebCreator?

- **Data_SaveReason:long** – preddefinovaná množina hodnôt dôvodu vykonania tohto uloženia. (automatické ukladanie, ToOCSTransitionSave, ToCSITransitionSave atď.)

- **Data_SaveType:long** – preddefinovaná množina hodnôt typu uloženia (Uložiť ako, Publikovať, manuálne, OMSave atď.). 

- **Data_SrcDoc_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie).

- **Data_SrcDoc_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_SrcDoc_ChunkingType:long** – ako je dokument uložený v SharePointe. 

- **Data_SrcDoc_EdpState:long** – stav ochrany podnikových údajov v dokumente.

- **Data_SrcDoc_Ext:string** – prípona dokumentu.

- **Data_SrcDoc_Extension:string** – prípona dokumentu.

- **Data_SrcDoc_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona).

- **Data_SrcDoc_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365.

- **Data_SrcDoc_FqdnHash:string** – hodnota hash miesta uloženia dokumentu.

- **Data_SrcDoc_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa.

- **Data_SrcDoc_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov.

- **Data_SrcDoc_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument.

- **Data_SrcDoc_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.).

- **Data_SrcDoc_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

- **Data_SrcDoc_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument).

- **Data_SrcDoc_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS.

- **Data_SrcDoc_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäti.

- **Data_SrcDoc_IsSyncBacked:bool** – otvára sa dokument z priečinka, ktorý používa aplikáciu synchronizácie zálohovania OneDrivu?

- **Data_SrcDoc_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.).

- **Data_SrcDoc_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.).

- **Data_SrcDoc_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu.

- **Data_SrcDoc_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu).

- **Data_SrcDoc_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.).

- **Data_SrcDoc_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude.

- **Data_SrcDoc_ServerDocId:string** – nezmeniteľný identifikátor pre dokumenty uložené v cloude.

- **Data_SrcDoc_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.).

- **Data_SrcDoc_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI).

- **Data_SrcDoc_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16Data_SrcDoc_SessionId:long – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu.

- **Data_SrcDoc_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

- **Data_SrcDoc_SizeInBytes:long** – veľkosť dokumentu v bajtoch.

- **Data_SrcDoc_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu.

- **Data_SrcDoc_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“.

- **Data_SrcDoc_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný).

- **Data_SrcDoc_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude.

- **Data_SrcDoc_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa.

- **Data_SrcDoc_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“.

- **Data_StopwatchDuration:long** – celkový čas aktivity.

- **Data_TypeOfSaveDialog:long** – preddefinovaná množina hodnôt dialógového okna (RUN_SAVEAS_DLG,RUN_SAVEMEDIA_DLG, RUN_SAVEAS_VIDEO_DLG atď.)

- **DstDoc** – nové umiestnenie dokumentu. 

- **SrcDoc** – pôvodné umiestnenie dokumentu.


#### <a name="officepowerpointdocoperationsavelegacy"></a>Office.PowerPoint.DocOperation.SaveLegacy

Zhromažďuje sa vždy, keď PowerPoint vykoná uloženie pomocou cesty staršieho kódu. Zahŕňa typ výsledku úspešnosti alebo zlyhania pre metriku výkonu pri ukladaní a metaúdaje relevantného dokumentu.  Zlyhania uloženia môžu mať za následok stratu údajov.  Spoločnosť Microsoft používa tieto údaje, aby sa zabezpečilo fungovanie funkcie podľa očakávaní a obsah používateľa sa úspešne zachoval.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemetryResult:long** – obsahuje tento záznam denníka celú potrebnú telemetriu dokumentu (polia Data_Doc_*)? Ak nie, prečo?

- **Data_CppUncaughtExceptionCount:long** – nezachytené natívne výnimky počas spustenej aktivity.

- **Data_DetachedDuration:long** – časový úsek, počas ktorého bola aktivita odpojená/nespustená.

- **Data_Doc_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie).

- **Data_Doc_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_Doc_ChunkingType:long** – ako je dokument uložený v SharePointe.

- **Data_Doc_EdpState:long** – stav ochrany podnikových údajov v dokumente.

- **Data_Doc_Ext:string** – prípona dokumentu.

- **Data_Doc_Extension:string** – prípona dokumentu.

- **Data_Doc_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona).

- **Data_Doc_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365.

- **Data_Doc_FqdnHash:string** – hodnota hash miesta uloženia dokumentu.

- **Data_Doc_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa.

- **Data_Doc_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov.

- **Data_Doc_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument.

- **Data_Doc_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.).

- **Data_Doc_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

- **Data_Doc_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument).

- **Data_Doc_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS.

- **Data_Doc_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäti.

- **Data_Doc_IsRtcAlwaysOn** – má hodnotu true, ak je kanál v reálnom čase (RTC) pre tento súbor vždy zapnutý.

- **Data_Doc_IsSyncBacked:bool** – otvára sa dokument z priečinka, ktorý používa aplikáciu synchronizácie zálohovania OneDrivu?

- **Data_Doc_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.).

- **Data_Doc_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.).

- **Data_Doc_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu.

- **Data_Doc_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu).

- **Data_Doc_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.).

- **Data_Doc_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude.

- **Data_Doc_ServerDocId:string** – nezmeniteľný identifikátor pre dokumenty uložené v cloude.

- **Data_Doc_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.).

- **Data_Doc_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI). 

- **Data_Doc_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16.

- **Data_Doc_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu.

- **Data_Doc_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

- **Data_Doc_SizeInBytes:long** – veľkosť dokumentu v bajtoch.

- **Data_Doc_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu.

- **Data_Doc_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“.

- **Data_Doc_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný).

- **Data_Doc_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude.

- **Data_Doc_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa.

- **Data_Doc_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“.

- **Data_DstDoc_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie).

- **Data_DstDoc_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_DstDoc_ChunkingType:long** – ako je dokument uložený v SharePointe.

- **Data_DstDoc_EdpState:long** – stav ochrany podnikových údajov v dokumente.

- **Data_DstDoc_Ext:string** – prípona dokumentu.

- **Data_DstDoc_Extension:string** – prípona dokumentu.

- **Data_DstDoc_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona).

- **Data_DstDoc_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365.
    
- **Data_DstDoc_FqdnHash:string** – hodnota hash miesta uloženia dokumentu.

- **Data_DstDoc_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa.

- **Data_DstDoc_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov.

- **Data_DstDoc_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument.

- **Data_DstDoc_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.).

- **Data_DstDoc_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

- **Data_DstDoc_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument).

- **Data_DstDoc_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS.

- **Data_DstDoc_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäti.

- **Data_DstDoc_IsSyncBacked:bool** – otvára sa dokument z priečinka, ktorý používa aplikáciu synchronizácie zálohovania OneDrivu?

- **Data_DstDoc_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.).

- **Data_DstDoc_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.).

- **Data_DstDoc_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu.

- **Data_DstDoc_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu).

- **Data_DstDoc_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.).

- **Data_DstDoc_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude.

- **Data_DstDoc_ServerDocId:string** – nezmeniteľný identifikátor pre dokumenty uložené v cloude.

- **Data_DstDoc_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.).

- **Data_DstDoc_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI).

- **Data_DstDoc_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16.

- **Data_DstDoc_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu.

- **Data_DstDoc_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

- **Data_DstDoc_SizeInBytes:long** – veľkosť dokumentu v bajtoch.

- **Data_DstDoc_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu.

- **Data_DstDoc_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“.

- **Data_DstDoc_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný).

- **Data_DstDoc_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude.

- **Data_DstDoc_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa.

- **Data_DstDoc_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“.

- **Data_FileType:long** – preddefinovaná množina hodnôt interného typu súboru.

- **Data_fLifeguarded:bool** – či mal dokument niekedy chránenú životnosť (funkciou na riešenie chýb dokumentov bez zobrazenia výzvy používateľovi).

- **Data_SaveReason:long** – preddefinovaná množina hodnôt dôvodu vykonania tohto uloženia. (automatické ukladanie, ToOCSTransitionSave, ToCSITransitionSave atď.)

- **Data_SaveType:long** – preddefinovaná množina hodnôt typu uloženia (Uložiť ako, Publikovať, manuálne, OMSave atď.).

- **Data_SrcDoc_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie).

- **Data_SrcDoc_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_SrcDoc_ChunkingType:long** – ako je dokument uložený v SharePointe.

- **Data_SrcDoc_EdpState:long** – stav ochrany podnikových údajov v dokumente.

- **Data_SrcDoc_Ext:string** – prípona dokumentu.

- **Data_SrcDoc_Extension:string** – prípona dokumentu.

- **Data_SrcDoc_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona).

- **Data_SrcDoc_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365.

- **Data_SrcDoc_FqdnHash:string** – hodnota hash miesta uloženia dokumentu. 

- **Data_SrcDoc_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa.

- **Data_SrcDoc_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov.

- **Data_SrcDoc_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument.

- **Data_SrcDoc_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.).
    
- **Data_SrcDoc_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

- **Data_SrcDoc_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument).

- **Data_SrcDoc_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS.

- **Data_SrcDoc_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäti.

- **Data_SrcDoc_IsSyncBacked:bool** – otvára sa dokument z priečinka, ktorý používa aplikáciu synchronizácie zálohovania OneDrivu?

- **Data_SrcDoc_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.).

- **Data_SrcDoc_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.).

- **Data_SrcDoc_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu.

- **Data_SrcDoc_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu).

- **Data_SrcDoc_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.).

- **Data_SrcDoc_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude.

- **Data_SrcDoc_ServerDocId:string** – nezmeniteľný identifikátor pre dokumenty uložené v cloude.

- **Data_SrcDoc_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.).

- **Data_SrcDoc_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI).

- **Data_SrcDoc_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16.

- **Data_SrcDoc_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu.

- **Data_SrcDoc_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

- **Data_SrcDoc_SizeInBytes:long** – veľkosť dokumentu v bajtoch.

- **Data_SrcDoc_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu.

- **Data_SrcDoc_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“.

- **Data_SrcDoc_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný).

- **Data_SrcDoc_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude.

- **Data_SrcDoc_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa.

- **Data_SrcDoc_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“.

- **Data_StopwatchDuration:long** – celkový čas aktivity.

- **Data_TypeOfSaveDialog:long** – preddefinovaná množina hodnôt dialógového okna (RUN_SAVEAS_DLG,RUN_SAVEMEDIA_DLG, RUN_SAVEAS_VIDEO_DLG atď.).

- **Doc** – aktuálny dokument na uloženie.

- **DstDoc** – nové umiestnenie dokumentu (v prípade akcie Uložiť ako).

- **SrcDoc** – pôvodné umiestnenie dokumentu (v prípade akcie Uložiť ako).

#### <a name="officepowerpointpptmacshellprintinfo"></a>Office.PowerPoint.PPT.Mac.Shell.PrintInfo

Zhromažďujú sa vždy, keď sa dokončí operácia tlače PDF súboru alebo exportovania PDF súboru a obsahuje informácie o type rozloženia, ako aj úspešnosti operácie. Tieto informácie sú kritické pri identifikácii úspešnosti operácií tlače PDF súborov a exportu PDF súborov pre našu aplikáciu.

Zhromažďujú sa tieto polia:

- **Data_ExportAsPDFSucceed** – boolovská hodnota označujúca, či bol export PDF súboru úspešný.

- **Data_SavePrintLayoutType** – typ rozloženia pri tlači v čase začatia operácie tlače alebo exportu.


#### <a name="officepowerpointpptsharedslideshowfailure"></a>Office.PowerPoint.PPT.Shared.SlideShow.Failure

Zhromažďuje informácie o zlyhaniach počas prezentácie ako kľúčovej funkcie pre PowerPoint. Spoločnosť Microsoft zhromažďuje tieto údaje v prípade výskytu chyby počas prezentácie na zlepšenie používateľského prostredia prezentácie. Spoločnosť Microsoft používa tieto údaje na získanie diagnostických informácií o tom, kde chyba sa vyskytuje, keď používateľ používa prezentáciu.

Zhromažďujú sa tieto polia:

- **CountOArtErrors** – celkový počet chýb v OArt

- **CountOtherErrors** – zobrazuje celkový počet ostatných chýb

- **CountPPTErrors** – celkový počet chýb v PPT

- **CountSlideShowErrors** – celkový počet chýb prezentácie

- **FirstOArtError** – prvý výskyt chyby v OArt

- **FirstOtherError** – prvý výskyt chyby v inej oblasti

- **FirstPPTError** – prvý výskyt chyby v PPT

- **FirstSlideShowError** – prvý výskyt chyby v prezentácii

    
#### <a name="officepowerpointrunprintoperation"></a>Office.PowerPoint.RunPrintOperation

Zhromažďujú sa vždy, keď sa dokončí operácia tlače PDF súboru a obsahuje informácie o type rozloženia, použití čísel snímok, ako aj úspešnosti operácie. Tieto informácie sú kritické pri identifikácii úspešnosti operácií tlače PDF súborov pre našu aplikáciu.

Zhromažďujú sa tieto polia:

- **Data_PrintWithSlideNumbers** – boolovská hodnota označujúca, či používateľ tlačí s číslami snímok.

- **Data_SavePrintLayoutType** – typ rozloženia pri tlači v čase začatia operácie tlače alebo exportu.

- **Data_Success** – boolovská hodnota označujúca, či bola tlač úspešná.


#### <a name="officeprojectprojectfilesave"></a>Office.Project.ProjectFileSave

Project uloží súbor. Táto udalosť označuje uloženie v Projecte. Umožňuje spoločnosti Microsoft merať úspešnosť Projectu pri ukladaní súboru, čo je dôležité, aby nedochádzalo k stratám údajov dokumentu.

Zhromažďujú sa tieto polia:

  - **Data\_TriggerTime** – čas uloženia

  - **Data\_FileType** – typ súboru, v ktorom sa projekt uloží
 
#### <a name="officesessionactivitystart"></a>Office.Session.Activity.Start

Umožňuje zistiť, kedy sa spustila relácia doplnku Data Streamer.  Umožňuje sledovanie stavu funkcie a monitorovanie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Activity_Name** – názov aktivity „Session“

- **Activity_CV** – ID na koreláciu udalostí počas relácie pripojenia

- **Activity_StartStopType** – spustenie

- **Activity_DateTimeTicks** – dátum a čas aktivity

#### <a name="officesessionactivitystop"></a>Office.Session.Activity.Stop

Umožňuje zistiť, kedy sa skončila relácia doplnku Data Streamer. Používa sa na sledovanie stavu funkcie a monitorovanie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Activity_Name** – názov aktivity „Session“

- **Activity_CV** – ID na koreláciu udalostí počas relácie pripojenia

- **Activity_StartStopType** – zastavenie

- **Activity_DateTimeTicks** – dátum a čas aktivity

#### <a name="officestreamdeviceactivitystart"></a>Office.StreamDevice.Activity.Start

Umožňuje zistiť, či je začiatok streamovania zdroja údajov úspešný.   Umožňuje sledovanie stavu funkcie a monitorovanie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Datasource_Type** -informácia o sériovom zariadení alebo službe aplikácie

- **DataSource_Name** – názov pripojeného zdroja údajov

- **Activity_Name** – názov aktivity „StreamDeviceData“ alebo „StreamFileData“

- **Activity_CV** – ID na koreláciu udalostí počas relácie pripojenia

- **Activity_StartStopType** – spustenie

- **Activity_DateTimeTicks** – dátum a čas aktivity

#### <a name="officestreamdeviceactivitystop"></a>Office.StreamDevice.Activity.Stop

Umožňuje zistiť, či je koniec streamovania zdroja údajov úspešný.   Umožňuje sledovanie stavu funkcie a monitorovanie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Datasource_Type** -informácia o sériovom zariadení alebo službe aplikácie

- **DataSource_Name** – názov pripojeného zdroja údajov

- **Activity_Name** – názov aktivity „StreamDeviceData“ alebo „StreamFileData“

- **Activity_CV** – ID na koreláciu udalostí počas relácie pripojenia

- **Activity_StartStopType** – zastavenie

- **Activity_DateTimeTicks** – dátum a čas aktivity

#### <a name="officetargetedmessagingabexperimentmessagetrigger"></a>Office.TargetedMessaging.ABExperimentMessageTrigger

Sleduje počet používateľov, ktorí prijímajú správy BizBar a správy dynamického plátna zo služby TargetedMessagingService (TMS). Tieto údaje sú veľmi dôležité pri zisťovaní, aké správy používatelia dostávajú a na akom povrchu, aby sme mohli zabezpečiť, že dostanú všetky správy, ktoré pre nich môžu byť dôležité v súvislosti s ďalším používaním produktu. Tiež sú potrebné na presné meranie úspešnosti našich experimentov a kampaní spustených prostredníctvom TMS.

Zhromažďujú sa tieto polia:

  - **Data\_Surface** – názov povrchu, pre ktorý je táto správa doručená službou určená

  - **Data\_Flight** – identifikátor skupiny funkcií ECS/CT, ktorý sa použil na doručenie tejto správy

  - **Data\_CampaignId** – identifikátor kampane, ktorej je táto správa súčasťou

  - **Data\_MessageId** – identifikátor tejto správy doručenej službou

  - **Data\_TransactionId** – identifikátor tejto transakcie so službou

  - **Data\_TriggerPoint** – krok, v ktorom bola táto udalosť zaznamenaná (prijatie správy, zobrazenie správy)

#### <a name="officetextfontpickerfontselectedwin32"></a>Office.Text.FontPickerFontSelected.Win32

Táto udalosť označuje, či bolo stiahnuté písmo vykreslené správne. Používa sa na označenie úspešnosti alebo zlyhania stiahnutia písma.

Zhromažďujú sa tieto polia:

  - **Názov písma (Data\_Font)** – názov písma vybratého vo výbere písma

  - **Kliknutie používateľa (Data\_FClick)** – označuje výber položky používateľom pomocou myši

#### <a name="officetextresourceclientrequestresourceinternal"></a>Office.Text.ResourceClient.RequestResourceInternal

Táto udalosť označuje, či bolo písmo stiahnuté správne. Používa sa na označenie úspešnosti alebo zlyhania vykreslenia stiahnutého písma.

Zhromažďujú sa tieto polia:

  - **Data\_FontToken** – názov súboru prostriedkov, ktorý sa uloží

  - **Data\_HTTPResult** – výsledok požiadavky HTTP

  - **Data\_HTTPStatusCode** – kód HTTP vrátený z požiadavky HTTP

  - **Data\_isInternetOn** – či sme mali pripojenie pri pokuse o načítanie zdroja

  - **Data\_RequestUrl** – URL adresu zdroja CDN, ktorý sa pokúšame načítať



#### <a name="officetranslatordocumenttranslated"></a>Office.Translator.DocumentTranslated

Zhromažďuje informácie o úspešnosti alebo zlyhaní prekladu celého dokumentu pomocou používateľského spúšťača v službe Translator SDX. Je to veľmi dôležité na vyhodnotenie stavu funkcie prekladača a reagovanie na všetky výpadky, ktoré sa môžu vyskytnúť. Monitoruje stav scenára „Preložiť dokument“ vo Worde.

Zhromažďujú sa tieto polia:

- **Data.actionSource** – ako bol spustený preklad vybratého textu.

- **Data.bodyBackgroundColor** – farba pozadia kontajnera motívu balíka Office.

- **Data.bodyForegroundColor** – farba popredia kontajnera motívu balíka Office.

- **Data.browserLang** – jazyk aktuálneho zobrazenia prehliadača.

- **Data.browserOnline** – zastarané.

- **Data.browserPlatform** – platforma prehliadača.

- **Data.browserUserAgent** – agent používateľa prehliadača.

- **Data.colorDepth** – hĺbka systémovej farby.

- **Data.contentLanguage** – zistený jazyk obsahu, ktorý sa má preložiť.

- **Data.controlBackgroundColor** – farba pozadia ovládacieho prvku motívu balíka Office.

- **Data.controlForegroundColor** – farba popredia ovládacieho prvku motívu balíka Office.

- **Data.correlationId** – jedinečný identifikátor požiadavky odoslanej do služby.

- **Data.crossSessionId** – jedinečný identifikátor používateľa.

- **Data.crossSessionStartTime** – časová pečiatka UTC spustenia relácie prekladu.

- **Data.currentTime** – časová pečiatka UTC odoslania správy telemetrie.

- **Data.displayLanguage** – jazyk zobrazenia balíka Office.

- **Data.documentSourceLang** – jazyk obsahu dokumentu.

- **Data.documentTargetLang** – jazyk, do ktorého sa preloží dokument.

- **Data.environment** – prostredie služby, kam je požiadavka odoslaná.

- **Data.errorMessage** – chybové hlásenie poskytnuté službou.

- **Data.eventActionType** – typ udalosti telemetrie.

- **Data.eventTagId"** – jedinečný identifikátor riadka kódu, ktorý vytvoril túto správu telemetrie.

- **Data.flights** – povolené skupiny funkcií.

- **Data.fileSize** – veľkosť wordového súboru, ktorý sa má preložiť.

- **Data.fileSource** – miesto, kde je wordový súbor hosťovaný (offline, online).

- **Data.fileType** – prípona wordového súboru.

- **Data.innerHeight** – výška kontajnera bočnej tably.

- **Data.innerWidth** – šírka kontajnera bočnej tably.

- **Data.lookupSourceLang** – nepoužíva sa v prípade prekladu dokumentu.

- **Data.lookupTargetLang** – nepoužíva sa v prípade prekladu dokumentu.

- **Data.officeHost** – aplikácia balíka Office, ktorá hosťuje bočnú tablu.

- **Data.officeLocale** – jazyk používateľa balíka Office.

- **Data.officeMachineId** – jedinečný identifikátor zariadenia.

- **Data.officePlatform** – platforma zariadenia.

- **Data.officeSessionId** – identifikátor relácie balíka Office.

- **Data.officeUserId** – jedinečný identifikátor používateľa balíka Office.

- **Data.officeVersion** – verzia balíka Office.

- **Data.pageXOffset** – vodorovná poloha posúvania bočnej tably z ľavej strany tably.

- **Data.pageYOffset** – zvislá poloha posúvania bočnej tably z hornej strany tably.

- **Data.pixelDepth** – farebné rozlíšenie obrazovky.

- **Data.responseCode** – kód odpovede na požiadavku zo služby.

- **Data.responseTime** – uplynutý čas požiadavky. 

- **Data.resultType** – výsledok požiadavky.

- **Data.screenHeight** – výška obrazovky v pixeloch.

- **Data.screenLeft** – vodorovná súradnica okna vo vzťahu k obrazovke.

- **Data.screenTop** – zvislá súradnica okna vo vzťahu k obrazovke.

- **Data.screenWidth** – šírka obrazovky v pixeloch.

- **Data.selectedTab** – označuje, či je vybratá karta výberu alebo dokumentu.

- **Data.serverUrl** – URL adresa prekladateľskej služby.

- **Data.sessionId** – identifikátor relácie bočnej tably.

- **Data.sessionStartTime** – časová pečiatka UTC spustenia relácie prekladu.

- **Data.sourceTextHash** – hodnota hash textu na preklad.

- **Data.sourceTextLength** – dĺžka textu na preklad.

- **Data.sourceTextWords** – počet slov v texte na preklad.

- **Data.warningMessage** – upozorňujúca správa hlásená službou.


#### <a name="officetranslatortexttranslated"></a>Office.Translator.TextTranslated

Zhromažďuje informácie o úspešnosti alebo zlyhaní prekladu výberu, ktorý sa spustí akciou používateľa v službe Translator SDX. Je to veľmi dôležité na vyhodnotenie stavu funkcie prekladača a reagovanie na všetky výpadky, ktoré sa môžu vyskytnúť. Používa na monitorovanie stavu scenára „Preložiť vybratý text“ v Exceli, v PowerPointe a vo Word.

Zhromažďujú sa tieto polia:

- **Data.actionSource** – ako bol spustený preklad vybratého textu.

- **Data.bodyBackgroundColor** – farba pozadia kontajnera motívu balíka Office.

- **Data.bodyForegroundColor** – farba popredia kontajnera motívu balíka Office.

- **Data.browserLang** – jazyk aktuálneho zobrazenia prehliadača.

- **Data.browserOnline** – zastarané.

- **Data.browserPlatform** – platforma prehliadača.

- **Data.browserUserAgent** – agent používateľa prehliadača.

- **Data.colorDepth** – hĺbka systémovej farby.

- **Data.contentLanguage** – zistený jazyk obsahu, ktorý sa má preložiť.

- **Data.controlBackgroundColor** – farba pozadia ovládacieho prvku motívu balíka Office.

- **Data.controlForegroundColor** – farba popredia ovládacieho prvku motívu balíka Office.

- **Data.correlationId** – jedinečný identifikátor požiadavky odoslanej do služby.

- **Data.crossSessionId** – jedinečný identifikátor používateľa.

- **Data.crossSessionStartTime** – časová pečiatka UTC spustenia relácie prekladu.

- **Data.currentTime** – časová pečiatka UTC odoslania správy telemetrie.

- **Data.displayLanguage** – jazyk zobrazenia balíka Office.

- **Data.documentSourceLang** – nepoužíva sa v prípade vybratého textu.

- **Data.documentTargetLang** – nepoužíva sa v prípade vybratého textu.

- **Data.environment** – prostredie služby, kam je požiadavka odoslaná.

- **Data.errorMessage** – chybové hlásenie poskytnuté službou.

- **Data.eventActionType** – typ udalosti telemetrie.

- **Data.eventTagId"** – jedinečný identifikátor riadka kódu, ktorý vytvoril túto správu telemetrie.

- **Data.flights** – povolené skupiny funkcií.

- **Data.innerHeight** – výška kontajnera bočnej tably.

- **Data.innerWidth** – šírka kontajnera bočnej tably.

- **Data.lookupSourceLang** – jazyk aktuálne vybratého textu.

- **Data.lookupTargetLang** – jazyk, do ktorého sa aktuálne vybratý text preloží.

- **Data.officeHost** – aplikácia balíka Office, ktorá hosťuje bočnú tablu.

- **Data.officeLocale** – jazyk používateľa balíka Office.

- **Data.officeMachineId** – jedinečný identifikátor zariadenia.

- **Data.officePlatform** – platforma zariadenia.

- **Data.officeSessionId** – identifikátor relácie balíka Office.

- **Data.officeUserId** – jedinečný identifikátor používateľa balíka Office.

- **Data.officeVersion** – verzia balíka Office.

- **Data.pageXOffset** – vodorovná poloha posúvania bočnej tably z ľavej strany tably.

- **Data.pageYOffset** – zvislá poloha posúvania bočnej tably z hornej strany tably.

- **Data.pixelDepth** – farebné rozlíšenie obrazovky.

- **Data.responseCode** – kód odpovede na požiadavku zo služby.

- **Data.responseTime** – uplynutý čas požiadavky.

- **Data.resultType** – výsledok požiadavky.

- **Data.screenHeight** – výška obrazovky v pixeloch.

- **Data.screenLeft** – vodorovná súradnica okna vo vzťahu k obrazovke.

- **Data.screenTop** – zvislá súradnica okna vo vzťahu k obrazovke.

- **Data.screenWidth** – šírka obrazovky v pixeloch.

- **Data.selectedTab** – označuje, či je vybratá karta výberu alebo dokumentu.

- **Data.serverUrl** – URL adresa prekladateľskej služby.

- **Data.sessionId** – identifikátor relácie bočnej tably.

- **Data.sessionStartTime** – časová pečiatka UTC spustenia relácie prekladu.

- **Data.sourceTextHash** – hodnota hash textu na preklad.

- **Data.sourceTextLength** – dĺžka textu na preklad.

- **Data.sourceTextWords** – počet slov v texte na preklad.

- **Data.warningMessage** – upozorňujúca správa hlásená službou.

#### <a name="officewordexperimentationdocumentstatsoncloseandsuspend"></a>Office.Word.Experimentation.DocumentStatsOnCloseAndSuspend

Táto udalosť zaznamenáva štatistické údaje dokumentu pre každý dokument, keď sa Office Word zavrie alebo pozastaví.  Udalosť sa používa na koreláciu úprav dokumentu, veľkosti dokumentu atď. s chybami ukladania dokumentu, zdieľania dokumentu a online spolupráce na dokumente.

Zhromažďujú sa tieto polia:

- **Data_BkmkRefCount** – počet odkazov na záložky v dokumente.

- **Data_CharacterCount** – počet znakov v dokumente.

- **Data_CharactersWithSpaceCount** – počet znakov vrátane medzier v dokumente.

- **Data_ChartCount** – počet grafov v dokumente.

- **Data_CitationCount** – počet citácií v dokumente.

- **Data_DocumentLocation** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_ETW_TrackbackTag** – identifikuje miesto v kóde, z ktorého sa táto udalosť spustila (zatvorenie alebo pozastavenie).

- **Data_EndnoteDocCount** – počet vysvetliviek v dokumente.

- **Data_FootnoteDocCount** – počet poznámok pod čiarou v dokumente.

- **Data_HasBibliography** – označuje, či dokument obsahuje bibliografiu.

- **Data_HasHeader** – označuje, či dokument obsahuje hlavičku.

- **Data_IsImeUsed** – označuje, či bol v dokumente použitý editor IME.

- **Data_IsPageCountInProgress** – označuje, či sa momentálne spracúva počet strán v dokumente..
    
- **Data_IsTouchUsed** – označuje, či bol v dokumente použitý dotykový vstup.

- **Data_IsTrackChangesOn** – označuje, či bolo v dokumente zapnuté sledovanie zmien.

- **Data_LineCount** – počet riadkov v dokumente.

- **Data_MainPdod** – identifikátor dokumentu v procese programu Office Word.

- **Data_PageCount** – počet strán v dokumente.

- **Data_PageNumberFieldCount** – počet polí pre číslo strany v dokumente.

- **Data_ParagraphCount** – počet odsekov v dokumente.

- **Data_PicCount** – počet obrázkov v dokumente.

- **Data_RsidCount** – identifikátor počtu uložených revízií v dokumente.

- **Data_TocCount** – počet obsahov v dokumente.

- **Data_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_UserActionID** – toto údajové pole sa nepoužíva (hodnota je vždy 0).

- **Data_UserActionName** – vždy „DocumentStatsOnCloseAndSuspend“.

- **Data_UserInteractionTimeMsec** – počet milisekúnd, počas ktorých používateľ aktívne pracoval s dokumentom.
    
- **Data_WordCount** – počet slov v dokumente.

#### <a name="officewordfilenewcreatenewfile"></a>Office.Word.FileNew.CreateNewFile

Táto udalosť označuje vytvorenie nového dokumentu v programe Office Word a sleduje úspešnosť alebo zlyhanie tejto operácie. Udalosť sa používa na monitorovanie, či tvorba nového dokumentu funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

  - **Data\_DirtyState** – či bol dokument vytvorený v zmenenom stave (so zmenami, ktoré je potrebné uložiť)

  - **Data\_ErrorID** – identifikátor chyby v prípade zlyhania operácie

  - **Data\_MainPdod** – identifikátor dokumentu počas tejto relácie procesu

  - **Data\_UsesCustomTemplate** – označuje, či bol dokument vytvorený pomocou vlastnej šablóny

#### <a name="officewordfilesaveactcmdgosubsaveas"></a>Office.Word.FileSave.ActCmdGosubSaveAs

Táto udalosť označuje, že používateľ ukladá zmeny do nového dokumentu. Udalosť monitoruje, či ukladanie do nového dokumentu funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov.

- **Data_DetachedDuration** – ako dlho bola aktivita odpojená od vlákna.

- **Data_Doc_AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť.

- **Data_Doc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.
    
- **Data_Doc_ChunkingType** – jednotky slúžiace na prírastkové otvorenie dokumentu.

- **Data_Doc_EdpState** – nastavenie ochrany elektronických údajov dokumentu.

- **Data_Doc_Ext** prípona dokumentu (docx, xlsb, pptx atď.)

- **Data_Doc_FileFormat** – verzia protokolu formátu súboru.

- **Data_Doc_Fqdn** – názov domény OneDrivu alebo SharePointu Online.

- **Data_Doc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – zaznamenáva, ako bol dokument otvorený.

- **Data_Doc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_Doc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.
    
- **Data_Doc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_Doc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.
    
- **Data_Doc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_Doc_IsRtcAlwaysOn** – má hodnotu true, ak je kanál v reálnom čase (RTC) pre tento súbor vždy zapnutý.

- **Data_Doc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_Doc_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_Doc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_Doc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_Doc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie.

- **Data_Doc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_Doc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_Doc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).

- **Data_Doc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_Doc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_Doc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_Doc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_Doc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_Doc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_Doc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_Doc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_EditorDisablingRename** – identifikátor prvého editora, ktorý spôsobil vypnutie možnosti premenovania.

- **Data_EditorsCount** – počet editorov v dokumente.

- **Data_LastLoggedTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie, keď pokus o uloženie zlyhá dvakrát (používa sa na diagnostiku kvality údajov).

- **Data_MoveDisabledReason** – chyba, pri ktorej sa vypne možnosť premiestnenia dokumentu.

- **Data_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania.

- **Data_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania dokumentu.

- **Data_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania.

    
#### <a name="officewordfilesaveactfconfirmsavedoccoreautorecoverysave"></a>Office.Word.FileSave.ActFConfirmSaveDocCoreAutoRecoverySave

Táto udalosť označuje, že Office Word ukladá automaticky obnovený dokument, ktorý ešte nebol uložený. Umožňuje spoločnosti Microsoft zisťovať chyby automatického obnovenia, čo je dôležité pre bezpečnosť údajov v dokumente.  Udalosť monitoruje, či ukladanie automaticky obnoveného dokumentu funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

- **Data_DetachedDuration** – ako dlho bola aktivita odpojená od vlákna.

- **Data_Doc_AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť.

- **Data_Doc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.
    
- **Data_Doc_ChunkingType** – jednotky slúžiace na prírastkové otvorenie dokumentu.

- **Data_Doc_EdpState** – nastavenie ochrany elektronických údajov dokumentu.

- **Data_Doc_Ext** prípona dokumentu (docx, xlsb, pptx atď.)

- **Data_Doc_FileFormat** – verzia protokolu formátu súboru.

- **Data_Doc_Fqdn** – názov domény OneDrivu alebo SharePointu Online.

- **Data_Doc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – zaznamenáva, ako bol dokument otvorený.

- **Data_Doc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_Doc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.

- **Data_Doc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_Doc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.
    
- **Data_Doc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_Doc_IsRtcAlwaysOn** – má hodnotu true, ak je kanál v reálnom čase (RTC) pre tento súbor vždy zapnutý.

- **Data_Doc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_Doc_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_Doc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_Doc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_Doc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie.

- **Data_Doc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_Doc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_Doc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).

- **Data_Doc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_Doc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_Doc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_Doc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_Doc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_Doc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_Doc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_Doc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_Doc_WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI.

- **Data_FailureClass** – celé číslo predstavujúce triedu zlyhania pri zlyhaniach prechodu na OCS.
    
- **Data_MainPdod** – identifikátor dokumentu v procese programu Office Word.

- **Data_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania.

- **Data_OCSSyncbackSaveStarted** – príznak, ktorý označuje, že toto uloženie súvisí s uložením so synchronizáciou zálohovania.

- **Data_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania tohto dokumentu.

- **Data_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania.

- **Data_SaveInitiateKind** – celé číslo, ktoré označuje spôsob spustenia ukladania.

- **Data_SrcDocIsUnnamedOrNew** – označuje, či ukladaný dokument je nový.


#### <a name="officewordfilesaveactfconfirmsavedoccorequerysave"></a>Office.Word.FileSave.ActFConfirmSaveDocCoreQuerySave

Táto udalosť označuje, že Office Word zobrazí používateľovi výzvu na uloženie zmien pri pokuse o zatvorenie dokumentu. Umožňuje spoločnosti Microsoft monitorovať, či ukladanie pri ukončení funguje podľa očakávaní, aby nedochádzalo k strate údajov dokumentu. Udalosť monitoruje, či ukladanie pri ukončení funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov.

- **Data_DetachedDuration** – ako dlho bola aktivita odpojená od vlákna.

- **Data_Doc_AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť.

- **Data_Doc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_Doc_ChunkingType** – jednotky slúžiace na prírastkové otvorenie dokumentu.

- **Data_Doc_EdpState** – nastavenie ochrany elektronických údajov dokumentu.

- **Data_Doc_Ext** prípona dokumentu (docx, xlsb, pptx atď.)

- **Data_Doc_FileFormat** – verzia protokolu formátu súboru.

- **Data_Doc_Fqdn** – názov domény OneDrivu alebo SharePointu Online.

- **Data_Doc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – zaznamenáva, ako bol dokument otvorený.

- **Data_Doc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_Doc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.

- **Data_Doc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_Doc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.
    
- **Data_Doc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_Doc_IsRtcAlwaysOn** – má hodnotu true, ak je kanál v reálnom čase (RTC) pre tento súbor vždy zapnutý.

- **Data_Doc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_Doc_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_Doc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_Doc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_Doc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie.

- **Data_Doc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_Doc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_Doc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).

- **Data_Doc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_Doc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_Doc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_Doc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_Doc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_Doc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_Doc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_Doc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_Doc_WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI.

- **Data_DstDoc_AccessMode** – označuje, či je cieľový dokument iba na čítanie alebo editovateľný.

- **Data_DstDoc_EdpState** – nastavenie ochrany elektronických údajov cieľového dokumentu.

- **Data_DstDoc_Ext** – prípona cieľového dokumentu (docx, xlsb, pptx atď.).

- **Data_DstDoc_FileFormat** – verzia protokolu formátu súboru cieľového dokumentu.

- **Data_DstDoc_Location** – označuje, ktorá služba poskytne ukladací priestor pre cieľový dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_DstDoc_LocationDetails** – označuje, ktorý známy lokálny priečinok uložil cieľový dokument.

- **Data_DstDoc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_DstDoc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu pre cieľový dokument.

- **Data_FailureClass** – celé číslo predstavujúce triedu zlyhania pri zlyhaniach prechodu na OCS.

- **Data_LocationPickerSaveStatus** – celočíselná hodnota označujúca akciu, ktorá spustila uloženie z dialógového okna Uložiť pri skončení.

- **Data_MainPdod** – identifikátor dokumentu v procese programu Office Word.

- **Data_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania.

- **Data_OCSSyncbackSaveStarted** – príznak, ktorý označuje, že toto uloženie súvisí s uložením so synchronizáciou zálohovania. 

- **Data_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania tohto dokumentu.

- **Data_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania.

- **Data_SaveInitiateKind** – celé číslo, ktoré označuje spôsob spustenia ukladania.

- **Data_SrcDocIsUnnamedOrNew** – označuje, či ukladaný dokument je nový.


#### <a name="officewordfilesavesaveassavefile"></a>Office.Word.FileSave.SaveAsSaveFile

Táto udalosť označuje, že Office Word ukladá dokument do nového dokumentu. Umožňuje spoločnosti Microsoft zisťovať chyby funkcie Uložiť ako, čo je dôležité na zabránenie strate údajov dokumentu. Udalosť monitoruje, či funkcia Uložiť ako funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov.

- **Data_AddDocTelemResDst** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti pre cieľový dokument. Používa sa na diagnostiku kvality údajov.

- **Data_AddDocTelemResSrc** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti pre zdrojový dokument. Používa sa na diagnostiku kvality údajov.

- **Data_DetachedDuration** – ako dlho bola aktivita odpojená od vlákna.

- **Data_Doc_AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť.

- **Data_Doc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_Doc_ChunkingType** – jednotky slúžiace na prírastkové otvorenie dokumentu.

- **Data_Doc_EdpState** – nastavenie ochrany elektronických údajov dokumentu.

- **Data_Doc_Ext** prípona dokumentu (docx, xlsb, pptx atď.)

- **Data_Doc_FileFormat** – verzia protokolu formátu súboru.

- **Data_Doc_Fqdn** – názov domény OneDrivu alebo SharePointu Online.

- **Data_Doc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_Doc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.

- **Data_Doc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_Doc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.

- **Data_Doc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_Doc_IsRtcAlwaysOn** – má hodnotu true, ak je kanál v reálnom čase (RTC) pre tento súbor vždy zapnutý.

- **Data_Doc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_Doc_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_Doc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_Doc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_Doc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_Doc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_Doc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).

- **Data_Doc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_Doc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_Doc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_Doc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_Doc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_Doc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_Doc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_DstDoc_AccessMode** – označuje, či je cieľový dokument iba na čítanie alebo editovateľný.

- **Data_DstDoc_AssistedReadingReasons** – preddefinovaná množina hodnôt toho, prečo bol cieľový dokument otvorený v režime asistovaného čítania.
    
- **Data_DstDoc_ChunkingType** – jednotky slúžiace na prírastkové otvorenie dokumentu.

- **Data_DstDoc_EdpState** – nastavenie ochrany elektronických údajov cieľového dokumentu.

- **Data_DstDoc_Ext** prípona dokumentu (docx, xlsb, pptx atď.).

- **Data_DstDoc_FileFormat** – verzia protokolu formátu súboru.

- **Data_DstDoc_Fqdn** – názov domény OneDrivu alebo SharePointu Online pre cieľový dokument.

- **Data_DstDoc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény pre cieľový dokument.

- **Data_DstDoc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_DstDoc_InitializationScenario** – zaznamenáva, ako bol cieľový dokument otvorený.

- **Data_DstDoc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností otvorenej požiadavky pre cieľový dokument.
    
- **Data_DstDoc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre cieľový dokument alebo používateľa.

- **Data_DstDoc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_DstDoc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.

- **Data_DstDoc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_DstDoc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_DstDoc_Location** – označuje, ktorá služba poskytla ukladací priestor pre cieľový dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_DstDoc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_DstDoc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_DstDoc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie pre cieľový dokument.

- **Data_DstDoc_ReadOnlyReasons** – dôvody, prečo bol cieľový dokument otvorený iba na čítanie. 

- **Data_DstDoc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_DstDoc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_DstDoc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_DstDoc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).
    
- **Data_DstDoc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_DstDoc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_DstDoc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_DstDoc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_DstDoc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_DstDoc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_DstDoc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_DstDoc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu pre cieľový dokument.
    
- **Data_DstDoc_WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI.

- **Data_FailureClass** – celé číslo predstavujúce triedu zlyhania pri zlyhaniach prechodu na OCS.

- **Data_LocationPickerPropagateToSaveTime,spLapsedMsec** – čas v milisekundách, ktorý trvalo, kým sa spustilo ukladanie po získaní výsledku z okna výberu umiestnenia.

- **Data_LocationPickerSaveStatus** – stav vrátený oknom na výber umiestnenia.

- **Data_MainPdod** – identifikátor dokumentu v procese programu Office Word.

- **Data_MoveDisabledReason** – chyba, pri ktorej sa vypne možnosť premiestnenia dokumentu.

- **Data_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania.

- **Data_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania tohto dokumentu.

- **Data_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania.

- **Data_SaveInitiateKind** – celé číslo, ktoré označuje spôsob spustenia ukladania.

- **Data_SrcDoc_AccessMode** – označuje, či je zdrojový dokument iba na čítanie alebo editovateľný.

- **Data_SrcDoc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_SrcDoc_ChunkingType** – jednotky slúžiace na prírastkové otvorenie dokumentu.

- **Data_SrcDoc_EdpState** – nastavenie ochrany elektronických údajov zdrojového dokumentu.

- **Data_SrcDoc_Ext** – prípona zdrojového dokumentu (docx, xlsb, pptx atď.).

- **Data_SrcDoc_FileFormat** – verzia protokolu formátu súboru zdrojového dokumentu.

- **Data_SrcDoc_Fqdn** – názov domény OneDrivu alebo SharePointu Online pre zdrojový dokument.

- **Data_SrcDoc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény pre zdrojový dokument.

- **Data_SrcDoc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_SrcDoc_InitializationScenario** – zaznamenáva, ako bol dokument otvorený.

- **Data_SrcDoc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_SrcDoc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.

- **Data_SrcDoc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_SrcDoc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.

- **Data_SrcDoc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_SrcDoc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.
    
- **Data_SrcDoc_Location** – označuje, ktorá služba poskytla zdrojový dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_SrcDoc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_SrcDoc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_SrcDoc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie.

- **Data_SrcDoc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_SrcDoc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_SrcDoc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_SrcDoc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_SrcDoc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).

- **Data_SrcDoc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_SrcDoc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_SrcDoc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_SrcDoc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_SrcDoc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_SrcDoc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_SrcDoc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_SrcDoc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_SrcDoc_WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI.

- **Data_SrcDocIsUnnamedOrNew** – označuje, či ukladaný dokument je nový.


#### <a name="officevisiosharedfeatureexperimentation"></a>Office.Visio.Shared.FeatureExperimentation

Táto udalosť sleduje zoskupovanie funkcií pre používateľov. Pomáha nám určiť úspech alebo neúspech skupín funkcií.

Zhromažďujú sa tieto polia:

  - **Data\_Enable:bool** – hodnota true označuje, že funkcia je povolená pre aktuálneho používateľa

  - **Data\_Feature:string** – názov funkcie

  - **Data\_Flighted:bool** – hodnota true označuje, že funkcia je povolená

  - **Data\_Licensed:bool** – hodnota true označuje, že na funkciu sa vzťahuje kontrola licencie

  - **Data\_Subscriber:bool** – hodnota true označuje, že používateľ má predplatenú licenciu

#### <a name="officevisiosharedrefreshsmartdiagram"></a>Office.Visio.Shared.RefreshSmartDiagram

Táto udalosť zachytáva zlyhania obnovenia diagramu, keď je súbor vytvorený cez DV. Pomáha nám to ladiť zlyhania a problémy v obnovení údajov v diagrame DV.

Zhromažďujú sa tieto polia:

  - **Data\_ConnectorsBasedOnSequence:bool** – má hodnotu true, ak obnovený diagram bol pôvodne vytvorený pomocou konektora na základe možnosti postupnosti

  - **Data\_DialogError**:**string** – chyba počas obnovovania inteligentného diagramu

  - **Data\_FileError:string** – reťazec chyby, keď pripojený excelový súbor je neplatný

  - **Data\_OverwriteSelected**:**bool** – má hodnotu true, ak používateľ počas obnovenia vybral možnosť prepísania diagramu

  - **Data\_WarningShown**:**bool** – má hodnotu true, ak sa počas obnovenia údajov používateľovi zobrazila nejaká výstraha

#### <a name="officevisiosharedwritebacktoexcel"></a>Office.Visio.Shared.WritebackToExcel

Táto udalosť zachytáva zlyhania spätného zapisovania Excelu, keď je súbor vytvorený cez DV. Pomáha nám to ladiť zlyhania a problémy v spätnom zapisovaní údajov do Excelu v diagrame DV.

Zhromažďujú sa tieto polia:

  - **Data\_ConnectorsBasedOnSequence:bool** – hodnota true znamená, že konektory sú vytvorené na základe nastavení postupnosti

  - **Data\_DataSourceType:string** – toto pole označuje, či je diagram vytvorený z tabuľky alebo z vlastného rozsahu

  - **Data\_DialogError:string** – typ vlastnej chyby počas vytvárania inteligentného diagramu prostredníctvom Excelu

  - **Data\_NoOfShapesAdded:int** – počet tvarov pridaných počas funkcie spätného zapisovania do Excelu

  - **Data\_NoOfShapesDeleted:int** – počet tvarov odstránených počas funkcie spätného zapisovania do Excelu

  - **Data\_OverwriteSelected:bool** – má hodnotu true, ak používateľ vybral možnosť prepísania údajov

  - **Data\_SourceDataModified:bool** – hodnota true označuje, že zdrojové údaje sú upravené

  - **Data\_WarningShown:bool** – hodnota true označuje, že používateľovi sa zobrazila výstraha aktualizácie údajov

  - **Data\_WarningShownBecauseOfPresenceOfFormula:bool** – hodnota true označuje, že používateľovi sa zobrazila výstraha z dôvodu prítomnosti vzorca v Exceli

  - **Data\_WarningShownToAddNextStepID:bool** – hodnota true označuje, že používateľovi sa zobrazila výstraha z dôvodu chýbajúceho identifikátora ďalšieho kroku v Exceli

  - **Data\_WarningShownToConvertToTable:bool** – hodnota true označuje, že používateľovi sa zobrazila výstraha na skonvertovanie excelových údajov do tabuľkového formátu

#### <a name="officewordworddocumentdirtyflagchanged"></a>Office.Word.Word.DocumentDirtyFlagChanged

Táto udalosť označuje, že Office Word upravuje dokument, v ktorom sa zmenil interný stav dokumentu na zmenený (dirty). Umožňuje spoločnosti Microsoft vyhodnotiť stav funkcie úpravy dokumentu. Udalosť predstavuje signál úprav používateľa. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac.

Zhromažďujú sa tieto polia:

  - **Data\_CollectionTime** – časová pečiatka udalosti

  - **Data\_DocumentLocation** – typ umiestnenia dokumentu

  - **Data\_DocumentLocationDetails** – podtyp umiestnenia dokumentu

  - **Data\_FAlwaysSaveEnabled** – označuje, či bola povolená možnosť Vždy uložiť

  - **Data\_FirstEditTime** – časová pečiatka prvej úpravy

  - **Data\_NumberCoAuthors** – počet spoluautorov upravujúcich dokument počas relácie

  - **Data\_NumberOfTimesDocumentDirtied** – počet úprav dokumentu

  - **Data\_Pdod** – identifikátor dokumentu v procese programu Office Word

  - **Data\_UrlHash** – hodnota hash cesty dokumentu

  - **Data\_ViewKind** – typ zobrazenia Wordu
### <a name="application-status-and-boot-subtype"></a>*Podtyp Stav aplikácie a podtyp spustenia*

Určenie, či sa vyskytli konkrétne udalosti funkcie, napríklad spustenie alebo ukončenie, a či je funkcia spustená.

#### <a name="officeextensibilityofficejsappactivated"></a>Office.Extensibility.OfficeJS.Appactivated

Táto udalosť zaznamenáva informácie o neočakávaných vypnutiach balíka Office. Umožňuje nám to identifikovať zlyhania alebo nereagovania v produkte, aby ich bolo možné riešiť.

Zhromažďujú sa tieto polia:

  - **Data\_AirspaceInitTime:integer** – čas potrebný na inicializovanie komponentu Airspace balíka Office

  - **Data\_AllShapes:integer** – počet tvarov v dokumente

  - **Data\_APIInitTime:integer** – čas potrebný na inicializovanie modulu API Visia

  - **Data\_AppSizeHeight** – výška okna doplnku

  - **Data\_AppSizeWidth** – šírka okna doplnku

  - **Data\_AppURL** – URL adresa doplnku; zaznamenáva úplnú URL adresu doplnkov z obchodu a URL doménu pre doplnky iné ako z obchodu

  - **Data\_AuthorsCount:integer** – počet autorov, ktorí upravovali dokument v tejto relácií

  - **Data\_BackgroundPages:integer** – počet strán na pozadí v diagrame

  - **Data\_BootTime:integer** – čas potrebný na spustenie Visia

  - **Data\_Browser** – reťazec prehliadača s informáciami o prehliadači, ako sú napríklad typ a verzia

  - **Data\_ChildWindowMixedModeTime:integer** – čas potrebný na zapnutie zmiešaného režimu vo Visiu (podriadené okno môže mať iné DpiAwareness z nadradeného okna)

  - **Data\_CommentsCount:integer** – počet komentárov v dokumente

  - **Data\_ConnectionCount:integer** – počet pripojení údajov v diagrame

  - **Data\_ContentMgrInitTim:integer** –čas potrebný na inicializovanie správcu obsahu

  - **Data\_CreateMainFrameTime:integer** – vytvorenie času hlavného rámu

  - **Data\_CreatePaletteTime:integer** – čas potrebný na vytvorenie globálnej palety farieb

  - **Data\_DispFormatCount:integer** – počet údajových grafík v diagrame

  - **Data\_Doc\_Ext:string** – prípona dokumentu

  - **Data\_Doc\_Fqdn:string** – miesto uloženia dokumentu (SharePoint.com, live.net), k dispozícii len pre domény v Office 365

  - **Data\_Doc\_FqdnHash:string** – hodnota hash miesta uloženia dokumentu

  - **Data\_Doc\_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnutia celého dokumentu)

  - **Data\_Doc\_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäte

  - **Data_Doc_IsRtcAlwaysOn** – má hodnotu true, ak je kanál v reálnom čase (RTC) pre tento súbor vždy zapnutý.

  - **Data\_Doc\_IsSyncBacked:bool** – má hodnotu true, ak ide o serverový dokument, ktorý existuje lokálne a je synchronizovaný so serverom (napr. prostredníctvom klientskej aplikácie OneDrive alebo ODB)

  - **Data\_Doc\_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.)

  - **Data\_Doc\_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive)

  - **Data\_Doc\_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude

  - **Data\_Doc\_ServerDocId:string** – nemenný identifikátor pre dokumenty uložené v cloude

  - **Data\_Doc\_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu

  - **Data\_Doc\_SizeInBytes:long** – veľkosť dokumentu v bajtoch

  - **Data\_Doc\_SpecialChars:long** – dlhá bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu

  - **Data\_Doc\_SyncBackedType** – indikátor typu dokumentu (lokálny alebo v službe) 

  - **Data\_Doc\_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude

  - **Data\_DpiAwarenessTime:integer** – čas potrebný na zapnutie funkcie Per Monitor Dpi Awareness

  - **Data\_DurationToCompleteInMilliseconds:double** – čas potrebný na dokončenie funkcie Uložiť ako v milisekundách

  - **Data\_ErrorCode:int** – 0 pre úspech, celé číslo pre zlyhanie pri ukladaní

  - **Data\_FailureReason:integer** – dôvod zlyhania asynchrónneho ukladania

  - **Data\_FileExtension** – prípona súboru otvoreného diagramu

  - **Data\_FileHasDGMaster:bool** – má hodnotu true, keď súbor obsahuje údajovú grafiku

  - **Data\_FileHasImportedData:bool** – má hodnotu true, keď súbor obsahuje importované údaje

  - **Data\_FileHasShapesLinked:bool** – má hodnotu true, keď súbor má prepojené tvary na údaje

  - **Data\_FileIOBytesRead:int** – celkový počet bajtov prečítaných počas ukladania

  - **Data\_FileIOBytesReadSquared:int** – druhá mocnina poľa Data\_FileIOBytesRead

  - **Data\_FileIOBytesWritten:int** – celkový počet bajtov zapísaných počas ukladania

  - **Data\_FileIOBytesReadWritten:int** – druhá mocnina poľa Data\_FileIOBytesWritten

  - **Data\_FilePathHash:binary** – binárna hodnota hash cesty k súboru

  - **Data\_FilePathHash: binary** – identifikátor GUID cesty k súboru

  - **Data\_FileSize** – veľkosť dokumentu v bajtoch

  - **Data\_ForegroundPages:integer** – počet strán v popredí v diagrame

  - **Data\_ForegroundShapes:integer** – celé číslo počtu tvarov na stranách v popredí

  - **Data\_GdiInitTime:integer** – čas potrebný na inicializovanie modulu GDI

  - **Data\_HasCoauthUserEdit:bool** – má hodnotu true, ak dokument bol upravený v relácii spolutvorby

  - **Data\_HasCustomPages:bool** – má hodnotu true, ak dokument obsahuje vlastné strany

  - **Data\_HasCustPatterns:bool** – má hodnotu true, ak súbor obsahuje vlastné vzory

  - **Data\_HasDynConn:bool** – má hodnotu true, ak dokument obsahuje dynamické pripojenie

  - **Data\_HasScaledPages:bool** – má hodnotu true, ak dokument obsahuje strany so zmenou mierky

  - **Data\_HasUserWaitTime:bool** – má hodnotu true, ak sa počas ukladania zobrazí dialógové okno súboru

  - **Data\_InitAddinsTime:integer** – čas potrebný na inicializovanie a načítanie COM Add

  - **Data\_InitBrandTime:integer** – čas potrebný na inicializovanie úvodnej obrazovky a značkových komponentov balíka Office

  - **Data\_InitGimmeTime:integer** – čas potrebný na inicializovanie komponentu balíka Office

  - **Data\_InitLicensingTime:integer** – čas potrebný na inicializovanie licenčného komponentu balíka Office

  - **Data\_InitMsoUtilsTime:integer** – čas inicializovania komponentu MSOUTILS balíka Office

  - **Data\_InitPerfTime:integer** – čas inicializovania komponentu Performance balíka Office

  - **Data\_InitTCOTime:integer** – čas potrebný na inicializovanie správcu komponentov balíka Office

  - **Data\_InitTrustCenterTime:integer** – čas potrebný na inicializovanie komponentu centra dôveryhodnosti balíka Office

  - **Data\_InitVSSubSystemsTime:integer** – čas potrebný na inicializovanie komponentov Visia

  - **Data\_InternalFile:bool** – má hodnotu true, ak súbor je interný. Napr. vzorkovnica

  - **Data\_IsAsyncSave:bool** – má hodnotu true, ak ukladanie bolo asynchrónne

  - **Data\_IsAutoRecoveredFile:bool** – má hodnotu true, ak súbor bol automaticky obnovený

  - **Data\_IsEmbedded:bool** – má hodnotu true, ak súbor Visia bol vložený v inej aplikácii

  - **Data\_IsInfinitePageDisabledForAllPages:bool** – určuje, či je funkcia Infinite Page zakázaná pre všetky strany v dokumente

  - **Data\_IsIRMProtected:bool** – má hodnotu true, ak súbor je chránený technológiou IRM

  - **Data\_IsLocal:bool** – má hodnotu true, ak súbor je lokálny

  - **Data\_IsRecoverySave:bool**  – má hodnotu true, ak sa ukladanie spustilo z dôvodu obnovenia

  - **Data\_IsShapeSearchPaneHiddenState:bool** – má hodnotu true, ak bola tabla vyhľadávania tvaru skrytá pre dokument

  - **Data\_IsSmartDiagramPresentInActivePageOfFile:bool** – má hodnotu true, ak sa vizuálny diagram inteligentných údajov nachádza na aktívnej strane súboru

  - **Data\_IsSmartDiagramPresentInFile:bool** – má hodnotu true, ak sa vizuálny diagram inteligentných údajov nachádza v súbore

  - **Data\_IsUNC:bool** – má hodnotu true, ak cesta k súboru je v súlade s konvenciou UNC

  - **Data\_LandscapePgCount:integer** – počet strán s orientáciou na šírku v diagrame

  - **Data\_Layers:integer** – počet vrstiev v diagrame

  - **Data\_LoadProfileTime:integer** – počas potrebný na načítanie nástroja na profilovanie balíka Office

  - **Data\_LoadRichEditTim:integer** – čas načítania komponentu Rich edit

  - **Data\_LoadVisIntlTime:integer** – čas potrebný na načítanie medzinárodnej knižnice DLL Visia

  - **Data\_Location:integer** – umiestnenie súboru, z ktorého bol otvorený, 0 lokálny, 1 sieť, 2 SharePoint, 3 web

  - **Data\_MasterCount:integer** – počet predlôh v diagrame

  - **Data\_MaxCoauthUsers:integer** – maximálny počet používateľov spolutvoriacich v ľubovoľnom čase v relácii Filesystem, Registry, First Party, SDX

  - **Data\_MaxTilesAutoSizeOn:integer** – maximálny počet dlaždíc strany, pre ktoré bola automatická veľkosť povolená

  - **Data\_MsoBeginBootTime:integer** čas spustenia MSO

  - **Data\_MsoDllLoadTime:integer** – čas potrebný na načítanie knižnice DLL MSO

  - **Data\_MsoEndBootTime:integer** – čas potrebný na dokončenie spúšťania MSO

  - **Data\_MsoInitCoreTime:integer** – čas potrebný na spustenie komponentu balíka Office MSO

  - **Data\_MsoInitUITime:integer** – čas potrebný na spustenie používateľského rozhrania komponentu balíka Office MSO

  - **Data\_MsoMigrateTime:integer**  – čas potrebný na migrovanie nastavení používateľa pri prvom spustený, ak používateľ inovoval z predchádzajúcej verzie

  - **Data\_NetworkIOBytesRead:int** – celkový počet sieťových bajtov prečítaných počas ukladania

  - **Data\_NetworkIOBytesReadSquared:int** – druhá mocnina poľa Data\_NetworkIOBytesRead

  - **Data\_NetworkIOBytesWritten:int** – celkový počet sieťových bajtov zapísaných počas ukladania

  - **Data\_NetworkIOBytesWrittenSquared: int** – druhá mocnina poľa NetworkIOBytesWritten

  - **Data\_OartStartupTime:integer** – čas potrebný na inicializovanie komponentu balíka Office OART

  - **Data\_OleInitTime:integer** – čas inicializovania komponentu OLE balíka Office

  - **Data\_OpenDurationTimeInMs:integer** – čas do otvorenia súboru v milisekundách

  - **Data\_OriginatedFromTemplateID:integer** – identifikátor šablóny, z ktorej bol vytvorený diagram. NULL pre šablóny tretích strán

  - **Data\_Pages:integer** – počet strán v dokumente

  - **Data\_PositionToolbarsTime:integer** – čas potrebný na umiestnenie panelov s nástrojmi na svoje miesto

  - **Data\_ReadOnly:bool** – má hodnotu true, ak súbor je len na čítanie

  - **Data\_RecordSetCount:integer** – počet množín záznamov v diagrame

  - **Data\_RecoveryTime:integer** – čas potrebný na otvorenie súborov obnovenia

  - **Data\_ReviewerPages:integer** – počet strán recenzentov v diagrame

  - **Data\_RibbonTime:integer** – čas potrebný na zobrazenie stavového riadka

  - **Data\_RoamingSettingsStartupTime:integer** – čas potrebný na vytvorenie a načítanie všetkých momentálne prenesených nastavení Visia

  - **Data\_SchemeMgrStartupTime:integer** – čas potrebný na inicializovanie správcu schémy

  - **Data\_SDX\_AssetId** – existuje LEN pre doplnky z obchodu. OMEX priradí doplnku AssetId, keď sa zaradí do obchodu

  - **Data\_SDX\_BrowserToken** – identifikátor, ktorý sa nachádza vo vyrovnávacej pamäti prehliadača

  - **Data\_SDX\_HostJsVersion** – verzia Office.js špecifická pre platformu (napr. outlook web16.01.js). Obsahuje povrch rozhrania API pre doplnky

  - **Data\_SDX\_Id** – identifikátor GUID doplnku, ktorý ho jedinečne identifikuje

  - **Data\_SDX\_InstanceId** – predstavuje pár dokumentov k doplnku

  - **Data\_SDX\_MarketplaceType** – označuje, odkiaľ bol doplnok nainštalovaný

  - **Data\_SDX\_OfficeJsVersion** – toto je verzia Office.js, ktorá sa presmeruje na verziu špecifickú pre platformu.

  - **Data\_SDX\_Version** – verzia doplnku

  - **Data\_ShellCmdLineTime:integer** – čas potrebný na analyzovanie a vykonanie príkazov jadra na príkazovom riadku

  - **Data\_Size:long** – veľkosť súboru v bajtoch

  - **Data\_StartEndTransactionTime:integer** – čas potrebný na inicializovanie komponentov Visia

  - **Data\_STNInitTime:integer** – čas potrebný na inicializovanie konfigurácie okna vzorkovnice

  - **Data\_Tag:string** – jedinečný identifikátor na identifikáciu udalosti Uložiť ako

  - **Data\_ThemeCount:integer** – počet motívov v diagrame

  - **Data\_TimeStamp** – časová pečiatka času zavretia dokumentu

  - **Data\_UIInitTime:integer** – čas inicializovania používateľského rozhrania

  - **Data\_WasSuccessful:bool** – má hodnotu true, ak uloženie ako bolo úspešné

  - **Data\_WinLaunchTime:integer** – čas potrebný na spustenie úvodnej tably Visia atď.)

  - **Office.Visio.FileCharacteristicsVisio** – zachytáva vlastnosti súboru v čase spustenia súboru pre Visio C2R a Dev16. Táto udalosť nám pomáha kategorizovať a ladiť chyby v súvislosti s vlastnosťami dokumentu, čo nám zasa umožňuje rýchlejšie zisťovať prvotné príčiny problémov a vyriešiť ich k spokojnosti zákazníkov.

  - **Office.Visio.Shared.BootStats** – táto udalosť zhromažďuje čas spustenia pre aplikáciu Visio Win32. Zhromažďuje rôzne polia o spúšťaní rôznych komponentov, ako napríklad čas načítania pásu s nástrojmi alebo čas inicializácie aplikácie. Táto udalosť sa používa na meranie výkonu spúšťania pre Visio.

  - **Office.Visio.Shared.FileOpen** – táto udalosť zhromažďuje štatistiku otvárania súborov pre Visio. Používa sa na monitorovanie miery úspešných a neúspešných otvorení súborov a mapuje ju s niekoľkými vlastnosťami, ako je napríklad veľkosť súboru. Vlastnosti súboru nám umožňujú rýchlejšie ladiť problémy a zistiť ich prvotnú príčinu.

  - **Office.Visio.Shared.Filesave** – táto udalosť zhromažďuje štatistiku ukladania súborov pre Visio. Používa sa na monitorovanie miery úspešných a neúspešných uložení súborov a mapuje ju s niekoľkými vlastnosťami, ako je napríklad veľkosť súboru a miesto ukladania, napr. cloud/lokálne. Vlastnosti súboru nám umožňujú rýchlejšie ladiť problémy a zistiť ich prvotnú príčinu.

  - **Office.Visio.Shared.FilesaveAs** – táto udalosť zhromažďuje štatistiku funkcie Uložiť ako pre Visio. Používa sa na monitorovanie miery úspešných a neúspešných uložení súborov a mapuje ju s niekoľkými vlastnosťami, ako je napríklad veľkosť súboru a miesto ukladania, napr. cloud/lokálne. Vlastnosti súboru nám umožňujú rýchlejšie ladiť problémy a zistiť ich prvotnú príčinu.

  - **Office.Visio.Shared.PostSave** – táto udalosť zachytáva dôvod zlyhania pre zlyhanie pri ukladaní súboru.

  - **Office.Visio.VisioFileSaveAs** – táto udalosť zhromažďuje štatistiku funkcie Uložiť ako pre Visio Dev16. Používa sa na monitorovanie miery úspešných a neúspešných uložení súborov pod iným názvom a mapuje ju s niekoľkými vlastnosťami, ako je napríklad veľkosť súboru a miesto ukladania, napr. cloud/lokálne. Vlastnosti súboru nám umožňujú rýchlejšie ladiť problémy a zistiť ich prvotnú príčinu.

  - **Office.Visio.VisioFileSaveAsync** – táto udalosť zhromažďuje štatistiku funkcie ukladania súborov asynchrónne pre Visio Dev16. Používa sa na monitorovanie miery úspešných a neúspešných asynchrónnych uložení súborov a mapuje ju s niekoľkými vlastnosťami, ako je napríklad veľkosť súboru a miesto ukladania, napr. cloud/lokálne. Vlastnosti súboru nám umožňujú rýchlejšie ladiť problémy a zistiť ich prvotnú príčinu.

  - **Office.Visio.VisioFileSaveSync** – táto udalosť zhromažďuje štatistiku funkcie ukladania súborov synchrónne pre Visio Dev16. Používa sa na monitorovanie miery úspešných a neúspešných synchrónnych uložení súborov a mapuje ju s niekoľkými vlastnosťami, ako je napríklad veľkosť súboru a miesto ukladania, napr. cloud/lokálne. Vlastnosti súboru nám umožňujú rýchlejšie ladiť problémy a zistiť ich prvotnú príčinu. Táto udalosť nám pomáha monitorovať príčiny zlyhania uloženia súboru.

#### <a name="officeextensibilitysandboxodpactivationhanging"></a>Office.Extensibility.Sandbox.ODPActivationHanging

Zhromažďuje informácie, keď spúšťanie balíka Office trvá neočakávane dlho (> 5 sekúnd). Používa sa na zisťovanie a riešenie problémov so spúšťaním doplnkov balíka Office.
 
Zhromažďujú sa tieto polia:

- **AppID** – ID aplikácie.

- **AppInfo** – údaje týkajúce sa typu doplnku (pracovná tabla alebo režimu bez používateľského rozhrania alebo obsahu atď.) a typu poskytovateľa (omen, SharePoint, systém súborov atď.).

- **AppInstanceId** – ID inštancie aplikácie. 

- **AssetId** – ID položky aplikácie.

- **NumberOfAddinsActivated** – počítadlo aktivovaných doplnkov.

- **RemoterType** – špecifikuje typ služby Remoter (dôveryhodná, nedôveryhodná, Win32webView, dôveryhodná funkcia definovaná používateľom atď.), ktorý sa používa na aktiváciu doplnku.

- **StoreType** – pôvod aplikácie.

- **TimeForAuth** – čas strávený na overenie. 

- **TimeForSandbox** – čas strávený v Sandboxe.

- **TimeForServerCall** – čas strávený volaním servera. 

- **TotalTime** – celkový strávený čas.


#### <a name="officeoutlookdesktopexchangepuidandtenantcorrelation"></a>Office.Outlook.Desktop.ExchangePuidAndTenantCorrelation

Táto udalosť zhromažďuje identifikátor PUID používateľa a identifikátor nájomníka raz za reláciu. Korelácia identifikátora PUID a nájomníka je nevyhnutná na porozumenie a diagnostiku problémov s Outlookom na základe jednotlivých nájomníkov.

Zhromažďujú sa tieto polia:

  - **CollectionTime** – časová pečiatka udalosti

  - **ConnId** – identifikátor spojenia: identifikátor spojenia analyzujúceho identifikátor PUID a identifikátor nájomníka OMS

  - **OMSTenantId** – jedinečný identifikátor nájomníka generovaný spoločnosťou Microsoft

  - **PUID** – identifikátor PUID Exchangeu na jedinečnú identifikáciu používateľov


#### <a name="officeoutlookmacmacolkactivationstate"></a>Office.Outlook.Mac.MacOLKActivationState

Zhromažďuje informácie o tom, ako je Outlook aktivovaný, napríklad s predplatným alebo multilicenciou. Údaje sú monitorované, aby sa nezobrazovali žiadne výkyvy v zlyhaniach. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie. 

Zhromažďujú sa tieto polia:

- **SetupUIActivationMethod** – spôsob aktivácie Outlooku, ako je napríklad predplatné alebo multilicencia.

#### <a name="officepowerpointdocoperationopen"></a>Office.PowerPoint.DocOperation.Open 

Táto udalosť sa zhromažďuje vždy, keď PowerPoint otvorí súbor. Zahŕňa informácie o úspechu, podrobnosti o zlyhaní, metriku výkonu a základné podrobnosti o súbore vrátane typu formátu súboru a metaúdajov dokumentu. Tieto informácie sú potrebné na zabezpečenie, že PowerPoint dokáže úspešne otvoriť súbory bez zníženia výkonu. Umožňuje nám diagnostikovať problémy, ktoré zistíme.

Zhromažďujú sa tieto polia:

  - **Data\_AddDocTelemetryResult** – označuje, či tento záznam denníka má všetku potrebnú telemetriu dokumentu (polia Data\_Doc\_\*)

  - **Data\_AddDocumentToMruList** – trvanie spustenia metódy AddDocumentToMruList

  - **Data\_AlreadyOpened** – označuje, či bol tento dokument už niekedy otvorený (v rámci kontextu tej istej relácie procesu)

  - **Data\_AntiVirusScanMethod** – preddefinovaná množina hodnôt typu skenovania antivírusu (IOAV, AMSI, žiadny atď.)

  - **Data\_AntiVirusScanStatus** – preddefinovaná množina hodnôt skenovania antivírusu, ktoré prebieha pre každý otvorený dokument (NoThreatsDetected, Failed, MalwareDetected atď.)

  - **Data\_AsyncOpenKind** – preddefinovaná množina hodnôt možností asynchrónnosti (Collab, ServerOnly, SyncBacked, NotAsync)

  - **Data\_CancelBackgroundDownloadHr** – označuje, či bolo sťahovanie dokumentu prerušené. Ak áno, aký bol výsledok prerušenia.

  - **Data\_CheckForAssistedReadingReasons** – trvanie spustenia metódy CheckForAssistedReadingReasons v milisekundách

  - **Data\_CheckForDisabledDocument** – trvanie spustenia metódy CheckForDisabledDocument v milisekundách

  - **Data\_CheckForExistingDocument** – trvanie spustenia metódy CheckForExistingDocument v milisekundách

  - **Data\_CheckIncOpenResult** – trvanie spustenia metódy CheckIncOpenResult v milisekundách

  - **Data\_CheckLambdaResult** – trvanie spustenia metódy CheckLambdaResult v milisekundách

  - **Data\_CheckPackageForRequiredParts** – trvanie spustenia metódy CheckPackageForRequiredParts v milisekundách

  - **Data\_CheckPackageForSpecialCases** – trvanie spustenia metódy CheckPackageForSpecialCases v milisekundách

  - **Data\_CheckRequiredPartsLoaded** – trvanie spustenia metódy CheckRequiredPartsLoaded v milisekundách

  - **Data\_CheckWebSharingViolationForIncOpen** – trvanie spustenia metódy CheckWebSharingViolationForIncOpen v milisekundách
   
  - **Data_CloseAndReopenWithoutDiscard** – označuje, či bol dokument zavretý a opäť otvorený počas otvoreného procesu bez vyhodenia.

  - **Data\_ContentTransaction** – preddefinovaná množina hodnôt určujúcich, kedy je možné vytvoriť transakciu (AllowedOnLoadDocument, AllowedOnOpenComplete atď.)

  - **Data_CorrelationId** – identifikátor GUID odoslaný do PowerPointu procesom ProtocolHandler na koreláciu telemetrie. ProtocolHandler je samostatný proces, ktorý spracováva prepojenia balíka Office pre operačný systém.

  - **Data\_CppUncaughtExceptionCount:long** – nezachytené natívne výnimky počas spustenej aktivity

  - **Data\_CreateDocumentTimeMS** – trvanie spustenia metódy CreateDocumentTimeMS v milisekundách

  - **Data\_CreateDocumentToken** – trvanie spustenia metódy CreateDocumentToken v milisekundách

  - **Data\_CreateDocumentToW** – trvanie spustenia metódy CreateDocumentToW v milisekundách

  - **Data\_CreateDocWindow** – trvanie spustenia metódy CreateDocWindow v milisekundách

  - **Data\_CreateLocalTempFile** – trvanie spustenia metódy CreateLocalTempFile v milisekundách

  - **Data\_DetachedDuration:long** – časový úsek, počas ktorého bola aktivita odpojená/nespustená

  - **Data\_** – trvanie spustenia metódy DetermineFileType v milisekundách

  - **Data\_Doc\_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie alebo na čítanie a zapisovanie)

  - **Data\_Doc\_AssistedReadingReasons:long** – preddefinovaná množina hodnôt toho, prečo bol dokument otvorený v režime asistovaného čítania

  - **Data\_Doc\_ChunkingType:long** – ako je dokument uložený v SharePointe

  - **Data\_Doc\_EdpState:long** – stav ochrany podnikových údajov v dokumente

  - **Data\_Doc\_Ext:string** – prípona dokumentu

  - **Data\_Doc\_Extension:string** – prípona dokumentu

  - **Data\_Doc\_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona)

  - **Data\_Doc\_Fqdn:string** – miesto uloženia dokumentu (SharePoint.com, live.net), k dispozícii len pre domény Office 365

  - **Data\_Doc\_FqdnHash:string** – hodnota hash miesta uloženia dokumentu

  - **Data\_Doc\_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa

  - **Data\_Doc\_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov

  - **Data\_Doc\_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument

  - **Data\_Doc\_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool** – má hodnotu true, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky OPTIONS.

  - **Data\_Doc\_IsIncrementalOpen:bool** – určuje, či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnutia celého dokumentu)

  - **Data\_Doc\_IsOcsSupported:bool** – určuje, či dokument podporuje spolutvorbu pomocou novej služby OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool** – zobrazuje, či sa dokument otvára z lokálnej vyrovnávacej pamäte

  - **Data_Doc_IsRtcAlwaysOn** – má hodnotu true, ak je kanál v reálnom čase (RTC) pre tento súbor vždy zapnutý.

  - **Data\_Doc\_IsSyncBacked:bool** – či sa dokument otvára z priečinka, ktorý používa aplikáciu OneDrivu na synchronizáciu a zálohovanie

  - **Data\_Doc\_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.)

  - **Data\_Doc\_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.)

  - **Data\_Doc\_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu

  - **Data\_Doc\_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu)

  - **Data\_Doc\_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.)

  - **Data\_Doc\_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude

  - **Data\_Doc\_ServerDocId:string** – nemenný identifikátor pre dokumenty uložené v cloude

  - **Data\_Doc\_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.)

  - **Data\_Doc\_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long** – určuje, či je server založený na Office14, Office15 alebo Office16

  - **Data\_Doc\_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu

  - **Data\_Doc\_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

  - **Data\_Doc\_SizeInBytes:long** – veľkosť dokumentu v bajtoch

  - **Data\_Doc\_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu

  - **Data\_Doc\_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“

  - **Data\_Doc\_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný)

  - **Data\_Doc\_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude

  - **Data\_Doc\_UsedWrsDataOnOpen:bool** – má hodnotu true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa

  - **Data\_Doc\_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“

  - **Data\_DownloadExcludedData** – trvanie spustenia metódy DownloadExcludedData v milisekundách

  - **Data\_DownloadExcludedDataTelemetry** – preddefinovaná množina hodnôt stavu synchrónneho čakania na stiahnutie (SynchronousLogicHit, UserCancelled RunModalTaskUnexpectedHResult atď.)

  - **Data\_** – trvanie spustenia metódy DownloadFileInBGThread v milisekundách

  - **Data\_DownloadFragmentSize** – veľkosť fragmentu (stiahnuteľného kúska súboru), zvyčajne 3,5 MB

  - **Data\_ExcludedEmbeddedItems** – počet zip častí, ktoré sú vylúčené pre prvé vykreslenie

  - **Data\_ExcludedEmbeddedItemsSize** – celková veľkosť zip častí, ktoré sú vylúčené pre prvé vykreslenie

  - **Data\_ExcludedRequiredItems** – počet zip častí, ktoré sú vylúčené, ale požadované pre prvé vykreslenie

  - **Data\_ExcludedRequiredItemsSize** – celková veľkosť zip častí, ktoré sú vylúčené, ale požadované pre prvé vykreslenie

  - **Data\_ExecutionCount** – počet spustení protokolu IncOpen

  - **Data\_FailureComponent:long** – preddefinovaná množina hodnôt toho, ktorá súčasť spôsobila zlyhanie protokolu (Conflict, CSI, Internal atď.)

  - **Data\_FailureReason:long** – preddefinovaná množina hodnôt dôvodu zlyhania (FileIsCorrupt, BlockedByAntivirus atď.)

  - **Data\_FCreateNew** – označuje, či ide o nový prázdny dokument

  - **Data\_FCreateNewFromTemplate** – označuje, či ide o nový dokument zo šablóny

  - **Data_FErrorAfterDocWinCreation:boolean** – zobrazuje, či sa po vytvorení okna dokumentu vyskytla nejaká chyba alebo výnimka.

  - **Data\_FileUrlLocation** – preddefinovaná množina hodnôt miesta uloženia dokumentu (NetworkShare, LocalDrive, ServerOther atď.)

  - **Data\_FirstSlideCompressedSize** – komprimovaná veľkosť zip časti prvej snímky (zvyčajne Slide1.xml)

  - **Data\_FIsDownloadFileInBgThreadEnabled** – označuje, či je povolené sťahovanie vo vlákne na pozadí

  - **Data\_fLifeguarded:bool** – či mal dokument niekedy chránenú životnosť (funkciou na riešenie chýb dokumentov bez zobrazenia výzvy používateľovi)

  - **Data\_ForceReopenOnIncOpenMergeFailure** – príznak vyjadrujúci, či sme boli nútení znova otvoriť z dôvodu zlyhania zlúčenia v prírastkovom otváraní

  - **Data\_ForegroundThreadPass0TimeMS ** (len Mac) – celkový čas strávený vo vlákne v popredí pri prvom prechode

  - **Data\_ForegroundThreadPass1TimeMS ** (len Mac) – celkový čas strávený vo vlákne v popredí pri druhom prechode

  - **Data\_FWebCreatorDoc** – či je dokument vytvorený zo šablóny alebo rýchleho štartu

  - **Data\_HasDocToken** – či má tento dokument token dokumentu CSI (interný kód)

  - **Data\_HasDocument** – či má tento dokument dokument CSI (interný kód)

  - **Data\_InclusiveMeasurements -** – či trvania merania metód obsahujú trvanie volania podriadenej metódy

  - **Data\_IncompleteDocReasons** – preddefinovaná množina hodnôt toho, prečo bolo otvorenie neúplné (Unknown, DiscardFailure atď.)

  - **Data\_IncOpenDisabledReasons** – preddefinovaná množina hodnôt dôvodov zakázania prírastkového otvárania

  - **Data\_IncOpenFailureHr** – výsledok, prečo prírastkové otváranie zlyhalo

  - **Data\_IncOpenFailureTag** – značka (ukazovateľ na miesto v kóde) miesta zlyhania prírastkového otvárania

  - **Data\_IncOpenFallbackReason** – prečo sa prírastkové otváranie nespustilo

  - **Data\_IncOpenRequiredTypes** – preddefinovaná množina hodnôt typov obsahu potrebných na prvé vykreslenie (RequiredXmlZipItem, RequiredNotesMaster atď.)

  - **Data\_IncOpenStatus** – preddefinovaná množina hodnôt stavu prírastkového otvárania (Attempted, FoundExcludedItems, DocIncOpenInfoCreated atď.)

  - **Data\_InitFileContents** – trvanie spustenia metódy InitFileContents v milisekundách

  - **Data\_InitialExcludedItems** – počet zip častí, ktoré sú spočiatku vylúčené

  - **Data\_InitialExcludedItemsSize** – celková veľkosť zip častí, ktoré sú spočiatku vylúčené

  - **Data\_InitializationTimeMS** – (len Mac) čas na spustenie

  - **Data\_InitialRoundtripCount** – počet odpovedí servera potrebných na vytvorenie počiatočného zip archívu

  - **Data\_InitLoadProcess** – trvanie spustenia metódy InitLoadProcess v milisekundách

  - **Data\_InitPackage** – trvanie spustenia metódy InitPackage v milisekundách

  - **Data\_InitSecureReaderReasons** – trvanie spustenia metódy InitSecureReaderReasons v milisekundách

  - **Data\_IsIncOpenInProgressWhileOpen** – či je v prípade viacnásobného otvárania toho istého dokumentu protokol Inc open spustení spoločne s protokolom open?

  - **Data\_IsMultiOpen** – či podporujeme viacnásobné otvorenie

  - **Data\_IsOCS** – či bol dokument vo svojom poslednom známom stave v režime OCS

  - **Data\_IsODPFile** – či je dokument vo formáte Open Document Format používanom softvérom OpenOffice.org

  - **Data\_IsPPTMetroFile** – či je dokument vo formáte metro (pptx)

  - **Data\_LoadDocument** – trvanie spustenia metódy LoadDocument v milisekundách

  - **Data\_MeasurementBreakdown** – rozdelenie šifrovaných meraní (skrátená podrobná metóda perf)

  - **Data\_Measurements** – šifrované merania

  - **Data\_MethodId** – naposledy spustená metóda

  - **Data\_NotRequiredExcludedItems** – celkový počet položiek balíka PowerPointu, ktoré nie sú požadované pre prvé vykreslenie a vylúčené

  - **Data\_NotRequiredExcludedItemsSize** – celková veľkosť položiek balíka PowerPointu, ktoré nie sú požadované pre prvé vykreslenie a vylúčené

  - **Data\_NotRequiredExcludedParts** – celkový počet položiek zip častí, ktoré nie sú požadované pre prvé vykreslenie a vylúčené

  - **Data\_NotRequiredExcludedPartsSize** – celková veľkosť zip častí, ktoré nie sú požadované pre prvé vykreslenie a vylúčené

  - **Data\_OpenCompleteFailureHR** – výsledok dôvodu zlyhania protokolu OpenComplete

  - **Data\_OpenCompleteFailureTag** – značka (ukazovateľ na miesto v kóde) miesta zlyhania protokolu OpenComplete

  - **Data\_OpenLifeguardOption**– preddefinovaná množina hodnôt volieb pre operáciu ochrany životnosti (None, TryAgain, OpenInWebApp atď.)

  - **Data\_OpenReason** – preddefinovaná množina hodnôt spôsobu otvorenia tohto dokumentu (FilePicker, OpenFromMru, FileDrop atď.)

  - **Data\_OSRPolicy** – politika SecureReader

  - **Data\_OSRReason** – dôvody otvorenia tohto dokumentu v Secure Reader

  - **Data\_OtherContentTypesWithRequiredParts** – neštandardné typy obsahu, ktoré boli vylúčené, ale požadované pre prvé vykreslenie

  - **Data\_PrepCacheAsync** – príznak pre OcsiOpenPerfPrepCacheAsync

  - **Data\_PreviousDiscardFailed** – označuje, že predchádzajúci pokus o otvorenie/zavretie dokumentu neuvoľnil správne všetku pamäť

  - **Data\_PreviousFailureHr** – v prípade opätovného otvárania toho istého dokumentu, aký bol výsledok posledného zlyhania

  - **Data\_PreviousFailureTag** – v prípade opätovného otvárania toho istého dokumentu, aká bola značka posledného zlyhania (ukazovateľ na miesto v kóde)

  - **Data\_RemoteDocToken** – je povolené vzdialené otváranie (funkcia v štádiu prototypu, ktorá umožňuje otvoriť súbor zo služby namiesto z hostiteľa)?

  - **Data\_Repair** – či sa nachádzame v režime opravy dokumentu (pre poškodené dokumenty, ktoré sú opraviteľné)

  - **Data\_RequestPauseStats** – koľkokrát kód požadoval pozastavenie zaznamenávania výkonu

  - **Data\_RequiredPartsComressedSize** – celková veľkosť požadovaných častí PowerPointu potrebných na prvé vykreslenie

  - **Data\_RequiredPartsDownload** – celková veľkosť požadovaných častí PowerPointu, ktoré sú stiahnuté

  - **Data\_RequiredPartsRoundtripCount** – celkový počet cyklov (volaní hostiteľa) potrebných na získanie všetkých požadovaných častí PowerPointu na prvé vykreslenie

  - **Data\_RequiredZipItemsDownload** – celková veľkosť požadovaných zip položiek potrebných na prvé vykreslenie

  - **Data\_RequiredZipItemsRoundtripCount** – celkový počet cyklov (volaní hostiteľa) potrebných na získanie všetkých požadovaných zip položiek na prvé vykreslenie

  - **Data\_RoundtripsAfterMissingRequiredParts** – celkový počet cyklov (volaní hostiteľa) potrebných po nájdení chýbajúcich požadovaných častí PowerPointu

  - **Data\_RoundtripsAfterMissingRequiredZipItems** – celkový počet cyklov (volaní hostiteľa) potrebných po nájdení chýbajúcich požadovaných zip položiek

  - **Data\_** – celkový počet cyklov (volaní hostiteľa) potrebných po vytvorení balíka

  - **Data\_** – celkový počet cyklov (volaní hostiteľa) potrebných po stiahnutí všetkých požadovaných častí

  - **Data\_SetDocCoAuthAutoSaveable** – trvanie spustenia metódy SetDocCoAuthAutoSaveable v milisekundách

  - **Data\_SniffedFileType** – vzdelaný odhad navrhovaného typu súboru poškodeného dokumentu

  - **Data\_StartTime** – počítadlo výkonu po začatí otvárania

  - **Data\_StopwatchDuration:long** – celkový čas aktivity

  - **Data\_SyncSlides** – trvanie spustenia metódy SyncSlides v milisekundách

  - **Data\_TimerStartReason** – preddefinovaná množina hodnôt spôsobu spustenia časovača (CatchMissedSyncStateNotification, WaitingForFirstDownload atď.)

  - **Data\_TimeSplitMeasurements** – rozdelenie šifrovaných meraní (skrátená podrobná metóda perf)

  - **Data\_TimeToInitialPackage** – čas potrebný na vytvorenie počiatočného balíka

  - **Data\_TimeToRequiredPackage** – čas potrebný na vytvorenie požadovaného balíka

  - **Data\_TimeToRequiredParts** – čas potrebný na vytvorenie balíka so všetkými požadovanými časťami

  - **Data\_TotalRequiredParts** – celkový počet častí PowerPointu potrebných na prvé vykreslenie

  - **Data\_UnknownRequiredParts** – celkový počet neštandardných častí potrebných na prvé vykreslenie

  - **Data\_UnpackLinkWatsonId** – identifikátor Watson chyby pri otváraní dokumentu prostredníctvom URL adresy zdieľania cez OneDrive

  - **Data\_UnpackResultHint** – preddefinovaná množina hodnôt rozbalenia výsledkov URL adresy zdieľania (NavigateToWebWithoutError, UrlUnsupported, AttemptOpen atď.)

  - **Data\_UnpackUrl** – trvanie spustenia metódy UnpackUrl v milisekundách

  - **Data\_UpdateAppstateTimeMS** – trvanie spustenia metódy UpdateAppstate v milisekundách

  - **Data\_UpdateCoauthoringState** – trvanie spustenia metódy UpdateCoauthoringState v milisekundách

  - **Data\_UpdateReadOnlyState** – trvanie spustenia metódy UpdateReadOnlyState v milisekundách

  - **Data\_WACCorrelationId** – v prípade otvárania súboru v prehliadači získanie korelácie denníkov WebApp

  - **Data\_WasCachedOnInitialize** – či bol tento dokument uložený do vyrovnávacej pamäte počas inicializácie

  - **Data\_WBDirtyBeforeDiscard** – či sa pracovná vetva stala zmenenou (dirty) pred otvorením dokumentu

  - **Data\_ZRTOpenDisabledReasons** – prečo sa nepodarilo dokument z vyrovnávacej pamäte (Zero Round Trip)

#### <a name="officepowerpointpptdesktopbootime"></a>Office.PowerPoint.PPT.Desktop.Bootime

Táto udalosť zhromažďuje informácie o spustení PowerPointu. Zahŕňa spustenie PowerPointu v chránenom zobrazení, v režime asistovaného čítania, z makra, tlače, nového a prázdneho dokumentu, obnovenia dokumentu, z automatizácie a či ide o technológiu Klikni a spusti. Tiež zhromažďuje, ako dlho trvá spustenie PowerPointu. Tento údaj je veľmi dôležitý na to, aby sa zaručilo, že PowerPoint funguje správne pri spúšťaní z rôznych režimov. Spoločnosť Microsoft používa tieto údaje na zachytenie dlhého času spustenia pri otváraní PowerPointu z rôznych režimov.

Zhromažďujú sa tieto polia:

  - **AssistedReading** – v režime asistovaného čítania

  - **Automation** – z automatizácie

  - **Benchmark** – spustenie benchmarku výkonu

  - **Blank** – prázdny dokument

  - **BootTime** – čas spustenia relácie

  - **Embedding** – vloženie dokumentu

  - **IsC2R** – či ide o technológiu Klikni a spusti

  - **IsNew** – nový dokument

  - **IsOpen** – je otvorený

  - **Macro1** – spustenie makra

  - **Macro2** – spustenie makra

  - **NonStandardSpaceInCmdLine** – v príkazovom riadku je neštandardná medzera

  - **Print** – tlač dokumentu

  - **PrintDialog** – tlač dokumentu s dialógovým oknom

  - **PrintPrinter** – tlač dokumentu s tlačiarňou

  - **ProtectedView** – v chránenom zobrazení

  - **Regserver** – registrácia PowerPointu ako servera COM

  - **Restore** – obnovenie dokumentu

  - **Show** – zobrazenie dokumentu

  - **Time** – čas relácie

  - **UnprotectedView** – v nechránenom zobrazení

#### <a name="officepowerpointppthasuserediteddocument"></a>Office.PowerPoint.PPT.HasUserEditedDocument

Zhromažďuje sa, keď používateľ začne upravovať dokument. Spoločnosť Microsoft používa tieto údaje na vypočítanie aktívnych používateľov, ktorí upravovali powerpointový dokument.

Zhromažďujú sa tieto polia:

  - **CorrelationId** – identifikátor korelácie dokumentu

#### <a name="officeprojectbootandopenproject"></a>Office.Project.BootAndOpenProject

Project je spustený otvorením súboru. Táto udalosť označuje, že používateľ otvoril Office Project priradeným súborom. Obsahuje dôležité údaje o úspechu zaručenia, že Project sa môže spustiť a načítať súbor.

Zhromažďujú sa tieto polia:

  - **Data\_AlertTime** – čas, počas ktorého bolo aktívne dialógové okno spustenia.

  - **Data\_BootTime** – čas potrebný na spustenie Projectu

  - **Data\_CacheFileSize** – ak bol súbor uložený vo vyrovnávacej pamäti, veľkosť súboru

  - **Data\_EntDocType** – typ súboru, ktorý bol otvorený

  - **Data\_IsInCache** – označuje, či otvorený súbor bol uložený vo vyrovnávacej pamäti

  - **Data\_LoadSRAs** – či používateľ chce načítať SRA alebo nie

  - **Data\_Outcome** – celkový čas spustenia a otvorenia súboru.

  - **Data\_OpenFromDocLib** – či otvorný súbor Projectu bol z knižnice dokumentov

  - **Data\_ProjectServerVersion** – aktuálna verzia a zostava Projectu

#### <a name="officeprojectbootproject"></a>Office.Project.BootProject

Project je spustený bez otvorenia súboru. Táto udalosť označuje, že používateľ otvoril Office Project bez priradeného súboru. Obsahuje dôležité údaje o úspechu zaručenia, že Project sa môže spustiť.

Zhromažďujú sa tieto polia:

  - **Data\_BootTime** – čas potrebný na spustenie Projectu

  - **Data\_FileLoaded** – má hodnotu false, ak ide o otvorenie z vonkajšieho alebo nového prázdneho projektu

  - **Data\_IsEntOfflineWithProfile** – označuje, či používatelia sú v profesionálnej jednotke SKU a nie sú pripojení k serveru

  - **Data\_IsEntOnline** – označuje, či relácia Projectu je pripojená k projectovému serveru s podnikovými funkciami

  - **Data\_IsLocalProfile** – označuje, či relácia Projectu je pripojená k projectovému serveru s podnikovými funkciami

  - **Data\_ProjectServerVersion** – aktuálna verzia a zostava Projectu


#### <a name="officeprojectopenproject"></a>Office.Project.OpenProject

Project otvorí súbor. Táto udalosť označuje, že používateľ priamo otvára súbor Projectu. Obsahuje dôležité údaje o úspechu otvárania súborov v Projecte.

Zhromažďujú sa tieto polia:

  - **Data\_AgileMode** – definuje, či otvorený projekt je vodopádový alebo agilný

  - **Data\_AlertTime** – čas, počas ktorého bolo aktívne dialógové okno spustenia

  - **Data\_CacheFileSize** – ak bol súbor uložený vo vyrovnávacej pamäti, veľkosť súboru

  - **Data\_EntDocType** – typ súboru, ktorý bol otvorený

  - **Data\_IsInCache** – označuje, či otvorený súbor bol uložený vo vyrovnávacej pamäti

  - **Data\_LoadSRAs** – či používateľ chce načítať SRA alebo nie

  - **Data\_OpenFromDocLib** – či otvorný súbor Projectu bol z knižnice dokumentov

  - **Data\_Outcome** – celkový čas spustenia a otvorenia súboru

  - **Data\_Outcome** – celkový čas spustenia a otvorenia súboru.

  - **Data\_ProjectServerVersion** – aktuálna verzia a zostava Projectu

#### <a name="officesessionidproviderofficeprocesssessionstart"></a>Office.SessionIdProvider.OfficeProcessSessionStart

Vzťahuje sa na všetky aplikácie balíka Office pre Windows: win32 a UWP

Zhromažďujú sa tieto polia:

- **OfficeProcessSessionStart** – odosiela základné informácie na začiatku novej relácie balíka Office. Používa sa na spočítanie počtu jedinečných relácií, ktoré sa vyskytujú v danom zariadení. Používa sa ako signálna udalosť na uistenie sa, či je aplikácia v zariadení spustená alebo nie. Okrem toho slúži ako dôležitý signál pre celkovú spoľahlivosť aplikácie

- **AppSessionGuid** – identifikátor konkrétnej relácie aplikácie, ktorá sa začína v čase vytvorenia procesu a pretrváva až do konca procesu. Je formátovaný ako štandardný 128-bitový identifikátor GUID, ale skladá sa zo 4 častí. Tieto štyri časti sú v poradí 1. ID procesu 32-bitovej verzie, 2. ID relácie 16-bitovej verzie, 3. ID spustenia 16-bitovej verzie, 4. čas vytvorenia procesu 64-bitovej verzie v UTC 100ns.

- **processSessionId** – náhodne vytvorený identifikátor GUID na identifikáciu relácie aplikácie

- **UTCReplace_AppSessionGuid** – konštantná boolovská hodnota. Vždy hodnota True.

#### <a name="officetelemetryengineisprelaunch"></a>Office.TelemetryEngine.IsPreLaunch

Vzťahuje sa na všetky aplikácie UWP balíka Office.  Táto udalosť sa spustí pri prvom spustení aplikácie balíka Office po inovácii/inštalácii z obchodu. Je súčasťou základných diagnostických údajov, ktoré sa používajú na sledovanie, či ide o reláciu spustenia alebo nie.

Zhromažďujú sa tieto polia:

- **appVersionBuild** – číslo verzie zostavy aplikácie.

- **appVersionMajor** – číslo hlavnej verzie aplikácie.

- **appVersionMinor** – číslo vedľajšej verzie aplikácie.

- **appVersionRev** – číslo verzie revízie aplikácie.

- **sessionID** – náhodne vytvorený identifikátor GUID na identifikáciu relácie aplikácie

#### <a name="officetelemetryenginesessionhandoff"></a>Office.TelemetryEngine.SessionHandOff

Vzťahuje sa na všetky aplikácie Win32 balíka Office.  Táto udalosť nám pomáha zistiť, či sa vytvorila nová relácia na spracovanie udalosti otvorenia súboru iniciovanej používateľom. Ide o dôležité diagnostické informácie, ktoré sa používajú na odvodenie signálu spoľahlivosti a uistenie, že aplikácia funguje podľa očakávaní.

Zhromažďujú sa tieto polia:

- **appVersionBuild** – číslo verzie zostavy aplikácie.

- **appVersionMajor** – číslo hlavnej verzie aplikácie.

- **appVersionMinor** – číslo vedľajšej verzie aplikácie.

- **appVersionRev** – číslo verzie revízie aplikácie.

- **childsessionID** – náhodne vytvorený identifikátor GUID na identifikáciu relácie aplikácie

- **parentsessionId** – náhodne vytvorený identifikátor GUID na identifikáciu relácie aplikácie


#### <a name="officewordfileopenopencmdfilemrupriv"></a>Office.Word.FileOpen.OpenCmdFileMruPriv

Táto udalosť označuje, že Office Word otvára dokument zo zoznamu naposledy použitých súborov (MRU). Obsahuje aj kritické údaje o výkone otvárania súboru a je udalosťou spustenia aplikácie z pohľadu používateľa. Udalosť monitoruje, či otvorenie súboru zo zoznamu naposledy použitých súborov funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov.

- **Data_BytesAsynchronous** – počet bajtov (komprimovaných), bez ktorých podľa nás dokážeme otvoriť dokument, ak by sme ich dostali predtým, než používateľ chce začať upravovať, prípadne uložiť.

- **Data_BytesAsynchronousWithWork** – počet bajtov (komprimovaných), bez ktorých by sme možno dokázali otvoriť súbor, alebo vyžadovalo by si to značné investície do kódu.

- **Data_BytesSynchronous** – počet bajtov (komprimovaných), ktoré musíme mať predtým, než môžeme začať otvárať súbor.

- **Data_BytesUnknown** – počet bajtov v častiach dokumentu, ktoré podľa nás nenájdeme. 

- **Data_DetachedDuration** – ako dlho bola aktivita odpojená od vlákna.

- **Data_Doc_AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť.

- **Data_Doc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_Doc_ChunkingType** – jednotky slúžiace na prírastkové otvorenie dokumentu.

- **Data_Doc_EdpState** – nastavenie ochrany elektronických údajov dokumentu.

- **Data_Doc_Ext** prípona dokumentu (docx, xlsb, pptx atď.)

- **Data_Doc_FileFormat** – verzia protokolu formátu súboru.

- **Data_Doc_Fqdn** – názov domény OneDrivu alebo SharePointu Online.

- **Data_Doc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – zaznamenáva, ako bol dokument otvorený.

- **Data_Doc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_Doc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.

- **Data_Doc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_Doc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.

- **Data_Doc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_Doc_IsRtcAlwaysOn** – má hodnotu true, ak je kanál v reálnom čase (RTC) pre tento súbor vždy zapnutý.

- **Data_Doc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_Doc_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_Doc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_Doc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_Doc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie.

- **Data_Doc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_Doc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov. 

- **Data_Doc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_Doc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).

- **Data_Doc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_Doc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_Doc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_Doc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_Doc_SpecialChars** – indikátor špeciálnych znakov v URL adrese dokumentu. 

- **Data_Doc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_Doc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_Doc_WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI.

- **Data_EditorDisablingRename** – identifikátor prvého editora, ktorý spôsobil vypnutie možnosti premenovania.

- **Data_EditorsCount** – počet editorov v dokumente.

- **Data_ForceReadWriteReason** – celočíselná hodnota vyjadrujúca príčinu vynútenia prechodu súboru do režimu čítania/zapisovania.

- **Data_FSucceededAfterRecoverableFailure** – označuje, že otvorenie bolo úspešné po oprave zlyhania počas otvárania dokumentu.

- **Data_LastLoggedTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie, keď pokus o otvorenie zlyhá dvakrát (používa sa na diagnostiku kvality údajov).

- **Data_LinkStyles** – označuje, či vytvárame prepojenie na štýly šablóny.

- **Data_MainPdod** – identifikátor dokumentu v procese programu Office Word.

- **Data_Measurements** – šifrovaný reťazec obsahujúci časové rozdelenie jednotlivých častí otvárania. Používa sa na meranie výkonu.

- **Data_MoveDisabledReason** – chyba, pri ktorej sa vypne možnosť premiestnenia dokumentu.

- **Data_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania.

- **Data_PartsUnknown** – počet častí dokumentu, pre ktoré sa nám nepodarilo získať údaje.

- **Data_RecoverableFailureInitiationLocationTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie miesta v kóde, kde sme sa pokúsili opraviť súbor pred jeho otvorením.

- **Data_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania tohto dokumentu.

- **Data_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania.

- **Data_SecondaryTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na pridanie doplňujúcich údajov o zlyhaní na otvorenie. 

- **Data_TemplateFormat** – formát súboru šablóny, na ktorej je dokument založený.

- **Data_UsesNormal** – označuje, či otvorený dokument je založený na normálnej šablóne.

- **PathData_Doc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.


#### <a name="officewordfileopenopenffileopenxstzcore"></a>Office.Word.FileOpen.OpenFFileOpenXstzCore

Táto udalosť označuje, že Office Word otvára dokument, na ktorý používateľ dvakrát klikol. Obsahuje aj kritické údaje o výkone otvárania súboru a je udalosťou spustenia aplikácie z pohľadu používateľa. Udalosť monitoruje, či otvorenie súboru dvojitým kliknutím na súbor funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov.
    
- **Data_BytesAsynchronous** – počet bajtov (komprimovaných), bez ktorých podľa nás dokážeme otvoriť dokument, ak by sme ich dostali predtým, než používateľ chce začať upravovať, prípadne uložiť.
    
- **Data_BytesAsynchronousWithWork** – počet bajtov (komprimovaných), bez ktorých by sme možno dokázali otvoriť súbor, alebo vyžadovalo by si to značné investície do kódu.

- **Data_BytesSynchronous** – počet bajtov (komprimovaných), ktoré musíme mať predtým, než môžeme začať otvárať súbor.
    
- **Data_BytesUnknown** – počet bajtov v častiach dokumentu, ktoré podľa nás nenájdeme.

- **Data_DetachedDuration** – ako dlho bola aktivita odpojená od vlákna.

- **Data_Doc_AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť.

- **Data_Doc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_Doc_ChunkingType** – jednotky slúžiace na prírastkové otvorenie dokumentu.

- **Data_Doc_EdpState** – nastavenie ochrany elektronických údajov dokumentu.

- **Data_Doc_Ext** prípona dokumentu (docx, xlsb, pptx atď.)

- **Data_Doc_FileFormat** – verzia protokolu formátu súboru.

- **Data_Doc_Fqdn** – názov domény OneDrivu alebo SharePointu Online.

- **Data_Doc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény.

- **Data_Doc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – zaznamenáva, ako bol dokument otvorený.

- **Data_Doc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.

- **Data_Doc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_Doc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.
    
- **Data_Doc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_Doc_IsRtcAlwaysOn** – má hodnotu true, ak je kanál v reálnom čase (RTC) pre tento súbor vždy zapnutý.

- **Data_Doc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_Doc_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).
    
- **Data_Doc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_Doc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_Doc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie.

- **Data_Doc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_Doc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_Doc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).
    
- **Data_Doc_ServerVersion** – verzia servera, ktorý ponúka službu. 

- **Data_Doc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_Doc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_Doc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_Doc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_Doc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_Doc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_Doc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_Doc_WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI.

- **Data_EditorDisablingRename** – identifikátor prvého editora, ktorý spôsobil vypnutie možnosti premenovania.

- **Data_EditorsCount** – počet editorov v dokumente.

- **Data_FSucceededAfterRecoverableFailure** – označuje, že otvorenie bolo úspešné po oprave zlyhania počas otvárania dokumentu.

- **Data_ForceReadWriteReason** – celočíselná hodnota vyjadrujúca príčinu vynútenia prechodu súboru do režimu čítania/zapisovania.
    
- **Data_LastLoggedTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie, keď pokus o otvorenie zlyhá dvakrát (používa sa na diagnostiku kvality údajov).

- **Data_LinkStyles** – označuje, či vytvárame prepojenie na štýly šablóny.

- **Data_MainPdod** – identifikátor dokumentu v procese programu Office Word.

- **Data_Measurements** – šifrovaný reťazec obsahujúci časové rozdelenie jednotlivých častí otvárania. Používa sa na meranie výkonu.
    
- **Data_MoveDisabledReason** – chyba, pri ktorej sa vypne možnosť premiestnenia dokumentu.

- **Data_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania.

- **Data_PartsUnknown** – počet častí dokumentu, pre ktoré sa nám nepodarilo získať údaje.

- **Data_RecoverableFailureInitiationLocationTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie miesta v kóde, kde sme sa pokúsili opraviť súbor pred jeho otvorením.

- **Data_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania tohto dokumentu.

- **Data_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania.

- **Data_SecondaryTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na pridanie doplňujúcich údajov o zlyhaní na otvorenie.

- **Data_TemplateFormat** – formát súboru šablóny, na ktorej je dokument založený.

- **Data_UsesNormal** – označuje, či otvorený dokument je založený na normálnej šablóne.


#### <a name="officewordfileopenopenifrinitargs"></a>Office.Word.FileOpen.OpenIfrInitArgs

Táto udalosť označuje, že Office Word otvára dokument prostredníctvom aktivácie COM alebo príkazového riadka. Obsahuje aj kritické údaje o výkone otvárania súboru a je udalosťou spustenia aplikácie z pohľadu používateľa. Udalosť monitoruje, či otvorenie súboru z príkazového riadka funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

  - **Data\_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov.

  - **Data\_BytesAsynchronous** – počet bajtov (komprimovaných), bez ktorých podľa nás dokážeme otvoriť dokument, ak by sme ich dostali predtým, než používateľ chce začať upravovať, prípadne uložiť

  - **Data\_BytesAsynchronousWithWork** – počet bajtov (komprimovaných), bez ktorých by sme možno dokázali otvoriť súbor, alebo vyžadovalo by si to značné investície do kódu

  - **Data\_BytesSynchronous** – počet bajtov (komprimovaných), ktoré musíme mať predtým, než môžeme začať otvárať súbor

  - **Data\_BytesUnknown** – počet bajtov v častiach dokumentu, ktoré podľa nás nenájdeme.

  - **Data\_Doc\_AccessMode** – označuje, či je dokument iba na čítanie alebo editovateľný

  - **Data\_Doc\_AssistedReadingReasons** – preddefinovaná množina hodnôt toho, prečo bol dokument otvorený v režime asistovaného čítania

  - **Data\_Doc\_ChunkingType** – jednotky slúžiace na prírastkové otvorenie dokumentu

  - **Data\_Doc\_EdpState** – nastavenie ochrany elektronických údajov dokumentu

  - **Data\_Doc\_Ext** – prípona dokumentu (docx, xlsb, pptx atď.)

  - **Data\_Doc\_FileFormat** – verzia protokolu formátu súboru

  - **Data\_Doc\_Fqdn** – názov domény OneDrivu alebo SharePointu Online

  - **Data\_Doc\_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény

  - **Data\_Doc\_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností otvorenej požiadavky

  - **Data\_Doc\_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia

  - **Data\_Doc\_InitializationScenario** – zaznamenáva, ako bol dokument otvorený

  - **Data\_Doc\_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa

  - **Data\_Doc\_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo

  - **Data\_Doc\_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce

  - **Data\_Doc\_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline

  - **Data_Doc_IsRtcAlwaysOn** – má hodnotu true, ak je kanál v reálnom čase (RTC) pre tento súbor vždy zapnutý.

  - **Data\_Doc\_IsSyncBacked** – príznak, ktorý označuje, že v počítači existuje automaticky synchronizovaná kópia dokumentu

  - **Data\_Doc\_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.)

  - **Data\_Doc\_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument

  - **Data\_Doc\_NumberCoAuthors** – počet používateľov v relácii spoločných úprav

  - **Data\_Doc\_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie

  - **Data\_Doc\_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie

  - **Data\_Doc\_ResourceIdHash** – anonymizovaný identifikátor dokumentu, ktorý sa používa na diagnostiku problémov

  - **Data\_Doc\_ServerDocId** – nemenný anonymizovaný identifikátor dokumentu, ktorý sa používa na diagnostiku problémov

  - **Data\_Doc\_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou

  - **Data\_Doc\_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.)

  - **Data\_Doc\_ServerVersion** – verzia servera, ktorý ponúka službu

  - **Data\_Doc\_SessionId** – verzia servera, ktorý ponúka službu

  - **Data\_Doc\_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online

  - **Data\_Doc\_SizeInBytes** – indikátor veľkosti dokumentu

  - **Data\_Doc\_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu

  - **Data\_Doc\_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý

  - **Data\_Doc\_SyncBackedType** – indikátor typu dokumentu (lokálny alebo v službe)

  - **Data\_Doc\_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu

  - **Data\_Doc\_WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI

  - **Data\_EditorDisablingRename** – identifikátor prvého editora, ktorý spôsobil vypnutie možnosti premenovania

  - **Data\_EditorsCount** – počet editorov v dokumente

  - **Data\_FSucceededAfterRecoverableFailure** – označuje, že otvorenie bolo úspešné po oprave zlyhania počas otvárania dokumentu

  - **Data\_ForceReadWriteReason** – celočíselná hodnota vyjadrujúca príčinu vynútenia prechodu súboru do režimu čítania/zapisovania

  - **Data\_LastLoggedTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie, keď pokus o otvorenie zlyhá dvakrát (používa sa na diagnostiku kvality údajov)

  - **Data\_LinkStyles** – označuje, či vytvárame prepojenie na štýly šablóny

  - **Data\_MainPdod** – identifikátor dokumentu v procese programu Office Word

  - **Data\_Measurements** – šifrovaný reťazec obsahujúci časové rozdelenie jednotlivých častí otvárania. Používa sa na diagnostikovanie výkonu otvárania.

  - **Data\_MoveDisabledReason** – chyba, pri ktorej sa vypne možnosť premiestnenia dokumentu

  - **Data\_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania

  - **Data\_PartsUnknown** – počet častí dokumentu, pre ktoré sa nám nepodarilo získať údaje

  - **Data\_RecoverableFailureInitiationLocationTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie miesta v kóde, kde sme sa pokúsili opraviť súbor pred jeho otvorením

  - **Data\_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania tohto dokumentu

  - **Data\_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania

  - **Data\_SecondaryTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na pridanie doplňujúcich údajov o zlyhaní na otvorenie.

  - **Data\_TemplateFormat** – formát súboru šablóny, na ktorej je dokument založený.

  - **Data\_UsesNormal** – označuje, či otvorený dokument je založený na normálnej šablóne.


#### <a name="officewordfileopenopenloadfile"></a>Office.Word.FileOpen.OpenLoadFile

Táto udalosť označuje, že Office Word otvára dokument prostredníctvom dialógového okna Otvoriť. Obsahuje aj kritické údaje o výkone otvárania súboru a je udalosťou spustenia aplikácie z pohľadu používateľa. Udalosť monitoruje, či otvorenie súboru z dialógového okna Otvoriť funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov.

- **Data_BytesAsynchronous** – počet bajtov (komprimovaných), bez ktorých podľa nás dokážeme otvoriť dokument, ak by sme ich dostali predtým, než používateľ chce začať upravovať, prípadne uložiť.

- **Data_BytesAsynchronousWithWork** – počet bajtov (komprimovaných), bez ktorých by sme možno dokázali otvoriť súbor, alebo vyžadovalo by si to značné investície do kódu.
    
- **Data_BytesSynchronous** – počet bajtov (komprimovaných), ktoré musíme mať predtým, než môžeme začať otvárať súbor.

- **Data_BytesUnknown** – počet bajtov v častiach dokumentu, ktoré podľa nás nenájdeme.

- **Data_DetachedDuration** – ako dlho bola aktivita odpojená od vlákna.

- **Data_Doc_AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť.

- **Data_Doc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_Doc_ChunkingType** – jednotky slúžiace na prírastkové otvorenie dokumentu.

- **Data_Doc_EdpState** – nastavenie ochrany elektronických údajov dokumentu.

- **Data_Doc_Ext** prípona dokumentu (docx, xlsb, pptx atď.)

- **Data_Doc_FileFormat** – verzia protokolu formátu súboru.

- **Data_Doc_Fqdn** – názov domény OneDrivu alebo SharePointu Online.

- **Data_Doc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – zaznamenáva, ako bol dokument otvorený.

- **Data_Doc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_Doc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.
    
- **Data_Doc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_Doc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.

- **Data_Doc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_Doc_IsRtcAlwaysOn** – má hodnotu true, ak je kanál v reálnom čase (RTC) pre tento súbor vždy zapnutý.

- **Data_Doc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_Doc_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_Doc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_Doc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_Doc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie.

- **Data_Doc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_Doc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov. 

- **Data_Doc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_Doc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).

- **Data_Doc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_Doc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_Doc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_Doc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_Doc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_Doc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_Doc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_Doc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_EditorDisablingRename** – identifikátor prvého editora, ktorý spôsobil vypnutie možnosti premenovania.

- **Data_EditorsCount** – počet editorov v dokumente.

- **Data_ForceReadWriteReason** – celočíselná hodnota vyjadrujúca príčinu vynútenia prechodu súboru do režimu čítania/zapisovania.
    
- **Data_FSucceededAfterRecoverableFailure** – označuje, že otvorenie bolo úspešné po oprave zlyhania počas otvárania dokumentu.

- **Data_LastLoggedTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie, keď pokus o uloženie zlyhá dvakrát (používa sa na diagnostiku kvality údajov).

- **Data_LinkStyles** – označuje, či vytvárame prepojenie na štýly šablóny.

- **Data_MainPdod** – identifikátor dokumentu v procese programu Office Word.

- **Data_Measurements** – šifrovaný reťazec obsahujúci časové rozdelenie jednotlivých častí otvárania. Používa sa na meranie výkonu.

- **Data_MoveDisabledReason** – chyba, pri ktorej sa vypne možnosť premiestnenia dokumentu.

- **Data_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania.

- **Data_PartsUnknown** – počet častí dokumentu, pre ktoré sa nám nepodarilo získať údaje.

- **Data_RecoverableFailureInitiationLocationTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie miesta v kóde, kde sme sa pokúsili opraviť súbor pred jeho otvorením.

- **Data_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania tohto dokumentu.

- **Data_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania.

- **Data_SecondaryTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na pridanie doplňujúcich údajov o zlyhaní na otvorenie.

- **Data_TemplateFormat** – formát súboru šablóny, na ktorej je dokument založený.

- **Data_UsesNormal** – označuje, či otvorený dokument je založený na normálnej šablóne.


### <a name="office-accessibility-configuration-subtype"></a>*Podtyp Konfigurácia zjednodušenia ovládania balíka Office*

Funkcie zjednodušenia ovládania balíka Office

#### <a name="officeaccessibilityaccessibilitytoolsessionpresencewin32"></a>Office.Accessibility.AccessibilityToolSessionPresenceWin32

Umožňuje zistiť, či má používateľ nástroj pomocných technológií pre ľudí s postihnutím, a jeho názov. Vďaka tomu môžeme zistiť, či sa u používateľa balíka Office vyskytnú problémy s konkrétnym nástrojom pomocných technológií pre ľudí s postihnutím.

Zhromažďujú sa tieto polia:

  - **Data\_Data\_Jaws** – označuje, či bol nástroj Jaws spustený počas relácie**Data\_Data\_Magic** – označuje, či bol nástroj Magic spustený počas relácie

  - **Data\_Data\_Magnify** – označuje, či bol nástroj Zväčšovacie sklo spustený počas relácie

  - **Data\_Data\_Narrator** – označuje, či bol nástroj Moderátor spustený počas relácie

  - **Data\_Data\_NVDA** – označuje, či bol nástroj NVDA spustený počas relácie

  - **Data\_Data\_SA** – označuje, či bol nástroj SA spustený počas relácie

  - **Data\_Data\_Supernova** – označuje, či bol nástroj Supernova spustený počas relácie

  - **Data\_Data\_SuperNovaessSuite** – označuje, či bol balík SuperNovaAccessSuite spustený počas relácie

  - **Data\_Data\_WinEyes** – označuje, či bol nástroj WinEyes spustený počas relácie

  - **Data\_Data\_ZoomText** – označuje, či bol nástroj ZoomText spustený počas relácie

#### <a name="officewordaccessibilitylearningtoolsreadaloudplayreadaloud"></a>Office.Word.Accessibility.LearningTools.ReadAloud.PlayReadAloud

Táto udalosť označuje, že Office Word číta nahlas text v dokumente. Predstavuje prezenčný signál funkcie zjednodušenia ovládania, ktorá umožňuje spoločnosti Microsoft vyhodnotiť stav funkcie čítania textu nahlas.

Zhromažďujú sa tieto polia:

  - **Data\_CharacterCount** – počet znakov v dokumente

  - **Data\_CharactersWithSpaceCount**  – počet znakov a medzier v dokumente

  - **Data\_IsPageCountInProgress** – počet spracúvaných strán

  - **Data\_LineCount** – počet riadkov v dokumente

  - **Data\_PageCount** – počet strán v dokumente

  - **Data\_ParagraphCount** – počet odsekov v dokumente

  - **Data\_Play** – či Word číta nahlas prvýkrát

  - **Data\_ViewKind** – typ zobrazenia dokumentu

  - **Data\_WordCount** – počet slov v dokumente

#### <a name="officewordaccessibilitylearningtoolsreadaloudstopreadaloud"></a>Office.Word.Accessibility.LearningTools.ReadAloud.StopReadAloud

Táto udalosť označuje, že Office Word prestal čítať nahlas text v dokumente. Umožňuje spoločnosti Microsoft vyhodnotiť stav funkcie čítania textu nahlas meraním trvania fungovania.

Zhromažďujú sa tieto polia:

  - Žiadne

### <a name="privacy-subtype"></a>*Podtyp ochrany osobných údajov*

Nastavenia ochrany osobných údajov v Office 

#### <a name="officeintelligentserviceprivacyconsentprivacyevent"></a>Office.IntelligentService.PrivacyConsent.PrivacyEvent

Táto udalosť predstavuje akciu spustenú používateľom alebo systémom, ktorá je súčasťou ochrany osobných údajov pre Office. Spustí sa v dialógových oknách ochrany osobných údajov First Run, dialógové okno Ochrana osobných údajov konta a upozornenia na ochranu osobných údajov. Udalosť sa používa na pochopenie nasledujúcich krokov: používateľský súhlas s nastavením ochrany osobných údajov v Office, používateľská zmena nastavenia ochrany osobných údajov v Office a aktualizácia nastavenia ochrany osobných údajov balíka Office v používateľských reláciách.

Zhromažďujú sa tieto polia:

  - **Data_ActionId** – akcia používateľa v dialógovom okne Ochrana osobných údajov

  - **Data_ControllerConnectedServicesState** – nastavenie politiky používateľa s doplnkovými voliteľnými online funkciami

  - **Data_DownloadedContentServiceGroupState** – používateľské nastavenie pre stiahnutý obsah 
 
  - **Data_ForwardLinkId** – prepojenie na dokumentáciu k ochrane osobných údajov pre scenár používateľa

  - **Data_HRESULT** – záznam chýb počas interakcie s dialógovým oknom Ochrana osobných údajov

  - **Data_IsEnterpriseUser** – Kategória používateľských licencií

  - **Data_OfficeServiceConnectionState** – nastavenie pre používateľov online funkcií

  - **Data_RecordRegistry** – záznam zobrazujúci dialógové okno podnikovej ochrany osobných údajov

  - **Data_Scenario** – scenár prvého spustenia založený na používateľskej licencii a kategórii

  - **Data_SeenInsidersDialog** – záznam znázorňujúci dialógové okno Ochrana osobných údajov insiderov

  - **Data_SendTelemetryOption** – používateľské nastavenie pre telemetriu

  - **Data_SendTelemetryOptionPolicy** – používateľské nastavenie ochrany osobných údajov pre telemetriu

  - **Data_UserCategory** – typ používateľského konta  

  - **Data_UserCCSDisabled** – prepísanie používateľom pre doplnkové voliteľné online funkcie

   - **Data_UserContentServiceGroupState** – nastavenie používateľa na analyzovanie obsahu

  - **Data_WillShowDialogs** – záznam používateľa, ktorý potrebuje vidieť dialógové okná ochrany osobných údajov First Run



## <a name="product-and-service-performance-data-events"></a>Udalosti údajov v kategórii Výkon produktov a služieb

Toto sú podtypy údajov v tejto kategórii:
- [Neočakávané ukončenie (zlyhanie) aplikácie](#unexpected-application-exit-crash-subtype)
- [Výkon funkcie aplikácie](#application-feature-performance-subtype)
- [Chyba aktivity aplikácie](#application-activity-error-subtype)

### <a name="unexpected-application-exit-crash-subtype"></a>*Podtyp Neočakávané ukončenie (zlyhanie) aplikácie*

Neočakávané ukončenia aplikácie a stav aplikácie, keď sa to stane.

#### <a name="officeappdomainunhandledexceptionhandlerfailed"></a>Office.AppDomain.UnhandledExceptionHandlerFailed

Táto udalosť zhromažďuje informácie o všetkých nespracovaných výnimkách pri používaní aplikácie Data Streamer. Tieto údaje sa používajú na monitorovanie stavu aplikácie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Exception** – zásobník volaní pre výnimku

- **Event Name** – názov udalosti je kategória udalosti a označenie udalosti.

#### <a name="officeapplesystemhealthappexitmacandios"></a>Office.Apple.SystemHealthAppExitMacAndiOS

Udalosť spustenia, ktorá zachytáva úspešné a neúspešné ukončenia aplikácie na ďalšie skúmanie.

Zhromažďujú sa tieto polia:

- **AffectedProcessResidentMemoryOnCrash** – rezidentná pamäť aplikácie, ktorá zlyhala.

- **AffectedProcessSessionID** – ID relácie procesu v predchádzajúcom ukončení.

- **AffectedProcessUnsymbolicatedChecksum** – ide s hodnotou hash zásobníka pre symbolizáciu.

- **AffectedProcessVirtualMemoryOnCrash** – virtuálna pamäť aplikácie, ktorá zlyhala.

- **AffectedSessionBuildNumber** – verzia aplikácie.

- **AffectedSessionDuration** – trvanie relácie v sekúnd pred zlyhaním.

- **AffectedSessionIDSMatch** – boolovská hodnota na overenie, či je hlásené ID relácie rovnaké, aké získala funkcia MERP.

- **AffectedSessionLongBuildNumber** – dlhé číslo zostavy.

- **AffectedSessionMERPSessionID** – ID relácie funkcie MERP.

- **AffectedSessionOSLocale** – miestne nastavenie operačného systému.

- **AffectedSessionOSVersion** – verzia operačného systému.

- **AffectedSessionStackHash** – hodnota hash sledovania zásobníka aplikácie, ktorá zlyhala.

- **AffectedSessionStartTime** – dátum a čas začatia relácie.

- **AffectedSessionUAEType** – enumerácia, ktorá poskytuje informácie o tom, o aký typ zlyhania išlo.

- **AffectedSessionVersion** – verzia aplikácie.

- **DeviceModel** – model hardvéru.

- **ExitWasGraceful** – bolo predchádzajúce ukončenie aplikácie úspešné?

#### <a name="officeextensibilitycomaddinunhandledexception"></a>Office.Extensibility.COMAddinUnhandledException

Udalosť vygenerovaná pri zlyhaní doplnku COM

Počítačová analýza: používa sa ako čitateľ vo výpočte stavu špecifického pre podnik pre doplnky, ktoré sa používajú na odvodenie počas pilotného procesu, či je doplnok „pripravený na inováciu“ v produkčnom okruhu.  
Globálne prehľady: používa sa na výpočet globálnej „pripravenosti“ nešpecifickej pre podnik pre doplnok, ktorý sa potom uverejní na lokalite readyforwindows.com a v ďalších nástrojoch, ako je napríklad Readiness Toolkit

Zhromažďujú sa tieto polia:

- **ScopeId** – rozsah aktuálneho vlákna

- **Method** – metóda balíka Office, kde došlo k výnimke

- **Interface** – rozhranie balíka Office, kde došlo k výnimke

- **AddinId** – identifikátor triedy doplnku

- **AddinProgId** – identifikátor programu doplnku

- **AddinFriendlyName** – popisný názov doplnku

- **AddinTimeDateStamp** – časová pečiatka doplnku z metaúdajov knižnice DLL

- **AddinVersion** – verzia doplnku

- **AddinFileName** – názov súboru doplnku bez cesty k súboru

- **VSTOAddIn** – či doplnok je VSTO

- **AddinConnectFlag** – správanie pri aktuálnom načítaní

- **LoadAttempts** – počet pokusov o načítanie doplnku

#### <a name="officeextensibilitycomaddinunhandledexceptionenterprise"></a>Office.Extensibility.COMAddinUnhandledExceptionEnterprise

Udalosť vygenerovaná pri zlyhaní doplnku COM.  Používa sa ako čitateľ vo výpočte stavu špecifického pre podnik pre doplnky, ktoré sa používajú na odvodenie počas pilotného procesu, či je doplnok „pripravený na inováciu“ v produkčnom okruhu.

Zhromažďujú sa tieto polia (tieto polia sa zapisujú ako zástupné objekty, aby sa zabránilo porušeniu existujúcich skriptov: AddinFriendlyName, AddinProgId, AddinVersion, AddinFileName):


- **AddinConnectFlag** – správanie pri aktuálnom načítaní.

- **AddinFileName** – prázdne pole – zastarané.

- **AddinFriendlyName** – prázdne pole – zastarané.

- **AddinId** – ID triedy doplnku.

- **AddinProgId** – prázdne pole – zastarané.

- **AddinTimeDateStamp** – časová pečiatka doplnku z metaúdajov knižnice DLL.

- **AddinVersion** – prázdne pole – zastarané.

- **Interface** – rozhranie balíka Office, kde došlo k výnimke.

- **LoadAttempts** – počet pokusov o načítanie doplnku.

- **Method** – metóda balíka Office, kde došlo k výnimke.

- **ScopeId** – rozsah aktuálneho vlákna.

- **VSTOAddIn** – či doplnok je VSTO.

#### <a name="officeextensibilitysandboxodpactivationheartbeat"></a>Office.Extensibility.Sandbox.ODPActivationHeartbeat

Doplnky balíka Office sa spúšťajú v sandboxe. Táto udalosť zhromažďuje informácie o prezenčných signáloch pri aktiváciách. Pri zlyhaní doplnku sa v tejto udalosti zhromažďujú informácie o dôvodoch zlyhania sa v prípade, že súvisia s naším sandboxom. Používa sa na vyšetrovanie, keď zákazníci eskalujú problémy.
 
Zhromažďujú sa tieto polia:

- **AppID** – ID aplikácie.

- **AppInfo** – údaje týkajúce sa typu doplnku (pracovná tabla alebo režimu bez používateľského rozhrania alebo obsahu atď.) a typu poskytovateľa (omen, SharePoint, systém súborov atď.).

- **AppInstanceId** – ID inštancie aplikácie. 

- **AssetId** – ID položky aplikácie.

- **ErrorCode** – celkový strávený čas. 

- **NumberOfAddinsActivated** – počítadlo aktivovaných doplnkov.

- **RemoterType** – špecifikuje typ služby Remoter (dôveryhodná, nedôveryhodná, Win32webView, dôveryhodná funkcia definovaná používateľom atď.), ktorý sa používa na aktiváciu doplnku.

- **StoreType** – pôvod aplikácie.

#### <a name="officeextensibilityvbatelemetrybreak"></a>Office.Extensibility.VbaTelemetryBreak

Udalosť vygenerovaná, keď sa v súbore s povolenými makrami vyskytne chyba kompilácie alebo spustenia

Počítačová analýza: používa sa ako čitateľ vo výpočte stavu špecifického pre podnik pre typy makra (napr. makrá vo Worde, makrá v Exceli atď.), ktoré sa používajú na odvodenie počas pilotného procesu, či je doplnok „pripravený na inováciu“ v produkčnom okruhu.

Zhromažďujú sa tieto polia:

- **TagId** – identifikátor značky telemetrie

- **BreakReason** – dôvod prerušenia (spustenie, kompilácia, iná chyba)

- **SolutionType** – typ riešenia (dokument, šablóna, doplnok aplikácie, doplnok COM)

- **Data.ErrorCode** – kód chyby ohlásený nástrojom VBA


#### <a name="officefindtimeappfailedtostart"></a>Office.FindTime.AppFailedToStart

Zhromažďuje sa, ak spustenie aplikácie zlyhá z dôvodu výskytu neočakávanej chyby počas spúšťania. Používa na sledovanie výnimiek a zlyhaní.  Pomáha monitorovať a ladiť stav aplikácie.

Zhromažďujú sa tieto polia: 

- **DateTime** – časová pečiatka pri prihlasovaní udalosti.

- **EventName** – názov udalosti, ktorá sa práve zaznamenáva

#### <a name="officeoutlookdesktophangbucketmetrics"></a>Office.Outlook.Desktop.HangBucketMetrics

Zhromažďuje čas nereagovania pre nereagovania Outlooku – jedinečný identifikátor pre informácie o nereagovaní, uplynutom čase a zásobníku volaní. Údaje sa používajú na rozpoznávanie a identifikovanie zlyhaní aplikácií, aby ich bolo možné opraviť ich v budúcich aktualizáciách.

Zhromažďujú sa tieto polia:

  - **BucketId** – hodnota hash zásobníka volaní

  - **ElapsedTotal** – celkový čas strávený vo volaní

  - **ElapsedHanging** – čas nereagovania strávený vo volaní

#### <a name="officeoutlookdesktophangreportingscopeperfmetrics"></a>Office.Outlook.Desktop.HangReportingScopePerfMetrics

Zhromažďuje čas trvania základných scenárov Outlooku – switchfolder, switchmodule, sendmailoutbox, openitemclassic, sendmailtransport. Tieto údaje sa aktívne monitorujú na zisťovanie abnormálnych problémov s výkonom. Používa sa na zisťovanie a diagnostiku problémov s výkonom, ako aj na zlepšenie výkonu pri každej aktualizácii.

Zhromažďujú sa tieto polia:

  - **ElapsedTotal** – celkový čas strávený vo volaní

  - **ScopeId** – názov funkcie s vyhlásením alebo vlastným názvom priradeným prostredníctvom definície rozsahu

#### <a name="officeoutlookdesktopwatsonbuckets"></a>Office.Outlook.Desktop.WatsonBuckets

Toto pravidlo zhromažďuje informácie o zlyhaní z denníkov udalostí, keď Outlook zlyhal v predchádzajúcej relácii.

Tieto údaje sa aktívne monitorujú na zisťovanie abnormálnych nereagovaní. Používajú sa na rozpoznávanie a identifikovanie nereagovaní, aby ich bolo možné opraviť ich v budúcich aktualizáciách.

Zhromažďujú sa tieto polia:

  - **BucketId** – hodnota hash zásobníka volaní

  - **ElapsedTotal** – celkový čas strávený vo volaní

  - **ElapsedHanging** – čas nereagovania strávený vo volaní

#### <a name="officepowerpointsession"></a>**Office.PowerPoint.Session**

Zhromažďuje použitia funkcie v jednotlivých reláciách PowerPointu.Tieto údaje sa používajú na výpočet pomeru neželaného ukončenia PowerPointu pri používaní funkcie. Pomer neželaného ukončenia PowerPointu je kľúčový signál na zaručenie, že PowerPoint funguje podľa očakávania.

Zhromažďujú sa tieto polia:

  - **Flag** – príznaky relácie

  - **Usage** – použitia funkcie

#### <a name="officepowerpointuaedialog"></a>Office.PowerPoint.UAE.Dialog

Zhromažďuje sa vždy, keď sa PowerPoint neželane ukončí, keď je otvorené dialógové okno navrchu hlavného okna PowerPointu. Tieto informácie sú dôležité na zachytenie neželaných ukončení PowerPointu z dôvodu aktívneho dialógového okna, ktoré blokuje hlavné okno PowerPointu. Spoločnosť Microsoft používa tieto údaje na diagnostiku problému, aby sa zaručilo, že PowerPoint funguje podľa očakávaní.

Zhromažďujú sa tieto polia:

  - **DlgCnt** – celkový počet otvorených dialógových okien pri zlyhaní relácie

  - **DlgId** – identifikátor otvoreného dialógového okna

  - **IdType** – typ identifikátora otvoreného dialógového okna

  - **InitTime** – čas inicializovania zlyhanej relácie

  - **SessionId** – identifikátor zlyhanej relácie

  - **TopId** – identifikátor horného dialógového okna

  - **Version** – verzia zlyhanej relácie

#### <a name="officepowerpointuaedocument"></a>Office.PowerPoint.UAE.Document

Táto udalosť zhromažďuje informácie o tom, ktorá funkcia sa používa v dokumente, keď sa PowerPoint neželane ukončí. Tieto funkcie môžu zahŕňať prezentáciu, otváranie, ukladanie alebo úpravu dokumentu, spolutvorbu alebo vypínanie. Tieto informácie sú dôležité na zachytenie neželaných ukončení PowerPointu pri používaní funkcie. Spoločnosť Microsoft používa tieto údaje na diagnostiku problému, aby sa zaručilo, že PowerPoint funguje podľa očakávaní.

Zhromažďujú sa tieto polia:

  - **CoauthFlag** – príznaky používania spolutvorby

  - **CommandFlag** – príznaky úpravy dokumentu

  - **FileIOFlag** – príznaky používania IO súboru

  - **InitTime** – čas inicializovania zlyhanej relácie

  - **Location** – umiestnenie dokumentu

  - **ServerDocId** – identifikátor dokumentu na serveri

  - **SessionId** – identifikátor zlyhanej relácie

  - **UrlHash** – hodnota hash URL adresy dokumentu

  - **Usage** – použitia funkcie

  - **Version** – verzia zlyhanej relácie

#### <a name="officepowerpointuaeopen"></a>Office.PowerPoint.UAE.Open

Táto udalosť sa zhromažďuje vždy, keď sa PowerPoint neželane ukončí počas otvárania dokumentu. Tieto informácie sú dôležité na zachytenie neželaných ukončení PowerPointu počas otvárania dokumentu. Spoločnosť Microsoft používa tieto údaje na diagnostiku problému, aby sa zaručilo, že PowerPoint funguje podľa očakávaní.

Zhromažďujú sa tieto polia:

  - **FileUrlLocation** – URL umiestnenie dokumentu

  - **Flag** – príznaky otvorenia

  - **InitTime** – čas inicializovania zlyhanej relácie

  - **Location** – umiestnenie dokumentu

  - **OpenReason** – dôvod otvorenia

  - **ServerDocId** – identifikátor dokumentu na serveri

  - **SessionId** – identifikátor zlyhanej relácie

  - **UrlHash** – hodnota hash URL adresy dokumentu

  - **Version** – verzia zlyhanej relácie

#### <a name="officepowerpointuaesession"></a>Office.PowerPoint.UAE.Session

Táto udalosť zhromažďuje informácie o tom, ktorá funkcia sa používala, keď sa relácia PowerPointu neželane ukončila.Tieto informácie sú dôležité na zachytenie neželaných ukončení PowerPointu. Spoločnosť Microsoft používa tieto údaje na diagnostiku problému, aby sa zaručilo, že PowerPoint funguje podľa očakávaní.

Zhromažďujú sa tieto polia:

  - **Flag** – príznaky relácie

  - **InitTime** – čas inicializovania zlyhanej relácie

  - **PreviousSessionId** – identifikátor zlyhanej relácie

  - **Usage** – použitia funkcie

  - **Version** – verzia zlyhanej relácie

#### <a name="officepowerpointuaeshutdown"></a>Office.PowerPoint.UAE.Shutdown

Táto udalosť sa zhromažďuje, keď sa PowerPoint neželane ukončí počas vypínania. Tieto informácie sú dôležité na zachytenie neželaných ukončení PowerPointu počas vypínania. Spoločnosť Microsoft používa tieto údaje na diagnostiku problému, aby sa zaručilo, že PowerPoint funguje podľa očakávaní.

Zhromažďujú sa tieto polia:

  - **InitTime** – čas inicializovania zlyhanej relácie

  - **SessionId** – identifikátor zlyhanej relácie

  - **Stage** – fáza vypnutia

  - **Version** – verzia zlyhanej relácie

#### <a name="officepowerpointuaeslideshow"></a>Office.PowerPoint.UAE.SlideShow

Táto udalosť sa zhromažďuje, keď sa PowerPoint neželane ukončí počas vypínania. Tieto informácie sú dôležité na zachytenie neželaných ukončení PowerPointu počas vypínania. Spoločnosť Microsoft používa tieto údaje na diagnostiku problému, aby sa zaručilo, že PowerPoint funguje podľa očakávaní.

Zhromažďujú sa tieto polia:

  - **InitTime** – čas inicializovania zlyhanej relácie

  - **Mode** – režim prezentácie

  - **SessionId** – identifikátor zlyhanej relácie

  - **State** – stav prezentácie

  - **Version** – verzia zlyhanej relácie

#### <a name="officeprogrammabilitytelemetryaddincrash"></a>Office.Programmability.Telemetry.AddInCrash

Udalosť vygenerovaná pri načítaní doplnku COM. Tieto informácie sú dôležité na určenie, či doplnok spôsobil zlyhanie aplikácie balíka Office. Používajú sa na posúdenie globálnej kompatibility doplnku s aplikáciami balíka Office.

Zhromažďujú sa tieto polia:

  - **CLSID** – identifikátor triedy doplnku

  - **ConnectFlag** – správanie pri aktuálnom načítaní doplnku

  - **FileName** – názov súboru doplnku bez cesty k súboru

  - **FriendlyName** – popisný názov doplnku

  - **Interface** – rozhranie balíka Office, kde došlo k výnimke

  - **LoadAttempts** – počet pokusov o načítanie doplnku

  - **Method** – metóda balíka Office, kde došlo k výnimke

  - **OfficeApplication** – aplikácia balíka Office, v ktorej došlo k výnimke

  - **OfficeVersion** – verzia balíka Office

  - **ProgID** – identifikátor programu doplnku

#### <a name="officesystemsystemhealthungracefulappexitmacandios"></a>Office.System.SystemHealthUngracefulAppExitMacAndiOS

Udalosť spustenia, ktorá zachytáva neúspešné ukončenia aplikácie na ďalšie skúmanie.

Zhromažďujú sa tieto polia:

- **AffectedProcessAppBuild** – číslo zostavy.

- **AffectedProcessAppBuildRevision** – číslo revízie zostavy.

- **AffectedProcessAppMajorVer** – číslo hlavnej verzie aplikácie.

- **AffectedProcessAppMinorVer** – číslo vedľajšej verzie aplikácie.

- **AffectedProcessAppName** – názov aplikácie.

- **AffectedProcessResidentMemoryOnCrash** – rezidentná pamäť aplikácie, ktorá zlyhala.

- **AffectedProcessUnsymbolicatedChecksum** – ide s hodnotou hash zásobníka pre symbolizáciu.

- **AffectedProcessVirtualMemoryOnCrash** – virtuálna pamäť aplikácie, ktorá zlyhala.

- **AffectedSessionDuration** – trvanie relácie v sekúnd pred zlyhaním.

- **AffectedSessionLongBuildNumber** – dlhé číslo zostavy.

- **CrashedProcessSessionID** – ID relácie procesu v zlyhaní aplikácie.

- **DetectionTime** – dátum a čas zlyhania aplikácie.
    
- **DeviceModel** – model hardvéru.

- **MERPSessionID** – ID relácie funkcie MERP.

- **ReportingOsLocaleTag** – miestne nastavenie operačného systému.

- **ReportingOSVerStr** – verzia operačného systému.

- **SessionBuildNumber** – verzia aplikácie, ktorá zlyhala.

- **SessionIDSMatch** – boolovská hodnota na overenie, či je hlásené ID relácie rovnaké, aké získala funkcia MERP.

- **SessionVersion** – verzia aplikácie, ktorá zlyhala – **StackHash** – hodnota hash sledovania zásobníka aplikácie, ktorá zlyhala.

- **UAEType** – enumerácia, ktorá poskytuje informácie o tom, o aký typ zlyhania išlo.

#### <a name="officethisaddinstartupfailed"></a>Office.ThisAddIn.StartupFailed

Táto udalosť zhromažďuje informácie o výnimke, ktorá sa vyskytne počas spúšťania aplikácie Data Streamer. Tieto údaje sa používajú na monitorovanie stavu aplikácie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Exception** – zásobník volaní pre výnimku

- **Event Name** – názov udalosti je kategória udalosti a označenie udalosti.


### <a name="application-feature-performance-subtype"></a>*Podtyp Výkon funkcie aplikácie*

Dlhý čas odozvy alebo nízky výkon v prípadoch ako spustenie aplikácie alebo otvorenie súboru.

#### <a name="officeextensibilityrichapimethodinvocation"></a>Office.Extensibility.RichApiMethodInvocation

Keď zákazník použije doplnok balíka Office a zavolá rozhranie Rich API na poskytnutie služby, spustí sa táto udalosť. Používa sa na meranie spoľahlivosti služby, jej výkonu a používania pri vyvolaní metódy rozhrania Rich API.
 
Zhromažďujú sa tieto polia:

- **Api** – úplný názov rozhrania API.

- **DispFlag** – bitový príznak s popisom typu volania metódy (napr.: 0x1 = METHOD, 0x2 = PROPERTYGET, 0x4 = PROPERTYPUT, 0x8 = PROPERTYPUTREF).

- **DispId** – ID odosielania volanej metódu.

- **HResult** – hodnota HResult volania metódy.

- **Latency** – časové oneskorenie volania v mikrosekundách.

- **ReqId** – identifikátor GUID dávkovej žiadosti, ktorej súčasťou je táto metóda.

- **TypeId** – identifikátor GUID rozhrania, v ktorom je táto metóda volaná.


#### <a name="officemanageabilityserviceapplypolicy"></a>Office.Manageability.Service.ApplyPolicy

Veľmi dôležitá telemetria na sledovanie zlyhania\\úspešnosti použitia nastavení cloudovej politiky na databázu Registry. Pole LastError obsahuje informáciu o tom, prečo a kde zlyhalo použitie politiky v databáze Registry.

Zhromažďujú sa tieto polia:

  - **Data.ApplyLogMsg** – hlásenie výnimky, ak sa vyskytla, počas aplikovania politiky

  - **Data.Cid** – dynamicky generovaný identifikátor korelácie odoslaný do služby, keď sa uskutočnilo volanie služby na načítanie cloudovej politiky. Používa sa na koreláciu, ktoré volanie spôsobilo problém počas aplikovania politík v cloude.

  - **Data.Last Error** – jedna z piatich hodnôt reťazcov (enumerátorov) na zaznamenanie toho, ktorá fáza aplikovania politiky sa vykonávala, keď sa vyskytla výnimka

#### <a name="officeoutlookdesktopbootperfmetrics"></a>Office.Outlook.Desktop.BootPerfMetrics

Táto udalosť zhromažďuje čas potrebný na spustenie Outlooku. Čas spúšťania Outlooku sa aktívne monitoruje na zisťovanie a diagnostiku regresií. Používa sa aj na diagnostikovanie eskalácií zákazníkov, ako aj na postupné zlepšovanie výkonu spúšťania.

Zhromažďujú sa tieto polia:

  - **AddinElapsedTotal** – celkový čas strávený načítavaním doplnkov

  - **CredPromptCount** – počet zobrazených výziev na zadanie poverení

  - **ElapsedTotal** – celkový čas strávený spúšťaním

  - **IsLoggingEnabled** – či je zapisovanie do denníka povolené

  - **ShowChooseProfileDlg** – či sa zobrazilo dialógové okno výberu profilu

  - **ShowFirstRunDlg** – či ide o prvé spustenie Outlooku

  - **ShowIMAPSrchfldWarningDlg** – výstrahy v prípade konta IMAP s ANSI PST

  - **ShowNeedSupportDlg** – dialógové okno podpory spustené zlyhaním pri spustení

  - **ShowSafeModeDlg** – či sa relácia otvorila v núdzovom režime

  - **ShowScanPstDlg** – zobrazuje, či sa pri kontrole opravy ukladacieho priestoru zobrazilo chybové hlásenie


#### <a name="officeoutlookmacbootperf"></a>Office.Outlook.Mac.BootPerf

Táto udalosť zhromažďuje čas potrebný na spustenie Outlooku. Čas spúšťania Outlooku sa aktívne monitoruje na zisťovanie a diagnostiku regresií. Používa sa aj na diagnostikovanie eskalácií zákazníkov, ako aj na postupné zlepšovanie výkonu spúšťania.

Zhromažďujú sa tieto polia:

- **MacOLKBootPerfDuration** – celkový čas strávený spúšťaním.

- **MacOLKBootPerfID** – identifikátor času stráveného spúšťaním.


#### <a name="officeoutlookmacperformanceunresponsive"></a>Office.Outlook.Mac.PerformanceUnresponsive

Používa sa na identifikovanie problémov s vplyvom na používateľov v Outlooku, ktoré sa môžu prejaviť v zníženom výkone. 

Zhromažďujú sa tieto polia:

- **Duration** – čas, ktorý uplynul pri zníženom výkone.

- **EventType** – typ udalosti so zníženým výkonom.


#### <a name="officeperformanceboot"></a>Office.Performance.Boot

Táto udalosť sa zhromažďuje pri spustení aplikácie balíka Office. Obsahuje informácie o tom, či spustenie bolo iniciované otvorením súboru alebo spustením prostredníctvom ponuky Štart, či išlo o prvé spustenie aplikácie, aké množstvo pamäte aplikácia používa a či sa používateľovi zobrazilo nejaké blokujúce používateľské rozhranie. Používa sa na meranie rýchlosti spustenia aplikácií balíka Office a množstva pamäte, ktoré používajú pri štarte, aby sa zaistilo, že je to prijateľné pre používateľa.

Zhromažďujú sa tieto polia:

  - **ActivationKind** – zobrazuje, či sa aplikácia spustila spustením z ponuky Štart, otvorením súboru alebo prostredníctvom automatizácie OLE.

  - **FirstBoot** – zobrazuje, či išlo o prvé spustenie aplikácie.

  - **InitializationDuration** – trvanie prvej inicializácie procesu balíka Office v mikrosekundách.

  - **InterruptionMessageId** – ID dialógového okna, ak bolo spustenie prerušené dialógovým oknom s výzvou pre používateľa na zadanie údajov.

  - **TotalWorkingSetMB** – množstvo pamäte v megabajtoch v pracovnej sade procesu.

  - **VirtualSetMB** – množstvo pamäte v megabajtoch vo virtuálnej sade procesu. (Len MacOS/iOS)

  - **WorkingSetPeakMB** – najväčšie množstvo pamäte v megabajtoch, ktoré bolo doteraz v pracovnej sade procesu.

#### <a name="officeuxofficeinsidershowofficeinsiderdlg"></a>Office.UX.OfficeInsider.ShowOfficeInsiderDlg

Kritické sledovanie signálu interakcie používateľa s dialógovým oknom Zapojte sa do programu Office Insider. Používa sa na identifikáciu všetkých problémov s vykonaním zmien iniciovaných používateľmi, ako je napríklad zapojenie sa do programu Office Insider alebo vystúpenie z neho a zmena úrovne programu Office Insider.

Zhromažďujú sa tieto polia:

- **Data_AcceptedContactMeNew** – označuje, či používateľ prijal, že bude kontaktovaný spoločnosťou Microsoft pri zapojení do programu Office Insider.

- **Data_InsiderLevel** – úroveň programu Insider pri otvorení dialógového okna „Zapojte sa do programu Office Insider“.

- **Data_InsiderLevelNew** – úroveň programu Insider pri zatvorení dialógového okna „Zapojte sa do programu Office Insider“.

- **Data_IsInternalUser** – označuje, či je aplikácia spustená s prihlasovacími údajmi podnikového konta Microsoft.

- **Data_IsInternalUserInit** – označuje, či kód dokázal určiť, či je aplikácia spustená s prihlasovacími údajmi podnikového konta Microsoft.

- **Data_OpenNewsletterWebpage** – označuje, či sa spustilo prepojenie prihlásenia na odber bulletinu Office Insider s podmienkou, že sa používateľ zapojil do programu Office Insider, funkcia odberu bulletinu je zapnutá a používateľ nezrušil otvorenie webovej stránky prihlásenia na odber bulletinu Office Insider.
    
- **Data_RegisterInsider** – stav registrácie v programe Office Insider.

- **Data_RegisterInsiderHr** – výsledný kód registrácie v programe Office Insider.

#### <a name="officeuxofficeinsidercanshowofficeinsiderslab"></a>Office.UX.OfficeInsider.CanShowOfficeInsiderSlab

Sledovanie aktivity, či sa blok Office Insider môže zobrazovať používateľovi na karte Konto v používateľskom rozhraní Office Backstage.

Zhromažďujú sa tieto polia:

  - **Data_CanShow** – označuje, či sa blok Office Insider môže zobrazovať používateľovi na karte Konto v používateľskom rozhraní Office Backstage.
  
  - **Data_Event** – nepoužíva sa

  - **Data_EventInfo** – nepoužíva sa

  - **Data_Reason** – nepoužíva sa


#### <a name="officevisiosharedvisiofilerender"></a>Office.Visio.Shared.VisioFileRender

Táto udalosť zachytáva čas vykreslenia súboru. Pomáha nám uchovávať výkon vykresľovania súboru pod kontrolou.

Zhromažďujú sa tieto polia:

  - **Data\_AvgTime: integer** – priemerný čas vykreslenia kresby Visia v relácii

  - **Data\_CompositeSurfEnabled: bool** * má hodnotu true, ak je povolený režim kompozitného vykresľovania

  - **Data\_Count: integer** – koľkokrát Visio vykreslilo kresbu v relácii

  - **Data\_FirstRenderTime: long** – trvanie vykreslenia súboru pri prvom spustení v milisekundách

  - **Data\_MaxTime: integer** – maximálny čas vykreslenia diagramu Visia v relácii

#### <a name="officevisiovisiofileopenreliability"></a>Office.Visio.VisioFileOpenReliability

Táto udalosť zhromažďuje údaje o výkone otvárania súborov pre Visio Dev16. Používa sa na monitorovanie výkonu funkcie otvárania súborov a spája ho s vlastnosťami súboru, ako je napríklad veľkosť súboru, pre Visio Dev16. Vlastnosti súboru nám umožňujú rýchlejšie ladiť problémy a zistiť ich prvotnú príčinu.

Zhromažďujú sa tieto polia:

  - **Data\_CorrelationId: string** – identifikátor korelácie dokumentu

  - **Data\_DocIsEnterpriseProtected: bool** – má hodnotu true, ak je dokument chránený technológiou Windows Information Protection

  - **Data\_DocumentId: string** – identifikátor GUID cesty k súboru

  - **Data\_DurationToCompleteInMilliseconds: double** – čas potrebný na dokončenie funkcie Uložiť ako v milisekundách

  - **Data\_DurationToCompleteInMillisecondsSquared: double** – druhá mocnina poľa DurationToCompleteInMilliseconds

  - **Data\_ErrorCode: integer** – interný kód chyby pre zlyhanie otvárania súboru

  - **Data\_Extension\_Docs: string** – prípona súboru otvoreného diagramu

  - **Data\_FileIOBytesRead: int** – celkový počet bajtov prečítaných počas ukladania

  - **Data\_FileIOBytesReadSquared: int** – druhá mocnina poľa Data\_FileIOBytesRead

  - **Data\_FileIOBytesWritten: int** – celkový počet bajtov zapísaných počas ukladania

  - **Data\_FileIOBytesReadWritten: int** – druhá mocnina poľa Data\_FileIOBytesWritten

  - **Data\_FileName: binary** – binárna hodnota hash názvu súboru

  - **Data\_FileOpenDownloadDurationInMs: long** – trvanie do stiahnutia súboru v milisekundách

  - **Data\_FileOpenEndDurationInMs: long** – trvanie do otvorenia súboru v milisekundách

  - **Data\_FileOpenTimeStamp: time:** – časová pečiatka začatia otvárania súboru

  - **Data\_FilePathHash: binary** – identifikátor GUID cesty k súboru

  - **Data\_FileSize: long** – veľkosť dokumentu v bajtoch

  - **Data\_FileType: string** – prípona súboru otvoreného diagramu

  - **Data\_IsInternalFile: bool** – má hodnotu true, ak ide o interný súbor. Napr. vzorkovnica

  - **Data\_IsIRM: bool** – má hodnotu true, ak súbor je chránený technológiou IRM

  - **Data\_IsReadOnly: bool** – má hodnotu true, ak súbor je len na čítanie

  - **Data\_IsSuccess: bool** – má hodnotu true, ak otvorenie súboru bolo úspešné

  - **Data\_Location: string** – umiestnenie súboru, napr. Local, SharePoint, OneDrive, WopiConsumer, WopiBusiness, GenericThirdPartyConsumer

  - **Data\_NetworkIOBytesRead: int** – celkový počet sieťových bajtov prečítaných počas ukladania

  - **Data\_NetworkIOBytesReadSquared: int** – druhá mocnina poľa Data\_NetworkIOBytesRead

  - **Data\_NetworkIOBytesWritten: int** – celkový počet sieťových bajtov zapísaných počas ukladania

  - **Data\_NetworkIOBytesWrittenSquared: int** – druhá mocnina poľa NetworkIOBytesWritten

  - **Data\_OpenLocation:integer** – umiestnenie súboru, z ktorého bol otvorený, 0 lokálny, 1 sieť, 2 SharePoint, 3 web

  - **Data\_Size\_Docs: integer** 

  - **Data\_Tag: string** – jedinečný identifikátor na identifikáciu udalosti Uložiť ako

  - **Data\_WasSuccessful:bool** – má hodnotu true, ak otvorenie ako bolo úspešné

### <a name="application-activity-error-subtype"></a>*Podtyp Chyba aktivity aplikácie*

Chyby funkčnosti funkcie alebo používateľského rozhrania.

#### <a name="officeairspacebackendwin32graphicsdriversofthang"></a>Office.AirSpace.Backend.Win32.GraphicsDriverSoftHang 

Táto udalosť pomáha spoločnosti Microsoft oddeľovať dlhé nereagovania ovládača grafickej karty od krátkych, čo pomáha pri rozhodovaní o tom, ktoré ovládače grafickej karty môžu mať problémy. Ovládač grafickej karty používateľa spôsobil nereagovanie balíka Office, ale vplyv nereagovania ešte nie je známy.

Zhromažďujú sa tieto polia:

  - **Údaje\_InDeviceCall** – metóda zavolaná grafickou kartou, ktorá spôsobila nereagovanie

  - **Data\_Timeout** – ako dlho nereagovanie trvalo

#### <a name="officeextensibilitysandboxodperrornotification"></a>Office.Extensibility.Sandbox.ODPErrorNotification

Sleduje rôzne upozornenia na chyby získané zo sandboxu. Používa sa na zisťovanie scenárov chýb v sandboxe a zvyšovanie produktivity používateľa pomocou opravy.
 
Zhromažďujú sa tieto polia:

- **AppID** – ID aplikácie.

- **AppUrl** – vyčistená URL adresa aplikácie. 

- **Result** -výsledný kód chyby.


#### <a name="officegraphicsarcexceptions"></a>Office.Graphics.ARCExceptions 

Tieto informácie o nahlásení výnimky sú dôležité na posúdenie celkového stavu zásobníka grafiky, ako aj na identifikáciu častí kódu, v ktorých sa zlyhania vyskytujú s vysokou frekvenciou, aby sa stanovili priority skúmania. Tieto informácie o nahlásení výnimky sú dôležité na posúdenie celkového stavu zásobníka grafiky, ako aj na identifikáciu častí kódu, v ktorých sa zlyhania vyskytujú s vysokou frekvenciou. Pomáhajú inžinierovi určiť, ktoré zlyhania vykresľovania ovplyvňujú väčšinu používateľov, čo nám umožní stanoviť priority nášho skúmania s cieľom vyriešenia problémov, ktoré budú mať najväčší úžitok pre používateľov.

Zhromažďujú sa tieto polia:

  - **Data\_HResult** – chybový kód vrátený zo zlyhania

  - **Data\_TagCount** – počet všetkých zlyhaní, ktoré sa vyskytli

  - **Data\_TagID** – identifikátor zlyhania, ktoré sa vyskytlo

#### <a name="officeoutlookdesktopcalendaracceptcalsharenavigatetosharedfolder_error"></a>Office.Outlook.Desktop.Calendar.AcceptCalShareNavigateToSharedFolder\_Error

Táto udalosť zhromažďuje informácie, keď dôjde k zlyhaniu pri navigácii do zdieľaného kalendára. Tieto údaje sa používajú na monitorovanie stavu rozhrania API zdieľania kalendára, ako aj interakcie Outlooku so zdieľanými kalendármi.

Zhromažďujú sa tieto polia:

  - **FailedCaseHResult** – chybový kód vrátený zo zlyhania

#### <a name="officeoutlookdesktopedpedpopenstorefailure"></a>Office.Outlook.Desktop.EDP.EDPOpenStoreFailure

Úspešné alebo neúspešné otvorenie e-mailového ukladacieho priestoru chráneného technológiou Enterprise Data Protection na základe výsledku volania rozhrania API systému Windows na získanie kľúča na dešifrovanie ukladacieho priestoru. Táto udalosť sa používa na diagnostikovanie jedného z najčastejších problémov s technológiou Enterprise Data Protection, ktorý môže zabrániť spusteniu Outlooku. Primárnou príčinou zlyhania je interakcia Outlooku s rozhraním API systému Windows, ktoré sa používa na dešifrovanie kľúča ukladacieho priestoru.

Zhromažďujú sa tieto polia:

  - **HVA Activity** **-** s vlastnými údajovými poliami

  - **IsFlightOn** – označuje, či EDPDecryption Flight je povolené

#### <a name="officeoutlookdesktopndbcorruptionresult"></a>Office.Outlook.Desktop.NdbCorruptionResult

Udalosti Office.Outlook.Desktop.NdbCorruptionResult a Office.Outlook.Desktop.NDBCorruptStore.Warning sa zhromažďujú, keď zistíme poškodenie súboru súborov PST/OST používateľa. Keď zistíme poškodenie, spoločnosť Microsoft zhromažďuje formát databázy, miesto zistenia a malé množstvo kontextu o poškodení. Poškodenie súborov OST/PST zabraňuje používateľom v prístupe k e-mailom. Tieto údaje sa aktívne monitorujú na zisťovanie abnormálnej aktivity. Našou snahou je skúmať a diagnostikovať problémy na obmedzenie straty údajov zákazníkov.

Zhromažďujú sa tieto polia:

  - **0** – názov procesu, ktorý nahlásil poškodenie

  - **1** * logická hodnota, ktorá označuje, či si používateľ vybral nový súbor alebo nie

  - **2** – počet ďalších procesov, ktoré majú otvorenú databázu

#### <a name="officeoutlookdesktopndbcorruptstorewarning"></a>Office.Outlook.Desktop.NDBCorruptStore.Warning

Udalosti Office.Outlook.Desktop.NdbCorruptionResult a Office.Outlook.Desktop.NDBCorruptStore.Warning sa zhromažďujú, keď zistíme poškodenie súboru súborov PST/OST používateľa. Keď zistíme poškodenie, spoločnosť Microsoft zhromažďuje formát databázy, miesto zistenia a malé množstvo kontextu o poškodení. Poškodenie súborov OST/PST zabraňuje používateľom v prístupe k e-mailom. Tieto údaje sa aktívne monitorujú na zisťovanie abnormálnej aktivity. Našou snahou je skúmať a diagnostikovať problémy na obmedzenie straty údajov zákazníkov.

Zhromažďujú sa tieto polia:

  - **CollectionTime** – čas zhromaždenia

  - **Context** – kontext poškodeného ukladacieho priestoru, kde sa zistilo poškodenie

  - **CreatedWithVersion** – (voliteľné) pole s verziou ukladacieho priestoru

  - **Details** – podrobnosti o zlyhaní

  - **NdbType** – typ ukladacieho priestoru, môže byť 0 = NdbUndefined; 1 = NdbSmall; 2 = NdbLarge; 3 = NdbTardis

  - **ProcessName** – názov procesu spôsobujúceho poškodenie ukladacieho priestoru

  - **PstVersion** – verzia súboru MSPST32.DLL

  - **Version** – verzia formátu súboru ukladacieho priestoru

#### <a name="officeoutlookdesktopoutlookcalendarusageerrmeetrcptforwardactionsruleo16"></a>Office.Outlook.Desktop.OutlookCalendarUsageErr.MeetRcpt.ForwardActions.Rule.O16

Táto udalosť zhromažďuje úspech a neúspech akcie Preposlať, Preposlať ako prílohu a Preposlať vo formáte iCalendar pre odpovede na jednoduché, opakované a výnimočné schôdze v zobrazení Outlooku Pošta, Kalendár a Inšpektor. Miera zlyhania akcií Preposlať, Preposlať ako prílohu a Preposlať vo formáte iCalendar sa aktívne monitoruje na zisťovanie anomálií. Abnormálna štatistika označuje zlyhanie schopnosti Outlooku vykonávať základné operácie kalendára. Tieto údaje sa používajú aj na diagnostiku ďalších problémov súvisiacich s kalendárom, ktoré sa môžu zistiť.

Zhromažďujú sa tieto polia:

  - **CountExceptionForward** – počet preposlaných výnimiek schôdzí.

  - **CountExceptionForwardAsiCal** – počet preposlaných výnimiek schôdzí ako iCal.

  - **CountExceptionForwardInSplit** – počet preposlaných výnimiek schôdzí z ponuky Rozdeliť na páse s nástrojmi.

  - **CountExceptionForwardWithAttach** – počet preposlaných výnimiek schôdzí ako príloha.

  - **CountExceptionForward** – počet preposlaných opakovaných schôdzí.

  - **CountExceptionForwardAsiCal** – počet preposlaných opakovaných schôdzí ako iCal.

  - **CountRecurringForwardInSplit** – počet preposlaných opakovaných schôdzí z ponuky Rozdeliť na páse s nástrojmi.

  - **CountExceptionForwardWithAttach** – počet preposlaných opakovaných schôdzí ako príloha.

  - **CountSingleForward** – počet preposlaných jednotlivých schôdzí.

  - **CountSingleForwardAsiCal** – počet preposlaných jednotlivých schôdzí ako iCal.

  - **CountSingleForwardInSplit** – počet preposlaných jednotlivých schôdzí z ponuky Rozdeliť na páse s nástrojmi.

  - **CountSingleForwardWithAttach** – počet preposlaných jednotlivých schôdzí ako príloha.

  - **HResult** – kód chyby.

  - **OlkViewName** – označuje zobrazenie Pošta, Kalendár alebo Inšpektor.

#### <a name="officeoutlookdesktopoutlookcalendarusageerrmeetrcptreplyactionsruleo16"></a>Office.Outlook.Desktop.OutlookCalendarUsageErr.MeetRcpt.ReplyActions.Rule.O16

Táto udalosť zhromažďuje úspech a neúspech akcie Odpovedať, Odpovedať všetkým, Odpovedať okamžitou správou a Odpovedať všetkým okamžitou správou pre odpovede na jednoduché, opakované a výnimočné schôdze v zobrazení Outlooku Pošta, Kalendár a Inšpektor. Miera zlyhania akcií Odpovedať, Odpovedať všetkým, Odpovedať okamžitou správou a Odpovedať všetkým okamžitou správou sa aktívne monitoruje na zisťovanie anomálií. Abnormálna štatistika označuje zlyhanie schopnosti Outlooku vykonávať základné operácie kalendára. Tieto údaje sa používajú aj na diagnostiku ďalších problémov súvisiacich s kalendárom, ktoré sa môžu zistiť.

Zhromažďujú sa tieto polia:

  - **CountExceptionReply** – počet odpovedí na výnimky schôdzí.

  - **CountExceptionReplyAll** – počet odpovedí všetkým na výnimky schôdzí.

  - **CountExceptionReplyAllWithIM** – počet odpovedí všetkým okamžitou správou na výnimky schôdzí.

  - **CountExceptionReplyWithIM** – počet odpovedí okamžitou správou na výnimky schôdzí.

  - **CountRecurringReply** – počet odpovedí na opakované schôdze.

  - **CountRecurringReplyAll** – počet odpovedí všetkým na opakované schôdze.

  - **CountRecurringReplyAllWithIM** – počet odpovedí všetkým okamžitou správou na opakované schôdze.

  - **CountRecurringReplyWithIM** – počet odpovedí okamžitou správou na opakované schôdze.

  - **CountSingleReply** – počet odpovedí na jednotlivé schôdze.

  - **CountSingleReplyAll** – počet odpovedí všetkým na jednotlivé schôdze.

  - **CountSingleReplyAllWithIM** – počet odpovedí všetkým okamžitou správou na jednotlivé schôdze.

  - **CountSingleReplyWithIM** – počet odpovedí okamžitou správou na jednotlivé schôdze.

  - **HResult** – kód chyby.

  - **OlkViewName** – označuje zobrazenie Pošta, Kalendár alebo Inšpektor.

#### <a name="officeoutlookdesktopoutlookprivsdlgsingleuserloadfail"></a>Office.Outlook.Desktop.OutlookPrivsDlgSingleUser.LoadFail

Toto pravidlo zhromažďuje chyby zdieľania kalendára pri pridávaní nového používateľa (typu EX alebo SMTP) z adresára. Tieto údaje sa používajú na diagnostikovanie a riešenie problémov zistených v dialógovom okne Zdieľanie kalendára

Zhromažďujú sa tieto polia:

  - **CountAccountWizardEnd** – koľkokrát sa dialógové okno staršieho sprievodcu ukončilo

  - **CountCreatePIMAccount** – koľkokrát používateľ vytvoril profil PIM

#### <a name="officeoutlookmacmacolkasserts"></a>Office.Outlook.Mac.MacOLKAsserts

Používa sa na identifikovanie problémov s vplyvom na používateľov v Outlooku, ktoré sa môžu prejaviť ako zlyhania alebo znížená funkčnosť. 

Zhromažďujú sa tieto polia:

- **Category** – typ vyhodnotenia.

- **CollectionTime** – čas zhromaždenia vyhodnotenia.


#### <a name="officeoutlookmacmacolkerrors"></a>Office.Outlook.Mac.MacOLKErrors

Používa sa na identifikovanie problémov s vplyvom na používateľov v Outlooku, ktoré sa môžu prejaviť ako zlyhania alebo znížená funkčnosť. 

Zhromažďujú sa tieto polia:

- **Category** – typ chyby.

- **CollectionTime** – čas zhromaždenia chyby.

- **ThreadId** – identifikátor vlákna.


#### <a name="officesystemsystemhealthasserts"></a>Office.System.SystemHealthAsserts

Chyby, ktoré táto udalosť identifikuje, nám pomáhajú porozumieť tomu, kedy sa zhoršuje zákaznícka skúsenosť. Mnohé z týchto vyhodnotení ShipAssert vedú k zlyhaniam a vďaka týmto informáciám je možné mnohé z nich vyriešiť. Zhromažďuje vyhodnotenia ShipAssert z produktu, čo nám pomáha identifikovať chyby.

Zhromažďujú sa tieto polia:

 - **Count** – počet jednotlivých nahlásených vyhodnotení.

  - **EndTime** – čas, v ktorom sa vyskytlo posledné nahlásené vyhodnotenie

  - **ErrorGroup** – Skupinový identifikátor každého vyhodnotenia

  - **FirstTimeStamp** – čas prvého výskytu vyhodnotenia

  - **Trackback** – jedinečný identifikátor konkrétneho vyhodnotenia

#### <a name="officesystemsystemhealtherrorsetwshim"></a>Office.System.SystemHealthErrorsEtwShim

Táto udalosť sa používa na identifikovanie problémov ovplyvňujúcich zákazníkov v rámci spustenej aplikácie, ktorá sa môžu prejaviť ako zlyhania alebo zhoršená funkčnosť. Zaznamenáva chyby, ktoré sa vyskytujú počas spustenia procesu.

Zhromažďujú sa tieto polia:

  - **EndTime** – čas výskytu poslednej nahlásenej chyby

  - **Trackback** – jedinečný identifikátor konkrétnej chyby

  - **ErrorGroup** – Skupinový identifikátor každej chyby

  - **Count** – počet jednotlivých chýb

  - **FirstTimeStamp** – čas prvého výskytu chyby

#### <a name="officesystemsystemhealtherrorsulsandasserts"></a>Office.System.SystemHealthErrorsUlsAndAsserts

Táto udalosť sa používa na identifikovanie problémov ovplyvňujúcich zákazníkov v rámci spustenej aplikácie, ktorá sa môžu prejaviť ako zlyhania alebo zhoršená funkčnosť. Zaznamenáva chyby, ktoré sa vyskytujú počas spustenia procesu.

Zhromažďujú sa tieto polia:

  - **EndTime** – čas výskytu poslednej nahlásenej chyby

  - **Trackback** – jedinečný identifikátor konkrétnej chyby

  - **ErrorGroup** – Skupinový identifikátor každej chyby

  - **Count** – počet jednotlivých chýb

  - **FirstTimeStamp** – čas prvého výskytu chyby

#### <a name="officesystemsystemhealtherrorsulsworkaround"></a>Office.System.SystemHealthErrorsUlsWorkaround

Táto udalosť sa používa na identifikovanie problémov ovplyvňujúcich zákazníkov v rámci spustenej aplikácie, ktorá sa môžu prejaviť ako zlyhania alebo zhoršená funkčnosť. Zaznamenáva chyby, ktoré sa vyskytujú počas spustenia procesu.

Zhromažďujú sa tieto polia:

  - **EndTime** – čas výskytu poslednej nahlásenej chyby

  - **Trackback** – jedinečný identifikátor konkrétnej chyby

  - **ErrorGroup** – Skupinový identifikátor každej chyby

  - **Count** – počet jednotlivých chýb

#### <a name="officesystemsystemhealtherrorswithouttag"></a>Office.System.SystemHealthErrorsWithoutTag

Táto udalosť sa používa na identifikovanie problémov ovplyvňujúcich zákazníkov v rámci spustenej aplikácie, ktorá sa môžu prejaviť ako zlyhania alebo zhoršená funkčnosť. Zaznamenáva chyby, ktoré sa vyskytujú počas spustenia procesu.

Zhromažďujú sa tieto polia:

Count – počet jednotlivých chýb

  - **EndTime** – čas výskytu poslednej nahlásenej chyby

  - **ErrorCode** – identifikátor chyby

  - **ErrorGroup** – Skupinový identifikátor každej chyby

  - **ErrorId** – identifikátor chyby

  - **FirstTimeStamp** – čas prvého výskytu chyby

  - **Trackback** – jedinečný identifikátor konkrétnej chyby

#### <a name="officesystemsystemhealtherrorswithtag"></a>Office.System.SystemHealthErrorsWithTag

Táto udalosť sa používa na identifikovanie problémov ovplyvňujúcich zákazníkov v rámci spustenej aplikácie, ktorá sa môžu prejaviť ako zlyhania alebo zhoršená funkčnosť. Zaznamenáva chyby, ktoré sa vyskytujú počas spustenia procesu.

Zhromažďujú sa tieto polia:

  - **Count** – počet jednotlivých chýb

  - **EndTime** – čas výskytu poslednej nahlásenej chyby

  - **ErrorCode** – identifikátor chyby

  - **ErrorGroup** – Skupinový identifikátor každej chyby

  - **ErrorId** – identifikátor chyby

  - **FirstTimeStamp** – čas prvého výskytu chyby

  - **Trackback** – jedinečný identifikátor konkrétnej chyby

## <a name="device-connectivity-and-configuration-data-events"></a>Udalosti údajov v kategórii Pripojiteľnosť a konfigurácia zariadenia

Toto sú podtypy údajov v tejto kategórii:

- [Pripojiteľnosť a konfigurácia zariadenia](#device-connectivity-and-configuration-subtype)


### <a name="device-connectivity-and-configuration-subtype"></a>*Podtyp Pripojiteľnosť a konfigurácia zariadenia*

Stav sieťového pripojenia a nastavenia zariadenia, napríklad pamäte.

#### <a name="officeairspaceairspacelocalblocklistdriverupdated"></a>Office.AirSpace.AirSpaceLocalBlocklistDriverUpdated

Používateľ aktualizoval ovládač grafickej karty, ktorý predtým spôsoboval zlyhania balíka Office, a teda sa už nepoužíval na vykresľovanie. Táto udalosť informuje spoločnosť Microsoft o tom, že používatelia, ktorí predtým neboli v optimálnom stave vykresľovania, sa opäť nachádzajú v odporúčanom stave vykresľovania.

Zhromažďujú sa tieto polia:

  - **Data\_BlockedDriverVersion** – verzia ovládača, ktorá bola zaradená na zoznam blokovaných položiek.

  - **Data\_DeviceId** – identifikátor zariadenia grafickej karty, ktoré bolo zaradené na zoznam blokovaných položiek.

  - **Data\_UpdatedDriverVersion** – verzia aktualizovaného ovládača

#### <a name="officeairspaceairspacelocalblocklistinfo"></a>Office.AirSpace.AirSpaceLocalBlocklistInfo

Podrobné informácie o ovládači grafickej karty používateľa, ktorý spôsobil viacnásobné nedávne zlyhania aplikácií balíka Office. Balík Office nebude používať túto grafickú kartu v tejto relácii balíka Office (bude namiesto toho používať softvérové vykresľovanie), kým sa ovládač neaktualizuje. Táto udalosť informuje spoločnosť Microsoft o ovládačoch grafickej karty, ktoré spôsobujú problémy v balíku Office, aby sa mohli identifikovať trendy a aby bolo možné analyzovať vplyv takýchto ovládačov na používateľa. Informuje spoločnosť Microsoft o tom, koľko používateľov sa nachádza v tomto podoptimálnom stave.

Zhromažďujú sa tieto polia:

  - **Data\_AllAppsBlocked** – či sú všetky aplikácie balíka Office na zozname blokovaných položiek

  - **Data\_BlockedDeviceId** – identifikátor zariadenia grafickej karty, ktoré bolo zaradené na zoznam blokovaných položiek

  - **Data\_BlockedDriverVersion** – verzia ovládača, ktorá bola zaradená na zoznam blokovaných položiek

  - **Data\_CrashHistory** – reťazec, ktorý predstavuje históriu ovládača grafickej karty, ktorá spôsobovala zlyhania, na analýzu

  - **Data\_SecsBetweenCrashes** – ako často sa vyskytujú zlyhania ovládača karty

#### <a name="officeairspaceairspacewincompisenabled"></a>Office.AirSpace.AirSpaceWinCompIsEnabled

Táto udalosť zhromažďuje informácie o tom, či sa používa najnovšia platforma vykresľovania na nižšej úrovni založená na Windows Composition.

Keďže najnovšia platforma vykresľovania na nižšej úrovni sa vyvinula a začína sa vydávať zákazníkom, táto udalosť umožňuje spoločnosti Microsoftu zistiť, koľko používateľov má jednotlivé verzie, aby sa zabezpečilo, že platforma bude bez chýb.

Zhromažďujú sa tieto polia:

  - **Data\_WinCompEnabled** –či sa používa riešenie založené na Windows Composition

#### <a name="officeairspacebackendwin32graphicsdriverhangdetectorblocklistapp"></a>Office.AirSpace.Backend.Win32.GraphicsDriverHangDetectorBlocklistApp

Zistilo sa, že grafická karta používateľa spôsobuje dlhé alebo nezvratné nereagovania. Balík Office nebude používať túto grafickú kartu v tejto relácii balíka Office (bude namiesto toho používať softvérové vykresľovanie), kým sa ovládač neaktualizuje. Táto udalosť informuje spoločnosť Microsoft o ovládačoch grafickej karty, ktoré spôsobujú problémy v balíku Office, aby sa mohli identifikovať trendy a aby bolo možné analyzovať vplyv takýchto ovládačov na používateľa. Takisto pomáha pri informovaní o tom, koľko používateľov sa nachádza v tomto podoptimálnom stave.

Zhromažďujú sa tieto polia:

  - **Data\_AppName** – v ktorej aplikácii došlo k nereagovaniam ovládača grafickej karty

#### <a name="officeairspacebackendwin32graphicsdriverhangdetectorregistrywrite"></a>Office.AirSpace.Backend.Win32.GraphicsDriverHangDetectorRegistryWrite

Office zistil, že ovládač grafickej karty používateľa spôsobil nereagovanie, ktoré by sa malo analyzovať pri ďalšom spustení aplikácie balíka Office. Táto udalosť sa používa na určenie, či by bolo pre používateľa vhodnejšie používať iný ovládač alebo adaptér grafickej karty. Pri výskyte vzorov môže spoločnosť Microsoft vykonávať úpravy, aby čo balík Office fungoval čo najplynulejšie.

Zhromažďujú sa tieto polia:

  - **Data\_HangDetected** – či sa zistilo nereagovanie

  - **Data\_InDeviceCall** – v ktorom volaní vykresľovania grafickej karty sa Office nachádzal, keď došlo k nereagovaniu

  - **Data\_Timeout** – ako dlho nereagovanie trvalo, ak sa zariadenie z neho zotavilo

  - **Data\_UnrecoverableCommand** – či sa z nereagovania v tomto príkaze vykresľovania grafickej karty zariadenie zvyčajne zotaví.

#### <a name="officeairspacebackendwin32localblocklistactivity"></a>Office.AirSpace.Backend.Win32.LocalBlocklistActivity

Podrobné informácie o ovládači grafickej karty používateľa, ktorý spôsobil viacnásobné nedávne zlyhania aplikácií balíka Office. Balík Office nebude používať túto grafickú kartu v tejto relácii balíka Office (bude namiesto toho používať softvérové vykresľovanie), kým sa ovládač neaktualizuje. Táto udalosť informuje spoločnosť Microsoft o ovládačoch grafickej karty, ktoré spôsobujú problémy v balíku Office, aby sa mohli identifikovať trendy a aby bolo možné analyzovať vplyv takýchto ovládačov na používateľa. Informuje spoločnosť Microsoft o tom, koľko používateľov sa nachádza v tomto podoptimálnom stave.

Zhromažďujú sa tieto polia:

  - **Data.AllAppsBlocked** – či sú všetky aplikácie balíka Office na zozname blokovaných položiek

  - **Data.BlockedDeviceId** – identifikátor zariadenia grafickej karty, ktoré bolo zaradené na zoznam blokovaných položiek

  - **Data.BlockedDriverVersion** – verzia ovládača, ktorá bola zaradená na zoznam blokovaných položiek

  - **Data.CrashHistory System.String** – reťazec, ktorý predstavuje históriu ovládača grafickej karty, ktorá spôsobovala zlyhania, na analýzu

  - **Data.SecsBetweenCrashes** – ako často sa vyskytujú zlyhania ovládača karty

#### <a name="officeairspacebackendwin32localblocklistdriverupdatedactivity"></a>Office.AirSpace.Backend.Win32.LocalBlocklistDriverUpdatedActivity

Používateľ aktualizoval ovládač grafickej karty, ktorý predtým spôsoboval zlyhania balíka Office, a teda sa už nepoužíval na vykresľovanie. Táto udalosť informuje spoločnosť Microsoft o tom, že používatelia, ktorí predtým neboli v optimálnom stave vykresľovania, sa opäť nachádzajú v odporúčanom stave vykresľovania.

Zhromažďujú sa tieto polia:

  - **Data\_BlockedDeviceId** – identifikátor zariadenia grafickej karty, ktoré bolo zaradené na zoznam blokovaných položiek

  - **Data\_BlockedDriverVersion** – verzia ovládača, ktorá bola zaradená na zoznam blokovaných položiek

  - **Data\_UpdatedDriverVersion** – verzia aktualizovaného ovládača

#### <a name="officegraphicsspritememcorrupt"></a>Office.Graphics.SpriteMemCorrupt

Táto udalosť nahlasuje chyby zistené v telemetrii účtovania pamäte sprajtov. Je to dôležité na posúdenie stavu telemetrie používania grafickej pamäte. Tieto informácie sú potrebné na overenie správnosti našej telemetrie SpriteMem.

Zhromažďujú sa tieto polia:

  - **Data\_CurrentSpriteMem** – celkové množstvo pamäte, ktoré je aktívne vyhradené na to, aby obsahovalo sprajty (obrázky), ktoré tvoria obsah obrazovky.

  - **Data\_Function** – názov funkcie, ktorá sa pokúša uvoľniť pamäť sprajtov.

  - **Data\_SpriteMemToRemove** – množstvo pamäte, ktoré sa má odstrániť z priradenia pre sprajty.

#### <a name="officepowerpointpptsharednointernetconnectivity"></a>Office.PowerPoint.PPT.Shared.NoInternetConnectivity

Táto udalosť sa zhromažďuje vždy, keď PowerPoint zistí, že internetové pripojenie nie je k dispozícii. Spoločnosť Microsoft používa tieto údaje na získanie diagnostických informácií o internetovom pripojení používateľa, aby mohla porozumieť tomu, ako to ovplyvňuje pripojenie k službám Office.

Zhromažďujú sa tieto polia:

- **Data\_IsNexusDetected:bool** – zobrazuje, či je k dispozícii internetové pripojenie pri volaní služby Nexus (hodnota true) alebo pri volaní rozhrania API všeobecnej webovej služby (hodnota false)
