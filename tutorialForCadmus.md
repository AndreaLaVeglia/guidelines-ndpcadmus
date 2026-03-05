# Guida pratica all'utilizzo di Cadmus

>a cura di Andrea La Veglia (per chiarimenti: [alaveglia@unisa.it](mailto:alaveglia@unisa.it))

INDICE
- [1 Aggiunta di item](#1-aggiunta-di-un-item)
- [2 Aggiunta di part](#2-aggiunta-delle-parts)

Cadmus è un framework di descrizione modulare, nel senso che offre la possibilità di strutturare le informazioni in moduli componibili. In particolare l'architettura di Cadmus è costituita da **_items_** e da **_parts_**.  


## 1. Aggiunta di un _item_

L'_item_ è come una scatola che contiene al suo interno elementi correlati tra loro e riferiti al contenitore che sono le _parts_.  
L'_item_ corrisponde ad un  manoscritto/unità codicologica, un disegno, un'edizione, un testo a stampa, un item iconografico o di una persona. La descrizione analitica dell'_item_ si articolerà tramite l'inserimento di diverse _parts_ (Cf. [Documentazione online di Cadmus](https://myrmex.github.io/overview/cadmus/dev/models/)). 

Il primo passaggio per il catalogatore è dunque la creazione di un nuovo _item_, andando sul bottone in basso a sinistra nella visualizzazione dell'editor di Cadmus_NDP.

![aggiunta item](./additem.png)<figcaption>Aggiunta di un item in Cadmus.</figcaption>

### Metadati identificativi (identity)

Per la creazione di un nuovo _item_ bisogna inserire i seguenti metadati obbligatori che costituiscono l'etichetta (_**label**_) dell'_item_: 
- `title` = indica il titolo rappresentativo dell'item. A seconda del tipo di item si seguiranno queste convenzioni stabilite
  - **manoscritto**: Città secondo la lingua del catalogo, abbreviazione della biblioteca, secondo le [abbreviazioni di cui alla tabella in appendice](#abbreviazioni-biblioteche), segnatura.
- `description` 
- `facet`provvede ad indicare la tipologia di item, specificando dunque se si tratti di manoscritti, disegni o stampe, oppure di un item iconografico o di una persona.



### Flags

I flags sono le "bandierine" che segnalano lo stato editoriale della catalogazione dell'oggetto di riferimento (ms, frg, ...) in Cadmus.

> NB Dal momento della creazione dell'item bibliologico fino al suo completamento, per segnalare agli altri contributori che è ancora in lavorazione, bisogna selezionare lo stato di `draft`. 
Dopo il completamento della scheda si potrà selezionare `complete` e togliere la spunta a `draft`.

## 2. Aggiunta delle _parts_

Dopo aver creato l'_item_, ossia la "scatola" che rappresenta l'oggetto che si sta catalogando, si può procedere all'aggiunta delle parti di Cadmus utili a descrivere l'oggetto in questione.  

L' elemento _part_ è un **set di dati** coerente che si riferisce all'item al quale viene correlato (Cf. [Documentazione di Cadmus](https://cadmus.fusi-soft.com/docs/data-architecture)).  
Si veda di seguito lo screenshot di esempio per l'aggiunta di una parte. 

![Aggiunta di Part](addpart.png)<figcaption>Aggiunta di una part in Cadmus.</figcaption>

In Cadmus per ogni tipologia di oggetto è stato predisposto un modello descrittivo/interpretativo che suggerisce l'utilizzo di specifiche parts.

Si riportano di seguito gli schemi di catalogazione da seguire per:
- [manoscritti](#manuscript), 
- [frammenti](#fragment)
- [edizioni di testi a stampa (edizione "ideale")](#print-edition)
- [esemplare di testo a stampa](#print-instance)
- [progetto dei disegni](#drawings-project)
- [disegno](#drawing-item)
- [iconografia](#iconography)
- [persona](#person)

### **manuscript**

  - _identity_
    - [metadata](#metadata)
    - [shelfmarks](#shelfmarks)
    - [links](#links)
    - [categories](#categories)  
  - _history_
    - [chronotopes](#chronotopes)
    - [historical events](#historical-events)
    - [note](#note)
  - _material_
    - [bindings](#bindings)
    - [sheet labels](#sheet-labels)
    - [material description](#material-description) 
    - [watermarks](#watermarks)
    - [preservation states](#preservation-states)
  - _content_
    - [contents](#contents)
    - [layouts](#layouts)
    - [decorations](#decorations)
    - [iconography instructions](#iconography-instructions) 
    - [hands](#hands)
    - [edits](#edits)
    - [notable word forms](#notable-word-forms) 
  - _editorial_
    - [note](#note)
  - _references_
    - [references](#references) (mostly used for Zotero bibliography)

### **fragment**

  - _identity_
    - [metadata](#metadata)
    - [shelfmarks](#shelfmarks)
    - [links](#links)
    - [categories](#categories)  
  - _history_
    - [chronotopes](#chronotopes)
    - [historical events](#historical-events)
    - [note](#note)
  - _material_
    - [support](#support)
    - [rulings](#rulings)
    - [labels](#labels)
    - [decorated counts](#decorated-counts)
    - [measurements](#measurements)
    - [preservation states](#preservation-states)
  - _content_
    - [contents](#contents)
    - [layout](#layout)
    - [decorations](#decorations)
    - [iconography instructions](#iconography-instructions)
    - [hands](#hands)
    - [edits](#edits)
    - [notable word forms](#notable-word-forms)
  - _editorial_
    - [note](#note)
  - _references_
    - [references](#references)

### **print edition**

  - _identity_
    - [metadata](#metadata)
    - [links](#links)
    - [categories](#categories)  
  - _history_
    - [chronotopes](#chronotopes)
  - _content_
    - [fonts](#fonts)
    - [layouts](#layouts)
    - [watermarks](#watermarks)
    - [figurative plan](#figurative-plan)
    - [note](#note)
  - _editorial_
    - [note](#note)
  - _references_
    - [references](#references)

### **print instance**

  - _identity_
    - [metadata](#metadata)
    - [links](#links)
    - [shelfmarks](#shelfmarks)
    - [categories](#categories)  
  - _history_
    - [historical events](#historical-events)
    - [note](#note)
  - _material_
    - [bindings](#bindings)
    - [sheet labels](#sheet-labels)
    - [measurements](#measurements)
    - [preservation states](#preservation-states)
  - _content_
    - [layouts](#layouts)
    - [figurative plan implementation](#figurative-plan-implementation)
    - [decorations](#decorations)
    - [edits](#edits)
    - [notable word forms](#notable-word-forms)
  - _editorial_
    - [note](#note)
  - _references_
    - [references](#references)

### **drawings project**

  - _identity_
    - [metadata](#metadata)
    - [links](#links)
    - [shelfmarks](#shelfmarks)
  - _history_
    - [chronotopes](#chronotopes)
    - [historical events](#historical-events)
    - [note](#note)
  - _material_
    - [bindings](#bindings)
    - [preservation states](#preservation-states)
    - [decorated counts](#decorated-counts)
  - _content_
    - [comment](#comment)
  - _editorial_
    - [note](#note)
  - _references_
    - [references](#references)

### **drawing item**

  - _identity_
    - [metadata](#metadata)
    - [links](#links)
    - [shelfmarks](#shelfmarks)
  - _history_
    - [chronotopes](#chronotopes)
    - [historical events](#historical-events)
    - [note](#note)
  - _material_
    - [drawing tech](#drawing-tech)
    - [watermarks](#watermarks)
    - [preservation states](#preservation-states)
  - _content_
    - [flags](#flags)
    - [edits](#edits)
    - [iconography instructions](#iconography-instructions)
  - _editorial_
    - [note](#note)
  - _references_
    - [references](#references)

### **iconography**

  - _identity_
    - [metadata](#metadata)
  - _relations_
    - [links](#links)
    - [categories](#categories)
    - [note](#note)
  - _content_
    - [flags](#flags)
    - [comment](#comment)
    - [note](#note)
  - _editorial_
    - [note](#note)
  - _references_
    - [references](#references)

### **person**

  - _identity_
    - [metadata](#metadata)
    - [names](#names)
    - [categories](#categories)
    - [links](#links)
  - _history_
    - [historical events](#historical-events)
    - [note](#note)
  - _editorial_
    - [note](#note)
  - _references_
    - [references](#references)





## 3 Elenco analitico (in ordine alfabetico) delle part
Di seguito si riportano in ordine alfabetico le parts di CADMUS NDP (che sono richiamate nelle singole sezioni dedicate ad ogni items). All'intero di ogni part si ritrovano dei _bricks_ che servono ad inserire una tipologia ancora più specifica di dato. Per l'elenco analitico dei bricks, si rimanda alla sezione successiva, ma ogni brick è richiamato all'interno delle parts in cui è implementato.

### bindings
### categories
text categories are a cross-reference taxonomy used to define the text type (e.g. comment) from the philological point of view
### chronotopes
### contents
### decorations
### edits
### hands
### historical events
### iconography instructions
### layouts
Questa part dàinformazioni sulle dimensioni fisiche della pagina le misure dello specchio di scrittura.   

Di seguito le informazioni utili per compilare i campi di questa part.

| campo | descrizione|
|---|---|
| `sample` | carta di esempio
| `range` | range di carte a cui si applica il layout
| `rulings` | Tecnica di rigatura
| `derolez` | numero nella classificazione di Derolez

#### Formula
Un po' più di attenzione merita il campo `formula`.
In questo campo vanno inseriti:
- il valore numerico delle dimensioni (nel formato altezza x larghezza [HxW]) 
- La formula dello **Specchio rigato**.  
I due valori sono separati dal segno = e ne risulta la formula così composta:  

Una volta inserita la formula, è possibile generare lo schema del layout ed estrarre le singole dimensioni andando a cliccare sulla freccia verso il basso a destra di `formula` e poi andando in `dimensioni` si possono importare i singoli valori numerici.

#### Note

Le informazioni aggiuntive contenute in **Disposizione del testo** vanno aggiunte come nota.
### links
### material description
### metadata
Con questa parte si attribuiscono all'item dei metadati generici.  
Convenzionalmente qui si deve inserire un EID e le informazioni e le informazioni sull'autorialità della scheda
#### type=EID 

 L'EID è un ID user-friendly è strutturato convenzionalmente secondo le seguenti parti:

1. indica il *facet*, ossia la tipologia di item secondo la seguente tabella
| facet | abbreviazione per EID |
|---|---|
| manoscritto | ms |
| testo a stampa | inc/stamp |
| edizione | ed |
| frammento ! fr |
| iconografia | ... |
2. sigla standard della città di provenienza o di edizione;
3. sigla della biblioteca o archivio in cui è contenuto il manufatto da descrivere, utilizzando le [abbreviazioni](#abbreviazioni-biblioteche) stabilite convenzionalmente; 
4. parte numerica della segnatura del manoscritto o dell'incunabolo 

**1** e **2** sono separate da un underscore ( **_** ), le altre parti da un trattino intermedio ( **-** )

Quindi nel caso del manoscritto mediceo l'EID risulta: `ms_fi-bml-86`

>NB tutte le lettere sono minuscole
#### Autorialità della scheda
#### `author` 
indica l'autore della catalogazione nell'ambiente Cadmus nel caso in cui abbia fatto un lavoro di catalogazione  "di prima mano"
#### `revisor` 
indica l'autore della catalogazione nell'ambiente Cadmus nel caso in cui abbia fatto un lavoro di catalogazione  "di seconda mano"
### notable word forms
### note
### preservation states
### references
### sheet labels
### watermarks





## 4. Elenco analitico (in ordine alfabetico) dei bricks

## APPENDICI
### Abbreviazioni biblioteche
Se una biblioteca non è presente si prega di segnalarlo via email in modo che si possa poi stabilire una sigla convenzionale e univoca all'interno del progetto.
| Città                        | Biblioteca                                                                 | Sigla  |
|-------------------------------|---------------------------------------------------------------------------|--------|
| Ascoli Piceno                 | Biblioteca comunale                                                        | BCom   |
| Belluno                       | Biblioteca capitolare Lolliniana                                           | BL     |
| Bergamo                       | Biblioteca civica Angelo Mai                                               | BCiv   |
| Berlin                        | Staatlichen Museen, Kupferstichkabinett u. Sammlung der Zeichnungen       | StMu   |
| Berlin                        | Staatsbibliothek Preussischer Kulturbesitz                                 | SB     |
| Bologna                       | Biblioteca comunale dell'Archiginnasio                                     | BCom   |
| Bologna                       | Biblioteca universitaria                                                   | BU     |
| Boston                        | Isabella Stewart Gardner Museum                                            | ISGM   |
| Brescia                       | Biblioteca civica Queriniana                                               | BCiv   |
| Budapest                      | Eötvös Loránd Tudomány Egyetem Könyvtára                                   | ELTEK  |
| Cagliari                      | Biblioteca universitaria                                                   | BU     |
| Cambridge                     | University Library                                                         | UB     |
| Cambridge (Mass., USA)        | Harvard College Libraries, Houghton Library                                | HL     |
| Capetown                      | National Library of South Africa                                           | NLSA   |
| Chantilly                     | Bibliothèque du château                                                    | BdC    |
| Chiavari                      | Archivio Notarile                                                         | AN     |
| Città del Vaticano            | Biblioteca Apostolica Vaticana                                             | BAV    |
| Cologny                       | Fondation Martin Bodmer                                                   | FMB    |
| Cortona                       | Biblioteca Comunale e dell'Accademia Etrusca                               | BCom   |
| Crema                         | Biblioteca Comunale                                                        | BCom   |
| Eton                          | College Library                                                           | CL     |
| Firenze                       | Biblioteca Medicea Laurenziana                                             | BML    |
| Firenze                       | Biblioteca Nazionale Centrale                                              | BNCF   |
| Firenze                       | Biblioteca Riccardiana                                                    | BR     |
| Frankfurt am Main             | Stadt und Universaitäts-Bibliothek                                        | SUB    |
| Genova                        | Biblioteca Durazzo                                                        | BDur   |
| Hamburg (Altona)              | Schulbibliothek des Christianeum                                           | BC     |
| Imola                         | Biblioteca Comunale                                                        | BCom   |
| København                     | Kongelige Bibliotek                                                       | KB     |
| London                        | British Library                                                           | BL     |
| Madrid                        | Biblioteca Nacional de España                                             | BN     |
| Manchester                    | John Rylands University Library                                           | UB     |
| Milano                        | Veneranda Biblioteca Ambrosiana                                            | VBA    |
| Milano                        | Biblioteca Nazionale Braidense                                             | BNB    |
| Milano                        | Biblioteca dell'Archivio Storico e Trivulziana                             | BT     |
| Modena                        | Biblioteca Estense Universitaria                                           | BU     |
| Mumbai                        | The Asiatic Society of Mumbai                                             | ASM    |
| Napoli                        | Biblioteca Nazionale                                                       | BN     |
| Napoli                        | Biblioteca Oratoriana del Monumento Nazionale dei Girolamini di Napoli     | BOG    |
| New Haven                     | Beinecke Library (Yale University)                                        | BL     |
| New York                      | H.P. Kraus                                                                | Kraus  |
| New York                      | Morgan Library & Museum                                                   | ML     |
| Novara                        | Biblioteca Comunale                                                        | BCom   |
| Oxford                        | Bodleian Library                                                          | BL     |
| Padova                        | Biblioteca Civica                                                         | BCiv   |
| Padova                        | Biblioteca del Seminario Vescovile                                        | BSem   |
| Paris                         | Bibliothèque nationale de France (Arsenal)                                 | BnFArs |
| Paris                         | Bibliothèque nationale de France (Richelieu)                               | BnF    |
| Parma                         | Biblioteca Palatina                                                       | BPal   |
| Perugia                       | Biblioteca Comunale Augusta                                               | BCom   |
| Piacenza                      | Biblioteca Comunale Passerini Landi                                        | BCom   |
| Ravenna                       | Biblioteca Comunale Classense                                             | BCom   |
| Reggio Emilia                  | Archivio di Stato                                                         | AS     |
| Rimini                        | Biblioteca Civica Gambalunga                                              | BCiv   |
| Roma                          | Biblioteca Angelica                                                       | BA     |
| Roma                          | Biblioteca Casanatense                                                    | Bcas   |
| Roma                          | Biblioteca dell'Accademia Nazionale dei Lincei e Corsiniana               | BANLC  |
| Roma                          | Biblioteca Nazionale Centrale                                             | BNC    |
| San Daniele del Friuli         | ...                                                                       | ...    |