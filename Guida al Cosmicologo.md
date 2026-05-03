# 📖 Il Cosmicologo - AV Edition 🔞
## Guida Completa per l'Utilizzo

---

## 📋 Indice
1. [Introduzione](#introduzione)
2. [Caratteristiche Principali](#caratteristiche-principali)
3. [Gestione Film](#gestione-film)
4. [Ricerca e Filtri](#ricerca-e-filtri)
5. [Gestione Alias](#gestione-alias)
6. [Import/Export](#importexport)
7. [Statistiche](#statistiche)
8. [Modalità Dark](#modalità-dark)
9. [Formati Supportati](#formati-supportati)
10. [Domande Frequenti](#domande-frequenti)

---

## 🎬 Introduzione

**Il Cosmicologo - AV Edition** è un'applicazione web completa per la gestione e catalogazione di una collezione di film. È costruita in HTML/CSS/JavaScript puro e funziona completamente nel browser con salvataggio automatico in localStorage.

### Caratteristiche Principali
- ✅ Gestione completa del database
- ✅ Ricerca avanzata con alias
- ✅ Import/Export in 3 formati
- ✅ Statistiche in tempo reale
- ✅ Dark mode integrata
- ✅ Responsive design
- ✅ Paginazione automatica
- ✅ Salvataggio locale permanente

---

## 🌟 Caratteristiche Principali

### 1. **Database Locale**
- I dati sono salvati automaticamente nel **localStorage del browser**
- Non richiede server o connessione internet
- I dati persistono tra le sessioni
- Supporta centinaia di film senza rallentamenti

### 2. **Interfaccia Intuitiva**
- Layout responsive che si adatta a desktop e mobile
- Moduli di inserimento ordinati e facili da usare
- Tabella interattiva con hover effects
- Toast notifications per feedback immediato

### 3. **Ricerca Intelligente**
- Ricerca in tempo reale mentre digiti
- Supporta ricerca per Studio, Attrici, Titolo, Genere
- Sistema di alias per trovare film con nomi alternativi
- Evidenziazione dei risultati trovati

### 4. **Gestione Avanzata**
- Modifica rapida di singoli film
- Eliminazione con conferma
- Annulla l'ultima eliminazione
- Ordinamento per qualsiasi colonna

---

## 🎥 Gestione Film

### Aggiungere un Film

1. **Compilare il Modulo di Inserimento**:
   - **Studio**: Nome dello studio/produttore
   - **Attrici**: Nomi separati da virgola (es: `Anna, Maria, Giulia`)
   - **Titolo**: Titolo del film (obbligatorio)
   - **Genere**: Genere/categoria (es: `azione, commedia`)
   - **URL Locandina**: Link all'immagine della locandina (opzionale)
   - **Nome Disco**: Identificativo del disco/cartella (opzionale)

2. **Fare clic su "➕ Aggiungi Film"**
3. Ricevi conferma con toast notification ✅

**Nota**: Il film non verrà aggiunto se manca il Titolo o se esiste già un film identico.

### Modificare un Film

1. **Fare clic su "✏️"** nella riga del film da modificare
2. Il modulo si popola automaticamente con i dati del film
3. Modificare i campi desiderati
4. Il bottone cambia in **"💾 Salva Modifiche"**
5. Fare clic per salvare
6. Ricevi conferma della modifica ✏️

### Eliminare un Film

1. **Fare clic su "🗑️"** nella riga del film
2. Confermare l'eliminazione (non sarà reversibile finché non ricarichi la pagina)
3. Il bottone **"♻️ Annulla"** appare per ripristinare l'ultimo film eliminato
4. Clicca "♻️ Annulla" per ripristinare entro la stessa sessione

### Svuotare il Database

- **Pulsante "🗑️ Svuota"** nella toolbar elimina TUTTI i film
- Richiede conferma
- Questa azione non può essere annullata
- Usa con cautela!

---

## 🔍 Ricerca e Filtri

### Ricerca Base

- **Campo di ricerca "🔍 Cerca nel tuo archivio..."**
- Digita per filtrare film in tempo reale
- La ricerca è case-insensitive (maiuscole/minuscole non importa)
- Cerca in: Studio, Attrici, Titolo, Genere

### Ricerca Avanzata con Alias

Il sistema di alias permette di trovare film anche usando nomi alternativi:

**Esempio**:
- Se configuri un alias per "Dee Williams" → `dee williams, darling, sharon darling`
- Cercando "darling" troverai tutti i film di "dee williams"
- La ricerca espande automaticamente i termini agli alias configurati

### Ordinamento

- **Clicca sull'intestazione di qualsiasi colonna** per ordinare
- Primo clic: ordine crescente (A→Z)
- Secondo clic: ordine decrescente (Z→A)
- L'ordinamento si applica ai risultati filtrati

### Paginazione

- Se ci sono più di 10 film visualizzati, appare il controllo di paginazione
- Naviga con **"◀ Prev"** e **"Next ▶"**
- Mostra: `Pagina attuale / Totale pagine`
- I pulsanti si disabilitano automaticamente ai limiti

---

## 🏷️ Gestione Alias

Gli alias permettono di ricercare un'attrice usando nomi alternativi, pseudonimi o varianti.

### Aprire il Gestione Alias

- **Clicca il bottone "🏷️ Alias"** nel modulo di inserimento
- Si apre una modale con i controlli di gestione

### Aggiungere un Alias

1. Nel campo "Nome principale": inserisci il nome principale (es: `maria rossi`)
2. Nel campo "alias1,alias2,alias3": inserisci gli alias separati da virgola
   - Esempio: `maria r, mr, maria`
3. Clicca **"+ Aggiungi"**
4. L'alias appare nella lista sopra

**Formato**: `Nome Principale;alias1,alias2,alias3`

### Visualizzare gli Alias Configurati

- La lista mostra tutti gli alias configurati
- Nome principale in **blu** (primario)
- Alias associati in piccolo grigio sotto

### Eliminare un Alias

- Clicca **"Elimina"** accanto all'alias che vuoi rimuovere
- Richiede conferma
- I film non vengono eliminati, solo gli alias

### Ripristinare gli Alias di Default

- Clicca **"Ripristina Default"** nella modale
- Ritorna ai 3 alias di esempio originali:
  - `nome principale` → [alias1, alias2, nome principale]
  - `dee williams` → [dee williams, darling, sharon darling]
  - `samantha tits` → [samantha tits, melody ura, cecilia boom, cresina]

**Nota**: Gli alias importati da file vengono salvati automaticamente in localStorage.

---

## 📥📤 Import/Export

### Esportare i Dati

#### **📄 Esporta TXT**
- Esporta in formato testo semplice
- Formato riga: `Studio - Attrici - Titolo _ Genere`
- Include sezione alias alla fine
- File: `Cosmicologo AVE.txt`

**Esempio**:
```
Studio A - Attrice 1, Attrice 2 - Titolo Film _ azione, commedia
Studio B - Attrice 3 - Titolo Film 2 _ horror

### ALIAS ###
dee williams;dee williams,darling,sharon darling
```

#### **📊 Esporta CSV**
- Formato Excel/Fogli Google compatibile
- Colonne: Studio | Attrici | Titolo | Genere | Locandina | Disco
- Include sezione alias
- File: `Cosmicologo AVE.csv`

#### **💻 Backup JSON**
- Formato JSON completo con metadati
- Include versione, data, count film, count alias
- Retrocompatibile con vecchie versioni
- File: `Cosmicologo AVE.json`

**Struttura JSON**:
```json
{
  "versione": "1.0",
  "data": "2024-01-15T10:30:45.123Z",
  "filmCount": 42,
  "aliasCount": 5,
  "film": [...],
  "alias": {...}
}
```

#### **🤖 Esporta Telegram**
- Formato ottimizzato per condivisione su Telegram
- Include hashtag automatici per ogni field
- Formattazione con emoji e separatori
- File: `Cosmicologo AVE TG.txt`

**Formato**:
```
Studio A - Attrice 1 - Titolo Film

🎬 #Studio_A
🚺 #Attrice_1
🏷 #azione, #commedia
━━━━━━━━━━
```

### Importare i Dati

#### **📁 Importa TXT**
1. Clicca **"📁 TXT"** (bottone turchese chiaro)
2. Seleziona un file `.txt` creato da questa app
3. Inserisce i film + gli alias nel database
4. Ricevi conferma con numero di film importati

#### **📁 Importa CSV**
1. Clicca **"📁 CSV"** (bottone turchese)
2. Seleziona un file `.csv` con struttura corretta
3. Deve avere almeno Studio, Attrici, Titolo
4. Importa gli alias se presenti nella sezione finale

**Formato CSV atteso**:
```
Studio,Attrici,Titolo,Genere,Locandina,Disco
Studio A,"Attrice 1, Attrice 2",Titolo Film,azione,http://...,Disco1
```

#### **📁 Importa JSON**
1. Clicca **"📁 JSON"** (bottone azzurro)
2. Seleziona un file `.json` da backup precedente
3. Supporta sia formato vecchio (array) che nuovo (oggetto)
4. Importa film e alias automaticamente

### Gestione Duplicati

- L'app previene l'importazione di film duplicati
- Un film è considerato duplicato se ha **Titolo + Studio identici**
- Se provi a importare un duplicato, viene saltato silenziosamente
- Ricevi comunque il numero esatto di film importati

---

## 📊 Statistiche

### Visualizzare le Statistiche

- Clicca **"🏆 Top 5 - Visualizza Statistiche Approfondite 📊"**
- La sezione si espande mostrando 3 carte

### Dati Mostrati

1. **🏢 Top 5 Studio**
   - I 5 studio più rappresentati nel tuo archivio
   - Numero di film per ogni studio

2. **🚺 Top 5 Attrici**
   - Le 5 attrici più presenti
   - Conta gli stessi nomi anche se in righe diverse
   - Conta l'alias come lo stesso nome

3. **#️⃣ Top 5 Generi**
   - I 5 generi più frequenti
   - Generi multipli vengono contati singolarmente
   - Se un film ha genere "azione, commedia", entrambi vanno nel conteggio

### Aggiornamento Automatico

- Le statistiche si aggiornano ogni volta che:
  - Aggiungi un film
  - Modifichi un film
  - Elimini un film
  - Esporti/Importi film
  - Ripristini un film

---

## 🌙 Modalità Dark

### Attivare/Disattivare

- Clicca il bottone **"🌙"** nella toolbar
- Alterna istantaneamente tra light e dark mode
- L'impostazione si salva automaticamente in localStorage

### Colori Dark Mode

- **Background**: Grigio scuro (#1a1a1a)
- **Testo**: Grigio chiaro (#e0e0e0)
- **Contenitori**: Grigio molto scuro (#2d2d2d)
- **Accent**: Azzurro (per contrasto)

### Persistenza

- Se attivi dark mode, rimane attiva anche ricaricando la pagina
- Salvato in: `localStorage['darkMode']`

---

## 💾 Salvataggio Automatico

### Quando Vengono Salvati i Dati

1. **Dopo ogni azione**:
   - Aggiunta film
   - Modifica film
   - Eliminazione film
   - Importazione film
   - Aggiunta/eliminazione alias

2. **Memorizzazione**:
   - Film: `localStorage['filmDB_textOnly']`
   - Alias: `localStorage['aliasDB']`
   - Dark mode: `localStorage['darkMode']`

### Recupero Dati

- All'apertura della pagina, carica automaticamente:
  - Ultimo database salvato
  - Ultimi alias configurati
  - Ultima preferenza di dark mode

### Backup Consigliati

⚠️ **Avviso di Backup**:
- Appare dopo 5+ modifiche senza backup
- Colore rosso: "⚠️ Salva il backup!"
- Scompare dopo aver esportato un backup

---

## 📋 Formati Supportati

### Campi Film

Ogni film ha questi campi (salvati nel database):

| Campo | Tipo | Obbligatorio | Descrizione |
|-------|------|--------|-------------|
| **Studio** | Testo | No | Nome dello studio/produttore |
| **Attrici** | Testo | No | Nomi separati da virgola |
| **Titolo** | Testo | **Sì** | Titolo film (identificativo) |
| **Genere** | Testo | No | Genere/categoria (virgola per multipli) |
| **Locandina** | URL | No | Link a immagine locandina |
| **Disco** | Testo | No | Identificativo disco/cartella |

### Generi Codificati

L'app riconosce automaticamente questi generi e li colora:

| Genere | Colore | Badge |
|--------|--------|-------|
| `compilation`, `porn_for_women` | Verde | azione |
| `bbw`, `ssbbw`, `muscular` | Arancione | commedia |
| `incest`, `family` | Rosso | drammatico |
| `bdsm`, `extreme`, `fisting`, `prolapse` | Nero | horror |
| `pregnant` | Rosa chiaro | sci-fi |
| `piss`, `puke`, `scat` | Marrone | mafia |
| `futanari`, `transsexual`, `pegging` | Viola | thriller |

---

## ❓ Domande Frequenti

### D: Dove sono salvati i miei dati?
**R**: Nel browser, in `localStorage`. Non vengono caricati su server. Rimangono sul tuo computer/dispositivo.

### D: Posso usare questa app offline?
**R**: Sì! Una volta caricata, funziona completamente offline. I dati vengono salvati localmente.

### D: Cosa succede se cancello i dati del browser?
**R**: Perderai il database e gli alias. Mantieni sempre un backup JSON sul computer!

### D: Quanti film posso aggiungere?
**R**: Teoricamente illimitati, ma localStorage ha un limite di ~5-10 MB. Saranno migliaia di film.

### D: Come faccio a condividere il mio database con un'altra persona?
**R**: Esporta in JSON, invia il file, l'altra persona lo importa nella sua installazione.

### D: Posso modificare un film?
**R**: Sì! Clicca il bottone ✏️ nella riga del film. Modifica e salva le modifiche.

### D: L'annulla funziona sempre?
**R**: Solo per l'ultima eliminazione, nella stessa sessione del browser. Se ricarichi la pagina, non potrai più annullare.

### D: Come funziona la ricerca con alias?
**R**: Se configuri "maria" con alias "mr, m.r.", cercando "mr" troverai tutti i film di "maria".

### D: Posso ordinare in modo personalizzato?
**R**: Clicca l'intestazione di qualsiasi colonna (Studio, Attrici, Titolo, Genere) per ordinare A→Z o Z→A.

### D: La locandina è obbligatoria?
**R**: No! È opzionale. Se non metti un URL, vedrai "❌" nella colonna HDD. Hover sopra per non visualizzare nulla.

### D: Cosa significa la colonna HDD?
**R**: È il campo "Disco" - l'identificativo del disco/cartella dove il film è salvato. Purely informativo.

### D: Posso usarla su mobile?
**R**: Sì! L'app è responsive. Non tutti i pulsanti sono però funzionali al 100% su mobile (meglio desktop per modifiche).

### D: Come faccio un backup del mio database?
**R**: Clicca **"💾 JSON"** per esportare in formato JSON. Salva il file sul computer.

### D: Posso importare file da Excel?
**R**: Sì! Esporta il tuo foglio Excel come CSV, poi usa **"📁 CSV"** per importare. Assicurati le colonne siano nello stesso ordine.

### D: Le statistiche si aggiornano in tempo reale?
**R**: Sì! Ogni volta che modifichi il database, le statistiche si ricalcolano automaticamente. Vedi i numeri aggiornati dopo ogni azione.

### D: Posso avere più copie della app aperte?
**R**: Sì, ma condividono lo stesso localStorage. Se modifichi in una finestra, l'altra non si aggiornerà (ricarica per vedere i cambiamenti).

### D: Come resetto tutto ai valori di default?
**R**: Per gli alias: clicca "Ripristina Default". Per i film: usa "🗑️ Svuota". Non c'è modo di resettare l'intero localStorage da qui (usa il browser dev tools).

---

## 🛠️ Struttura Tecnica

### Stack Tecnologico
- **HTML5**: Markup semantico
- **CSS3**: Design responsive con variabili CSS
- **JavaScript (Vanilla)**: Logica applicativa pura
- **LocalStorage API**: Persistenza dati
- **File API**: Import/Export

### Nessuna Dipendenza
L'app è completamente indipendente. Non richiede:
- ❌ Framework (React, Vue, etc)
- ❌ Librerie esterne (jQuery, etc)
- ❌ Server/Backend
- ❌ Connessione internet

### Performance
- ⚡ Caricamento istantaneo
- ⚡ Ricerca in tempo reale
- ⚡ Salvataggio automatico
- ⚡ Lazy loading immagini

---

## 📝 Note Finali

### Consigli per l'Uso

1. **Backup Regolari**: Esporta in JSON ogni settimana
2. **Alias Organizzati**: Mantieni alias coerenti e riconoscibili
3. **Titoli Unici**: Usa titoli univoci per evitare confusione
4. **Generi Standardizzati**: Usa gli stessi generi, non variazioni
5. **Pulizia Periodica**: Rimuovi film non più nella collezione

### Limiti Conosciuti

- ⚠️ LocalStorage è specifico del browser (non sincronizzato)
- ⚠️ Eliminare dati del browser cancella il database
- ⚠️ La ricerca è case-insensitive (non distingue maiuscole)
- ⚠️ Non supporta upload di immagini (solo URL)

### Suggerimenti per Miglioramenti Futuri

- API cloud sync
- Upload locandine direttamente
- Filtri multipli avanzati
- Esportazione PDF
- Integrazione Telegram bot
- Condivisione lista pubblica

---

## 📞 Supporto

Questa app è standalone e open. Se riscontri problemi:

1. Verifica che il browser supporti localStorage
2. Prova a disabilitare le estensioni del browser
3. Controlla la console (F12) per eventuali errori
4. Fai un backup prima di esperimenti
5. Prova con un browser diverso

---

**Buon catalogo! 🎬🍿**

*Ultima Revisione: 2024*
*Versione: 1.0*
