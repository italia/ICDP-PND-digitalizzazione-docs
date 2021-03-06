Metadati tecnici
=================

I metadati tecnici possono essere interni o esterni al file della
risorsa digitale. Quelli “interni” sono informazioni descrittive
generate dall’applicativo o dallo strumento che produce il file, e sono
memorizzati all’interno del file (per esempio, i file testuali generati
da un programma di videoscrittura o i file immagine prodotti da una
fotocamera o da uno scanner sono corredati da metadati tecnici interni).
Quelli “esterni” sono codificati in un file separato che accompagna il
file originale e vengono anche definiti “file *sidecar* ” (per esempio,
i file XMP che accompagnano le diverse tipologie di file RAW prodotti
dalle fotocamere). Generalmente, i file *sidecar* vengono scritti da
applicazioni di post-produzione durante la modifica del file originale.
Talvolta, come per i metadati tecnici interni, anche il set dei metadati
descrittivi può essere rappresentato all’esterno del file.

Exif
----

I metadati Exif (*Exchangeable Image file format*) [39]_ descrivono i
parametri tecnici utilizzati al momento dell’acquisizione dell’immagine,
ovvero della scansione o dello scatto fotografico. Le informazioni
registrate nei metadati Exif possono riguardare:

-  specifiche dell’hardware usato per creare l’immagine (per esempio,
   modello di fotocamera, ottiche, flash e altra apparecchiatura, con i
   loro parametri di scatto);

-  data, ora ed eventuale posizione geografica della creazione;

-  nome o altre caratteristiche dell’autore;

-  eventuali licenze d’uso dell’immagine (*Copyright*©, *Creative
   Commons*, ecc.);

-  informazioni colorimetriche (spazio-colore, punto di bianco, profilo
   ICC, ecc.);

-  eventuale proiezione piana di uno spazio curvo (per esempio,
   equi-rettangolare, altrimenti detta “latitudine/longitudine” o, più
   impropriamente, “360°”).

IPTC
----

I metadati IPTC (*Information Interchange Model*) [40]_, conosciuti anche
come IPTC-NAA-Standard, sono una struttura dati che può essere applicata
a file immagine, video e ad alcuni formati audio. In generale sono
metadati interni, ma possono essere anche rappresentati come metadati
esterni in formato JSON [41]_ e YAML [42]_. Vengono compilati laddove sia
necessario garantire un livello minimo di descrizione degli oggetti
digitali. Le regole di compilazione e la mappatura vanno descritte nel
documento di progettazione.

BWF
---

I metadati BWF (*Broadcast Wave Format*), standardizzati dalla *European
Broadcasting Union* (EBU) [43]_, si usano per i file audio in formato
WAVE. Questi consentono la memorizzazione di un numero limitato di dati
descrittivi all'interno del file WAVE. Questa scelta permette la
conservazione del collegamento tra metadati e audio digitale. Tuttavia,
nel caso contrario – metadati e contenuti separati dal file digitale –
occorre fare ricorso all’utilizzo dello standard METS.

XMP
---

Il formato XMP (*eXtensible Metadata Platform*), creato da Adobe e
successivamente standardizzato nella norma ISO 16684-1:2012 [44]_, è una
descrizione del processo di modifica del file per la codifica di
informazioni significative su un progetto (titoli e descrizioni, parole
chiave ricercabili e informazioni aggiornate sull'autore e sul
*copyright*, e tutte le informazioni sulle azioni di modifica avvenute
sul file).

I metadati XMP possono essere interni ed esterni al file. Vengono
codificati all’interno del file, come nel caso dei file .pdf o .jpg, o
scritti esternamente in file separati, come nel caso in cui occorra
descrivere file RAW acquisiti da una fotocamera o scanner.

All’interno del METS, sezione <amdSec>, gli standard adottati per la
descrizione di tali caratteristiche tecniche sono:

-  NISO-MIX (NISO *Metadata for Images* in XML schema - *Still
   images*) [45]_ per le immagini;

-  AUDIO-MD e VIDEO-MD [46]_ per la codifica dei metadati tecnici dei
   documenti sonori e audiovisivi.

.. [39] Exif è stato creato dalla Japan Electronic Industries Development
   Association (JEIDA). La versione 2.1 è datata 12 giugno 1998, la
   versione 2.2 è dell'aprile 2002 ed è anche conosciuta come Exif
   Print. Attualmente Exif non è supportata da aziende od organizzazioni
   che seguono gli standard, tuttavia è il formato utilizzato da tutti i
   produttori di fotocamere.

.. [40] https://iptc.org/

.. [41] https://iptc.org/std/photometadata/specification/iptc-pmd-techreference_2019.1.json

.. [42] https://iptc.org/std/photometadata/specification/iptc-pmd-techreference_2019.1.yml

.. [43] https://www.loc.gov/preservation/digital/formats/fdd/fdd000356.shtml

.. [44] https://www.iso.org/standard/57421.html

.. [45] https://www.loc.gov/standards/mix/

.. [46] https://www.loc.gov/standards/amdvmd/
