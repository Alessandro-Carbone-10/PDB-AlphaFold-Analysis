# Analisi di Strutture Proteiche Metamorfiche: Il caso RfaH

## Panoramica del Progetto
 L'obiettivo del progetto è stato sviluppare uno script Python che confronti le predizioni di AlphaFold con le strutture sperimentali (PDB) della proteina RfaH. L'obiettivo non è solo calcolare l'errore globale, ma mappare l'errore locale contro la confidenza del modello (pLDDT per residuo amminoacidico) per determinare se l'IA è "consapevole" della propria incertezza nelle regioni metamorfiche o se genera artefatti errati con alta confidenza.

## Tecnologie e Librerie Utilizzate
*   **Linguaggio:** Python
*   **Ambiente:** Jupyter Notebook
*   **Librerie Principali:** Biopython (per l'elaborazione delle sequenze e dei dati strutturali), Matplotlib (per la visualizzazione dei dati), py3Dmol (per la visualizzazione 3D delle molecole)

## Risultati 
<img width="1189" height="627" alt="image" src="https://github.com/user-attachments/assets/e1d091ee-6943-4541-8405-75ac24adcc58" />

<img width="997" height="520" alt="image" src="https://github.com/user-attachments/assets/8c8a62d5-aa3c-41fd-9ee4-d06e8e008ebd" />
<img width="997" height="520" alt="image" src="https://github.com/user-attachments/assets/74b53ba2-9cde-467c-bac2-f401937ba515" />

## Metodologia
*   Importazione e parsing dei file PDB.
*   Elaborazione e processamento delle stringhe per l'allineamento tramite Superposizione (Bio.PDB.Superimposer).
*   Calcolo della media quadratica delle distanze tra atomi corrispondenti, confronto delle metriche e generazione dei grafici.
*   Visualizzazione e confronto visivo delle proteine sovrapposte (py3Dmol).
