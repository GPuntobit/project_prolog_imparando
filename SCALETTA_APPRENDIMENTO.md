# Scaletta di Apprendimento: Prolog, Lisp e Qute

Questa scaletta fornisce un percorso strutturato per imparare Prolog, Lisp e Qute, seguendo un approccio progressivo e didattico.

---

## PARTE 1: PROLOG

### 📚 LIVELLO BASE - Fondamenti (Settimane 1-4)

#### Introduzione e Ambiente

- [ ] Cos'è Prolog e perché è diverso dai linguaggi imperativi
- [ ] Paradigma della programmazione logica
- [ ] Ambiente di sviluppo: installazione di SWI-Prolog
- [ ] Primi passi con il REPL (Read-Eval-Print Loop)

#### Sintassi e Termini Base

- [ ] Termini Prolog: atomi, numeri, variabili, strutture
- [ ] Convenzioni di naming (atomi minuscoli, variabili maiuscole)
- [ ] Fatti semplici: come rappresentare conoscenza
- [ ] Query semplici: come interrogare la base di conoscenza
- [ ] Commenti e documentazione

#### Regole e Deduzione

- [ ] Definizione di regole con `:-`
- [ ] Concetto di clausola (testa e corpo)
- [ ] Regole condizionali (if-then)
- [ ] Backtracking: come Prolog esplora le soluzioni
- [ ] Esempi pratici: genealogia, classificazioni

#### Liste e Pattern Matching

- [ ] Notazione `[Head|Tail]`
- [ ] Operazioni base: append, member, length
- [ ] Pattern matching su liste
- [ ] Liste annidate
- [ ] Concetto di unificazione (`=`)
- [ ] Unificazione vs assegnazione
- [ ] Pattern matching strutturale
- [ ] Variabili anonime (`_`)

### 🔧 LIVELLO INTERMEDIO - Programmazione (Settimane 5-8)

#### Ricorsione e Strutture

- [ ] Ricorsione su liste
- [ ] Caso base e caso ricorsivo
- [ ] Ricorsione su strutture annidate
- [ ] Accumulatori e ricorsione tail-recursive
- [ ] Esempi: somma, lunghezza, reverse
- [ ] Alberi e strutture ricorsive
- [ ] Grafi: rappresentazione e attraversamento

#### Controllo del Flusso

- [ ] Operatori logici: congiunzione `,` (AND), disgiunzione `;` (OR), negazione `\+` (NOT)
- [ ] Precedenza degli operatori
- [ ] Combinazioni complesse
- [ ] Cut (`!`) e controllo del backtracking
- [ ] Cut verde vs cut rosso
- [ ] `fail` e `true`
- [ ] Alternative al cut: `once/1`, `if-then-else`
- [ ] Best practices: evitare cut non dichiarativi

#### Predicati Built-in e I/O

- [ ] Confronti: `=`, `\=`, `==`, `\==`, `@<`, `@>`
- [ ] Aritmetica: `is/2`, operatori aritmetici
- [ ] Type checking: `atom/1`, `number/1`, `var/1`, `nonvar/1`
- [ ] Input/Output: `write/1`, `read/1`, `format/2`
- [ ] Manipolazione termini: `functor/3`, `arg/3`, `=..`
- [ ] Lettura/scrittura file
- [ ] Parsing di dati strutturati

### 🚀 LIVELLO AVANZATO - Tecniche Avanzate (Settimane 9-10)

#### CLP(FD) - Constraint Logic Programming

- [ ] Introduzione ai vincoli su domini finiti
- [ ] Dichiarazione: `:- use_module(library(clpfd))`
- [ ] Vincoli aritmetici: `#=`, `#<`, `#>`, `#\=`
- [ ] Labeling e ricerca di soluzioni
- [ ] Esempi: puzzle, scheduling, ottimizzazione

#### Metaprogrammazione e Codice Dinamico

- [ ] `call/1` e predicati di ordine superiore
- [ ] `maplist/3`, `foldl/4`, `include/3`
- [ ] Manipolazione dinamica del codice
- [ ] Term expansion e macro
- [ ] Tabelle dinamiche (`assert/1`, `retract/1`)

#### Gestione Errori e Debugging

- [ ] `must_be/2` per validazione input
- [ ] Gestione errori con `catch/3` e `throw/1`
- [ ] Predicati di validazione custom
- [ ] Debugging: `trace/0`, `spy/1`
- [ ] Best practices per codice robusto

#### Strutture Dati e Persistenza

- [ ] Dizionari e associazioni
- [ ] Quando usare strutture vs liste
- [ ] Serializzazione termini
- [ ] Database Prolog
- [ ] Integrazione con sistemi esterni

### 💼 PROGETTI PRATICI - Applicazioni (Settimane 9-10)

- [ ] Sistema esperto semplice
- [ ] Parser per linguaggi formali
- [ ] Risolutore di puzzle (Sudoku, N-Queens)
- [ ] Sistema di raccomandazioni
- [ ] Analizzatore sintattico

---

## PARTE 2: LISP

### 📚 LIVELLO BASE - Fondamenti (Settimane 11-14)

#### Introduzione e Ambiente Lisp

- [ ] Storia e filosofia di Lisp
- [ ] Dialetti principali: Common Lisp, Scheme, Clojure
- [ ] Ambiente di sviluppo: installazione (SBCL, Clozure CL, o altro)
- [ ] REPL e ciclo read-eval-print

#### Sintassi e Semantica Base

- [ ] S-expressions: atomi e liste
- [ ] Notazione prefissa e parentesi
- [ ] Atomi, numeri, stringhe, simboli
- [ ] Liste: `(car list)`, `(cdr list)`, `cons`
- [ ] Quote e valutazione: `'`, `quote`, `eval`
- [ ] Funzioni speciali vs funzioni ordinarie

#### Funzioni e Definizioni

- [ ] `defun`: definire funzioni
- [ ] Parametri e argomenti
- [ ] Valori di ritorno: `return`, valori multipli
- [ ] Scope e binding: variabili locali e globali
- [ ] Documentazione inline con docstrings

#### Ricorsione e Liste

- [ ] Ricorsione su liste
- [ ] Ricorsione tail-recursive
- [ ] Operazioni su liste: `append`, `reverse`, `member`
- [ ] Liste associative: `assoc`, `pairlis`

### 🔧 LIVELLO INTERMEDIO - Programmazione Funzionale (Settimane 15-18)

#### Funzioni di Ordine Superiore

- [ ] Funzioni come valori first-class
- [ ] `lambda`: funzioni anonime
- [ ] `apply` e `funcall`
- [ ] Closure e lexical scoping
- [ ] Mapping: `mapcar`, `mapcan`, `map`
- [ ] Folding: `reduce`
- [ ] Esempi pratici di HOF

#### Iterazione e Strutture Dati

- [ ] Costrutti iterativi: `loop`, `do`, `dolist`, `dotimes`
- [ ] Array e vettori
- [ ] Hash tables
- [ ] Strutture (`defstruct`)

#### I/O e File System

- [ ] Stream: input e output
- [ ] Lettura/scrittura file
- [ ] Formattazione: `format`
- [ ] Parsing e generazione di testo
- [ ] Serializzazione

#### Package System e Organizzazione

- [ ] Namespace e packages
- [ ] `defpackage` e `in-package`
- [ ] Export e import
- [ ] Organizzazione del codice
- [ ] Best practices per modularità

### 🚀 LIVELLO AVANZATO - Caratteristiche Avanzate (Settimane 19-20)

#### Macros

- [ ] Perché le macro sono potenti
- [ ] `defmacro`: definire macro
- [ ] Backquote e comma: `` ` ``, `,`, `,@`
- [ ] Macro vs funzioni: quando usare cosa
- [ ] Esempi: `when`, `unless`, macro custom

#### Sistema di Oggetti (CLOS)

- [ ] Introduzione a CLOS (Common Lisp Object System)
- [ ] Classi: `defclass`
- [ ] Metodi: `defmethod`
- [ ] Eredità multipla
- [ ] Generic functions e method combination

#### Gestione Errori e Ottimizzazione

- [ ] Sistema di condizioni: `error`, `warn`, `signal`
- [ ] `handler-case` e `handler-bind`
- [ ] Restart e recovery
- [ ] Best practices per gestione errori
- [ ] Compilazione: `compile-file`, `load`
- [ ] Dichiarazioni: `declare`, `optimize`
- [ ] Profiling e debugging
- [ ] Tipi e type declarations
- [ ] Inline functions

### 💼 PROGETTI PRATICI - Applicazioni (Settimane 19-20)

- [ ] Interprete Lisp semplice
- [ ] Sistema di simboli e valutazione
- [ ] Parser e generatore di codice
- [ ] Applicazione web (con framework Lisp)
- [ ] Tool di automazione

#### Integrazione e Librerie

- [ ] Quicklisp: gestione pacchetti
- [ ] Librerie comuni e utili
- [ ] FFI (Foreign Function Interface)
- [ ] Integrazione con C e altri linguaggi
- [ ] Deployment e distribuzione

---

## PARTE 3: QUTE

### 📚 LIVELLO BASE - Fondamenti (Settimane 21-24)

#### Introduzione e Ambiente Qute

- [ ] Cos'è Qute: linguaggio ibrido Prolog-Lisp
- [ ] Introduzione a Qute: storia e filosofia
- [ ] Caratteristiche ibride: logica + funzionale
- [ ] Installazione e configurazione ambiente Qute
- [ ] REPL e ciclo di sviluppo
- [ ] Struttura base di un programma Qute
- [ ] Differenze e somiglianze con Prolog e Lisp
- [ ] Quando usare Qute vs Prolog vs Lisp

#### Sintassi Base

- [ ] Sintassi e semantica Qute
- [ ] Termini e atomi in Qute
- [ ] Liste e strutture dati
- [ ] Variabili e binding
- [ ] Pattern matching e unificazione
- [ ] Commenti e documentazione

#### Programmazione Logica (Stile Prolog)

- [ ] Fatti e regole (stile Prolog)
- [ ] Query e risoluzione
- [ ] Backtracking in Qute
- [ ] Predicati e clausole
- [ ] Esempi: database logici, relazioni

#### Programmazione Funzionale (Stile Lisp)

- [ ] Definizione di funzioni (stile Lisp)
- [ ] Funzioni come valori first-class
- [ ] Valutazione eager vs lazy
- [ ] Closure e scope
- [ ] Ricorsione in Qute

### 🔧 LIVELLO INTERMEDIO - Integrazione Paradigmi (Settimane 25-26)

#### Integrazione Logica-Funzionale

- [ ] Combinare predicati e funzioni
- [ ] Chiamare funzioni da predicati
- [ ] Usare predicati come funzioni
- [ ] Pattern matching ibrido
- [ ] Esempi di codice ibrido
- [ ] Esempi pratici in Qute

#### Strutture Dati e Manipolazione

- [ ] Liste: operazioni logiche e funzionali
- [ ] Alberi e strutture ricorsive
- [ ] Mapping e filtering
- [ ] Accumulatori e folding
- [ ] Trasformazioni di dati

#### Controllo del Flusso in Qute

- [ ] Operatori logici: AND, OR, NOT
- [ ] Costrutti condizionali
- [ ] Iterazione e ricorsione
- [ ] Gestione del backtracking
- [ ] Cut e controllo esplicito

### 🚀 LIVELLO AVANZATO - Tecniche Avanzate (Settimane 27-28)

#### Metaprogrammazione

- [ ] Macro e code generation
- [ ] Manipolazione di codice
- [ ] Quote e eval
- [ ] Predicati di ordine superiore
- [ ] Esempi avanzati

#### Moduli e Organizzazione

- [ ] Struttura di progetti Qute
- [ ] Namespace e packages
- [ ] Import ed export
- [ ] Librerie e dipendenze
- [ ] Best practices organizzative

#### Ottimizzazione e Performance

- [ ] Profiling codice Qute
- [ ] Ottimizzazione query logiche
- [ ] Efficienza funzionale
- [ ] Memoization e caching
- [ ] Best practices performance

### 💼 PROGETTI PRATICI - Applicazioni Ibride (Settimane 27-28)

- [ ] Sistema che combina logica e funzionale
- [ ] Parser con valutazione logica
- [ ] Sistema di regole con funzioni
- [ ] Trasformazione dati con query logiche
- [ ] Integrazione di paradigmi

#### Integrazione e Deployment

- [ ] Interoperabilità con Prolog
- [ ] Interoperabilità con Lisp
- [ ] Chiamate a librerie esterne
- [ ] Deployment applicazioni Qute
- [ ] Tooling e strumenti di sviluppo

---

## Risorse Consigliate

### Per Prolog

- Materiale nella cartella `docs/`:
  - `Programming In Prolog PDF.pdf`
  - `PROLOG PROGRAMMING FOR ARTIFICIAL INTELLIGENCE - lvan Bratko.pdf`
  - `LucidiProlog.pdf`
  - Altri PDF su Prolog nella cartella

### Per Lisp

- Materiale nella cartella `docs/`:
  - `Basic_Lisp_Overview_s_Numeric_Functions.pdf`
  - `lisp-p1.pdf`
  - `lispintro.pdf`
  - `ilmiolisp_08-2016-1.pdf`
  - `Dispensa2.pdf`

### Per Qute

- Materiale nella cartella `docs/`:
  - `Qute_A_PrologLisp_Type_Language_for_Logic_Programm.pdf`
  - `Qute_a_prolog_lisp_type_language_for_log.pdf`

### Pratica

- Esercizi progressivi per ogni fase
- Progetti incrementali che combinano concetti
- Code review e refactoring
- Partecipazione a comunità Prolog, Lisp e Qute

---

## Note Finali

Questa scaletta è progettata per un percorso completo di circa 28 settimane:

- **Settimane 1-10**: Prolog (fondamenti e avanzato)
- **Settimane 11-20**: Lisp (fondamenti e avanzato)
- **Settimane 21-28**: Qute (linguaggio ibrido)

Con un ritmo di 2-3 ore di studio per settimana. Adatta il ritmo alle tue esigenze e approfondisci gli argomenti che ti interessano di più. La sezione su Qute presuppone una buona conoscenza sia di Prolog che di Lisp, essendo un linguaggio che combina entrambi i paradigmi.

**Buono studio!**
