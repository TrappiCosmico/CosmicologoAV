# ⚡ Guida: Funzione "Incolla Rapido"

## 🎯 Cos'è

La funzione **"Incolla Rapido"** è un campo speciale che ti permette di inserire dati in formato compatto:

```
Studio - Attrici - Titolo
```

I dati verranno automaticamente divisi e assegnati ai rispettivi campi del form.

---

## 📋 Formato Atteso

```
FORMATO:  Studio - Attrici - Titolo
```

### Componenti
- **Studio**: Nome dello studio/produttore
- **Attrici**: Nomi delle attrici (separati da virgola se più di una)
- **Titolo**: Titolo del film

### Separatore
- Usa esattamente **` - `** (spazio-trattino-spazio) come separatore

---

## 💡 Esempi di Utilizzo

### Esempio 1: Singola Attrice
```
Input:
WarnerBros - Keanu Reeves - The Matrix

Risultato:
Studio: WarnerBros
Attrici: Keanu Reeves
Titolo: The Matrix
```

### Esempio 2: Più Attrici
```
Input:
WarnerBros - Keanu Reeves, Laurence Fishburne - The Matrix

Risultato:
Studio: WarnerBros
Attrici: Keanu Reeves, Laurence Fishburne
Titolo: The Matrix
```

### Esempio 3: Titolo con Trattini
```
Input:
MGM - Sean Connery, Honor Blackman - From Russia - with Love

Risultato:
Studio: MGM
Attrici: Sean Connery, Honor Blackman
Titolo: From Russia - with Love

NOTA: Il titolo può contenere " - " - la funzione lo gestisce!
```

### Esempio 4: Studio Composito
```
Input:
Universal Pictures - Scarlett Johansson, Chris Evans - Black Widow

Risultato:
Studio: Universal Pictures
Attrici: Scarlett Johansson, Chris Evans
Titolo: Black Widow
```

---

## 🚀 Come Usarla

### Step 1: Localizza il Campo
Troverai il campo **"⚡ Incolla Rapido"** sotto la riga di Genere/Locandina/Disco.

### Step 2: Incolla o Digita il Dato
Formato: `Studio - Attrici - Titolo`

Esempio:
```
WarnerBros - Keanu Reeves, Laurence Fishburne - The Matrix
```

### Step 3: Premi ENTER
- Premi **INVIO** o **ENTER** sulla tastiera
- Oppure fai Ctrl+Enter

### Step 4: Controlla i Campi
I tre campi si popoleranno automaticamente:
- Studio ✅
- Attrici ✅
- Titolo ✅

### Step 5: Completa gli Altri Campi
Se vuoi aggiungere:
- Genere
- URL Locandina
- Nome Disco

Compila questi campi manualmente (sono opzionali).

### Step 6: Clicca "➕ Aggiungi Film"
Il film verrà inserito nel database.

---

## ✨ Caratteristiche

### ⚡ Automatico
- Parsing automatico al pressione di ENTER
- Focus automatico su Genere dopo il parsing
- Campo Incolla Rapido si svuota dopo l'uso

### 🔍 Validazione
- Controlla che il formato sia corretto
- Verifica che nessun campo sia vuoto
- Mostra messaggi di errore chiari

### 🎯 Intuitivo
- Messaggio di conferma: "✅ Campi compilati!"
- Feedback immediato con toast notification
- Se sbagliato: "❌ Formato non valido!"

### ✅ Intelligente
- Gestisce titoli con ` - ` al interno
- Trim automatico degli spazi
- Case-sensitive (mantiene maiuscole/minuscole)

---

## ⚠️ Errori Comuni

### ❌ Errore 1: Formato Sbagliato
```
❌ SBAGLIATO:
WarnerBros, Keanu Reeves, The Matrix     (virgola al posto di -)
WarnerBros -Keanu Reeves- The Matrix     (spazi mancanti)
WarnerBros - Keanu Reeves The Matrix     (manca ultimo -)

✅ CORRETTO:
WarnerBros - Keanu Reeves - The Matrix
```

### ❌ Errore 2: Campo Vuoto
```
❌ SBAGLIATO:
- Keanu Reeves - The Matrix    (Studio vuoto)
WarnerBros -  - The Matrix     (Attrici vuoto)
WarnerBros - Keanu Reeves -    (Titolo vuoto)

✅ CORRETTO:
WarnerBros - Keanu Reeves - The Matrix
```

### ❌ Errore 3: Separatore Errato
```
❌ SBAGLIATO:
WarnerBros| Keanu Reeves | The Matrix    (pipe al posto di -)
WarnerBros-- Keanu Reeves-- The Matrix   (doppio trattino)

✅ CORRETTO:
WarnerBros - Keanu Reeves - The Matrix
```

---

## 📊 Workflow Consigliato

### Scenario 1: Inserimento Rapido (Solo Essenziale)
```
1. Incolla: WarnerBros - Keanu Reeves - The Matrix
2. Premi ENTER
3. Clicca "➕ Aggiungi Film"
4. FATTO! ✅
```

**Tempo**: ~3 secondi

### Scenario 2: Inserimento Completo
```
1. Incolla: WarnerBros - Keanu Reeves - The Matrix
2. Premi ENTER
3. Compila Genere: azione, fantascienza
4. Compila URL Locandina: https://...
5. Compila Disco: Disco_01
6. Clicca "➕ Aggiungi Film"
7. FATTO! ✅
```

**Tempo**: ~30 secondi

### Scenario 3: Modifica Post-Inserimento
```
1. Incolla: WarnerBros - Keanu Reeves - The Matrix
2. Premi ENTER
3. Clicca "➕ Aggiungi Film"
4. [Film inserito]
5. Se vuoi modificare, clicca ✏️ sulla riga
6. Modifica singoli campi
7. Clicca "💾 Salva Modifiche"
```

---

## 🔄 Interazione con Altre Funzioni

### Con il Campo di Modifica
- Se stai modificando un film, il campo Incolla Rapido **non interferisce**
- Il form rimane pulito finché non clicchi "➕ Aggiungi Film"

### Con Annulla/Pulisci
- Se clicchi **"♻️ Annulla"**, il campo Incolla Rapido si svuota insieme agli altri
- Se clicchi **"🗑️ Svuota"**, tutto viene cancellato incluso il campo

### Con Import/Export
- La funzione Incolla Rapido è **locale solo nel form**
- Non viene esportata nei file TXT/CSV/JSON
- Utile solo per inserimento manuale rapido

---

## 💡 Pro Tips

### 🎯 Tip 1: Copia da Fonti Esterne
Se hai una lista in un documento, copia semplicemente la riga nel formato corretto e incolla nel campo.

### 🎯 Tip 2: Incolla Multiplo
Non puoi incollare più film contemporaneamente. Fai uno per volta, ma il processo è velocissimo (3 secondi).

### 🎯 Tip 3: Nomi con Spazi
```
✅ OK: Universal Pictures - Scarlett Johansson - Black Widow
✅ OK: 20th Century Fox - Angelina Jolie - Tomb Raider 2023
✅ OK: Paramount Pictures - Tom Cruise - Mission Impossible

I nomi sono preservati esattamente come li scrivi!
```

### 🎯 Tip 4: Gestione Attrici Multiple
```
✅ Scrivi così: Studio - Attrice1, Attrice2, Attrice3 - Titolo

Nel campo Attrici vedrai:
Attrice1, Attrice2, Attrice3

Puoi modificare dopo se necessario con ✏️
```

### 🎯 Tip 5: Titoli Complessi
```
✅ Titoli con " - ":
Studio - Attrice - Harry Potter - Chamber of Secrets
→ Titolo: Harry Potter - Chamber of Secrets

✅ Titoli con numeri:
Studio - Attrice - Fast & Furious 7
→ Titolo: Fast & Furious 7

✅ Titoli con caratteri speciali:
Studio - Attrice - The Matrix (1999)
→ Titolo: The Matrix (1999)
```

---

## 🛠️ Troubleshooting

### Problema: Il Parsing non Funziona
**Soluzione**: Verifica che il formato sia esattamente `Studio - Attrici - Titolo` con spazi intorno al trattino.

### Problema: Il Campo Rimane Vuoto dopo ENTER
**Soluzione**: È normale! Il campo si pulisce automaticamente dopo un parsing riuscito. Controlla i campi Studio, Attrici, Titolo.

### Problema: I Dati non Compaiono
**Soluzione**: Verifica che abbiate almeno 3 sezioni separate da ` - ` (spazio-trattino-spazio).

### Problema: Focus non Va su Genere
**Soluzione**: Ricarica la pagina o verifica che JavaScript sia abilitato.

---

## 📝 Note Finali

- ✅ La funzione è **completamente opzionale**
- ✅ Puoi continuare a usare il metodo manuale di compilazione
- ✅ Il campo Incolla Rapido non è obbligatorio
- ✅ Perfetto per importazioni rapide da liste esterne
- ✅ Zero effetto sugli altri campi se non usato

---

**Versione**: 1.0  
**Data Implementazione**: 2024  
**Icona**: ⚡ (Incolla Rapido)
