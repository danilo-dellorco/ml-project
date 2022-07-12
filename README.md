L'obiettivo è quello di utilizzare il dataset [Patient Survival Prediction](https://www.kaggle.com/datasets/mitishaagarwal/patient) per effettuare il training diversi classificatori, al fine di predirre se un paziente sopravvivrà o morirà sulla base dei *parametri vitali* registrati al momento dell'ingresso in ospedale. Per fare ciò si effettua innanzitutto una fase di **Data Exploration**, in modo da ricavare informazioni utili sui dati da utilizzare, e comprendere quali sono le feature probabilmente più rilevanti ai fini della classificazione. Dopo aver splittato il dataset in **Testing e Training Set**, si procede conj l'**Ingegneria delle Features** sul Training Set, rimuovendo le features con *valori nulli*, *poco correlate* con il target, ed applicando la *feature selection*. Successivamente si esegue una fase di **Model Selection** sui vari classificatori considerati, effettuando il *tuning dei loro iperparametri*. Infine, si eseguono tutti i **Classificatori** con le features ed i parametri individuati in precedenza, effettuando un confronto tra le prestazioni ottenute.

## Indice

- **Operazioni Preliminari**
    - Installazione dipendenze
    - Import delle Librerie
    - Caricamento del sataset
    - Funzioni e variabili user-defined
    $$$$
- **Data Exploration**
    - Descrizione del Dataset
    - Bilanciamento delle classi
    - Distribuzione delle Features
    - Visualizzazione campi non nulli
    - Conversione Features e Mapping
    - Correlazione tra le Features
    - Analisi delle Features
    $$$$
- **Criterio di Performance Evaluation**
    - Training & Test Splitting
    - Scelta della Metrica
    - Risultati sul Dataset originale
    $$$$
- **Features Engineering**
    - Rimozione features con valori nulli
    - Rimozione features con bassa varianza
    - Rimozione features con bassa correlazione col target
    - Feature Selection
    - Confronto Prestazioni
    - Imputazione dei dati mancanti
    - Altri tentativi di Miglioramento
        - SMOTE
    $$$$
- **Model Selection** e **Classificazione**
    - Logistic Regression Classifier
    - Decision Tree Classifier
    - Naive Bayes Classifier
    - Random Forest Classifier
    - AdaBoost Classifier
    - Linear Discriminant Analysis
    - Support Vector Machine
    - KNeighbors Classsifier
    - MLP Classifier
    $$$$
- **Contronto e Conclusioni**