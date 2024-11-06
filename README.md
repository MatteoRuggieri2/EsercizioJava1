# Programmazione ad Oggetti

## Esercizio 3

Si realizzi la classe Java `SchedaPersona` contenente le seguenti informazioni:

- `String nome`: contiene il nome e cognome
- `String indirizzo`: contiene l’indirizzo
- `String numero`: contiene il numero di telefono

La classe, oltre a definire i vari metodi di tipo mutator e accessor (getter e setter) per l’inizializzazione ed il reperimento degli attributi privati, dovrà implementare i seguenti metodi:

- **`boolean equals(Object s)`**  
  Ritorna `true` nel caso in cui l’oggetto ricevuto sia di tipo `SchedaPersona` (attraverso l’operatore `instanceof`) e che gli attributi siano uguali (si consiglia di utilizzare un confronto *case-insensitive*), `false` in caso contrario.

- **`boolean contains(String s)`**  
  Ritorna `true` nel caso in cui uno degli attributi contenga la stringa ricevuta come parametro, `false` in caso contrario (si consiglia di utilizzare un confronto *case-insensitive*).

- **`String toString()`**  
  Costruisce una rappresentazione stampabile della scheda.

Si realizzi, inoltre, la classe JUnit `SchedaPersonaTest` che istanzia 3 o più schede, le popola con dei dati ed esegue test specifici per verificare il corretto funzionamento dei metodi definiti.

### Suggerimenti:

- Per eseguire il confronto *case-insensitive* si può usare il metodo `equalsIgnoreCase` della classe `String`, oppure convertire dapprima entrambe le stringhe in maiuscolo (`toUpperCase`) e poi confrontarle.
- Per verificare se una stringa è contenuta in un’altra utilizzare il metodo `indexOf` della classe `String`.
