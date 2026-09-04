# Optimizacija hiperparametara metodama bez izvoda

## Opis projekta

Projekat se bavi poređenjem osnovnih metoda optimizacije hiperparametara mašinskog učenja koje ne
koriste izvod funkcije cilja: **Grid Search**, **Random Search** i **Nelder-Mead** (simplex metoda).
Cilj je empirijski uporediti kvalitet pronađenih rešenja, broj potrebnih evaluacija i vreme
izvršavanja svake od metoda na dva skupa podataka i dva modela mašinskog učenja, te izvesti
zaključke o tome koja metoda predstavlja najbolji kompromis kvalitet/cena.


## Skup podataka

Koriste se dva ugrađena `sklearn.datasets` skupa 
- **Breast Cancer Wisconsin** — 569 instanci, 30 numeričkih atributa, binarna klasifikacija
  (maligni/benigni), blago neuravnotežen (~63%/37%).
- **Digits** — 1797 instanci, 64 atributa (8×8 slike cifara), 10 klasa, približno uravnotežen.

Modeli koji se optimizuju: **SVM (RBF kernel)** i **Random Forest** 

**Metodologija evaluacije** (prati referentni rad Yang & Shami, 2020, poglavlje 7.1): #todo 

## Struktura projekta

```
.
├── README.md
├── requirements.txt
├── notebooks/
│   ├── 01_EDA.ipynb                    # analiza skupa podataka
│   ├── 02_grid_search.ipynb            # Grid Search (SVM + Random Forest, oba skupa)
│   ├── 03_random_search.ipynb          # Random Search (SVM + Random Forest, oba skupa)
│   ├── 04_nelder_mead.ipynb            # Nelder-Mead (SVM + Random Forest, oba skupa)
│   └── 05_poredjenje_zakljucci.ipynb   
├── results/                    # all_results.csv — generiše se pokretanjem svesaka 02–04
```


## Korišćena literatura

1. Yang, L., & Shami, A. (2020). *On hyperparameter optimization of machine learning algorithms:
   Theory and practice.* Neurocomputing.
   [PDF](https://www.eng.uwo.ca/oc2/publications/thepublicationpdfs/2020_YangShami_NeuroComputing.pdf)

## Članovi tima

- Anja Čolić — 1059/2024


## Pokretanje

Sveske pregledati i pokretati ovim redosledom:

#todo

