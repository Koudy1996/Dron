# Dron – srovnání pohonných jednotek (v0.1)

**Stav:** pracovní ekonomicko-technická databáze, aktualizace 2026-11-06.  
**Cíl:** vybrat jedinou nejvýhodnější pohonnou jednotku pro univerzální UAV, nikoli vyvíjet čtyři výrobní varianty.

> **Důležité:** Technická data sériových motorů jsou oddělena od **inženýrských odhadů** upravených pohonných jednotek a **nezávazných scénářů OEM cen**. Nejde o schválený letecký návrh ani o cenové nabídky výrobců. Čísla pro upravené TSI nemají zatím oporu v motorové zkoušce.

## Zadané společné podmínky

- Roční výroba v ČR: **300 až 1 000 UAV**; předpokládáme 1 motor na UAV.
- Cíl mise: užitečné zatížení **200–350 kg**, vytrvalost **6–8 hodin**, schopnost provozu do **5 000 m n. m.**.
- Požadovaná výkonová rezerva v 5 000 m: **alespoň 85 % maximálního vzletového výkonu**; jde o projektový požadavek, nikoli doloženou charakteristiku všech motorů.
- Palivo: přednostně **automobilový benzín RON 95/98**.
- **Závazná volba:** třílistá kompozitová **vrtule s pevným stoupáním za letu** (případně nastavitelné stoupání při montáži na zemi). Bez constant-speed regulace.
- Provozní plán: až **1 000 hodin/rok**, celkový životní cyklus letounu **5 000–10 000 hodin**.
- Finanční model: **EUR bez DPH**, výrobní náklady v sérii, **bez R&D a certifikace**.

## 1. Technické parametry – doložený základ

| Parametr | VW 1.0 TSI EA211 evo2 (DUSA) | VW 1.5 TSI EA211 evo2 (DXDB) | Rotax 914 UL2 | Rotax 915 iS |
|---|---:|---:|---:|---:|
| Konstrukce | řadový 3válec, turbo | řadový 4válec, turbo | boxer 4válec, turbo | boxer 4válec, turbo |
| Objem | 999 cm³ | 1 498 cm³ | 1 211,2 cm³ | 1 352 cm³ |
| Vrtání × zdvih | 74,5 × 76,4 mm | 74,5 × 85,9 mm | 79,5 × 61,0 mm | 84,0 × 61,0 mm |
| Max. vzletový/jmenovitý výkon | 85 kW | 110 kW | 84,5 kW (5 minut) | 104 kW (5 minut) |
| Otáčky maximálního výkonu | 5 500–5 600/min | 5 000–6 000/min | 5 800/min | 5 800/min |
| Výrobcem doložený maximální trvalý výkon | **nezjištěno pro leteckou konverzi** | **nezjištěno pro leteckou konverzi** | 73,5 kW při 5 500/min | 99 kW při 5 500/min |
| Max. točivý moment | 200 Nm | 250 Nm | 144 Nm | nezjištěno v použité produktové specifikaci |
| Příprava paliva | přímé vstřikování | přímé vstřikování | 2 karburátory | redundantní elektronické vstřikování |
| Palivo – požadované min. RON | 95 | 95 | 95 | 95 |
| Reduktor vrtule v základní dodávce | **ne** | **ne** | **ano**, i≈2,43 | **ano**, i≈2,54 |
| Dokumentovaná hmotnost dodávky motoru | přesná konfigurace DUSA **neověřena** | přesná konfigurace DXDB **neověřena** | **64,0 kg**, motor + reduktor, bez všech instalačních dílů | **82,2 kg**, vč. reduktoru/turba/intercooleru/výfuku, nikoli všech externích dílů |
| Výrobcem uvedené TBO | pro konverzi **nedoloženo** | pro konverzi **nedoloženo** | **2 000 h** | na aktuální produktové stránce **1 200 h** |
| Výšková schopnost | nutno ověřit po úpravách | nutno ověřit po úpravách | vysokohorská turbovarianta; výkon v 5 km ověřit z křivek | plný vzletový výkon do cca 4 570 m, maximální provozní výška 23 000 ft |

**Poznámka k Rotax 915 iS / TBO:** Aktuální produktová stránka výrobce uvádí **1 200 h**. Jiné sekundární podklady uvádějí 2 000 h (někdy jako cíl nebo pro specifické motory/rozšíření). Pro plán oprav se **nesmí automaticky použít 2 000 h** bez ověření platnosti podle sériového čísla a aktuální dokumentace Rotax.

**Poznámka k hmotnosti VW:** dříve diskutovaných 88 kg pro litrový TSI a 112 kg pro 1.5 TSI **nepovažujeme za porovnatelné, přesně ověřené hmotnosti jednotek DUSA/DXDB**. Nejsou proto uvedeny jako katalogově potvrzené.

## 2. Jednotná letecká instalace – zatím jen odhad

Instalace zahrnuje motor s nezbytným příslušenstvím, turbo, reduktor a tlumení torzních kmitů, chlazení s kapalinami, výfuk, lože, elektrické příslušenství a třílistou pevnou vrtuli. **Nezahrnuje nádrže, palivo, avioniku celého UAV ani konstrukci draku.**

| Parametr | 1.0 TSI | 1.5 TSI | Rotax 914 UL2 | Rotax 915 iS |
|---|---:|---:|---:|---:|
| Předpokládaná instalovaná hmotnost – interval | **125–160 kg** | **150–190 kg** | **90–105 kg** | **100–120 kg** |
| Výchozí pracovní hmotnost pro model | **134 kg** | **165 kg** | **94 kg** | **110 kg** |
| Požadovaných 85 % výkonu v 5 000 m | **72,25 kW** | **93,5 kW** | **71,8 kW** | **88,4 kW** |
| Je výkon v 5 000 m doložen? | **Ne** | **Ne** | **Ne ve zvolené konfiguraci a režimu** | **Ne pro přesně 5 000 m; hranice plného TO výkonu je níže** |
| Modelový průběžný cestovní výkon motoru (nikoli závazek návrhu) | 30–45 kW | 35–60 kW | podle draku / mise | podle draku / mise |
| Měrná spotřeba pro předběžné výpočty BSFC | **270–330 g/kWh** (předpoklad) | **270–330 g/kWh** (předpoklad) | přibl. **276 g/kWh** při max. trvalém výkonu; není to celá mapa | **280–310 g/kWh** (orientační pásmo, nikoli úplná mapa) |

### Předběžné provozní srovnání při STEJNÉM výkonu 40 kW

Při modelové hustotě benzínu 0,745 kg/l a BSFC 300 g/kWh je spotřeba **16,1 l/h**, a to **u libovolného motoru** se stejnou měrnou spotřebou. Objem motoru sám o sobě neurčuje spotřebu při stejném výkonu. U TSI to při pásmu 270–330 g/kWh odpovídá **14,5–17,7 l/h**. U Rotax 914 iS nelze bez konzistentní motorové mapy prohlásit konkrétní výhodu v cruise.

**Výškový a tepelný limit:** Zatím není prokázán dlouhodobý výkon ani spotřeba TSI v 5 000 m. Nelze zaměňovat špičkový výkon motoru s trvale udržitelným výkonem a výkonem po ztrátách reduktoru a vrtule. Pro plánované TSI úpravy počítat s novou kalibrací řídicí jednotky, mapou přeplňování, odvodem tepla, mazáním a zkouškami torzního systému.

## 3. OEM ceny – SCÉNÁŘE, nikoli nabídky (EUR/kus bez DPH)

**Význam sloupců:**
- **OEM motor** = nová dodávka motoru podle odpovídající dodavatelské specifikace. U TSI včetně potřebného automobilového příslušenství, ale **bez letecké konverze**; u Rotaxu se základním reduktorem.
- **Kompletní pohonná instalace** = komparativní náklad hotové jednotky podle oddílu 2, včetně přibližně 1 500 € za pevnou vrtuli a potřebné montáže a výrobní režie.
- Rozpětí záměrně obsahují nejistotu **dodavatelské slevy, výbavy, objemu objednávky a kusové zástavby**; náklady na vývoj, certifikaci a konstrukci draku se nezapočítávají.

| Motor | 300 ks/rok: OEM motor | 1 000 ks/rok: OEM motor | 300 ks/rok: komplet instalace | 1 000 ks/rok: komplet instalace |
|---|---:|---:|---:|---:|
| **VW 1.0 TSI** | **2 800–4 000 €** | **2 500–3 500 €** | **12 000–16 000 €** | **10 500–14 000 €** |
| **VW 1.5 TSI** | **3 500–5 000 €** | **3 000–4 300 €** | **14 000–18 000 €** | **12 500–16 000 €** |
| **Rotax 914 UL2** | **22 000–26 000 €** | **20 000–25 000 €** | **25 000–30 000 €** | **23 000–29 000 €** |
| **Rotax 915 iS** | **31 000–39 000 €** | **28 000–36 000 €** | **35 000–44 000 €** | **32 000–41 000 €** |

**Úroveň jistoty:** VW OEM **nízká** (neexistuje veřejný kontrakt ani závazná cena úprav); Rotax OEM **nízká** (veřejné dealerské ceny nejsou přímé OEM nabídky); ceny kompletních konverzí **nízká** (vyžadují kusovník, ověření turba/reduktoru a RFQ). Intervaly **neslouží jako cenové nabídky**.

### Veřejné cenové kotvy, ne OEM smlouvy

| Položka | Publikovaný údaj | Co říká a neříká |
|---|---:|---|
| Rotax 914 UL2, SE-Aviation | **27 050 €** | Veřejná nabídka nového motoru, nikoli velkoobjemový kontrakt; ověřit konfiguraci a dostupnost |
| Rotax 914 UL, Rotech, ceník 10. 9. 2026 | **37 571 USD** | Severoamerický veřejný ceník, FCA Vernon |
| Rotax 915 iS3A, Rotech, ceník 10. 9. 2026 | **48 475 USD** | Veřejný ceník podle konfigurace, nikoli OEM cena |
| Rotax 915 iS, Edge Performance | **37 355 €** | Veřejně zobrazovaná cena, ověřit finální podmínky |
| Rotax 915 iS, AEROHANGAR | **31 900 €** | Individuální inzerát motoru s nulovým náletem, **nikoli** důkaz standardní ceny nového továrního OEM motoru |
| E-Props Excalibur-3 CCW | **1 758 € bez DPH** | Třílistá, na zemi stavitelná vrtule pro některé tlačné konfigurace Rotax; série v modelu 1 500 € je předpoklad |
| Nový holý VW 1.5 TSI DXDB | na trhu existují jednotlivé nabídky v řádu **desítek tisíc Kč** | Holý motor nelze přímo srovnávat s provozuschopným OEM leteckým agregátem |

Pro přímou OEM nabídku je nezbytné poptat **300/500/1 000 ks ročně**, shodnou specifikaci obsahu dodávky, minimální odběr, dodací lhůty, cenu náhradních agregátů, způsob řešení záruky a servisních rezerv.

## 4. Rozhodovací pravidlo

Primární optimalizační funkce: **náklady za schopnost přepravovat požadovaný náklad po požadovanou dobu**, se zvláštním důrazem na hmotnost instalace a dlouhodobou provozní cenu. Nevybírat motor jen podle maximálního kW/€.

1. **VW 1.0 TSI:** levná jednotka; otázka je hmotnost a udržení 72,25 kW ve výšce 5 000 m.
2. **VW 1.5 TSI:** dražší/těžší, ale výkonová rezerva; musí kompenzovat přídavnou hmotnost měřitelným přínosem.
3. **Rotax 914 UL2:** nízká hmotnost, integrovaný reduktor a existující letecká dokumentace; vyšší cena a karburátorový systém.
4. **Rotax 915 iS:** vyšší výkon při nízké hmotnosti, redundantní vstřikování, ale vysoká pořizovací cena; ověřit relevantní TBO a cenu generálních oprav.

**Neuzavřené položky:** přesná vážená hmotnost DUSA/DXDB ve sjednocené konfiguraci; motorové mapy BSFC; výkon a teploty po 5 000 m; kompresorové mapy; cena a životnost reduktoru TSI; Rotax 915 iS TBO dle sériového čísla; **písemné OEM cenové nabídky**. Do získání těchto dat neoznačovat žádného kandidáta za prokazatelně nejlevnější při celkových provozních nákladech.

## 5. Zdroje (stav přístupu 2026-11-06)

### Primární technické podklady
- [Škoda Auto – technická data 1.0 TSI 85 kW a 1.5 TSI 110 kW](https://www.skoda-auto.com/_doc/0863bb55-f52f-477f-bdeb-a59b665436f9)
- [Škoda 2026 – specifikace DXDB 1.5 TSI (PDF)](https://www.skoda-media.de/model_motor/genpdf/27319/full)
- [Rotax – 914 UL/F, produktová stránka](https://www.flyrotax.com/cs/products/914-ul-f)
- [Rotax – 914 UL/F, technický list](https://www.flyrotax.com/assets/files/914-UL_Datasheet_2020.pdf)
- [Rotax – 915 iS, aktuální technické parametry a TBO](https://www.flyrotax.com/products/915-is-a-isc-a)
- [E-Props – Excalibur-3, tlačná konfigurace, cena a hmotnost](https://aircraft.e-props.fr/product_info.php?cPath=9000_9003&language=en&products_id=70005)

### Cenové kotvy
- [SE-Aviation – nový Rotax 914 UL2](https://eboutique.se-aviation.fr/produit/rotax-915-ul3/)
- [Rotech – ceník Rotax 2026](https://prices.rotech.ca/node/39)
- [Edge Performance – Rotax 915 iS](https://shop.edgeperformance.no/produkt/aviation-engines/rotax-4-takt-motorer/915is-engine)
- [AEROHANGAR – Rotax 915 iS s nulovým náletem](https://www.aerohangar.cz/en/engines-and-propellers/engines/rotax-915-is/)
- [E-Props – ceník vrtulí duben 2026](https://aircraft.e-props.fr/ordering.php)

**Doprovodná strojově čitelná tabulka:** [data/engines.csv](data/engines.csv).