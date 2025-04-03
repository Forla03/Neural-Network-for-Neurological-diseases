# Progetto di Riconoscimento Immagini Mediche con CNN

Questo progetto implementa una rete neurale convoluzionale (CNN) per il riconoscimento di immagini mediche. L'obiettivo principale è classificare correttamente le immagini fornite nel dataset e valutare le performance del modello sviluppato.

## Struttura della Rete Neurale

La rete neurale utilizzata è basata su un'architettura CNN, che include i seguenti strati:

- Strati convoluzionali per l'estrazione delle caratteristiche
- Strati di pooling per la riduzione della dimensionalità
- Strati completamente connessi per la classificazione finale

Le immagini sono preprocessate convertendole in scala di grigi e ridimensionandole a 128x128 pixel.

## Addestramento del Modello

L'addestramento del modello viene effettuato utilizzando un dataset diviso in:

- **Training set** per l'apprendimento
- **Test set** per la valutazione delle prestazioni

Durante l'addestramento, il modello utilizza la funzione di perdita `categorical_crossentropy` e l'ottimizzatore Adam. L'addestramento avviene per un numero prefissato di epoche con l'uso di tecniche di data augmentation per migliorare la generalizzazione.

## Risultati e Conclusioni

Dopo l'addestramento, il modello viene valutato in termini di accuratezza e perdita sul test set. I risultati ottenuti indicano che la CNN è in grado di riconoscere le immagini mediche con una buona precisione. Più in particolare, si sono ottenuti i seguenti risultati:

- Accuratezza finale sull'insieme di training: 86.89%
- Accuratezza finale sull'insieme di validazione: 88.44%

In conclusione, il modello rappresenta un primo passo verso un sistema di classificazione automatica delle immagini mediche, con potenziali applicazioni in ambito diagnostico.



## dataset author
@dataset{alzheimer_mri_dataset,
  author = {Falah.G.Salieh},
  title = {Alzheimer MRI Dataset},
  year = {2023},
  publisher = {Hugging Face},
  version = {1.0},
  url = {https://huggingface.co/datasets/Falah/Alzheimer_MRI}
}