# Guida pratica all'utilizzo di Cadmus

>a cura di Andrea La Veglia (per chiarimenti: [alaveglia@unisa.it](mailto:alaveglia@unisa.it))

INDICE
- [1 Aggiunta di item](#1-aggiunta-di-un-item)
- [2 Aggiunta di part](#2-aggiunta-delle-parts)

Cadmus è un framework di descrizione modulare, nel senso che offre la possibilità di strutturare le informazioni in moduli componibili. In particolare l'architettura di Cadmus è costituita da **_items_** e da **_parts_**.  


## 1. Aggiunta di un _item_

L'_item_ è come una scatola che contiene al suo interno elementi correlati tra loro e riferiti al contenitore che sono le _parts_.  
L'_item_ corrisponde ad un  manoscritto/unità codicologica, un disegno, un'edizione, un testo a stampa, un item iconografico o di una persona. La descrizione analitica dell'_item_ si articolerà tramite l'inserimento di diverse _parts_ (Cf. [Documentazione di Cadmus](https://cadmus.fusi-soft.com/docs/data-architecture)). 

Il primo passaggio per il catalogatore è dunque la creazione di un nuovo _item_, andando sul bottone in basso a sinistra nella visualizzazione dell'editor di Cadmus_NDP.

![aggiunta item](./additem.png)<figcaption>Aggiunta di un item in Cadmus.</figcaption>

### Metadati identificativi (identity)

Per la creazione di un nuovo _item_ bisogna inserire i seguenti metadati obbligatori che costituiscono l'etichetta (_**label**_) dell'_item_: 
- `title` = indica il titolo rappresentativo dell'item. A seconda del tipo di item si seguiranno queste convenzioni stabilite
  - **manoscritto**: 
- `description` 
- `facet`provvede ad indicare la tipologia di item, specificando dunque se si tratti di manoscritti, disegni o stampe, oppure di un item iconografico o di una persona.



### Flags

I flags sono le "bandierine" che segnalano lo stato editoriale della catalogazione dell'oggetto di riferimento (ms, frg, ...) in Cadmus.

> NB Dal momento della creazione dell'item bibliologico fino al suo completamento, per segnalare agli altri contributori che è ancora in lavorazione, bisogna selezionare lo stato di `draft`. 
Dopo il completamento della scheda si potrà selezionare `complete` e togliere la spunta a `draft`.

## 2. Aggiunta delle _parts_

Dopo aver creato la "scatola" che indica la 
Si riportano di seguito gli schemi di catalogazione da seguire per:
- [manoscritti](#manuscript), 
- [frammenti](#fragment)
- [edizioni di testi a stampa (edizione "ideale")](#print-edition)
- [esemplare di testo a stampa](#print-instance)
- [progetto disegni](#drawings-project)
- [disegno](#drawing-item)
- [iconografia](#iconography)
- [persona](#person)

### **manuscript**

  - _identity_
    - [metadata](#23--metadata)
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


## 2.2 Come si aggiunge una _part_

Un elemento _part_ è un **set di dati** coerente che si riferisce all'item al quale viene correlato (Cf. [Documentazione di Cadmus](https://cadmus.fusi-soft.com/docs/data-architecture)).  
DUnque, dopo aver creato un _item_ si può procedere alla parte fondamentale del lavoro, ossia l'aggiunta delle parti di Cadmus utili a descrivere l'item bibliologico in questione.  
Si veda di seguito lo screenshot di esempio per l'aggiunta di una parte. 

![Aggiunta di Part](addpart.png)<figcaption>Aggiunta di un item in Cadmus.</figcaption>




## 2.3 Guida all'utilizzo delle part
Di seguito si riportano in ordine alfabetico le parts di CADMUS NDP (che sono richiamate nelle singole sezioni dedicate ad ogni items)
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
### links
### material description
### metadata
Questa part è utile per per attribuire all'_item_ un EID (ID human friedly) e le informazioni sui catalogatori
#### EID 

 L'EID è strutturato convenzionalmente secondo le seguenti parti:

1. indica il *facet* 
2. sigla standard della città di provenienza o di edizione;
3. sigla della biblioteca o archivio in cui è contenuto il manufatto da descrivere; 
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









## 4. Aggiunta della bibliografia (references)


[torna all'indice](#linee-guida-per-il-trasferimento-di-schede-da-idp-a-cadmus)



