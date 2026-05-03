# 🗺️ Mappa Visuale - Il Cosmicologo

```
┌────────────────────────────────────────────────────────────────────────────┐
│                    📖 IL COSMICOLOGO - AV EDITION 🔞                        │
│                                                                              │
│  TITOLO: Titolo Principale Centrato                                         │
│  TEMA: Light/Dark mode automatico                                           │
└────────────────────────────────────────────────────────────────────────────┘

┌─ SEZIONE 1: MODULO DI INSERIMENTO ─────────────────────────────────────────┐
│                                                                              │
│  ┌─ RIGA 1 ────────────────────────────────────────────────────────────────┐
│  │  [🏢 Studio]        [🚺 Attrici]         [📝 Titolo]      [🏷️ Alias]   │
│  │  (1fr)              (2fr)                (2fr)             (1fr)         │
│  └──────────────────────────────────────────────────────────────────────────┘
│                                                                              │
│  ┌─ RIGA 2 ────────────────────────────────────────────────────────────────┐
│  │  [#️⃣ Genere]        [🖼️ URL Locandina]   [💿 Disco]    [➕ Aggiungi]   │
│  │  (2fr)              (2fr)                (1fr)           (1fr)           │
│  └──────────────────────────────────────────────────────────────────────────┘
│                                                                              │
│  ⚙️ editIndex = Campo nascosto (indice per modifica)                        │
│                                                                              │
│  Autocomplete (Datalist):                                                   │
│  - listaStudio (da database)                                                │
│  - listaAttrici (da database)                                               │
│  - listaGenere (da database)                                                │
└────────────────────────────────────────────────────────────────────────────┘

┌─ SEZIONE 2: RICERCA ───────────────────────────────────────────────────────┐
│                                                                              │
│  [🔍 Cerca nel tuo archivio...]  ← Ricerca in tempo reale                   │
│                                                                              │
│  Ricerca su:                                                                │
│  - Studio  ✓                                                                │
│  - Attrici ✓ (con espansione alias)                                        │
│  - Titolo  ✓                                                                │
│  - Genere  ✓                                                                │
│                                                                              │
│  Risultati: Case-insensitive, live filtering                                │
│  Paginazione: Automatica ogni 10 film                                       │
└────────────────────────────────────────────────────────────────────────────┘

┌─ SEZIONE 3: STATISTICHE (COLLAPSIBILE) ────────────────────────────────────┐
│                                                                              │
│  ┌─ HEADER (Clickable) ───────────────────────────────────────────────────┐
│  │ 🏆 Top 5 - Visualizza Statistiche Approfondite 📊                  [▼]   │
│  └────────────────────────────────────────────────────────────────────────┘
│                                                                              │
│  [Se Aperto - Grid 3 colonne]:                                              │
│  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐            │
│  │ 🏢 Top 5 Studio │  │ 🚺 Top 5 Attrici│  │ #️⃣ Top 5 Generi│            │
│  ├─────────────────┤  ├─────────────────┤  ├─────────────────┤            │
│  │ 1. Studio A (8) │  │ 1. Attrice X(15)│  │ 1. azione (22)  │            │
│  │ 2. Studio B (6) │  │ 2. Attrice Y(12)│  │ 2. commedia(18) │            │
│  │ 3. Studio C (5) │  │ ...             │  │ ...             │            │
│  └─────────────────┘  └─────────────────┘  └─────────────────┘            │
│                                                                              │
│  Aggiornamento: Automatico dopo ogni modifica                               │
└────────────────────────────────────────────────────────────────────────────┘

┌─ SEZIONE 4: TOOLBAR (Azioni) ──────────────────────────────────────────────┐
│                                                                              │
│  ┌─ GRUPPO 1: Import/Export/Tools ──────────────────────────────────────────┐
│  │                                                                           │
│  │  [🌙] [📁TXT] [📁CSV] [📁JSON] [🤖TG] [💾TXT] [💾CSV] [💾JSON]          │
│  │      Import           Import    Export                                   │
│  │                                                                           │
│  │  Colori:                                                                 │
│  │  - 🌙 Grigio scuro (dark mode toggle)                                   │
│  │  - 📁 Turchese (import)                                                 │
│  │  - 💾 Azzurro (export)                                                  │
│  │  - 🤖 Cyan (telegram)                                                   │
│  │                                                                           │
│  └──────────────────────────────────────────────────────────────────────────┘
│                                                                              │
│  ┌─ GRUPPO 2: Utility ──────────────────────────────────────────────────────┐
│  │                                                                           │
│  │  [♻️ Annulla] (nascosto fino a delete)  [🗑️ Svuota]                     │
│  │                                                                           │
│  │  File Input (nascosti):                                                  │
│  │  - fileImportTxt                                                         │
│  │  - fileImportJson                                                        │
│  │  - fileImportCsv                                                         │
│  │                                                                           │
│  └──────────────────────────────────────────────────────────────────────────┘
│                                                                              │
│  ⚡ Azioni:                                                                 │
│  - Import/Export: File handling tramite Blob                                │
│  - Dark mode: Toggle su body.classList                                      │
│  - Undo: Ripristina ultimoFilmEliminato                                     │
│  - Clear: Rimuove tutto il database                                         │
│                                                                              │
└────────────────────────────────────────────────────────────────────────────┘

┌─ SEZIONE 5: INFO BAR ──────────────────────────────────────────────────────┐
│                                                                              │
│  Totale: [42]  |  Trovati: [38]  |  ⚠️ Salva il backup!  |  Aggiornato: XX:XX:XX
│                                                                              │
│  Info in tempo reale:                                                       │
│  - Totale: Numero totale film                                               │
│  - Trovati: Film che matchano la ricerca                                    │
│  - Backup Warning: Dopo 5+ modifiche                                        │
│  - Timestamp: Ultimo aggiornamento                                          │
│                                                                              │
└────────────────────────────────────────────────────────────────────────────┘

┌─ SEZIONE 6: TABELLA FILM ──────────────────────────────────────────────────┐
│                                                                              │
│  HEADER (Clickable per ordinamento):                                        │
│  ┌──────┬─────────┬──────────┬───────────┬─────────┬────────┐              │
│  │ HDD  │ Studio  │ Attrici  │ Titolo    │ Genere  │ Azioni │              │
│  │ 70px │ (sort)  │ (sort)   │ (sort)    │ (sort)  │ 70px   │              │
│  └──────┴─────────┴──────────┴───────────┴─────────┴────────┘              │
│                                                                              │
│  RIGHE (una per film):                                                      │
│  ┌──────┬─────────────────┬────────────────────┬──────────────────┬────────┐ │
│  │ 🖼️   │ Studio A        │ Attrice 1, Att.2   │ [Titolo + Hover] │ ✏️ 🗑️  │ │
│  │      │                 │                    │   [Preview Img]  │        │ │
│  │ ❌   │ ...             │ ...                │ ...              │ ...    │ │
│  └──────┴─────────────────┴────────────────────┴──────────────────┴────────┘ │
│                                                                              │
│  COLONNA HDD:                                                               │
│  - Se Locandina: 🖼️ (hover mostra preview 576x576)                        │
│  - Se No: ❌                                                                │
│                                                                              │
│  COLONNA Genere:                                                            │
│  - Badge colorati per genere                                                │
│  - Più generi = più badge sulla stessa riga                                 │
│                                                                              │
│  COLONNA Azioni:                                                            │
│  - ✏️ Edit: Popola form e scroll su                                         │
│  - 🗑️ Delete: Richiede conferma                                            │
│                                                                              │
│  Interazioni:                                                               │
│  - Click header: Ordina per quella colonna                                  │
│  - Hover riga: Evidenzia con colore azzurro (rgba 52,152,219, 0.1)        │
│  - Click ✏️: Carica film nel modulo                                         │
│  - Click 🗑️: Elimina con conferma                                          │
│                                                                              │
│  Paginazione:                                                               │
│  - 10 film per pagina                                                       │
│  - Controlli sotto tabella                                                  │
│                                                                              │
└────────────────────────────────────────────────────────────────────────────┘

┌─ SEZIONE 7: PAGINAZIONE ──────────────────────────────────────────────────┐
│                                                                              │
│                    [◀ Prev] [2 / 5] [Next ▶]                                │
│                                                                              │
│  Controlli:                                                                 │
│  - Prev: Disabilitato se pagina 1                                           │
│  - Next: Disabilitato se ultima pagina                                      │
│  - Mostra: Pagina attuale / Pagine totali                                   │
│                                                                              │
│  Logica:                                                                    │
│  - Calcolo automatico: Math.ceil(filmFiltrati / 10)                        │
│  - Reset a pagina 1 quando si fa ricerca                                    │
│                                                                              │
└────────────────────────────────────────────────────────────────────────────┘

┌─ SEZIONE 8: MODALE ALIAS (nascosta di default) ─────────────────────────┐
│                                                                             │
│  [Overlay Semi-trasparente - 50% opacità]                                  │
│                                                                             │
│  ┌──────────────────────────────────────────────────────────────────────┐  │
│  │                    🏷️ Gestisci Alias                                 │  │
│  │                                                                      │  │
│  │  Formato: Nome Principale;alias1,alias2,alias3                     │  │
│  │                                                                      │  │
│  │  ┌──────────────────────────────────────────────────────────────┐  │  │
│  │  │ Lista Alias Configurati (scrollabile max 400px)             │  │  │
│  │  │                                                              │  │  │
│  │  │ ┌──────────────────────────────────────┐                    │  │  │
│  │  │ │ maria rossi (PRINCIPALE - Blu)       │  [Elimina]         │  │  │
│  │  │ │ maria r, mr, m.r., marie (grigio)   │                    │  │  │
│  │  │ └──────────────────────────────────────┘                    │  │  │
│  │  │                                                              │  │  │
│  │  │ ┌──────────────────────────────────────┐                    │  │  │
│  │  │ │ attrice2                             │  [Elimina]         │  │  │
│  │  │ │ attrice2, att2, a2                   │                    │  │  │
│  │  │ └──────────────────────────────────────┘                    │  │  │
│  │  └──────────────────────────────────────────────────────────────┘  │  │
│  │                                                                      │  │
│  │  Input Nuovo Alias:                                                │  │
│  │  [Nome principale]  [alias1,alias2,alias3]  [+ Aggiungi]          │  │
│  │   (flex:1)          (flex:2)                                       │  │
│  │                                                                      │  │
│  │  Bottoni:                                                           │  │
│  │  [Chiudi]              [Ripristina Default]                         │  │
│  │   (Secondary)           (Orange)                                    │  │
│  │                                                                      │  │
│  └──────────────────────────────────────────────────────────────────┘  │
│                                                                             │
│  Trigger: Clicca "🏷️ Alias"                                               │
│  Chiusura: Clicca "Chiudi" o click overlay                                 │
│                                                                             │
└────────────────────────────────────────────────────────────────────────────┘

┌─ SEZIONE 9: TOAST NOTIFICATIONS ──────────────────────────────────────────┐
│                                                                              │
│  Position: Fixed in basso a destra                                          │
│  Stack: Vertical (bottom: 20px, right: 20px)                               │
│  Auto-hide: 3 secondi                                                       │
│  Animation: slideIn + fadeOut                                               │
│                                                                              │
│  Esempi:                                                                    │
│  ✅ Film aggiunto!                                                          │
│  ❌ Film già presente!                                                      │
│  💾 Modifica salvata!                                                       │
│  📄 Testo Esportato                                                         │
│  📊 CSV Esportato                                                           │
│  ⚠️ Film rimosso                                                            │
│  ♻️ Film ripristinato!                                                      │
│                                                                              │
└────────────────────────────────────────────────────────────────────────────┘

```

---

## 🔄 FLUSSO DATI

```
┌─────────────────────────────────────────────────────────────────────────┐
│                         MEMORIZZAZIONE DATI                              │
└─────────────────────────────────────────────────────────────────────────┘

INSERIMENTO FILM
    ↓
aggiungiFilm() / preparaModifica()
    ↓
Validazione (Titolo obbligatorio, no duplicati)
    ↓
Film aggiunto/modificato nel array "database"
    ↓
salvaERenderizza()
    ↓
    ├─→ localStorage.setItem('filmDB_textOnly', JSON.stringify(database))
    ├─→ renderizzaFilm()  ← Aggiorna tabella
    ├─→ aggiornaSuggerimenti()  ← Aggiorna autocomplete
    └─→ Mostra toast di conferma

────────────────────────────────────────────────────────────────────────────

ELIMINAZIONE FILM
    ↓
eliminaFilm(index)  ← Richiede conferma
    ↓
Salva copia in "ultimoFilmEliminato"
    ↓
database.splice(index, 1)
    ↓
Mostra bottone "♻️ Annulla"
    ↓
salvaERenderizza()  ← Persiste cambio
    ↓
Se ripristinaFilm(): Ripristina dall'ultima copia salvata

────────────────────────────────────────────────────────────────────────────

RICERCA
    ↓
oninput="paginaCorrente=1; renderizzaFilm()"
    ↓
Legge valore da input#cerca
    ↓
espandiTermine(query)  ← Espande agli alias
    ↓
Filtra database per match
    ↓
renderizzaFilm() aggiorna tabella filtrata
    ↓
Mostra contatore "Trovati: X"

────────────────────────────────────────────────────────────────────────────

IMPORT/EXPORT
    ↓
Utente clicca bottone export
    ↓
esportaInTXT/CSV/JSON() crea contenuto
    ↓
Blob creato con tipo MIME corretto
    ↓
scarica() crea link temporaneo e trigger click
    ↓
Browser scarica file .txt/.csv/.json
    ↓
────────────────────────────────────────────────────────────────────────────
Utente clicca bottone import
    ↓
File picker (<input type="file"> nascosto)
    ↓
importaDaTXT/CSV/JSON() legge file
    ↓
Parse contenuto (split righe, parse JSON, ecc)
    ↓
Valida formato (colonne minime, struttura)
    ↓
normalizzeFilm() standardizza ogni film
    ↓
isDuplicato() previene duplicati
    ↓
Aggiungi al database con database.unshift()
    ↓
salvaERenderizza() persiste
    ↓
Mostra contatore film importati

────────────────────────────────────────────────────────────────────────────

ALIAS
    ↓
localStorage.getItem('aliasDB')  ← Carica all'avvio
    ↓
ALIAS_MAP = {...}  ← Mappa nome → [alias1, alias2, ...]
    ↓
toggleGestioneAlias() mostra modale
    ↓
renderizzaListaAlias() popola lista
    ↓
aggiungiAlias(): Aggiunge nuovo mapping
    ↓
salvaAliasDB() persiste: localStorage.setItem('aliasDB', ...)
    ↓
Se import/export: Alias salvati insieme ai film
    ↓
espandiTermine(query) usa ALIAS_MAP per ricerca espansa

```

---

## 🎨 SCHEMA COLORI

### Light Mode
```
--primary:          #3498db (Azzurro)
--secondary:        #2c3e50 (Blu Scuro)
--success:          #27ae60 (Verde)
--warning:          #ffd966 (Giallo)
--info:             #9b59b6 (Viola)
--light:            #eff6ff (Azzurro molto chiaro)

--bg-body:          #eef2f7 (Grigio molto chiaro)
--bg-container:     white
--text-main:        #333 (Grigio scuro)
--bg-table-header:  #f2f2f2 (Grigio leggero)
--bg-input:         white
--border-color:     #ddd (Grigio bordo)

--telegram:         #0088cc (Cyan)
```

### Dark Mode
```
--bg-body:          #1a1a1a (Nero)
--bg-container:     #2d2d2d (Grigio molto scuro)
--text-main:        #e0e0e0 (Grigio chiaro)
--bg-table-header:  #3d3d3d (Grigio scuro)
--bg-input:         #404040 (Grigio scuro)
--border-color:     #555 (Grigio bordo scuro)
--light:            #3d3d3d (Grigio molto scuro)
--primary:          #3498db (Azzurro - contrast)
```

### Badge Colori (Generi)
```
.badge-azione:      #6aa84f (Verde)
.badge-commedia:    #e69138 (Arancione)
.badge-drammatico:  #e24242 (Rosso)
.badge-horror:      #000000 (Nero)
.badge-sci-fi:      #eba2a2 (Rosa chiaro)
.badge-mafia:       #895129 (Marrone)
.badge-thriller:    #9b59b6 (Viola)
```

### Bottoni
```
.btn-add:           var(--success) = Verde
.btn-import-*:      #76a5af (Turchese)
.btn-export-*:      #6fa8dc (Azzurro)
.btn-telegram:      #0088cc (Cyan)
.btn-dark-mode:     #555555 (Grigio scuro)
.btn-undo:          #7f8c8d (Grigio)
.btn-clear:         #cc0000 (Rosso)
.btn-edit:          var(--warning) = Giallo
.btn-delete:        #e74c3c (Rosso)
```

---

## 📐 DIMENSIONI RESPONSIVE

```
Desktop (> 768px):
  .form-row-1:        grid-template-columns: 1fr 2fr 2fr 1fr
  .form-row-2:        grid-template-columns: 2fr 2fr 1fr 1fr
  .container:         max-width: 1200px
  
Mobile (≤ 768px):
  .form-row-1:        grid-template-columns: 1fr (stack)
  .form-row-2:        grid-template-columns: 1fr (stack)
  .container:         responsive width
  
Tabella:
  th:width:           70px per HDD, 70px per Azioni
  td:padding:         12px
  
  
Poster Preview (Hover):
  max-width:          576px
  max-height:         576px
  Position:           Absolute right (left: 100%)
```

---

## 🔐 STORAGE ALLOCATION

```
localStorage Keys:

1. filmDB_textOnly
   └─ Tipo: JSON String
   └─ Contenuto: Array di oggetti film
   └─ Dimensione: ~100 bytes per film
   └─ Limite: ~5-10 MB totali
   └─ Caricato al startup: ✓

2. aliasDB
   └─ Tipo: JSON String
   └─ Contenuto: Oggetto {principale: [aliases]}
   └─ Dimensione: ~50 bytes per alias
   └─ Persiste: ✓

3. darkMode
   └─ Tipo: String booleano ('true'/'false')
   └─ Contenuto: Preferenza tema
   └─ Caricato al startup: ✓

TOTALE OCCUPATO (esempio):
- 500 film: ~50 KB
- 100 alias: ~5 KB
- Preferenze: <1 KB
────────────────────
TOTALE: ~55 KB (10,000x capacità disponibile)
```

---

**Ultima Revisione: 2024**
