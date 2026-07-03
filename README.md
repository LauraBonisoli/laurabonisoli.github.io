# Sito personale — Laura Bonisoli

Sito statico a pagina singola, pronto per essere pubblicato gratuitamente con **GitHub Pages**.

## Struttura

```
laura-bonisoli-site/
├── index.html        ← la pagina del sito
├── assets/
│   ├── cv.pdf         ← il tuo CV (sostituiscilo quando lo aggiorni)
│   └── photo.jpg       ← foto non ancora usata nel sito (opzionale)
└── README.md
```

## Come pubblicarlo su GitHub Pages (passo passo)

### 1. Verifica/crea il tuo account GitHub
Vai su [github.com](https://github.com) e controlla se hai già un account con la tua email
(univr o personale). Se non lo trovi, creane uno nuovo — è gratuito.

### 2. Crea il repository giusto
Il nome del repository determina l'indirizzo del sito, quindi deve essere **esattamente**:

```
<tuo-username-github>.github.io
```

Esempio: se il tuo username è `laurabonisoli`, il repository deve chiamarsi
`laurabonisoli.github.io`. Il sito sarà poi raggiungibile su
`https://laurabonisoli.github.io`.

Per crearlo:
1. Clicca su **"New repository"** (icona **+** in alto a destra su GitHub).
2. Repository name: `<tuo-username>.github.io`
3. Visibilità: **Public**
4. Non aggiungere README, .gitignore o licenza (li aggiungiamo noi).
5. Clicca **Create repository**.

### 3. Carica i file
Nella pagina del repository appena creato:
1. Clicca **"uploading an existing file"** (link che appare nella pagina vuota del repo).
2. Trascina dentro **tutto il contenuto** di questa cartella (`index.html` e la cartella `assets/` con dentro `cv.pdf`) — non la cartella `laura-bonisoli-site` stessa, ma il suo contenuto.
3. Scrivi un messaggio di commit (es. "Primo caricamento sito") e clicca **Commit changes**.

### 4. Attiva GitHub Pages
1. Vai su **Settings** del repository (in alto).
2. Nel menu a sinistra clicca **Pages**.
3. Sotto "Build and deployment" → Source, seleziona **Deploy from a branch**.
4. Branch: **main**, cartella: **/ (root)** → **Save**.
5. Aspetta 1-2 minuti: comparirà un link tipo `https://<tuo-username>.github.io` — quello è il tuo sito online.

### 5. Aggiorna il CV nel tuo file .tex
Nel file `cv.tex`, sostituisci l'URL segnaposto con quello vero, ad esempio:

```latex
{\color{accent}\Mundus} \; \href{https://<tuo-username>.github.io}{<tuo-username>.github.io}
```

## Come modificare il contenuto in futuro

Tutto il testo (bio, pubblicazioni, talk, teaching, contatti) è dentro `index.html`,
in sezioni chiaramente separate e commentate. Puoi modificarlo direttamente su GitHub
(icona a matita in alto a destra sul file) senza bisogno di programmi particolari:
modifichi, scrivi un messaggio di commit, e il sito si aggiorna da solo in 1-2 minuti.

Per aggiornare il CV, carica il nuovo PDF in `assets/cv.pdf` con lo stesso nome — il link
"Download CV" nel sito continuerà a funzionare automaticamente.
