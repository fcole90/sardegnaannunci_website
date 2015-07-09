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

Un utente si può iscrivere solo come utente base, solo l'admin può conferire maggiori diritti.
I diritti potrebbero essere gestiti tramite flags.

**NB:** Se un moderatore nasconde l'annuncio di un altro moderatore, quest'ultimo non deve poter annullare l'azione del primo.


### Gestione annunci

Requisiti:

- database
- motore per le ricerche
- moderazione
- condivisione con i principali social network e via email
- galleria immagini
- possibilità di fare domande su un articolo in vendita (Amazon docet)
- acquisto annunci speciali
- pubblicità

### Acquisto annunci

Bisogna aggiungere la possibilità di aggiungere annunci premium, a pagamento,
e definire che privilegi abbiano (es. maggior numero di foto, miglior posizionamento)
e prevedere un metodo di pagamento.

- gestione metodo pagamento
- organizzazione speciale annunci
- privilegi utenti a pagamento

### Gestione Pagamenti

Pagamenti PayPal, se necessario anche tramite Carta di Credito, da valutare in base
alle esigenze delle persone della zona ed alla possibilità di pagare tramite PayPal
senza registrazione.

### Posizionamento pubblicitario

Sono già in nostro possesso diverse pubblicità che devono apparire sulla rivista.
Probabilmente la grafica sarà da rifare perché sono molto in stile web 1.1 (gif animate).
Anche gli spazi pubblicitari devono poter essere acquistati online.

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
- Linguaggio Backend: PHP, standard e presenta svariate librerie..
- DB relazionale: MariaDB, MySQL, PostgreSQL. Salvo esigenze specifiche, MySQL è già presente in quasi tutti i servizi di hosting.
- Framework UI: [Semantic UI](http://semantic-ui.com/), [Bootstrap](http://getbootstrap.com/2.3.2/).
- Framework Backend: Lavarel 5.1 oppure YII 2.

### Hosting

Attualmente disponibile hosting presso **godaddy**. Si può valutare un upgrade o sostituzione se le circostanze lo richiedano.

## Consegna

**Settembre 2015**

## Mother.say() ? multilang : monolang;

## Link utili per mantenere alta la qualità del codice
[Scrivere JS di qualità (per quanto possibile).](http://code.tutsplus.com/tutorials/the-essentials-of-writing-high-quality-javascript--net-15145)

#ToDo
Devono apparire dei banner pubblicitari, dove metterli?


 
