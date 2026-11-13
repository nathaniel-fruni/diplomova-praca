# Jemné doladenie jazykových modelov pre riešenie špecifických úloh – praktická časť diplomovej práce

Tento repozitár obsahuje praktickú časť diplomovej práce zameranej na klasifikáciu sentimentu slovenských textov. Postup práce sa riadi metodikou **CRISP-DM** (Cross-Industry Standard Process for Data Mining).

## Dataset

**[TUKE-KEMT/senti-sk](https://huggingface.co/datasets/TUKE-KEMT/senti-sk)** – dataset slovenských komentárov zo sociálnych sietí, z ktorých každý je označený sentimentom (negatívny, neutrálny alebo pozitívny).

## Metodika CRISP-DM

CRISP-DM rozdeľuje projekt do šiestich fáz. Fázy na seba nadväzujú, no postup je iteratívny, takže poznatky z neskorších fáz sa môžu premietnuť späť do predchádzajúcich.

### 1. Pochopenie problému (Business Understanding)

Vymedzenie cieľa práce, teda čo má model riešiť a prečo. Stanovujú sa kritériá úspešnosti a požiadavky na výsledné riešenie.

### 2. Pochopenie dát (Data Understanding)

Prvotné preskúmanie datasetu: štruktúra stĺpcov, rozdelenie tried, kvalita a konzistentnosť dát. Súčasťou je aj jazyková analýza textov (dĺžka, slovné druhy, jazyk komentárov), ktorej výsledkom sú odporúčania pre ďalšiu fázu.

### 3. Príprava dát (Data Preparation)

Čistenie a úprava dát na základe zistení z predchádzajúcej fázy, napríklad odstránenie duplicít a chybných záznamov a predspracovanie textu do podoby vhodnej na modelovanie.

### 4. Modelovanie (Modeling)

Výber, natrénovanie a ladenie modelov na klasifikáciu sentimentu.

### 5. Vyhodnotenie (Evaluation)

Porovnanie modelov pomocou zvolených metrík a posúdenie, či výsledky spĺňajú ciele stanovené v prvej fáze.

### 6. Nasadenie (Deployment)

Zhrnutie výsledkov a opis, ako by sa dal výsledný model prakticky použiť.

## Štruktúra repozitára

| Súbor | Popis |
|---|---|
| [`data_understanding.ipynb`](data_understanding.ipynb) | Fáza pochopenia dát |
| [`data_preparation.ipynb`](data_preparation.ipynb) | Fáza prípravy dát |

Notebooky sú pripravené na spustenie v [Google Colab](https://colab.research.google.com/).
