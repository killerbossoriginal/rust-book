# Introduzione

Benvenuto al *Linguaggio Di Programmazione Rust*, un libro introduttivo riguardo a Rust.
Il linguaggio di programmazione Rust ti aiuta a scrivere codice più affidabile, più velocemente.
Ergonomia di alto livello e controllo di basso livello sono spesso vantaggi nel design di linguaggi di programmazione; Rust combatte questo conflitto. Attraverso il bilanciamento di capacità tecniche e una grande esperienza di sviluppo (*development experience*), Rust ti dà l'opzione di controllare dettagli di basso livello (come l'utilizzo della memoria) senza tutti i problemi tradizionalmente associati a ciò.
## Per chi è Rust?

Rust è ideale per molte persone per una varietà di ragioni. Vediamo un po' dei gruppi più importanti.

### Team di Sviluppatori

Rust sta provando di essere uno strumento produttivo per collaborare in grandi team di sviluppatori con diversi livelli di competenza. Codice di basso livello è a rischio di vari bug subdoli, che molti altri linguaggi possono catturare solo tramite test intensivi e un controllo del codice fatto da sviluppatori con esperienza. In Rust, il compilatore gioca come portiere rifiutando di compilare codice con questi bug elusivi, includendo bug di concorrenza. Lavorando assieme ad un compilatore, il gruppo piò spendere il proprio tempo concentrandosi sulla logica del programma al posto che cacciando problemi. 

Rust porta anche molti strumenti alla programmazione di sistemi:

- Cargo, il gestore di dipendenze e compilatore, gestisce la aggiunta, la compilazione, la gestione delle dipendenze, indolore e consistente per l'ecosistema Rust.
- Lo strumento di formattazione Rustfmt che assicura uno stile consistente tra gli sviluppatori.
- Il rust-analyzer che permette agli ambienti di sviluppo integrati (IDE) di completare il codice e di mostrare gli errori.

Usando questi altri strumenti nell'ecosistema Rust, gli sviluppatori possono essere produttivi mentre scrivono codice di sistema.

### Studenti

Rust è per gli studenti e per chi è interessato ad imparare riguardo i concetti di sistemi. Usando Rust, molte persone hanno imparato concetti come lo sviluppo di sistemi operativi. La comunità p molto accogliente e felice di rispondere a domande degli studenti. Tramite cose come questo libro, il team di Rust vuole rendere i concetti di sistema accessibili a più persone, specialmente quelle nuove nel mondo della programmazione.

### Aziende

Centinaia di aziende, grandi e piccole, usano Rust nella produzione di una grande varietà di task, tra cui strumenti a linea di comando, servizi web, strumenti DevOps, device embedded, analisi e transcodifica di audio e video, criptovalute, bioinformatica, motori di ricerca, applicazioni IoT, machine learning e anche grandi parti del browser web Firefox.

### Sviluppatori Open Source

Rust è per le persone che vogliono costruire il linguaggio Rust stesso, la comunità, gli strumenti per sviluppatori e le librerie. Noi ameremmo di averti tra i contributori del linguaggio Rust.

### Persone a cui interessa Velocità e Stabilità

Rust è per le persone che bramano velocità e stabilità in una lingua. Con la velocità, indichiamo sia la velocità con cui il codice Rust può essere eseguito sia la velocità con cui Rust ti permette di  scrivere programmi. I controlli del compilatore Rust garantiscono la stabilità attraverso le funzionalità aggiunte e il refactoring. Ciò è in contrasto con il fragile codice legacy in linguaggi senza questi controlli, che gli sviluppatori hanno spesso paura di modificare. Presso alla ricerca di astrazioni a costo zero, funzionalità di livello superiore che si compilano per codice di livello inferiore veloce quanto il codice scritto manualmente, Rust si sforza di rendere il codice sicuro e veloce.

Il linguaggio Rust spera anche di aiutare molti utenti; quelli menzionati qui sono solo alcuni dei più grandi gruppi. Dopotutto, l'ambizione più grande di Rust è di eliminare lo scambio che i programmatori hanno accettato per decenni, servendo sicurezza *e* produttività, velocità *ed* ergonomia. Prova Rust e vedi se le sue scelte funzionano per te.

## Per chi è questo libro?

Questo libro da per scontato che tu hai scritto codice in un altro linguaggio ma non fa assunzioni su quale. Noi abbiamo provato a rendere il materiale accessibile ad una grande varietà di background di programmazione. Non spendiamo molto tempo parlando di cosa è la programmazione o come pensarci. Se sei completamente nuovo alla programmazione, saresti meglio servito con un libro specifico che ti introduce alla programmazione.

## Come usare questo libro

In generale, questo libro assume che lo stai leggendo in sequenza dall'inizio alla fine. Capitoli successivi potrebbero basarsi in concetti precedenti, e capitoli precedenti potrebbero non entrare nei dettagli su un argomento che verrà trattato in un capitolo futuro.

Troverai due tipi di capitoli in questo libro: capitoli di concetto e capitoli di progetto. Nei capitoli di concetto imparerai gli aspetti di Rust. Nei capitoli di progetto, costruiremo piccoli programmi assieme, applicando cosa hai imparato. I capitoli 2, 12 e 20 sono capitoli di progetto gli altri sono capitoli di concetto.

Il capitolo 1 spiega come installare Rust, come scrivere un programma che dice "Hello, world!", e come usare Cargo, il gestore di pacchetti e strumento di build di Rust. Il capitolo 2 mette le mani sull'introduzione a scrivere un programma in Rust, e ti farà costruire un giochino per indovinare numeri. Copre i concetti fondamentali in un alto livello, e nei capitoli successivi verranno spiegati dettagli aggiuntivi. Se vuoi sporcarti le mani da subito, il capitolo 2  è il posto per quello. Il capitolo 3 copre le funzioni di Rust che sono simili a quelle di altri linguaggi di programmazione, e nel capitolo 4 imparerai riguardo al sistema di proprietà di Rust ("ownership system"). Se sei un apprenditore particolarmente meticoloso che preferisce imparare tutti i dettagli prima di muoversi avanti, probabilmente vorrai andare direttamente al capitolo 3 e poi tornare al capitolo 2 quando vorrai lavorare su un progetto per applicare cosa hai imparato.

Il capitolo 5 parla degli structs e dei metodi, e il capitolo 6 copre gli enums, le espressioni `match`, e il gestore di flussi `if let`. Imparerai a usare gli struct e gli enums per creare tipi personalizzati in Rust.

Il capitolo 7, imparerai riguardo al sistema di moduli di Rust e riguardo alle regole sulla privacy per organizzare il tuo codice e la sua *Application Programming Interface* (API). Il capitolo 8 discute su alcune comuni strutture dati di raccolta che la libreria standard ti fornisce, come vettori, stringhe e mappe hash. Il capitolo 9 esplora le tecniche e la filosofia della gestione degli errori in Rust.

Il capitolo 10 entra in generics, traits e lifetimes, che ti danno la possibilita di definire del codice che si applica a tipi multipli. Il capitolo 11 è tutto riguardo al testing, che anche con le garanzie della sicurezza di Rust, è necessario per garantire una corretta logica di funzionamento. Nel capitolo 12, costruiremo la nostra implementazione di un subset di funzioni dallo strumento CLI `grep` per cercare all'interno di files. Per questo useremo molti concetti discussi nei capitoli precedenti.

Il capitolo 13 esplora closures e iterators: funzioni di Rust che arrivano dai linguaggi di programmazione funzionali. Nel capitolo 14, esamineremo Cargo più in profondità e parleremo riguardo le migliori pratiche per condividere le tue librerie con gli altri.
Il capitolo 15 discute dei puntatori intelligenti che la libreria standard offre e dei tratti che abilitano la sua funzionalità.

Nel capitolo 16 cammineremo attraverso differenti modelli di programmazione concorrente e parleremo riguardo al come Rust ti aiuta per programmare su molteplici thread senza paura. Nel capitolo 17, costruiremo su ciò esplorando la sintassi async/await di Rust e la leggerezza della concorrenza che loro supportano.

Nel capitolo 18 guarderemo a come comparare gli idiomi di Rust a quelli di linguaggi di programmazione ad oggetti a cui potresti essere familiare.

Il capitolo 19 è una referenza alle patterns e al pattern matching, che sono strumenti potenti di esprimere idee tramite programmi in Rust. Il capitolo 20 contiene un buffet di argomenti avanzati di interesse, incluso l'unsafe, le macros, qualcosa in aggiunta a lifetime, traits, types, function e closures.

Nel capitolo 21 completeremo un progetto dove implementeremo un server web multithread di basso livello!

Finalmente, alcune appendici contengono informazioni riguardo il linguaggio in un formato referenziale. L'appendice A copre le keywords, l'appendice b copre gli operatori e i simboli, l'appendice C copre i tratti derivabili dati dalla libreria standard, l'appendice D copre alcuni strumenti utili di sviluppo, l'appendice E spiega le edizioni di Rust, nell'appendice F potrai trovare altre traduzioni del libro, e nell'appendice G copriremo come Rust è fatto e cosa è Rust nightly.

Non c'è un modo sbagliato per leggere questo libro: se vuoi saltare avanti fallo! Probabilmente dovrai tornare indietro se farai confusione. Ma fai qualsiasi cosa funzioni per te.

<span id="ferris"></span>

Un importante parte del processo di apprendimento di Rust è imparare come leggere i messaggi di errore del compilatore: questo ti guiderà verso il lavorare con il codice. Ad esempio, potremmo darti molti esempi che non compilano assieme all'errore che il compilatore ti mostrerà in ciascuna situazione. Sappi che se prendi ed avvii un esempio a caso potrebbe non funzionare! Assicurati di leggere il testo attorno per vedere se l'esempio che stai provando ad avviare è fatto apposta per non funzionare. Ferris ti aiuterà a distinguere il codice che non è fatto per funzionare:

| Ferris                                                                                                      | Meaning                                         |
| ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------- |
| <img src="img/ferris/does_not_compile.svg" class="ferris-explain" alt="Ferris con un punto interrogativo"/> | Questo codice non funziona!                     |
| <img src="img/ferris/panics.svg" class="ferris-explain" alt="Ferris muovendo le mani"/>                     | Questo codice va in panico!                     |
| <img src="img/ferris/not_desired_behavior.svg" class="ferris-explain" alt="Ferris che muove una mano"/>     | Questo codice non produce l'effetto desiderato. |

In molte situazioni, ti guideremo attraverso la correzione del codice che non si compila.

## Codice Sorgente

Il codice sorgente può essere trovato su [GitHub][book].

[book]: https://github.com/killerbossoriginal/rust-book/tree/main/src
