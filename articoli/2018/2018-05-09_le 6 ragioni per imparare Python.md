# Le 6 ragioni per imparare Python

Perché dovresti imparare a programmare in Python?
Perché nell'ultimo anno è cresciuto molto l'interesse verso questo linguaggio?

Ho deciso di scrivere questo articolo in cui ti descrivo perchè, *secondo me*, nel 2018 è una **buona idea** imparare a programmare in Python.

> Oggi dozzine di sviluppatori di Google usano Python e siamo sempre alla ricerca di nuove persone che sappiano usarlo. - Peter Norvig, director of search quality at Google, Inc.


Prima di iniziare ad utilizzare Python, impiegai diverso tempo a capire quali fossero le ragioni che spingevano uno sviluppatore ad avvicinarsi a questo linguaggio.
Molti di loro erano veramente entusiasti di quanto riuscivano a fare.
*"Si può fare di tutto"*
*"Scrivo meno codice!"*
*"Che figata!"*
*"Mi ha trovato la fidanzata!"*

Così, spinto dai loro articoli e soprattutto dall’ultima frase, nel 2011 comprai Learning Python della O’Reilly.
Una guida di più di mille e duecento pagine ampiamente esaustiva sull’argomento.
La dimensione del libro era tale da mettere in soggezione anche i due libri di Tanenbaum.
Fu lì che capii due cose:
* era ora di andare in palestra ed allenare le braccia per usare quel libro
* era un linguaggio che poteva essere utilizzato con soddisfazione in diversi contesti 


*Una breve premessa*
In questo articolo non mi sentirai dire che è *“il miglior linguaggio di programmazione mai creato”*.
Non vuol dire **niente** come frase.
Non esiste neanche *“il miglior linguaggio di programmazione”*.
E’ una bufala creata per far leggere gli articoli.

E no, non è detto che tu debba provare ad utilizzarlo su di un nuovo progetto senza neanche capire se ha senso farlo.
La valutazione di un linguaggio di programmazione, *secondo me*, deve essere sempre contestualizzata in base al progetto che si deve gestire.
Usare un linguaggio di programmazione su sistemi di produzione *“tanto per provarne uno nuovo”* o *“perchè adesso fa figo”* o *“lo usano tutti”* non sono delle motivazioni serie.
Dillo al tuo responsabile quando usa nomi di linguaggi fuori luogo.
Mostra degli esempi su come una tecnologia usata male fa fare brutta figura alla tua azienda.
Sii responsabile del linguaggio che andrai ad utilizzare.

Non sono qua ad evangelizzare su Python e di quanto sia *figo* o *meno figo*.
Tanto meno voglio passare per uno dei tanti paraguru presenti in rete che hanno già **tutte le risposte** basandosi su dati di *anni fa*.
Quello che stai per leggere è frutto della **mia esperienza** e delle **ricerche** che ho fatto su questo linguaggio.

*Procediamo!*

# 1 - Python è facile da imparare

### La sintassi semplice
La sintassi utilizzata in Python è molto semplice.
E questo permette di avere un apprendimento **più rapido** rispetto ad altri linguaggi di programmazione.
Il codice viene scritto come una versione *semplificata* dell’inglese.
Quindi, risulta facilmente leggibile **anche** dai principianti.
Non sono presenti neanche simboli strani o abbreviazioni incomprensibili.
Questo risulta essere un enorme vantaggio quando si legge il codice.
Soprattutto quando devi leggerne uno che **non** hai scritto te!

Ti faccio un esempio:
```python
import random


def get_random_number():
   numbers = [1, 2, 3, 4, 5, 6]
   random_number = random.choice(numbers)
   return random_number


print(get_random_number())
```

Anche chi non ha mai letto una riga di codice scritta in Python, avrà capito cosa è stato scritto.
*Bello, vero?*

Nel libro **Clean Code**, *Robert C. Martin* scrisse: 
>Il rapporto tra tempo trascorso a leggere e scrivere (codice) è ben superiore a 10 a 1.

Sono sicuro che anche te stai pensando *"Quanto è vera questa frase!"*


### Risparmi tempo
Per scrivere del codice in Python non è richiesto di utilizzare alcun particolare costrutto. 
Ed è una grande cosa.
Perchè ti troverai a dover scrivere **molto meno codice** rispetto ad altri linguaggi di programmazione.

Un esempio molto semplice può essere fatto scrivendo il classico *"Hello World"*:
in Python:
```python
print("Hello World")
```
in Java:
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, world");
    }
}
```

Quando si scrivono applicazioni complesse, un linguaggio di programmazione che permette di scrivere in modo veloce, *fa la differenza*.
Soprattutto quando il tuo cliente pretende *quella modifica* prima di **subito**.

Mediamente, Python permette di scrivere *fino a* cinque volte meno righe di codice rispetto a Java ed addirittura dieci volte meno di C++.
I vantaggi che ne derivano sono molteplici:
* minor tempo di sviluppo
* minor tempo di manutenzione del codice
* minor costo di gestione del progetto

*Ovviamente sai perfettamente che se il codice è scritto male, neanche Python ti salva!*


### Indentazione
I  linguaggi di programmazione più diffusi, usano delle parentesi graffe o parole riservate per delimitare i blocchi di codice che si scrivono.
Python, invece, utilizza *l’indentazione*.
Questo permette di avere il codice organizzato in modo coerente a cui si aggiunge una notevole facilità di lettura ed eleganza nella stesura.
Se sbagli ad indentare, il codice non compila e viene restituito un errore di sintassi.
Python ti **obbliga** a scrivere codice in modo *leggibile*.
```python
import random


def get_random_number():
numbers = [1, 2, 3, 4, 5, 6] # non è stato indentato
   random_number = random.choice(numbers)
   return random_number


print(get_random_number())
```
Output
```python
 File "esempio.py", line 5
   numbers = [1, 2, 3, 4, 5, 6]
         ^
IndentationError: expected an indented block
```


### Multiparadigma

Python permette di scegliere quale paradigma utilizzare nel proprio progetto. 
Si può utilizzare *la programmazione procedurale* o quella *orientata agli oggetti*.
Oppure entrambe. 
O passare dall’una all’altra in base alle proprie esigenze.

### L’adozione in università
La facilità di apprendimento di Python è stata notata persino dalle maggiori università statunitensi.
Infatti, è andato a [rimpiazzare Java come primo linguaggio insegnato]. 
Anche da noi in Italia abbiamo affiancato se non sostituito Java con Python.


# 2 - Python è versatile

La peculiarità che più mi ha impressionato di questo linguaggio, riguarda la versatilità di utilizzo.

In questi anni ho usato Python per scrivere **script** e **reportistica** di vario genere.
**Questo stesso blog** e la relativa manutenzione del server li ho scritti in Python!
Ma la versatilità si estende a molti  ambienti totalmente *eterogenei* tra di loro:
* ambiente scientifico
* data science
* sviluppo web
* system automation ed administration
* finanza e trading
* scripting
* software GIS
* sicurezza e penetration test
* computer grafica
* sviluppo di videogiochi


# 3 - E’ lo standard de facto nel campo del data science e machine learning

Nel rapporto di stackoverflow [Why is Python Growing So Quickly?] viene evidenziato come l’**interesse** per il data science ed il machine learning stia facendo diventare Python **molto** popolare. 

Nel campo dell'analisi dei dati, Python presenta potentissime librerie quali:
* [NumPy] per lavorare con array, matrici multidimensionali, tensori
* [Matplotlib] per creare grafici
* [SciPy] per lavorare con algoritmi, algebra lineare, modelli, statistica,  l'integrazione, elaborazione di segnali ed immagini
* [Pandas] che è diventato uno standard per quanto riguarda l’analisi statistica

Nel campo della biologia, Python ha un'altra potentissima libreria: [Biopython] che serve ai biologi per il sequenziamento genetico. 
*Fico, vero?*

Nel campo del machine learning, Python ormai domina la scena grazie a librerie quali:
* [TensorFlow] per l’apprendimento automatico
* [Keras] per le reti neurali
* [scikit-learn] per il data mining e data analysis

*Secondo me*, chiunque volesse cimentarsi in questi campi, dovrebbe iniziare a prendere **sul serio** l’idea di imparare il Python.


# 4 - Ha un ecosistema formidabile

### Le librerie
L’ecosistema intorno a Python è **vivo**.
Ad oggi, sono presenti più di *[centotrentamila librerie]* di terze parti da poter utilizzare.
Se per gli smartphone *c’è un’app per tutto*, in Python *c’è una libreria per tutto*!

La sola *[libreria standard]* è ricca di funzionalità pronte all’utilizzo.
Di base è presente anche un *[framework per lo unit-test]*.

Lato web, c’è l’imbarazzo della scelta tra i framework da utilizzare:
* [Django]
* [Flask]
* [Web2py]
* [Pyramid]

solo per citarne alcuni.

### La community

Avere una community vibrante come quella di Python è molto importante per un linguaggio open source:
* è la [quinta community su stackoverflow] con oltre 524 mila follower e ben oltre 912 mila domande 
* ha oltre 2000 meetup sparsi per il mondo
* è il secondo linguaggio più utilizzato su [Github]

Inoltre, la community internazionale [PyCon] organizza ogni anno diverse conferenze sparse per il mondo.
Il PyCon di quest’anno [si svolge dal 9 al 17 Maggio a Cleveland].
L’Euro Python 2018, invece, [si svolge dal  23 al 29 Luglio ad Edimburgo].


### 5 - Quali aziende utilizzano Python?

Dato che Python è molto versatile, è utilizzato dalla **maggior parte** delle più famose aziende hi-tech del pianeta.
Se volessi provare ad entrare a lavorare per una di loro, **ti consiglierei** di imparare *bene* questo linguaggio.

**Google**
Python è stato utilizzato fin dalla nascita di Big G.
La filosofia di Google su questo linguaggio è stata: *“Python dove possiamo, C++ dove dobbiamo”*.
Lato server, Python è uno dei quattro linguaggi ufficiali che vengono utilizzati.
Gli altri tre sono il C++, Java e Go.

**Facebook**
In Facebook, Python è il terzo linguaggio più utilizzato.
Davanti ha il C++ e l’Hack *- un dialetto di PHP di loro invenzione -*.

**Spotify**
In Spotify, Python è utilizzato principalmente per fare data analysis e servizi di backend.

**Netflix**
In Netflix, Python è usato in decine di app che spaziano dall’analisi dei dati lato server al mantenimento attivo del servizio.

**Dropbox**
Il client desktop di Dropbox è scritto in Python. 
Una grossa fetta del codice che gira lato server è scritto in questo linguaggio.
Ma non solo: qui ci lavora il fondatore **Guido van Rossum** che è arrivato direttamente da Google.

**Reddit**
Il framework web web2py su cui gira Reddit è stato creato da loro e poi rilasciato open source.

**Youtube**
Anche Youtube ha a che fare con Python.
Le API sono scritte in questo linguaggio così come buona parte del codice che gira lato server.

**Pinterest**
Pinterest è stato riscritto in Flask dopo essere stato precedentemente sviluppato in Django.
Entrambi sono due popolari framework web di Python.

**Instagram**
Instagram è stato sviluppato usando Django.

**Red Hat**
In RedHat si fa un massiccio uso di Python:
Anaconda *- l’installer di Red Hat e Fedora -* , OpenStack ed Ansible [sono scritti in Python].


### 6 - Python ed il mercato del lavoro

**Python negli USA**

Secondo l’[analisi di Coding Dojo], Python è il terzo linguaggio più richiesto del 2017.
Se contiamo che il primo linguaggio è SQL *- che non è un linguaggio di programmazione -* si può dire che dopo Java, Python è il linguaggio più richiesto dell’ultimo anno.
*Non male!*
L’analisi effettuata da Coding Dojo si basa sulle offerte di lavoro trovate sul portale [indeed.com].
Ma anche guardando l’analisi effettuata da Stackoverflow nel loro articolo [incredible growth python] si arriva alla stessa conclusione: il 2017 è stato un anno di **interesse crescente** per Python.

**Python in Italia**

Come già saprai, i volumi e la virtuosità nell’utilizzo di determinate tecnologie, varia molto da paesi come gli USA e l’Italia.
Nel nostro Bel paese, l’utilizzo di Python è *più timido*.

Prendiamo ad esempio le richieste di lavoro inerenti a Java e Python.
*Utilizzo Java come metro di paragone perché è il linguaggio più richiesto dal nostro mercato.*

Dalle mie analisi, negli USA le richieste di lavoro per sviluppatori Java e Python possono avere un **rapporto di quasi 1:1**.
In Italia, il **rapporto scende a 4:1**. 
Ogni *quattro richieste* di sviluppatori Java ne abbiamo solo una di Python.

Da noi, le grandi aziende **preferiscono rimanere** su tecnologie quali Java e .Net.
E **non** sempre perché risultano essere i linguaggi migliori per i progetti su cui vengono utilizzati.
Piuttosto per termini di costi, continuità di progetto e **poca propensione** al cambiamento.

*E le richieste di lavoro in Italia su Python?*

Le richieste di lavoro riguardanti Python, ad oggi, si riducono a **tre categorie**:
* *sviluppo web*
  chi vuole sviluppare in Python, è facile che finisca a fare il web developer. 
Se cerchi sui maggiori siti di offerte di lavoro in Italia, ne trovi in ogni sua forma e declinazione: full stack web developer, backend developer, frontend developer.
* *analisi dei dati* 
 Il mercato intorno all'analisi dei dati sta crescendo anche nel nostro paese.
Buona parte delle offerte di lavoro riguardano la ricerca di data analyst, data scientist, data mining e machine learning.
Non male, perchè è un mercato sicuramente interessante ed in forte crescita.
* *devops*
Anche lato devops la richiesta di Python è sempre più crescente nel nostro mercato.
Purtroppo, questa è la categoria con meno richieste.
Speriamo che diventi più interessante nel corso dell'anno.


### Un consiglio

Al di là del fatto di imparare Python o meno, ricordati di **non diventare troppo specializzato** solo ed esclusivamente su di un solo linguaggio.
I tempi cambiano, le tecnologie evolvono in modo molto rapido.
**Soprattutto** se sei molto giovane, pensare di diventare il *tizio che ne sa di Java* potrebbe pagare subito. 
Ma tra dieci anni, sei sicuro che sarà la scelta *più sensata*?
Ricordati che essere specializzati *è importante* ma **essere spendibili sul mercato** lo è molto di più.


[rimpiazzare Java come primo linguaggio insegnato]: <https://cacm.acm.org/blogs/blog-cacm/176450-python-is-now-the-most-popular-introductory-teaching-language-at-top-u-s-universities/fulltext>
[Why is Python Growing So Quickly?]: <https://stackoverflow.blog/2017/09/14/python-growing-quickly/>
[NumPy]: <http://www.numpy.org/>
[Matplotlib]: <https://matplotlib.org/>
[SciPy]: <https://www.scipy.org/>
[Pandas]: <https://pandas.pydata.org/>
[Biopython]: <http://biopython.org/>
[TensorFlow]: <https://www.tensorflow.org/>
[Keras]: <https://keras.io/>
[scikit-learn]: <http://scikit-learn.org/stable/>
[centotrentamila librerie]: <https://pypi.python.org/pypi>
[libreria standard]: <https://docs.python.org/3/library/>
[framework per lo unit-test]: <https://docs.python.org/3.6/library/unittest.html>
[Django]: <https://www.djangoproject.com/>
[Flask]: <http://flask.pocoo.org/>
[Web2py]: <http://www.web2py.com/>
[Pyramid]: <https://trypyramid.com/>
[quinta community su stackoverflow]: <https://stackoverflow.com/questions/tagged/python>
[Github]: <https://octoverse.github.com/>
[PyCon]: <https://www.pycon.org/>
[si svolge dal 9 al 17 Maggio a Cleveland]: <https://us.pycon.org/2018/>
[si svolge dal  23 al 29 Luglio ad Edimburgo]: <https://ep2018.europython.eu/>
[sono scritti in Python]: <https://community.redhat.com/blog/2016/12/python-has-big-impact-at-red-hat/>
[analisi di Coding Dojo]: <http://www.codingdojo.com/blog/9-most-in-demand-programming-languages-of-2017/>
[indeed.com]:<https://www.indeed.com/>
[incredible growth python]: <https://stackoverflow.blog/2017/09/06/incredible-growth-python/>