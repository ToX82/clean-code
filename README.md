# Clean coding

### Regole generali
* Il codice scritto con uno stile di scrittura predefinito e uniforme è più facile da capire e modificare, il che significa meno tempo speso sulla manutenzione.
* Il codice deve essere facile da capire anche per le persone e non solo per le macchine.
* Il codice deve essere organizzato in modo che chiunque lo legga possa seguire facilmente il flusso delle informazioni e delle attività.
* Il codice deve essere scritto seguendo principi di programmazione estetici e ben strutturati, in modo che sia facile da leggere e comprendere.

### Ricorda
* Don't repeat yourself (DRY): Il codice non dovrebbe essere ripetitivo, ma dovrebbe essere organizzato in modo da essere riutilizzabile.
* Keep It Simple, Stupid (KISS): Il codice dovrebbe essere semplice e facile da comprendere, evitando la complessità inutile.
* You Aren't Gonna Need It (YAGNI): Dovresti evitare di implementare funzionalità che potrebbero essere necessarie in futuro ma che al momento non sono necessarie.
* Tieni a mente i principi SOLID quando progetti una classe / funzione:
   * Single Responsibility Principle: Ogni funzione dovrebbe avere una sola responsabilità e quindi un solo motivo per cambiare.
   * Open/Closed Principle: Le funzioni dovrebbero essere aperte per l'estensione ma chiuse per la modifica, il che significa che è possibile estendere le funzionalità senza dover modificare il codice esistente.
   * Liskov Substitution Principle: Le sottofunzioni dovrebbero essere utilizzabili al posto delle superfunzioni senza causare problemi.
   * Interface Segregation Principle: Usa funzioni più piccole e specifiche per rendere il codice più facile da capire e mantenere. Una classe non dovrebbe incorporare metodi non necessari al proprio funzionamento
   * Dependency Inversion Principle: Le dipendenze dovrebbero essere gestite invertendo la dipendenza dalle funzioni concrete a quelle astratte, il che significa che il codice dovrebbe dipendere dalle interfacce astratte e non dalle implementazioni concrete.
