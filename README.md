# Clean coding (la teoria della teoria)

### Regole generali
* Il codice scritto con uno stile di predefinito e uniforme è più facile da capire e modificare, il che significa meno tempo speso sulla manutenzione, soprattutto quando è necessario tornarci sopra dopo molto tempo.
* Il codice deve essere facile da capire anche per le persone e non solo per le macchine.
* Il codice deve essere organizzato in modo che chiunque lo legga possa seguire facilmente il flusso delle informazioni e delle attività.
* Il codice deve essere scritto seguendo principi di programmazione estetici e ben strutturati, in modo che sia facile da leggere e comprendere.
* Se un'istruzione è complicata, aggiungi un commento che ne spiega il funzionamento

### I princìpi sono prìncipi
* _Don't repeat yourself (`DRY`)_: Il codice non dovrebbe essere duplicato, ma dovrebbe essere organizzato in modo da essere riutilizzabile.
* _Keep It Simple, Stupid (`KISS`)_: Il codice dovrebbe essere semplice e facile da comprendere, evitando complessità inutili.
* _You Aren't Gonna Need It (`YAGNI`)_: Dovresti evitare di implementare funzionalità che potrebbero essere necessarie in futuro ma che al momento non sono necessarie.
* Tieni a mente i principi _`SOLID`_ quando progetti una classe o un metodo (per quanto possibile):
   * _Single Responsibility Principle_: Ogni funzione dovrebbe avere una sola responsabilità e quindi un solo motivo per cambiare.
   * _Open/Closed Principle_: Le funzioni dovrebbero essere aperte per l'estensione ma chiuse per la modifica, il che significa che è possibile estendere le funzionalità senza dover modificare il codice esistente.
   * _Liskov Substitution Principle_: Le sottofunzioni dovrebbero essere utilizzabili al posto delle superfunzioni senza causare problemi.
   * _Interface Segregation Principle_: Usa funzioni più piccole e specifiche per rendere il codice più facile da capire e mantenere. Una classe non dovrebbe incorporare metodi non necessari al proprio funzionamento
   * _Dependency Inversion Principle_: Le dipendenze dovrebbero essere gestite spostando la dipendenza dalle funzioni concrete a quelle astratte: il codice dovrebbe dipendere dalle interfacce astratte e non dalle implementazioni concrete.

# Gli strumenti (la pratica della teoria)
### Fatti aiutare dai linter
Ricordarsi tutte le regole a memoria è complicato. Fortunatamente gli editor di codice moderni offrono la possibilità di usare degli strumenti (o `linter`) che analizzano il codice sorgente ed evidenziano errori di programmazione, bug, errori stilistici e costrutti sospetti. Usali. In questo repository sono presenti alcuni linter che uso normalmente, con le regole che seguo nei miei progetti. Sentiti libero di prenderli, usarli, aggiornarli e di mandarmi delle migliorie, se lo ritieni.

### Automatizza i controlli e, quando possibile, le soluzioni
Oltre ai linter, che evidenziano i problemi, ci sono delle utilities che possono effettuare una correzione automatica, quando possibile. Alcuni esempi:

#### PHP
* Questo comando evidenzia tutti gli errori riscontrati da `phpcs` a riga di comando, nelle directory src e templates.

`phpcs --colors -p  ./src/* ./templates/*`
* Questo comando prova a correggerli

`phpcbf ./src ./templates`

#### JAVASCRIPT
* Questo comando evidenzia tutti gli errori riscontrati da `eslint` a riga di comando

`eslint webroot/js/custom.js`
* Questo comando prova a correggerli

`eslint webroot/js/custom.js --fix`

#### CSS
* Questo comando evidenzia tutti gli errori riscontrati da `stylelint` a riga di comando

`stylelint "./webroot/css/custom.css"`
* Questo comando prova a correggerli

`stylelint "./webroot/css/custom.css" --fix`
