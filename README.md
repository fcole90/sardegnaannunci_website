# SardegnaAnnunci - sviluppo sito web

## Definizione dei requisiti e delle specifiche

Deve essere possibile:

- login ed autenticazione degli utenti
- inserire e cercare annunci (stile Subito.it) con divisioni in categorie;
- inserire rubriche o articoli (solo admins), quindi parte blog;
- visualizzare e scaricare il pdf della rivista.

*La definizione è temporanea, possono nascere ulteriori necessità.*

## Gestione Utenti

Requisiti:

- database

Suddivisi in:

| Utente | diritti |
|-------:|---------|
| utente base | può creare ed eliminare i propri annunci |
| utente scrittore | oltre ai diritti di base può scrivere e cancellare articoli |
| utente moderatore | oltre ai diritti di base può moderare annunci di altri utenti |
| admin | tutti i diritti |

**NB:** Se un moderatore nasconde l'annuncio di un altro moderatore, quest'ultimo non deve poter annullare l'azione del primo.


### Gestione annunci

Requisiti:

- database
- motore per le ricerche
- moderazione
- condivisione con i principali social network e via email
- galleria immagini
- possibilità di fare domande su un articolo in vendita (Amazon docet)

### Gestione rubriche

Semplice parte blog, possibilmente divisa in categorie *da definire*.

- database
- divisione categorie
- ricerca su keyword
- condivisione automatica sui principali social network

### Gestione file PDF

Potrebbe essere sviluppato come variante di una delle categorie del blog, in modo da limitare ulteriore lavoro.

Ogni upload dovrebbe avere associata l'immagine di copertina e un breve riassunto stile "*In questo numero...*".


## Scelta dell'ambiente operativo e degli strumenti di sviluppo

- Webserver: Apache, standard de facto;
- Linguaggio Backend: PHP, standard e presenta svariate librerie oppure Python, meno supportato ma ottimo linguaggio.
- DB relazionale: MariaDB, MySQL, PostgreSQL. Salvo esigenze specifiche, MySQL è già presente in quasi tutti i servizi di hosting.
- Framework UI: *Da definire*, deve essere responsive ed adattarsi alle interfacce per dispositivi mobili. 
- Framework Backend: *Da definire*, deve essere ampiamente diffuso ma semplice ed adatto alle esigenze (forse YII per PHP o Django per Python).

### Hosting

Attualmente disponibile hosting presso **godaddy**. Si può valutare un upgrade o sostituzione se le circostanze lo richiedano.

## Consegna

**Settembre 2015**




 
