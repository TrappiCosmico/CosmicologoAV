# 🚀 Cosmicologo - Riepilogo Rapido

## Operazioni Veloci

### ➕ AGGIUNGERE UN FILM
1. Compila: Studio | Attrici | Titolo | Genere | URL Locandina | Disco
2. Clicca **"➕ Aggiungi Film"**
3. Ricevi conferma ✅

### ✏️ MODIFICARE UN FILM
1. Clicca **"✏️"** sulla riga del film
2. Modifica i campi
3. Clicca **"💾 Salva Modifiche"**

### 🗑️ ELIMINARE UN FILM
1. Clicca **"🗑️"** sulla riga del film
2. Conferma l'eliminazione
3. Se è l'ultimo, clicca **"♻️ Annulla"** per ripristinare

### 🔍 CERCARE FILM
- Digita nel campo di ricerca "🔍 Cerca nel tuo archivio..."
- Ricerca in: Studio, Attrici, Titolo, Genere
- Risultati in tempo reale

### 🏷️ GESTIRE ALIAS
1. Clicca bottone **"🏷️ Alias"**
2. Formato: `Nome Principale;alias1,alias2,alias3`
3. Es: `Maria Rossi;mr,maria r,m.r.`
4. I film di Maria Rossi appariranno cercando qualsiasi alias

### 📤 ESPORTARE DATI
- **📄 TXT**: Formato testo (con alias)
- **📊 CSV**: Excel/Fogli Google (con alias)
- **💾 JSON**: Backup completo (con metadati)
- **🤖 TG**: Formato Telegram (hashtag automatici)

### 📥 IMPORTARE DATI
- **📁 TXT**: Carica file .txt (con alias)
- **📁 CSV**: Carica file .csv (con alias)
- **📁 JSON**: Carica backup JSON

### 📊 STATISTICHE
Clicca **"🏆 Top 5"** per vedere:
- Top 5 Studio
- Top 5 Attrici
- Top 5 Generi

### 🌙 DARK MODE
Clicca bottone **"🌙"** per attivare/disattivare tema scuro

### 🗑️ SVUOTARE TUTTO
Clicca **"🗑️ Svuota"** per cancellare tutto il database
⚠️ Non reversibile!

---

## 📋 Campi Film

| Campo | Obbligatorio | Note |
|-------|--------|-------|
| **Studio** | ❌ No | Studio/Produttore |
| **Attrici** | ❌ No | Nomi separati da virgola |
| **Titolo** | ✅ **Sì** | Identificativo unico |
| **Genere** | ❌ No | Categoria (virgola per più) |
| **Locandina** | ❌ No | URL immagine |
| **Disco** | ❌ No | ID disco/cartella |

---

## 🎨 Generi Riconosciuti (con colore)

```
azione/commedia      → 🟩 Verde
commedia             → 🟧 Arancione
drammatico           → 🔴 Rosso
horror               → ⬛ Nero
sci-fi               → 🟥 Rosa
mafia                → 🟫 Marrone
thriller             → 🟪 Viola
```

**Generi specifici mappati**:
- Azione: `compilation`, `porn_for_women`
- Commedia: `bbw`, `ssbbw`, `muscular`
- Drammatico: `incest`, `family`
- Horror: `bdsm`, `extreme`, `fisting`, `prolapse`
- Sci-Fi: `pregnant`
- Mafia: `piss`, `puke`, `scat`
- Thriller: `futanari`, `transsexual`, `pegging`

---

## ⌨️ Scorciatoie Utili

| Azione | Come |
|--------|------|
| **Ordinare** | Clicca intestazione colonna (Studio, Attrici, Titolo, Genere) |
| **Pagina successiva** | Clicca **"Next ▶"** |
| **Pagina precedente** | Clicca **"◀ Prev"** |
| **Annulla eliminazione** | Clicca **"♻️ Annulla"** (solo ultima) |
| **Vai in cima** | Scroll up automatico dopo modifica |
| **Dark mode** | Clicca **"🌙"** |

---

## 💾 Salvataggio Automatico

✅ I dati si salvano automaticamente:
- Dopo ogni aggiunta film
- Dopo ogni modifica
- Dopo ogni eliminazione
- Dopo ogni importazione
- Dopo ogni cambio alias

📍 Salvati in: `localStorage` del browser
🔄 Caricati automaticamente all'apertura

---

## 📊 Contatori Info

Nella barra info vedi:
- **Totale**: Numero totale film nel database
- **Trovati**: Film risultanti dalla ricerca attuale
- **Aggiornato**: Data/ora ultimo aggiornamento
- **⚠️ Salva il backup!**: Appare dopo 5+ modifiche

---

## 🔐 Privacy & Dati

✅ **Nessun invio dati**
- I dati rimangono nel tuo computer
- Nessun server, nessun cloud
- Nessuna traccia online
- Completamente offline

⚠️ **Rischi**
- Se cancelli localStorage del browser: perdi tutto
- Se disattivi localStorage: l'app non funziona
- Se cambi browser: dati non sincronizzati

---

## 🆘 FAQ Veloce

**D: Dove sono i miei dati?**
R: In `localStorage` del browser, sul tuo computer

**D: Posso usarla offline?**
R: Sì, completamente offline dopo il primo caricamento

**D: Quanto spazio occupa?**
R: Pochi MB nel localStorage

**D: Perdo i dati ricaricando?**
R: No, sono salvati automaticamente

**D: Posso esportare?**
R: Sì! TXT, CSV, JSON. Clicca i bottoni nella toolbar

**D: Posso importare backup vecchi?**
R: Sì! JSON retrocompatibile con versioni precedenti

**D: Supporta mobile?**
R: Sì, responsive! Ma meglio desktop per input

**D: Posso avere backup automatici?**
R: No, ma puoi esportare JSON quando vuoi

**D: Quanti film posso avere?**
R: Migliaia! localStorage supporta ~5-10 MB

**D: Come resetto tutto?**
R: Clicca "🗑️ Svuota" - ⚠️ Irreversibile!

---

## 🎬 Workflow Consigliato

### **Installazione Iniziale**
1. Apri l'app nel browser
2. Aggiungi i tuoi primi film
3. Configura gli alias per le attrici frequenti
4. Attiva dark mode se preferisci

### **Uso Giornaliero**
1. Aggiungi/modifica film come necessario
2. Usa la ricerca per trovare filmografia
3. Consulta statistiche per overview
4. Dark mode notturna

### **Manutenzione Settimanale**
1. Esporta backup JSON (salva sul PC)
2. Pulisci alias non usati
3. Verifica statistiche
4. Aggiorna locandine se necessario

---

## 🎯 Consigli Pro

💡 **Alias intelligenti**: Crea alias per abbreviazioni, pseudonimi e varianti nome

💡 **Generi coerenti**: Usa sempre gli stessi generi (es: "azione" non "action")

💡 **Titoli univoci**: Non usare lo stesso titolo per produttori diversi

💡 **Backup regolari**: Esporta JSON settimanalmente, salva su Dropbox/Drive

💡 **Locandine**: Usa URL pubblici stabili (non link temporanei)

💡 **Ricerca rapida**: Gli alias rendono la ricerca potentissima!

---

## 📝 Formati Export

### **TXT** (Leggibile)
```
Studio A - Attrice 1, Attrice 2 - Titolo _ azione, commedia

### ALIAS ###
attrice1;attrice1,a1,att.1
```

### **CSV** (Excel)
```
Studio,Attrici,Titolo,Genere,Locandina,Disco
Studio A,"Attrice 1, Attrice 2",Titolo,azione,http://...,Disco1
```

### **JSON** (Backup)
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

### **Telegram** (Social)
```
Studio A - Attrice 1 - Titolo

🎬 #Studio_A
🚺 #Attrice_1
🏷 #azione, #commedia
━━━━━━━━━━
```

---

**Versione**: 1.0  
**Ultimo Aggiornamento**: 2024  
**Licenza**: Open Source
