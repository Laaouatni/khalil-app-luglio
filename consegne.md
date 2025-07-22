= Progettazione Web - Preparazione alla sessione II - 2024-2025
== Introduzione
Cari studenti,

Siete invitati a un recupero di progettazione web quest'estate.

Per superare questo esame, che si svolgerà su computer per una durata di 1h30, sarà necessario essere ben preparati ed efficienti.

Durante questa sessione, non sarà consentito alcun aiuto esterno, nessun documento, né alcuna intelligenza artificiale, comprese le versioni integrate in VSCode. Qualsiasi violazione di questa regola sarà considerata plagio.

L’unica risorsa autorizzata sarà la documentazione ufficiale MDN tramite il sito:
https://developer.mozilla.org/fr/docs/Web

Vi consiglio quindi di installare in VSCode l'estensione Go to MDN - Kamil Bysiec.

== Argomento
L'esercizio consisterà nel riprodurre il layout visivo di un sito web. Vi sarà fornito uno screenshot della versione mobile del sito.

Per esercitarvi, troverete allegato uno screenshot di un altro sito.

Si tratta di una versione semplificata del sito dell’Istituto Nazionale dell’Audiovisivo (INA):
https://madelen.ina.fr/content/les-femmes-savantes-75931

ATTENZIONE: il riquadro grigio non fa parte del sito web, è solo presente nello screenshot.

Vi sarà chiesto di sviluppare seguendo la strategia vista in classe:

HTML semantico + CSS3

Approccio mobile first

Nessun framework, nessun utilizzo di JavaScript al di fuori dei Web Components.

Non vi sarà quindi chiesta alcuna interazione dinamica (niente caroselli attivi), solo una riproduzione fedele del layout visivo.

Installate l'estensione Mobile in VS - wagdye (con l’iPhone 14 come dispositivo predefinito). Questa vista sarà il riferimento per la correzione.

== Lavoro richiesto
Riproducete nel modo più fedele possibile il layout che vi verrà fornito.

Seguite un approccio mobile first. Non avremo il tempo di costruire la versione desktop. Per simularla, vi basterà cambiare il colore del titolo in viola.

Per quanto riguarda i temi, lo screenshot rappresenta il tema chiaro (anche se ha un aspetto scuro). Simulerete il passaggio al tema scuro modificando il colore del titolo in blu.

Utilizzerete variabili CSS per i colori, definite nella radice.

Aggiungerete un semplice menu di accessibilità nascosto, composto da un solo link che punta alla sezione principale del sito.

Inserirete un commento per giustificare la vostra politica di accessibilità delle immagini, in conformità alle direttive RG2A.

Cambierete il colore del pulsante con un gradiente lineare nei colori a vostra scelta.

Trasformerete le miniature del vostro carosello in Web Components. Notate che l’ultima miniatura a sinistra deborda, ma non c’è barra di scorrimento orizzontale.

== Precisazioni
Il giorno dell’esame, vi saranno forniti alcuni elementi per farvi risparmiare tempo su dettagli secondari.

Vi saranno forniti: testi, codici colore, font e dimensioni, immagini, ecc.

Per sviluppare senza problemi, è necessario reimpostare le proprietà CSS applicate di default dal browser (non standard). Per questo, vi fornirò il foglio CSS da importare.

Allo stesso modo, dovrete reimpostare alcune proprietà dei tag utilizzati all’interno dei vostri Web Components.

Esempio di reset in un Web Component:

css
Copier
Modifier
*, *::before, *::after {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}
== Consigli
Il giorno dell’esame, non perdete tempo nei dettagli. Non cercate la precisione al pixel, a meno che non abbiate completato gli elementi essenziali.

Iniziate con una versione senza Web Component, poi trasformate il codice in un secondo momento.

Potete salvare versioni intermedie. Se vi doveste perdere nello sviluppo, potrete tornare facilmente a uno stato stabile e comunque presentare un lavoro coerente.

Esercitatevi usando VSCode diviso in tre pannelli: codice, immagine, estensione mobile.

Non dimenticate gli aspetti semantici del web: tag, lingua della pagina, ecc.

Ecco un elenco non esaustivo di proprietà e direttive CSS che vi saranno utili:

less
Copier
Modifier
@import | @font-face | background | linear-gradient | text-align | padding |
font-size | font-weight | line-height | margin | color | border |
border-radius | overflow | font-family | width | display |
vertical-align | last-child | :root