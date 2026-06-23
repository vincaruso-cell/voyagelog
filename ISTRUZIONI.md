# VoyageLog — Istruzioni di installazione

## Cosa hai creato

Un'app web completa per il diario di viaggio che funziona nel browser del telefono.
Non serve installare nulla. Funziona su Android, iPhone e PC.

---

## FASE 1 — Pubblica l'app su GitHub Pages (gratis)

### Passo 1: Crea un account GitHub
1. Vai su **https://github.com**
2. Clicca **Sign up** e registrati (è gratis)
3. Usa la tua email Gmail

### Passo 2: Crea un repository
1. Una volta loggato, clicca il **+** in alto a destra → **New repository**
2. Nome: `voyagelog` (tutto minuscolo)
3. Seleziona **Public**
4. Spunta **Add a README file**
5. Clicca **Create repository**

### Passo 3: Carica il file index.html
1. Nella pagina del repository, clicca **Add file** → **Upload files**
2. Trascina il file `index.html` nella finestra
3. Clicca **Commit changes** (il grande pulsante verde)

### Passo 4: Attiva GitHub Pages
1. Clicca **Settings** (in alto a destra nella pagina del repository)
2. Nel menu a sinistra, clicca **Pages**
3. Sotto **Source**, seleziona **Deploy from a branch**
4. Sotto **Branch**, seleziona **main** e poi **/ (root)**
5. Clicca **Save**

### Passo 5: Accedi all'app
- Dopo 2-3 minuti, l'app sarà disponibile all'indirizzo:
  **https://TUO-USERNAME.github.io/voyagelog/**
- Sostituisci `TUO-USERNAME` con il tuo nome utente GitHub

### Aggiungi l'app al telefono (come se fosse un'app vera)
**Android (Chrome):**
1. Apri l'indirizzo nel browser Chrome
2. Tocca i tre puntini in alto a destra
3. Tocca **Aggiungi a schermata Home**

**iPhone (Safari):**
1. Apri l'indirizzo in Safari
2. Tocca il pulsante di condivisione (quadrato con freccia)
3. Tocca **Aggiungi a schermata Home**

---

## FASE 2 — Configura Google Drive (opzionale ma consigliato)

Questo ti permette di sincronizzare i dati tra telefono e PC.

### Passo 1: Crea un progetto su Google Cloud
1. Vai su **https://console.cloud.google.com**
2. Accedi con il tuo account Google (vin.caruso@gmail.com)
3. In alto, clicca su **Seleziona un progetto** → **Nuovo progetto**
4. Nome: `VoyageLog`
5. Clicca **Crea**

### Passo 2: Abilita Google Drive API
1. Nel menu a sinistra, vai su **API e servizi** → **Libreria**
2. Cerca **Google Drive API**
3. Clicca su di essa → clicca **Abilita**

### Passo 3: Crea le credenziali OAuth
1. Nel menu a sinistra, vai su **API e servizi** → **Credenziali**
2. Clicca **+ Crea credenziali** → **ID client OAuth 2.0**
3. Se richiesto, configura la **schermata di consenso OAuth**:
   - Seleziona **Esterno** → **Crea**
   - Nome app: `VoyageLog`
   - Email supporto: la tua email Gmail
   - Scorri in basso → **Salva e continua** per tutti i passaggi
4. Torna a **Credenziali** → **+ Crea credenziali** → **ID client OAuth 2.0**
5. Tipo applicazione: **Applicazione web**
6. Nome: `VoyageLog Web`
7. Sotto **Origini JavaScript autorizzate**, clicca **+ Aggiungi URI** e inserisci:
   `https://TUO-USERNAME.github.io`
8. Clicca **Crea**
9. Copia il **Client ID** che appare (es: `123456789.apps.googleusercontent.com`)

### Passo 4: Configura l'app
1. Apri VoyageLog nel browser
2. Clicca l'icona **Impostazioni** ⚙️ in alto a destra
3. Incolla il **Client ID** nel campo apposito
4. Clicca **Connetti**
5. Accedi con il tuo account Google
6. I dati si sincronizzeranno automaticamente su Drive nella cartella **VoyageLog**

---

## Come usare l'app

### Diario 📖
- Tocca **Diario** in basso
- Premi **+** per nuova voce
- Inserisci data, titolo, resoconto, meteo, vento, distanza, umore
- Le voci si salvano automaticamente

### Note 🎤
- Tocca **Note** in basso
- **Nota vocale**: premi il pulsante rosso per registrare, premi di nuovo per fermare
  - La posizione GPS viene rilevata automaticamente durante la registrazione
- **Nota testuale**: scrivi e tocca "Posizione GPS" per geolocalizzarla, poi "Salva"

### Checklist ✅
- Tocca **Liste** in basso
- Hai già 3 categorie predefinite: Viveri, Attrezzatura, Medicine
- Aggiungi categorie con **Nuova categoria**
- Aggiungi elementi con il campo di testo in fondo a ogni categoria
- Tocca il checkbox per spuntare/deselezionare
- **Reset** deseleziona tutto (utile per ripetere la lista)

### Passage Plan ⚓
- Tocca **Rotta** in basso
- Inserisci la velocità media in nodi
- Tocca **Aggiungi** per ogni waypoint:
  - Scrivi il nome (es: "Porto di Genova")
  - Le coordinate le puoi inserire a mano, prendere dal GPS, o scegliere sulla mappa
- L'app calcola automaticamente: distanza, rotta (°), ETA
- Esporta in formato **GPX** (compatibile con Navionics, OpenCPN, ecc.) o **testo**

---

## Backup dei dati

Anche senza Google Drive, puoi fare backup manuale:
1. Vai in **Impostazioni** ⚙️
2. Tocca **Esporta backup (JSON)**
3. Salva il file sul tuo dispositivo o Drive
4. Per ripristinare: **Importa backup** e scegli il file

---

## Problemi comuni

**"Il microfono non funziona"**
→ Il browser deve avere il permesso per il microfono. Quando l'app lo chiede, dì "Consenti".

**"Le note vocali non si sentono"**
→ Controlla che il volume del telefono sia alzato.

**"Il GPS non funziona"**
→ Devi essere all'aperto o con la localizzazione attiva sul telefono.

**"I dati sono scomparsi"**
→ I dati sono nel browser. Se hai cancellato la cache del browser, usa sempre il backup su Drive.

---

*VoyageLog v1.0 — Buona navigazione!* ⚓
