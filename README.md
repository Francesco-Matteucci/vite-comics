# DC Comics Project

## Descrizione

Questo progetto rappresenta un sito dinamico che visualizza fumetti della DC Comics utilizzando **Vue.js**. I dati dei fumetti sono gestiti attraverso un file JSON che viene importato e passato ai componenti tramite `props`. È stato utilizzato **Sass** per la gestione avanzata degli stili e **Bootstrap** per il layout responsive e l'ottimizzazione mobile.

## Struttura del Progetto

- **Vue.js**: Gestione dei componenti e del passaggio di dati tramite `props`.
- **Sass**: Utilizzato per la gestione centralizzata degli stili e delle variabili.
- **Bootstrap**: Per il layout responsive e componenti predefiniti.
- **File JSON**: Contiene i dati dei fumetti (titoli, immagini, prezzi).

### Cartelle

  - `src/components`: Contiene i componenti Vue.js utilizzati nel progetto.
  - `AppHeader.vue`: Il componente header con il logo e la navigazione dinamica.
  - `AppMain.vue`: Il componente principale, che visualizza le card dei fumetti.
  - `AppHero.vue`: Una sezione che mostra delle icone.
  - `AppFooter.vue`: Il footer del sito con varie sezioni informative.
  - `ComicCard.vue`: Un componente che rappresenta ogni singolo fumetto come card.
  
- `src/assets`: Contiene le immagini e il file JSON con i dati dei fumetti.
- `style`: Contiene i file Sass, tra cui `_variables.scss` e `general.scss` per le regole globali e le variabili di stile.
