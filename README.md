# Progetto di rilevazione di anomalie nel traffico di rete - NSL-KDD Dataset

## Descrizione del progetto

Questo progetto si concentra sull'analisi del **traffico di rete** per identificare anomalie che potrebbero indicare minacce informatiche, come attacchi DDoS, brute force o tentativi di accesso non autorizzati. Utilizzando il **dataset NSL-KDD**, che contiene sia traffico legittimo che attività sospette, ho condotto un'analisi per rilevare comportamenti anomali e potenzialmente dannosi, offrendo insights che possono aiutare a prevenire attacchi.

Il progetto si conclude con la creazione di una **dashboard interattiva in Power BI** che presenta i risultati dell'analisi in modo chiaro e intuitivo.

## La finalità di questo progetto

L'idea centrale dietro questo progetto è legata all'importanza crescente della **cybersecurity** in un mondo digitale sempre più connesso. Le reti aziendali sono frequentemente bersaglio di attacchi informatici, che possono compromettere dati sensibili e causare danni significativi. **Monitorare e analizzare il traffico di rete** in tempo reale è essenziale per rilevare e mitigare potenziali minacce.

### Perché un'analisi statistica invece del machine learning?

Ho scelto di adottare un'**analisi statistica** piuttosto che strumenti di machine learning per diverse ragioni:
1. **Semplicità e chiarezza**: L'analisi statistica consente di identificare anomalie in modo chiaro, utilizzando metodi come la * *deviazione standard* * e i * *punteggi di rischio* *. Ciò permette di comprendere facilmente i dati senza la complessità degli algoritmi di machine learning.
2. **Interpretabilità**: I risultati statistici sono immediatamente comprensibili e interpretabili dagli operatori di rete. In molti casi, le aziende di piccole e medie dimensioni preferiscono strumenti che forniscono risposte semplici e dirette, piuttosto che modelli predittivi complessi che possono essere difficili da spiegare.
3. **Focalizzazione su pattern anomali**: L'obiettivo era concentrarsi su anomalie evidenti e comportamenti fuori dalla norma. Le soglie e le regole statistiche (come il calcolo della media e la deviazione standard) sono sufficienti per rilevare picchi di traffico o attività sospette in molti scenari.
   
L'analisi statistica offre quindi un approccio diretto ed efficace per il rilevamento di anomalie, senza la necessità di creare modelli complessi di apprendimento automatico, che richiedono tempo di addestramento e test.

## Dataset utilizzato

Ho utilizzato il **dataset NSL-KDD** disponibile su [Kaggle](https://www.kaggle.com/datasets/hassan06/nslkdd). Questo dataset è una versione migliorata del classico KDD'99, noto per la sua applicazione nel rilevamento di intrusioni di rete. Contiene una combinazione di traffico legittimo e tentativi di attacco.

Per l'analisi ho distinto i dati in due parti:
- **NSL-KDD Train Set**: Utilizzato per calcolare le soglie di rischio e condurre le prime analisi.
- **NSL-KDD Test Set**: Utilizzato per valutare il modello di rischio e testare l'efficacia delle soglie definite.

Ho scelto di usare i file **train** e **test** separatamente per simulare un'analisi che possa essere ripetibile su set di dati futuri, garantendo così che le soglie definite siano valide anche su nuovi dati.

## Funzionalità principali

- **Calcolo del Punteggio di Rischio**: Un sistema di valutazione del rischio basato su variabili come i byte inviati (`src_bytes`), i tentativi di login falliti e il protocollo di rete.
- **Rilevamento delle Anomalie**: Identificazione di eventi anomali attraverso analisi statistiche basate sulla deviazione standard.
- **Simulazione Temporale**: Aggiunta di una colonna `timestamp` per simulare il monitoraggio temporale del traffico e osservare i picchi sospetti.
- **Dashboard Interattiva in Power BI**: Visualizzazione dei risultati in una dashboard interattiva per comprendere meglio i pattern di traffico e le anomalie.

## Grafici utilizzati

Diversi tipi di grafici sono stati utilizzati per esplorare e visualizzare i dati:

1. **Distribuzione delle Etichette**: Un grafico a barre che mostra la proporzione di traffico normale e attacchi.
2. **Boxplot per `src_bytes`**: Un grafico che evidenzia la distribuzione dei byte inviati e identifica outlier.
3. **Grafico a Linee del Traffico per Protocollo**: Rappresenta l'andamento del traffico in base ai protocolli di rete (`tcp`, `udp`, `icmp`).
4. **Grafico a Linee basato sul Timestamp**: Mostra l'andamento del traffico (byte inviati) nel tempo.
5. **Mappa di Calore del Traffico**: Mostra l'intensità del traffico per ora e giorno.

## Dashboard in Power BI

Il progetto include una **dashboard interattiva in Power BI**, che consente di visualizzare le anomalie e i pattern di traffico di rete nel tempo. Questa dashboard facilita l'analisi dei dati e permette di filtrare eventi sospetti, migliorando così la capacità di risposta alle minacce.

### Link alla dashboard e al progetto

- **[PDF della Dashboard Power BI](https://github.com/username/project-name/PowerBI-Dashboard.pdf)** 
- **[Link al Progetto su GitHub](https://github.com/username/project-name)** 

## Credits

- **Michele Pinzan**: Sviluppo del progetto e analisi dei dati.
- **NSL-KDD Dataset**: Dati utilizzati per l'analisi del traffico di rete. Dataset scaricabile da [Kaggle](https://www.kaggle.com/datasets/hassan06/nslkdd).
  
## License

Questo progetto è distribuito sotto la licenza **GNU General Public License v3.0**. Consulta il file [LICENSE](https://github.com/username/project-name/blob/main/LICENSE) per i dettagli.
