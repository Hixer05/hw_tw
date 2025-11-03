# Progetto C




## Info generali

William Brusa (0001162700)




## Struttura

Il sito web segue le direttive indicate nella consegna, contiene tutto il css (partizionato da opportuni commenti) nel file `style.css`.




## Design e Palette Colori

Il sito utilizza una palette ispirata al tema &ldquo;Gruvbox&rdquo;, prediligendo colori poco affaticanti per la vista e ad alto contrasto.
Sono state definite variabili CSS (`:root { --color-primary, ... }`) per tutti i colori principali, di sfondo, testo ed elementi UI. 




## Tipografia

Scelte font di tipo &ldquo;system-ui&rdquo;, con fallback a Segeo UI e Arial, per massima leggibilità e supporto multipiattaforma.
Tutte le dimensioni dei font sono espresse in unità relative (`rem`, `em`, `vw`), così da adattarsi alle preferenze dell’utente.




## Layout Responsive / Mobile First

L’intero layout adotta un approccio mobile-first, con breakpoint progressivi a 480px, 768px, 1024px e 1280px.
Sono usate proprietà CSS come `flex` e `grid` per garantire adattabilità delle sezioni principali, dei menu, delle griglie di esercizi e delle sidebar.
Le tabelle degli esercizi usano un wrapper `.table-wrapper` con `overflow-x: auto` per l’usabilità su dispositivi piccoli, senza compromettere la semantica HTML della `<table>`.




## Semantica e Landmark

Struttura logica con `<header>`, `<nav>`, `<main>`, `<aside>`, `<footer>`.
Uso di ruoli e landmark ARIA ove utile (`aria-label`, `aria-current`, &hellip;).
Breadcrumb e menu di navigazione sono sempre costruiti con elementi semantici (`<ol>`, `<ul>`, ecc.).




## Accessibilità

Presenza di focus visibile su tutti gli elementi interattivi (`:focus-visible`): bordo esterno colorato e offset ben visibile, personalizzato con variable CSS.
**Contenuto navigabile interamente da tastiera.**
Immagini e icone hanno tutti un `alt` appropriato o vengono marcati `aria-hidden=”true”` quando puramente decorative (es. emoji).
Testate, paragrafi, liste, badge: tutto con markup HTML semanticamente corretto.
Area chat e sezioni principali sono dotate di `aria-label` e `aria-live` dove opportuno.




## Animazioni

Animazioni leggere su carte, banner, e bottoni. 
Le animazioni sono fluide e di breve durata, non interrompendo la fruibilità o l’accessibilità.
I pulsanti e i link principali hanno transizioni di colore e spostamento per feedback visivo.

## Componentizzazione e Utility CSS

Uso intensivo di utility class (`.text-center`, `.badge`, `.card-link`) per ridurre duplicazioni.
Tutte le unità di spaziatura e radius sono variabili.

