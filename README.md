
# Esercizio Finale – Settimana 3: Sistema Utenti Dragon Ball Edition

## 💡 Obiettivo

Sviluppare un sistema gestionale per utenti ambientato nel mondo di **Dragon Ball**, utilizzando **i principali design pattern** studiati durante il corso.

Il sistema consente di:
- Registrare un personaggio (es. Goku o Vegeta)
- Assegnare dinamicamente una strategia di attacco
- Applicare trasformazioni con potenziamenti (Decorator)
- Ricevere notifiche da eventi globali (Observer)
- Utilizzare una singola entità globale per annunci (Singleton)

---

## 🧠 Design Pattern Utilizzati

### ✅ 1. Factory Method
- Classe: `PersonaggiFactory`
- Crea personaggi (`Goku`, `Vegeta`) in modo disaccoppiato.

### ✅ 2. Strategy
- Interfaccia: `StrategiaAttacco`
- Implementazioni: `Kamehameha`, `FinalFlash`
- I personaggi possono cambiare attacco a runtime.

### ✅ 3. Decorator
- Classe astratta: `DecoratorePersonaggio`
- Implementazione: `SuperSaiyan`
- Permette di aumentare il livello di potenza senza modificare le classi originali.

### ✅ 4. Observer
- Interfaccia: `Observer`
- Soggetto osservabile: `EventoDiGioco`
- Goku/Vegeta ricevono notifiche sugli eventi del gioco.

### ✅ 5. Singleton
- Classe: `GameMaster`
- Gestisce l’annuncio globale degli eventi con un’unica istanza centralizzata.

---

## 📝 Funzionalità Dimostrate nel `Main`

- Selezione personaggio da input utente
- Visualizzazione statistiche
- Assegnazione strategia di attacco
- Trasformazione in Super Saiyan
- Notifica evento globale "Freezer è atterrato su Namecc"
- Annuncio tramite `GameMaster` (singleton)

---

## ⚠️ Pattern Facade – Non Implementato


---
