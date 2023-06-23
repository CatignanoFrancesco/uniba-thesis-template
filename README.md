# Template tesi UniBa
Template in LaTeX per scrivere le tesi per l'Università degli Studi di Bari Aldo Moro.

Il template è ispirato alle seguenti <a href="https://www.uniba.it/it/ricerca/dipartimenti/scienze-politiche/didattica/laurearsi/linee-guida-per-la-redazione-della-tesi-di-laurea">linee guida</a>.

⚠️ ATTENZIONE: alcune regole potrebbero cambiare a seconda del dipartimento di appartenenza, per cui è necessario effettuare le relative modifiche al template.

Questo template rappresenta un punto di inizio per scrivere la propria tesi senza preoccuparsi delle impostazioni del documento.

# Struttura del progetto 🗄️
Il progetto è così strutturato:
- 📚 _capitoli_: la cartella che contiene tutti i file _.tex_ relativi ai capitoli
- 🖼️ _img_: la cartella che contiene le immagini usate all'interno del documento
- 📝 _abstract.tex_: il file che contiene l'abstract
- 🔖 _bibliography.bib_: il file per la bibliografia (vedere la <a href="https://www.overleaf.com/learn/latex/Bibliography_management_with_bibtex">documentazione</a> per scrivere inserire correttamente le citazioni)
- 📗 _front.tex_: il file per il frontespizio. Modificando questo file si può personalizzare la copertina della propria tesi
- 📄 _main.tex_: il file principale che contiene le impostazioni e la struttura del documento
- 📑 _main.pdf_: il pdf finale ottenuto dalla compilazione di _main.tex_ su cui verrà visualizzato il risultato

## Struttura del file _main.tex_ 📄
Questo è il file principale del progetto. Da qui parte la compilazione. È diviso in due parti: la prima contiene tutte le impostazioni generali del documento come il carattere utilizzato, la dimensione, i margini, i comandi personalizzati e i pacchetti importati, mentre la seconda parte contiene la struttura del documento ed è quella che verrà modificata più spesso all'interno del documento.

Per aggiungere un nuovo capitolo bisogna:
1. creare un file _nomefile.tex_ all'interno della cartella _capitoli_
2. inserire il comando ```\chapter{Nome Capitolo}``` all'inizio del file creato e riempire il documento
3. includere il file creato all'interno della seconda parte di _main.tex_ usando il comando ```\include{capitoli/nomefile.tex}```

Il capitolo avrà automaticamente un numero assegnato dal compilatore e verrà numerato anche nell'indice. Per evitare questo, basta anteporre al comando ```\include``` il comando ```\setcounter{secnumdepth}{-1}```.

## Struttura del documento di tesi 📑
Il documento è strutturato come segue:
- Frontespizio, cioè la copertina del documento
- Dedica
- Abstract
- Indice
- Capitolo 1, l'introduzione della tesi
- Capitolo 2, spiegazione di come inserire sezioni e sottosezioni
- Capitolo 3, spiegazione di tabelle, codici, formule matematiche, ecc.
- Conclusioni della tesi
- Ringraziamenti
- Bibliografia, dove sono raccolte le citazioni alla letteratura scientifica e alle fonti utilizzate per scrivere la tesi
