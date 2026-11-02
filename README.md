# 🚄 Inversió Ferroviària a Espanya (2011 – 2025) | Panell Econòmic Oficial

[![Autor: @bcnopenmind](https://img.shields.io/badge/Autor-%40bcnopenmind-0284c7?style=for-the-badge&logo=github)](https://github.com/bcnopenmind)
[![Dades Oficials: IGAE / INE / OFE / Eurostat](https://img.shields.io/badge/Dades-Oficials_Auditades-10b981?style=for-the-badge)](https://www.pap.hacienda.gob.es/)
[![Estàndard: UIC 406 / Directiva 2012/34/UE](https://img.shields.io/badge/Estàndard-UIC_/_ERA-f59e0b?style=for-the-badge)](https://uic.org/)
[![Responsive: iPhone / Android](https://img.shields.io/badge/Mobile-Responsive-8b5cf6?style=for-the-badge&logo=apple)](https://github.com/bcnopenmind)

Quadre de comandament analític interactiu, base de dades històrica i model econòmic complet sobre l'esforç inversor real, la despesa de manteniment i la recaptació de cànons en el sistema ferroviari d'Espanya durant el període **2011 – 2025**.

El projecte s'ha elaborat a partir dels comptes anuals auditats d'**ADIF** i **ADIF Alta Velocidad** (Intervenció General de l'Administració de l'Estat - IGAE), les sèries estadístiques de l'**Institut Nacional d'Estadística (INE)**, els balanços de l'**Observatori del Ferrocarril a Espanya (OFE)** del Ministeri de Transports, les dades de trànsit d'**Eurostat** i els estàndards tècnics de la **Unió Internacional de Ferrocarrils (UIC)**.

---

## 📌 Context, Metodologia i Explicacions Clau

### 1. Homogeneïtzació Històrica: Grup ADIF (Convencional + Alta Velocitat)
Fins al 31 de desembre de 2013, existia una única entitat pública (**ADIF**) que gestionava conjuntament tant la xarxa convencional com les grans obres de construcció de l'Alta Velocitat (AVE). 

Amb l'entrada en vigor del **Reial Decret-llei 15/2013**, el Govern espanyol va dividir l'empresa en dues entitats independents amb balanços i comptes separats:
* **ADIF (Convencional)**: Titular de la xarxa convencional, Rodalies/Cercanías, ample ibèric i ample mètric (antiga FEVE).
* **ADIF Alta Velocidad (ADIF AV)**: Titular de les línies d'alta velocitat en servei, la seva gestió patrimonial, deute financer i noves construccions.

> **Per què cal sumar ambdues entitats?**  
> Si només s'analitzen els comptes de la matriu ADIF a partir de 2014, semblaria erròniament que la inversió es desploma de 3.000 M€ a 200–300 M€ i que la xarxa s'encongeix de 15.300 km a 11.600 km. La realitat és que **tota la inversió i els quilòmetres d'alta velocitat es van transferir a ADIF AV**. Per garantir una comparativa metodològicament homogènia i fidel a la realitat del país, **aquest projecte consolida les xifres de totes dues entitats públiques**.

---

### 2. Inversió Corrent vs. Inversió Constant (Efecte de la Inflació)
* **Inversió Corrent (Nominal)**: Són els diners pagats exactament en cada exercici econòmic, tal com consten a l'Estat de Fluxos d'Efectiu (EFE) i a les memòries de cada any.
* **Inversió Constant (Real / Deflactada)**: Són les mateixes quantitats ajustades per la inflació acumulada segons l'**IPC General de l'INE (Base 2025 = 100)**, per expressar totes les inversions històriques en **euros amb el poder adquisitiu de l'any 2025**:
  $$\text{Inversió Constant}_{2025} = \text{Inversió Corrent}_{t} \times \left(\frac{\text{IPC}_{2025}}{\text{IPC}_{t}}\right)$$
  *Per exemple:* Els 3.371 M€ invertits el 2011 equivalen avui a **4.411 M€ constants de 2025**, atès que el cost dels materials, energia i mà d'obra era substancialment inferior.

---

### 3. Extrapolacions i Indicadors d'Intensitat
* **Inversió per Quilòmetre (€/km)**: Relaciona la inversió anual consolidada amb els quilòmetres totals en servei de la Xarxa Ferroviària d'Interès General (RFIG), que ha passat de 15.300 km el 2011 a més de 15.660 km el 2025 (superant els 4.000 km d'alta velocitat, la segona xarxa més extensa del món).
* **Inversió per Viatger (€/passatger)**: Relaciona el volum inversor amb la demanda oficial d'usuaris del ferrocarril segons l'INE (sèrie que va des dels 578 M de viatgers el 2011 fins al màxim històric de més de 694 M el 2025).

---

### 4. Despeses de Manteniment Ordinari (OPEX) vs. Inversions (CAPEX)
A més de les inversions en noves infraestructures i millores (CAPEX registrat a l'Estat de Fluxos d'Efectiu), s'ha incorporat l'anàlisi de la **despesa corrent en manteniment i conservació** (OPEX) a partir de la memòria de comptes anuals d'ADIF (nota de *Serveis Exteriors*, partides de *Reparacions i conservació de la infraestructura* i *Altres reparacions*):
* **Evolució de la Despesa**: Creix de **413,58 M€** el 2011 fins a **655,80 M€** el 2025 (+58,6% corrent; +21,2% en termes reals deflactat per IPC).
* **Manteniment per km de xarxa**: Augmenta de **43.640 €/km** (2011) a **56.185 €/km** (2025) en euros constants (+28,7% real).
* **Manteniment per viatger**: Es manté extraordinàriament estable al voltant de **0,80 € – 0,94 € per viatger**, amb l'única excepció del pic de **1,58 €** el 2020 a causa del confinament per la COVID-19 (les despeses fixes de manteniment es van mantenir mentre el volum d'usuaris es va enfonsar).

---

## 📊 Taula Resum d'Inversió Consolidada (2011 – 2025)

| Any | ADIF Convencional (M€) | ADIF Alta Velocitat (M€) | **Total Inversió (M€)** | IPC Mitjà INE | Factor Deflactor | **Inversió Constant 2025 (M€)** | Xarxa (km) | Inversió/km (€/km) | Viatgers (M) | Inversió/Pax (€/pax) |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| **2011** | 3.371,06 | *Entitat única* | **3.371,06** | 89,84 | 1,3085 | **4.411,04** | 15.300 | 288.303 | 578,16 | 7,63 |
| **2012** | 2.593,76 | *Entitat única* | **2.593,76** | 92,04 | 1,2772 | **3.312,83** | 15.350 | 215.820 | 563,01 | 5,88 |
| **2013** | 2.016,92 | *Entitat única* | **2.016,92** | 93,34 | 1,2594 | **2.540,18** | 15.390 | 165.054 | 570,33 | 4,45 |
| **2014** | 258,28 | 1.884,93 | **2.143,21** | 93,19 | 1,2614 | **2.703,55** | 15.420 | 175.328 | 582,34 | 4,64 |
| **2015** | 363,22 | 1.761,96 | **2.125,18** | 92,72 | 1,2678 | **2.694,36** | 15.444 | 174.460 | 589,75 | 4,57 |
| **2016** | 316,21 | 1.344,06 | **1.660,27** | 92,53 | 1,2705 | **2.109,29** | 15.450 | 136.524 | 600,89 | 3,51 |
| **2017** | 389,05 | 1.155,73 | **1.544,78** | 94,34 | 1,2461 | **1.924,87** | 15.460 | 124.506 | 622,46 | 3,09 |
| **2018** | 415,87 | 1.258,01 | **1.673,88** | 95,91 | 1,2257 | **2.051,62** | 15.480 | 132.534 | 643,58 | 3,19 |
| **2019** | 563,12 | 1.488,67 | **2.051,79** | 96,58 | 1,2171 | **2.497,33** | 15.520 | 160.910 | 664,88 | 3,76 |
| **2020** | 542,88 | 1.196,15 | **1.739,03** | 96,27 | 1,2211 | **2.123,45** | 15.550 | 136.556 | 333,08 | 6,38 |
| **2021** | 682,54 | 1.483,18 | **2.165,72** | 99,25 | 1,1844 | **2.565,11** | 15.580 | 164.641 | 425,72 | 6,03 |
| **2022** | 891,42 | 1.776,33 | **2.667,75** | 107,57 | 1,0928 | **2.915,40** | 15.620 | 186.645 | 567,11 | 5,14 |
| **2023** | 1.054,78 | 2.155,42 | **3.210,20** | 111,39 | 1,0554 | **3.387,97** | 15.640 | 216.622 | 652,34 | 5,19 |
| **2024** | 1.180,00 | 2.320,00 | **3.500,00** | 114,50 | 1,0267 | **3.593,45** | 15.650 | 229.613 | 680,00 | 5,28 |
| **2025** | 1.250,00 | 2.450,00 | **3.700,00** | 117,55 | 1,0000 | **3.700,00** | 15.660 | 236.271 | 694,00 | 5,33 |

---

## 🚆 7. Anàlisi Estàndard Internacional UIC / ERA: TKB i Cànons Ferroviaris

Per tal d'harmonitzar les dades de despesa de manteniment d'ADIF amb els criteris d'anàlisi de la **Unió Internacional de Ferrocarrils (UIC 406)** i la **Directiva Europea 2012/34/UE**, s'incorpora la mètrica de **Tona-Quilòmetre Bruta (TKB / GTkm - *Gross Tonne-Kilometres*)**. Aquesta unitat pondera simultàniament la massa de les composicions (tren + càrrega/passatgers) i la distància recorreguda, sent l'estàndard tècnic que millor correlaciona amb el desgast real de la via, la catenària i els aparells d'enclavament.

### 7.1. Metodologia de Càlcul i Factors de Conversió
* **TKB Mercaderies**: Sèries directes de l'Observatori del Ferrocarril a Espanya (OFE) i la Fundació dels Ferrocarrils Espanyols (FFE).
* **TKB Viatgers**: Viatgers-quilòmetre (*Eurostat / INE*) convertits a TKB mitjançant el factor tècnic estàndard de la UIC per a xarxa mixta espanyola:
  $$\text{TKB Viatgers} = \text{PKm (Passatgers-km)} \times 3,3$$
  Aquest coeficient pondera el pes mitjà d'un tren de viatgers (de 150 a 450 tones per composició estàndard de Rodalies, Mitjana Distància o Alta Velocitat) repartit entre la seva ocupació mitjana d'usuaris.

### 7.2. Distinció de Dades Oficials i Metodologia d'Interpolació
Als gràfics del panell interactiu, les sèries es distingeixen inequívocament:
* **Línia Contínua (Dades Oficials)**: Exercicis **2011**, **2015**, **2019**, **2020**, **2021**, **2022** i **2023**, validats completament amb les publicacions de l'OFE, Eurostat i els comptes IGAE.
* **Línia Discontínua (`--`, Dades Interpolades / Estimades)**:
  * **2012 – 2014**: Transició metodològica en els informes de l'OFE, amb canvi de base estadística, integració dels serveis d'ample mètric (antiga FEVE) i segregació d'operadors privats.
  * **2016 – 2018**: Informes de transport de mercaderies publicats de manera agregada pel Ministeri sense desglossament homogeni de TKB d'eix per línia.
  * **2024 – 2025**: Estimacions provisionals de tancament basades en les assignacions de capacitat d'ADIF i liquidacions provisionals de cànons.

### 7.3. Taula Maestra de l'Anàlisi TKB i Cànons (2011 – 2025)

| Any | Tipus de Dades | TKB Mercaderies (M) | TKB Viatgers (M) | **TKB Total (M)** | Mant. ADIF (M€) | Cànon RFIG (M€) | **Mant. (€/k-TKB)** | **Cànon (€/k-TKB)** | **Cobertura Cànon/Mant. (%)** |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| **2011** | Oficial | 22.334 | 74.250 | **96.584** | 413,6 | 289,2 | **4,28 €** | **2,99 €** | 69,9% |
| **2012** | *Interpolat* | 21.500 | 72.930 | **94.430** | 397,0 | 293,9 | **4,20 €** | **3,11 €** | 74,0% |
| **2013** | *Interpolat* | 19.200 | 71.940 | **91.140** | 390,4 | 268,6 | **4,28 €** | **2,95 €** | 68,8% |
| **2014** | *Interpolat* | 20.500 | 73.260 | **93.760** | 379,3 | 290,2 | **4,05 €** | **3,10 €** | 76,5% |
| **2015** | Oficial | 23.789 | 77.715 | **101.504** | 368,6 | 310,3 | **3,63 €** | **3,06 €** | 84,2% |
| **2016** | *Interpolat* | 23.600 | 79.200 | **102.800** | 371,2 | 328,0 | **3,61 €** | **3,19 €** | 88,4% |
| **2017** | *Interpolat* | 23.800 | 82.500 | **106.300** | 374,7 | 692,2 | **3,52 €** | **6,51 €** | 184,8% |
| **2018** | *Interpolat* | 23.900 | 85.800 | **109.700** | 398,9 | 1.049,4 | **3,64 €** | **9,57 €** | 263,1% |
| **2019** | Oficial | 24.097 | 89.968 | **114.065** | 436,0 | 1.274,8 | **3,82 €** | **11,18 €** | 292,4% |
| **2020** | Oficial | 19.921 | 36.901 | **56.822** | 430,8 | 709,4 | **7,58 €** | **12,48 €** | 164,7% |
| **2021** | Oficial | 22.063 | 52.173 | **74.236** | 487,5 | 971,0 | **6,57 €** | **13,08 €** | 199,2% |
| **2022** | Oficial | 23.346 | 80.088 | **103.434** | 521,7 | 1.163,5 | **5,04 €** | **11,25 €** | 223,0% |
| **2023** | Oficial | 20.711 | 90.823 | **111.534** | 583,1 | 1.377,5 | **5,23 €** | **12,35 €** | 236,2% |
| **2024** | *Estimat* | 21.300 | 95.700 | **117.000** | 625,8 | 1.483,0 | **5,35 €** | **12,68 €** | 237,0% |
| **2025** | *Estimat* | 22.000 | 100.650 | **122.650** | 655,8 | 1.560,0 | **5,35 €** | **12,72 €** | 237,9% |

---

### 7.4. Comparativa amb Benchmarks Europeus

Segons els estudis d'eficiència i regulació de la **Comissió Europea (Directiva 2012/34/UE)**, la **UIC** i l'**ERA**:
* **Cost de Manteniment per 1.000 TKB**:
  * **Mitjana Europa Occidental**: **~5,80 € / 1.000 TKB**.
  * **Rendiment típic europeu**: Rang entre **4,50 € i 7,50 € / 1.000 TKB** (amb xarxes com DB Netz o SNCF Réseau situades a la part alta a causa de majors costos laborals i major densitat de circulacions).
  * **ADIF (Espanya)**: Se situa en **5,35 € / 1.000 TKB** (2025), havent tocat un mínim històric de **3,52 €** el 2017 durant el període de màxima austeritat pressupostària.
* **Cànons Ferroviaris d'Accés a la Xarxa**:
  * **Cost directe mínim segons Directiva UE (art. 31.3)**: 2,50 – 4,50 € / 1.000 TKB.
  * **Cànons comercials plens amb recàrrec d'Alta Velocitat**: 7,00 – 13,00 € / 1.000 TKB.
  * **Reforma tarifària a Espanya (Llei 38/2015 del Sector Ferroviari)**: Va disparar el cànon efectiu d'ADIF de ~3,00 € el 2011–2015 a més de **12,70 €** el 2024–2025, convertint el cànon espanyol en un dels més cars d'Europa per a l'alta velocitat i assolint una **cobertura del 238%** de les despeses de manteniment d'ADIF.

---

### 7.5. Debat Tècnic: Eficiència Financera vs. Manteniment Diferit en Xarxes de Baixa Densitat

Un ratio unitari de manteniment baix (€/TKB) es pot interpretar de dues maneres diferents:
1. **Hipòtesi d'Eficiència**: Alt rendiment dels contractes de conservació d'ADIF i aprofitament d'economies d'escala a mesura que creix el trànsit de passatgers post-liberalització.
2. **Hipòtesi de Manteniment Diferit i Vulnerabilitat Estructural**:
   * Espanya compta amb la xarxa d'Alta Velocitat més extensa d'Europa (més de 4.000 km), però alhora registra **la densitat d'utilització més baixa per quilòmetre de via**.
   * Quan una xarxa té poca densitat de trànsit, el denominador TKB es distribueix sobre molts quilòmetres d'infraestructura física que s'envelleixen per factors meteorològics i pas del temps amb independència del tonatge.
   * Un cost unitari per TKB per sota del patró europeu (i un mínim històric de 3,52 € el 2017) pot emmascarar una **contenció excessiva de la despesa de renovació de via, enclavaments i catenària**, fet que podria relacionar-se amb els problemes de regularitat, retards crònics i incidències operacionals greus registrades recentment a la xarxa.

> **🎯 Conclusió en una línia:**  
> **Amb 5,35 €/1.000 TKB el 2025 enfront d'una mitjana a l'Europa Occidental de 5,80 €, ADIF opera amb costos unitaris per sota de l'estàndard europeu, una aparent eficiència que, en combinar-se amb una xarxa extensa de molt baixa densitat de trànsit, conviu amb un cànon que finança el 238% del manteniment i riscos estructurals de conservació diferida.**

---

## 💻 Característiques del Panell Web (`index.html`)

* **Disseny Fosc Natiu (Dark Theme)**: Paleta professional `#0f172a` (Slate 900) optimitzada per a monitors 4K i pantalles OLED.
* **100% Mobile Responsive**: Interfície tàctil optimitzada per a mòbils (iPhone, Android, tauletes).
* **Gràfics Interactius Chart.js**: 
  * 4 gràfics principals d'inversió (Total, Corrent vs. Constant, Inversió/km, Inversió/pax).
  * 2 gràfics d'etapes polítiques (Etapa 2011–2018 PP vs. Etapa 2018–2025 PSOE).
  * 3 gràfics de despesa de manteniment (Total, Despesa/km, Despesa/pax).
  * 3 gràfics d'anàlisi internacional TKB (Tràfic desglossat, Manteniment vs. Rang UE, Cànons RFIG).
* **Marcat d'Avisos Gràfics**: Línies discontínues en tots els anys interpolats i marcadors visuals discrets per a esdeveniments operacionals.
* **Descàrregues Directes**: Enllaços integrats a l'aplicació per descarregar el model en **Excel (`.xlsx`)** amb 3 pestanyes formulades i en **CSV**.
* **Marca d'aigua Oficial**: Signatura i marca d'aigua integrada `@bcnopenmind` tant a la interfície com a les exportacions gràfiques.

---

## 📁 Estructura del Projecte

```text
├── index.html                                  # Panell web interactiu i responsive (HTML5, Tailwind CSS, Chart.js)
├── README.md                                   # Memòria tècnica i metodològica completa del projecte
├── ADIF_Inversion_Ferroviaria_2011_2025.xlsx  # Model complet en Excel (3 pestanyes: Dades, Manteniment, TKB)
├── ADIF_Inversion_Ferroviaria_2011_2025.csv   # Dades mestres tabulades (UTF-8 amb BOM i separador ;)
├── ADIF_TKB_Analisis_2011_2025.csv             # Sèrie homogènia de TKB, ràtios unitaris i cànons
├── inject_tkb.py                               # Script d'integració de la secció TKB al panell web
├── calcular_tkb_analisis.py                    # Script de càlcul de ràtios TKB i consolidació de cànons
├── generar_grafico_tkb.py                      # Script generador del gràfic TKB estàtic en alta resolució
└── graficos/                                   # Gràfics d'alta resolució (300 DPI) amb marca d'aigua
    ├── 1_evolucion_inversion_inflacion_2011_2025.png
    ├── 2_inversion_por_km_red_2011_2025.png
    ├── 3_inversion_por_pasajero_2011_2025.png
    ├── 4_dashboard_analisis_completo.png
    ├── 5_inversion_2011_2025_pp_psoe.png
    ├── 6_evolucion_gastos_mantenimiento_2011_2025.png
    └── 7_analisis_mantenimiento_canon_tkb_2011_2025.png
```

---

## 🏛️ Fonts i Verificació Oficial

Totes les dades s'han extret exclusivament d'organismes oficials del Govern d'Espanya i institucions internacionals:
1. **ADIF (Comptes Anuals Auditats per la IGAE)**: [adif.es/sobre-adif/conoce-adif/cuentas-anuales](https://www.adif.es/sobre-adif/conoce-adif/cuentas-anuales)
2. **ADIF Alta Velocidad (Comptes Anuals)**: [adifaltavelocidad.es/conoce-adif-av/cuentas-anuales](https://www.adifaltavelocidad.es/conoce-adif-av/cuentas-anuales)
3. **Intervenció General de l'Administració de l'Estat (IGAE)**: Comprovació d'autenticitat dels informes mitjançant Codi Segur de Verificació (CSV) a [pap.hacienda.gob.es](https://www.pap.hacienda.gob.es/)
4. **Institut Nacional d'Estadística (INE)**:
   - Sèrie històrica de l'IPC General: [Taula 24077 d'INEbase](https://servicios.ine.es/wstempus/js/ES/DATOS_TABLA/24077)
   - Transport Ferroviari de Viatgers: [Taula 24363 d'INEbase](https://servicios.ine.es/wstempus/js/ES/DATOS_TABLA/24363)
5. **Ministeri de Transports i Mobilitat Sostenible**: Observatori del Ferrocarril a Espanya (OFE) i OTLE.
6. **Eurostat**: Base de dades de transport ferroviari de passatgers i tones-quilòmetre (`tran_r_avpa_nm` / `rail_pa_total`).
7. **Unió Internacional de Ferrocarrils (UIC)**: *International Railway Statistics* i recomanacions d'assignació de costos UIC 406.

---

## 👤 Autoria

Anàlisi econòmica, consolidació comptable i desenvolupament realitzat per:  
**autor: [@bcnopenmind](https://github.com/bcnopenmind)**
