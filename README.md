# progetto_LTW_LB_AL

progetto per linguaggi e tecnologie per il web
università La Sapienza ,facoltà Ingegneria Informatica e Automatica trallalla

Breve guida a Xampp

XAMPP è una combinazione di software liberi. Il nome è un acronimo che deriva dalle lettere iniziali dei componenti principali. Il pacchetto di software comprende il web server Apache, il sistema di gestione del database relazionale MySQL o MariaDB (compatibile 100% con MySQL) e i linguaggi di scripting Perl e PHP. La X iniziale sta ad indicare i sistemi operativi Linux, Windows e Mac OS X.
    • Apache: il web server open source Apache è l’applicazione globale più diffusa per la consegna di contenuti web. L’applicazione server è messa a disposizione come software libero da Apache Software Foundation.
    • MySQL/MariaDB: XAMPP comprende uno dei database relazionali più conosciuti al mondo, ovvero MySQL. In combinazione con il web server Apache e il linguaggio di scripting PHP, MySQL serve per la memorizzazione dei dati per i servizi web. Nelle versioni più recenti di XAMPP, MySQL è stato sostituito da MariaDB, nato dalla scissione (“Fork”) dal progetto MySQL.
    • PHP: PHP è un linguaggio di scripting lato server che consente di creare pagine dinamiche o applicazioni. Si può utilizzare su tutte le piattaforme e supporta diversi sistemi di database.
    • Perl: il linguaggio di scripting Perl è usato per l’amministrazione del sistema, lo sviluppo web e la programmazione di rete. Inoltre si possono programmare così applicazioni web dinamiche simili a quelle scritte in PHP.

Un server XAMPP si può installare su Linux, Windows e Mac OS X con un file eseguibile facilmente e velocemente in un sistema di test locale. Il pacchetto di software contiene gli stessi componenti utilizzati sui web server comuni. Gli sviluppatori hanno così la possibilità di testare i progetti in locale e di trasferirli poi comodamente sui server esterni effettivi. 
XAMPP è stato messo a disposizione dal progetto no-profit Apache Friends. Le versioni con PHP 5.5, 5.6 o 7 sono scaricabili gratuitamente all’indirizzo www.apachefriends.org/it/download.html. 
Alla voce “Select Components” avete la possibilità di escludere dall’installazione singole componenti dal pacchetto dei software di XAMPP. Per creare un server di test locale si consiglia di lasciare le impostazioni standard, con cui vengono installate tutte le componenti disponibili. 
Importante: i siti web/applicazioni web vanno posti nella cartella xampp/htdocs
Ecco lo schema di funzionamento di Xampp per un sito web dinamico, ovvero quelle applicazioni web che interagiscono attivamente con l'utente, modificando le informazioni mostrate, in base alle informazioni da esso ricevute e che consentono anche un più rapido aggiornamento del sito web da parte dell'amministratore.


La gestione dei singoli componenti del server di test è possibile dal pannello di controllo di XAMPP. L’interfaccia utente registra tutte le azioni e consente di avviare o bloccare i singoli moduli con un click. Nel pannello di controllo di XAMPP sono disponibili diversi pulsanti:
    • Config: permette la configurazione di XAMPP e dei suoi singoli componenti
    • Netstat: indica tutti i processi in esecuzione sul computer locale
    • Shell: apre la shell di UNIX
    • Explorer: apre la cartella di XAMPP su Windows
    • Services: mostra tutti i servizi in esecuzione in background
    • Help: offre link a forum di aiuto
    • Quit: chiude il pannello di controllo di XAMPP
I singoli moduli di XAMPP vengono avviati grazie ai rispettivi pulsanti “Start”. I moduli avviati compaiono in verde nel pannello di controllo. 
Amministrare i moduli
Per ogni modulo di XAMPP nel pannello di controllo è a disposizione il tasto “admin”.
    • Cliccate sul pulsante admin del server Apache per arrivare all’indirizzo del vostro web server. Il pannello di controllo avvia in questo caso il vostro browser standard e venite inoltrati alla dashboard del localhost di XAMPP.  Alternativamente, aprite la dashboard seguendo il percorso localhost/dashboard/.
 Cliccando sul pulsante “admin” del modulo Apache, l’utente viene reindirizzato alla dashboard locale di XAMPP 
    • Utilizzate il pulsante admin del vostro modulo database per aprire phpMyAdmin. Qui gestite i database dei diversi progetti, che volete testare sul vostro XAMPP. In alternativa raggiungete l’interfaccia di amministrazione per il database MySQL andando su localhost/phpmyadmin/.
 L’utente gestisce i database del progetto in phpMyAdmin (raggiungibile dal pulsante “admin“ sul modulo database) 
Verificare l’installazione di XAMPP
Per essere certi che il server di test sia stato installato e configurato correttamente, è possibile creare una pagina di test PHP, caricarla sul localhost del vostro XAMPP e aprirla tramite browser.
    • Aprite la cartella XAMPP dal pulsante “Explorer” nel pannello di controllo e scegliete la cartella htdocs (C:\xampp\htdocs nell’installazione standard). In questa cartella vengono creati tutti i file per il sito che volete testare con XAMPP. La cartella htdocs comprende già i file utili alla configurazione del web server. Per alcuni progetti è necessario perciò creare una nuova cartella (ad esempio test).
    • Ora create una semplice pagina PHP nell’editor con il seguente contenuto e caricatelo nella cartella test con il nome test.php (C:\xampp\htdocs\test):
<html>
 <head>
  <title>Test PHP</title>
 </head>
 <body>
  <?php echo '<p>Hello World </p>'; ?>
 </body>
</html>
    • Nell’ultimo passaggio aprire il browser e richiamate la vostra pagina PHP all’indirizzo localhost/test/test.php. Se nella finestra del browser compaiono le parole “Hello World”, il vostro XAMPP è installato e configurato correttamente.
