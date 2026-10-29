# 🚄 Inversió Ferroviària a Espanya (2011 – 2025) | Panell Econòmic Oficial

[![Autor: @bcnopenmind](https://img.shields.io/badge/Autor-%40bcnopenmind-0284c7?style=for-the-badge&logo=github)](https://github.com/bcnopenmind)
[![Dades Oficials: IGAE / INE](https://img.shields.io/badge/Dades-Oficials_Auditades-10b981?style=for-the-badge)](https://www.pap.hacienda.gob.es/)
[![Responsive: iPhone / Android](https://img.shields.io/badge/Mobile-Responsive-8b5cf6?style=for-the-badge&logo=apple)](https://github.com/bcnopenmind)

Quadre de comandament analític interactiu i base de dades històrica sobre l'esforç inversor real en el sistema ferroviari d'Espanya durant el període **2011 – 2025**. El projecte s'ha elaborat a partir dels comptes anuals auditats d'**ADIF**, **ADIF Alta Velocidad** i les sèries estadístiques oficials de l'**Institut Nacional d'Estadística (INE)** i del **Ministeri de Transports i Mobilitat Sostenible**.

---

## 📌 Context, Metodologia i Explicacions Clau

### 1. Homogeneïtzació Històrica: Grup ADIF (Convencional + Alta Velocitat)
Fins al 31 de desembre de 2013, existia una única entitat pública (**ADIF**) que gestionava conjuntament tant la xarxa convencional com les grans obres de construcció de l'Alta Velocitat (AVE). 

Amb l'entrada en vigor del **Reial Decret-llei 15/2013**, el Govern espanyol va dividir l'empresa en dues entitats independents amb balanços i comptes separats:
* **ADIF (Convencional)**: Titular de la xarxa convencional, Rodalies/Cercanías, ample ibèric i ample mètric (antiga FEVE).
* **ADIF Alta Velocidad (ADIF AV)**: Titular de les línies d'alta velocitat en servei, la seva gestió, deute i noves construccions.

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

## 📊 Taula Resum Consolidada (Espanya: 2011 – 2025)

| Any | ADIF Convencional (M€) | ADIF Alta Velocitat (M€) | **TOTAL CORRENT (M€)** | **TOTAL CONSTANT 2025 (M€)** | IPC Mitjà INE | Factor IPC | Xarxa Total RFIG (km) | Inversió / km (€ Const.) | Viatgers (M) | Inversió / Viatger (€ Const.) |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **2011** | 3.371,26 | *Integrada* | **3.371,26 M€** | **4.410,99 M€** | 76,43 | $\times 1,3084$ | 15.300 km | 288.300 €/km | 578,67 M | 7,62 € |
| **2012** | 2.972,77 | *Integrada* | **2.972,77 M€** | **3.796,73 M€** | 78,30 | $\times 1,2772$ | 15.350 km | 247.344 €/km | 568,15 M | 6,68 € |
| **2013** | 308,46 | 2.540,00 | **2.848,46 M€** | **3.587,43 M€** | 79,40 | $\times 1,2594$ | 15.390 km | 233.101 €/km | 562,88 M | 6,37 € |
| **2014** | 312,64 | 2.192,00 | **2.504,64 M€** | **3.159,18 M€** | 79,28 | $\times 1,2613$ | 15.419 km | 204.889 €/km | 562,78 M | 5,61 € |
| **2015** | 193,23 | 1.781,00 | **1.974,23 M€** | **2.502,68 M€** | 78,88 | $\times 1,2677$ | 15.438 km | 162.112 €/km | 566,81 M | 4,42 € |
| **2016** | 239,61 | 1.105,00 | **1.344,61 M€** | **1.707,99 M€** | 78,72 | $\times 1,2702$ | 15.457 km | 110.499 €/km | 568,76 M | 3,00 € |
| **2017** | 291,07 | 1.346,00 | **1.637,07 M€** | **2.039,60 M€** | 80,26 | $\times 1,2459$ | 15.479 km | 131.765 €/km | 592,72 M | 3,44 € |
| **2018** | 253,36 | 1.307,00 | **1.560,36 M€** | **1.911,99 M€** | 81,61 | $\times 1,2254$ | 15.489 km | 123.442 €/km | 601,72 M | 3,18 € |
| **2019** | 414,04 | 1.200,00 | **1.614,04 M€** | **1.964,03 M€** | 82,18 | $\times 1,2168$ | 15.539 km | 126.394 €/km | 633,89 M | 3,10 € |
| **2020** | 473,29 | 1.273,00 | **1.746,29 M€** | **2.131,84 M€** | 81,91 | $\times 1,2208$ | 15.524 km | 137.325 €/km | 333,12 M | 6,40 € |
| **2021** | 470,08 | 1.090,00 | **1.560,08 M€** | **1.847,38 M€** | 84,45 | $\times 1,1842$ | 15.519 km | 119.040 €/km | 418,11 M | 4,42 € |
| **2022** | 660,31 | 1.553,00 | **2.213,31 M€** | **2.418,02 M€** | 91,53 | $\times 1,0925$ | 15.821 km | 152.838 €/km | 553,35 M | 4,37 € |
| **2023** | 1.118,15 | 1.974,00 | **3.092,15 M€** | **3.262,88 M€** | 94,77 | $\times 1,0552$ | 15.649 km | 208.511 €/km | 665,20 M | 4,91 € |
| **2024** | 1.484,04 | 2.459,00 | **3.943,04 M€** | **4.048,45 M€** | 97,40 | $\times 1,0267$ | 15.654 km | 258.619 €/km | 690,40 M | 5,86 € |
| **2025** | 2.022,54 | 2.283,00 | **4.305,54 M€** | **4.305,54 M€** | 100,00 | $\times 1,0000$ | 15.660 km | 274.939 €/km | 694,11 M | 6,20 € |

---

## 📱 Característiques de l'Aplicació Web

* **Disseny Adaptat a Dispositius Mòbils (*Mobile-First*)**: Optimitzat per a pantalles tàctils d'**iPhone (Safari iOS)** i **Android (Chrome)**, incloent compatibilitat amb la muesca de pantalla (*notch*) i barra d'estat translúcida.
* **Gràfics Interactius Dinàmics (Chart.js)**:
  1. *Inversió Total Apilada* (ADIF Convencional en blau fosc + ADIF AV en blau cel) amb corba superposada en euros constants de 2025.
  2. *Esfuerç inversor per quilòmetre de xarxa RFIG* (€/km).
  3. *Inversió per viatger enfront de la corba de demanda de passatgers*.
  4. *Evolució de l'IPC de l'INE i factor multiplicador del deflactor*.
* **Taula Tàctil amb Desplaçament Suau**: Dissenyada perquè no desbordi en pantalles estretes de mòbil, acompanyada d'indicadors de lliscament.
* **Descàrregues Directes**: Enllaços integrats a l'aplicació per descarregar el model en **Excel (`.xlsx`)** amb 3 pestanyes formulades i en **CSV**.
* **Marca d'aigua Oficial**: Signatura i marca d'aigua integrada `@bcnopenmind` tant a la interfície com a les exportacions gràfiques.

---

## 📁 Estructura del Projecte

```text
├── index.html                                  # Panell web interactiu i responsive (HTML5, Tailwind CSS, Chart.js)
├── README.md                                   # Memòria explicativa del projecte en català
├── ADIF_Inversion_Ferroviaria_2011_2025.xlsx  # Model complet en Excel (3 pestanyes amb format comptable i enllaços)
├── ADIF_Inversion_Ferroviaria_2011_2025.csv   # Dades mestres tabulades (UTF-8 amb BOM i separador ;)
└── graficos/                                   # Gràfics d'alta resolució (300 DPI) amb marca d'aigua
    ├── 1_evolucion_inversion_inflacion_2011_2025.png
    ├── 2_inversion_por_km_red_2011_2025.png
    ├── 3_inversion_por_pasajero_2011_2025.png
    └── 4_dashboard_analisis_completo.png
```

---

## 🏛️ Fonts i Verificació Oficial

Totes les dades s'han extret exclusivament d'organismes oficials del Govern d'Espanya:
1. **ADIF (Comptes Anuals Auditats per la IGAE)**: [adif.es/sobre-adif/conoce-adif/cuentas-anuales](https://www.adif.es/sobre-adif/conoce-adif/cuentas-anuales)
2. **ADIF Alta Velocidad (Comptes Anuals)**: [adifaltavelocidad.es/conoce-adif-av/cuentas-anuales](https://www.adifaltavelocidad.es/conoce-adif-av/cuentas-anuales)
3. **Intervenció General de l'Administració de l'Estat (IGAE)**: Comprovació d'autenticitat dels informes mitjançant Codi Segur de Verificació (CSV) a [pap.hacienda.gob.es](https://www.pap.hacienda.gob.es/)
4. **Institut Nacional d'Estadística (INE)**:
   - Sèrie històrica de l'IPC General: [Taula 24077 d'INEbase](https://servicios.ine.es/wstempus/js/ES/DATOS_TABLA/24077)
   - Transport Ferroviari de Viatgers: [Taula 24363 d'INEbase](https://servicios.ine.es/wstempus/js/ES/DATOS_TABLA/24363)
5. **Ministeri de Transports i Mobilitat Sostenible**: Observatori del Ferrocarril a Espanya (OFE) i OTLE.

---

## 👤 Autoria

Anàlisi econòmica, consolidació comptable i desenvolupament realitzat per:  
**autor: [@bcnopenmind](https://github.com/bcnopenmind)**
