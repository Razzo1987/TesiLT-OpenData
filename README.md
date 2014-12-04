TesiLT-OpenData
===============

Gli <b>Open Data</b> sono sia una pratica che un ideologia e in questi ultimi anni, grazie ad
internet, si stanno diffondendo sempre più. Secondo wikipedia per Open Data si intendono
*"alcune tipologie di dati liberamente accessibili a tutti, privi di brevetti o altre forme di
controllo che ne limitino la riproduzione e le cui restrizioni di copyright eventualmente si
limitano ad obbligare di citare la fonte o al rilascio delle modifiche allo stesso modo"*.
Open Data di per śe non vuol dire* e-participation* (partecipazione in processi di governo e di governance) o e-democracy, ma insieme ad essi costituisce i pilastri dell’Open
Government, l’idea in base alla quale la pubblica amministrazione deve essere aperta ai
cittadini in termini di trasparenza, di collaborazione e di partecipazione diretta al processo
decisionale.
I dati dono messi a disposizione dalla Pubblica Amministrazione in sola lettura agli
utenti, che possono essere suddivisi in 5 macro-categorie in base alle loro esigenze: Cittadini (trasparenza della PA o semplice informazione), Civil Hackers (volontari che sviluppano
applicazioni "utili"), Giornalisti (cercando dati specifichi per fare inchieste), Imprese (analisi di mercato o nuovo software) e la stessa Pubblica Amministrazione (migliorare le scelte
decisionali).
Nel 2007 sono inoltre stati definiti gli <b>8 principi dell’Open Governament Data</b> che
definiscono i prerequisiti che devono avere i dati del governo per considerarsi aperti quando
vengono resi pubblici. Questi principi, insieme al concetto di <b>dati a 5 stelle</b>, introdotto
da Tim Berners Lee nel 2006, hanno fatto da faro per guidare il processo di affermazione
degli Open Data.

A livello governativo il percorso è stato lungo, e ha coinvolto molti soggetti, a partire
dal presidente degli Stati Uniti d’America Barack <b>Obama</b> con una direttiva del 2009, fino
ad arrivare ad un importante passo nella legislazione Italiana che nel marzo 2013 ha definito che tutti i dati e documenti che le pubbliche amministrazioni pubblicano con qualsiasi
modalità, senza l’espressa adozione di una licenza d'uso, si intendono rilasciati come dati
aperti (<b>Open Data by default</b>). A livello regionale invece la situazione risulta ancora
frammentata: sono presenti regioni che hanno già approvato direttive in ambito Open Data, altre in cui l’iter burocrativo non si è ancora concluso e, purtroppo, alcune in cui non
ci si è ancora attivati in merito.

Il <b>Comune di Vigevano</b> il 23 maggio 2013 ha deliberato l’Adesione alle "Linee guida Open Data per gli enti locali", di Regione Lombardia e sperimentazione congiunta in
materia. Ciò ha permesso lo svolgimento dello stage presso il Laboratorio MiSS del Dipartimento di Informatica Sistemistica e Comunicazione (DISCo). l progetto prevedeva la
creazione di una demo di un portale Open Data seguendo le direttive richieste dal Comune
stesso.
Sono quindi state affrontate alcune soluzioni tecnologiche, cercando di comprendere la
loro architettura e si sono analizzate le caratteristiche da esse offerte:
• Socrata, una piattaforma sviluppata dall’omonimia società con sede negli Stati Uniti
d’America ha da poco annunciato il rilascio di una Community Edition con una
licenza Open Source, alcune sue parti sono già state rese disponibili e ne viene spiegato
il funzionamento.
• CKAN, invece, è da sempre stato Open Source e il suo codice è mantenuto dalla
Open Knowledge Foundation. Esso è utilizzato da diversi enti per gestire cataloghi
pubblici.
Le esigenze del Comune di Vigevano prevedono un integrazione a monte con la piattaforma GIT, implementata al fine di integrare, relazionare e rendere interoperabili i dati
in possesso dell’ente incaricato della gestione del territorio di competenza. GIT costituisce
la dorsale sulla quale i dati possono transitare al fine di acquisire un maggior livello di
accuratezza, attendibilità e completezza.
Vigevano necessita inoltre di un integrazione a valle con il portale dati.lombardia.it
sviluppato da Regione Lombardia, il quale vuole porsi l’obiettivo di raccogliere i dataset
contenenti i dati individuati come riutilizzabili dalle Pubbliche Amministrazioni interessate.
Ultima, ma non meno importante, richiesta è la presenza di un catalogo dei dataset pubblicati connettete anche i metadati al fine di agevolare l’integrazione tra la piattaforma
e applicazioni di terze parti. Il catalogo dovrà quindi essere realizzato in modo che per
ogni dataset sia anche possibile sapere immediatamente le intestazioni delle colonne in esso
contenuti.
La progettazione ha seguito le esigenze elencate e ha affrontato i problemi di sicurezza
e integrazione di GIT con il portale Open Data che verrà realizzato, è infatti possibile
permettere alla piattaforma di accedere direttamente ai dati di GIT oppure effettuare delle
esportazioni dei dati da GIT per caricarle sulla piattaforma in modo manuale o automatizzato.
Successivamente si è realizzata la piattaforma di demo, installando CKAN su macchina
virtuale e abilitando i componenti aggiuntivi che permettono la preview dei file, l’utilizzo
delle Web API, l’archiviazione dei file sul server e l’analisi automatica dei file caricati.
Infine si sono realizzate alcune delle funzionalità richieste per il catalogo. Si è riusciti
a creare il catalogo e salvarlo sul server in modo che sia facilmente accessibile, ma non a
collegare i metadati contenuti nei singoli dataset. Ciò è stato possibile attraverso la creazione di in trigger su una tabella del database di CKAN. Questa scelta è stata fatta al fine
di essere riutilizzabile anche in caso di aggiornamento di CKAN a una versione successiva.
Le conclusioni tratte dall’esperienza di questi mesi con la piattaforma CKAN evidenziano le problematiche di configurazione della piattaforma, e la necessità di una buona dose
di tempo ed energie per mantenere la piattaforma aggiornata. Si evincono quindi delle
forti criticità sulla scelta di questa piattaforma per la realizzazione del portale Open Data
voluto dal Comune di Vigevano.
