# Cose da controllare o implementare nella treebank 

__Maximal unit segmentation__
* dislocated solo nel caso di ripresa pronominale. In quel caso specifichiamo il tipo di dislocazione (`dislocated:obl`). Se ci sono casi in cui non è decidibile il tipo di relazione, lasciamo solo `dislocated`
* casi la prosodia indica che c'è una relazione tra clausole ma non c'è marker sintattico li annotiamo come `parataxis` anche se semanticamente la relazione è subordinante (es. "avevo sei anni, ho avuto un incidente" semanticamente indicherebbe una subordinata di tempo ma non essendoci il connettivo lo teniamo come paratassi)
* Reported speech:
  * caso standard > completiva. ccomp:reported
  * parataxis:insert per i casi di parenthetical verbs
  * Reported=Yes sulla root del subtree della frase riportata
* in generale teniamo parataxis:parenth per i casi di clausole inserite che interrompono la clausola principale mentre parataxis:insert per tutti gli epistemici
* conj:reform per i false starts

__Tokenisation__
pause piene: deprel discourse:filledpause; POS= INTJ
onomatopee: INTJ non ci sembra adatto, Ludovica suggerisce NOUN

__Repetition, false starts ecc__
Le ripetizioni e le false partenze (che non includono le parole interrotti, vedi sotto) sono conj:reform
Reparandum lo usiamo solamente quando c'è una parola interrotta.

__casi di _sì sì no_ ecc__
Da risolvere nella prossima riunione del Task

__modalità__
se il parlante canta, legge ... indicare nel MISC --> Manner=read|sing
