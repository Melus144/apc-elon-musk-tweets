# Pràctica Kaggle APC UAB 2021-22
### Nom: Adrià Melús
### DATASET: Elon Musk Tweets
### URL: [Elon Musk Tweets](https://www.kaggle.com/taruntiwarihp/elon-musk-tweets)
### Github: [APC- Elon Musk Tweets](https://github.com/Melus144/apc-elon-musk-tweets)
## Resum
El dataset utilitza dades referents a una gran llista de tweets sobre Elon Musk de la famosa xarxa social Twitter.
Tenim 25757 dades amb 3 atributs; Un és categòric (sentiment), un altre és contínu (tweet) i el restant és numèric (index) i no es fa servir ja que no aporta informació rellevant.
### Objectius del dataset
Volem aprendre a predir el sentiment (positiu o negatiu) d'un tweet sobre Elon Musk a partir de una gran llista d'aquests.
## Experiments
Durant aquesta pràctica hem realitzat diferents experiments relacionats amb escollir i entrenar varis models per la classificació de dades per aconseguir l'objectiu esmentat. 
### Preprocessat
Pel preprocessat de dades, s'ha fet una neteja dels tweets, eliminant la puntuació, els números, símbols com el @, enllaços, la paraula "elonmusk", les paraules buides i les "stop words".
Això ha permès que els text sigui molt més comprensible pels modelsi puguin treballar obtenint millors resultats.
### Model
| Model | Hiperparametres | Mètrica |
| [Logistic Regression](https://www.kaggle.com/prashant111/logistic-regression-classifier-tutorial) | solver='lbfgs', max_iter='400' | 86% | Nota: Si no s'afegeix el nombre maxim d'iteracions, l'algorisme no convergeix amb les iteracions per defecte.|
| [Naive Bayes](https://www.kaggle.com/prashant111/naive-bayes-classifier-in-python) | -- | 66% |
| [SVM](https://www.kaggle.com/prashant111/svm-classifier-tutorial) | -- | 88% |
| [Random Forest](https://www.kaggle.com/prashant111/random-forest-classifier-tutorial) | n_estimators=50 | 83% |
## Notebook
El Jupyter Notebook referent a la pràctica es troba en el directori "/notebooks/Practica3-E".
## Conclusions
Els millors models han estat Logistic Regression, SVM i Random Forest amb resultats molt similars (Aproximadament precisió del 86% i amb puntuació AUC del 93% ).
## Idees per treballar en un futur
Crec que seria interesant indagar més en l'entrenament dels models per millorar els seus resultats i quedar-se definitivament amb el model amb més marge de millora. El text preprocessat és adequat per poder seguir entrenant els models.