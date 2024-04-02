# Progetto "Digitiamo"


## Struttura delle cartelle

### data
La cartella "data" contiene i dati utilizzati nel progetto, suddivisi in varie categorie:
- `dataset_full_embedding`: dataset con articoli di entrambe le lingue e l'aggiunta della colonna "text_embedded", utilizzata per addestrare una rete neurale.
- `dataset_full_LLM`: dataset con articoli di entrambe le lingue utilizzato per il fine tuning del modello BERT.
- `dataset_jap_LLM`: dataset con articoli solo in lingua giapponese utilizzato per il fine tuning del modello BERT.
- `eng_df`: dataset raw con aggiunta di una colonna contenente le parole tokenizzate per la lingua inglese.
- `jap_df`: dataset raw con aggiunta di una colonna contenente le parole tokenizzate per la lingua giapponese.
- `english_news`, `japanese_news`: dataset raw originali.
- `test_d2v`, `train_d2v`: dataset di test e training con dati preprocessati usando un modello doc2vec.
- `test_w2v`, `train_w2v`: dataset di test e training con dati preprocessati usando un modello word2vec.

### models
La cartella "models" contiene i modelli addestrati durante il progetto, suddivisi in varie sottocartelle con i nomi dei modelli. Ogni sottocartella contiene i risultati e i modelli stessi in formato pickle. ***I modelli allenati su entrambe le lingue sono nella cartella "multi"***

### preprocessing
La cartella "preprocessing" contiene i modelli utilizzati per il preprocessing dei dati.

### Noto_Sans_JP
Questa cartella contiene i file necessari per utilizzare il font giapponese nei plot generati.

### notebooks
Nel progetto ci sono 3 Notebooks. 

- `digitiamo`: Prova alcuni modelli e preprocessing solo sui dati Giapponesi
- `Digitiamo_multi`: Prova Random Forest su dati di entrambe le lingue. Per fare questo modello ho usato un embedding multilingue preso da kaggle.
- `digitiamo_nn_Kaggle`: Prova alcuni modelli su cui ho fatto fine tuning e di una rete che ha un layer di embedding pre-trainato per gestire sia Giapponese che Inglese.



