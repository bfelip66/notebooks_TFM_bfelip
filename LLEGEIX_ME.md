# Documentació del repositori de dades i codi

**Títol del TFM:** *Estudi sobre la relació entre el creixement de l'extrema dreta i la violència contra les dones*

Aquest repositori conté el material computacional, les dades originals i els models estadístics utilitzats per investigar la relació entre l’indicador de vot a l'extrema dreta i diversos indicadors de violència masclista.

## 1. Estructura del repositori.

/
├── data/
│   ├── originals/         # Fonts originals (INE, Ministeris, CGPJ), sense processar
│   └── processats/    # Dataset unificat (rates_all_metrics_by_province_year_unified_final_FIXED.csv)
├── notebooks/
│   ├── 01_neteja_i_preparacio.ipynb
│   └── 02_analisi_exploratoria_i_descriptiva.ipynb
├── requirements.txt
└── Informe_analitic_visual_TFM_Bfelip.pdf

## 2. Requeriments tècnics.

L’anàlisi s’ha desenvolupat en un entorn **Python 3.8.8**. Per garantir la reproductibilitat dels resultats:

1. Instal·la **Python 3.8.8**.
2. Instal·la les dependències amb `pip`:

```bash
pip install -r requirements.txt
````

> [!NOTE]
> Si treballes amb entorns virtuals (recomanat), crea i activa l’entorn abans d’instal·lar les dependències.

---

## 3. Notes sobre metodologia i estadística.

Per abordar la naturalesa multidimensional de les dades, s'han aplicat tècniques avançades:

* **Control de la taxa de falsos descobriments (FDR):** aplicat a les matrius de correlació per corregir l'efecte de les comparacions múltiples.
* **Imputació de dades (LOCF):** s'ha utilitzat Last Observation Carried Forward en les sèries temporals per mantenir la coherència visual i analítica davant de possibles buits en el registre provincial.
* **Models d'Efectes Fixos (FE):** utilitzats per explotar la variació within (intra-provincial) i aïllar els efectes de variables temporals i territorials constants.

## Informe analític: instrument de transferència dissenyat per fer la recerca socialment accessible i metodològicament rigorosa.Mitjançant un disseny que prioritza la claredat i l'ús de suports versàtils, s'eliminen barreres d'entrada, transformant dades tècniques sobre extrema dreta i violència de gènere en coneixement estratègic i directament aplicable.

---

## 4. Autoria i contacte.

* **Autora:** Begoña Felip Bengochea (bfelip@uoc.edu)
* **Data:** gener 2026
