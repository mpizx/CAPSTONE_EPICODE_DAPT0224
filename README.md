# Rilevazione di Anomalie nel Traffico di Rete - NSL-KDD Dataset

## Descrizione del Progetto

Questo progetto si concentra sull'analisi del **traffico di rete** per identificare **anomalie** che potrebbero indicare minacce informatiche, come attacchi DDoS, brute force o tentativi di accesso non autorizzati. Utilizzando il **dataset NSL-KDD**, il progetto esamina il traffico di rete in base a variabili chiave, come i byte inviati e ricevuti, i tentativi di login falliti, i protocolli utilizzati, e calcola un punteggio di rischio per ciascun evento.

Inoltre, sono stati aggiunti **timestamp simulati** per creare un'analisi temporale che permette di osservare l'andamento del traffico e le anomalie nel tempo. I risultati sono stati visualizzati tramite **grafici avanzati** in Python e integrati in una **dashboard interattiva con Power BI**.

## Funzionalità Principali

- **Analisi dei log di rete**: Analizza i dati per rilevare comportamenti anomali.
- **Calcolo del punteggio di rischio**: Basato su variabili come byte inviati e tentativi falliti.
- **Rilevamento delle anomalie**: Tramite soglie predefinite e deviazione standard.
- **Simulazione temporale**: Aggiunta di una colonna `timestamp` per visualizzare le anomalie nel tempo.
- **Dashboard Power BI**: Una dashboard interattiva per monitorare i risultati in tempo reale.

## Dataset Utilizzato

Il dataset utilizzato è **NSL-KDD**, una versione migliorata del classico dataset KDD'99, che contiene log di rete con etichette per traffico normale e attacchi.

- **NSL-KDD Train Set**: [NSL_KDD_Train.csv](https://raw.githubusercontent.com/Mamcose/NSL-KDD-Network-Intrusion-Detection/refs/heads/master/NSL_KDD_Train.csv)
- **NSL-KDD Test Set**: [NSL_KDD_Test.csv](https://raw.githubusercontent.com/Mamcose/NSL-KDD-Network-Intrusion-Detection/refs/heads/master/NSL_KDD_Test.csv)

## Grafici e Visualizzazioni

Nel progetto sono stati utilizzati diversi tipi di grafici per esplorare i dati e individuare anomalie:

1. **Distribuzione delle Etichette**: Grafico a barre che mostra il numero di eventi normali rispetto agli attacchi.
2. **Boxplot per `src_bytes`**: Visualizza la distribuzione dei byte inviati, individuando outlier.
3. **Grafico a Linee del Traffico per Protocollo**: Mostra come varia il traffico in base al protocollo (`tcp`, `udp`, `icmp`).
4. **Istogramma del Numero di Connessioni**: Evidenzia il numero di connessioni per ciascun intervallo di tempo.
5. **Scatter Plot tra `src_bytes` e `dst_bytes`**: Visualizza la relazione tra byte inviati e ricevuti per ogni evento.
6. **Grafico a Linee basato sul Timestamp**: Monitora l'andamento del traffico `src_bytes` e `dst_bytes` nel tempo.
7. **Mappa di Calore basata sul Tempo**: Visualizza l'intensità del traffico per ore e giorni.

## Dashboard Power BI

La dashboard interattiva in **Power BI** consente di esplorare i dati visualizzati attraverso una serie di grafici. Le visualizzazioni principali includono:

- **Grafico a Linee del Traffico nel Tempo**: Mostra l'andamento del traffico `src_bytes` e `dst_bytes` nel tempo.
- **Mappa di Calore**: Visualizza l'intensità del traffico in base alle ore e ai giorni.
- **Grafico a Barre della Distribuzione delle Etichette**: Visualizza la distribuzione di traffico legittimo rispetto agli attacchi.

### Screenshots della Dashboard
- *(Aggiungi qui uno screenshot della tua dashboard Power BI una volta completata.)*

## Credits

- **Michele**: Sviluppo del progetto e analisi dei dati.
- **NSL-KDD Dataset**: Dati utilizzati per l'analisi del traffico di rete.

## License

Questo progetto è distribuito sotto la licenza **GNU General Public License v3.0**. Consulta il file [LICENSE](LICENSE) per i dettagli.
