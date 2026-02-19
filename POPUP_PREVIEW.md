# 🖼️ Anteprima Smart Sender

## Popup di Gestione

Quando clicchi sul pulsante Smart Sender nella finestra di composizione, vedrai un popup con:

### Header (blu)
```
📧 Smart Sender
Gestisci le associazioni email ↔ account
```

### Statistiche
```
┌─────────────────────┬─────────────────────┐
│   Associazioni      │    Visualizzate     │
│       47            │         47          │
│    totali           │                     │
└─────────────────────┴─────────────────────┘
```

### Barra di controllo
```
┌──────────────────────────────────────────────────┐
│ 🔍 Cerca destinatario o account...               │
└──────────────────────────────────────────────────┘
[Cancella tutto] [Esporta]
```

### Lista associazioni (scrollabile)
```
┌─────────────────────────────────────────────────────────┐
│ 📨 mario.rossi@azienda.com                              │
│ Mittente: Tu Lavoro <tuo.lavoro@company.com>            │
│                                          [🗑️ Elimina]    │
├─────────────────────────────────────────────────────────┤
│ 📨 anna.bianchi@cliente.it                              │
│ Mittente: Tu Lavoro <tuo.lavoro@company.com>            │
│                                          [🗑️ Elimina]    │
├─────────────────────────────────────────────────────────┤
│ 📨 amico@gmail.com                                      │
│ Mittente: Tu Personale <tu@gmail.com>                   │
│                                          [🗑️ Elimina]    │
└─────────────────────────────────────────────────────────┘
```

### Footer
```
Smart Sender v1.0.0 - I dati sono salvati localmente
```

## Funzionalità del Popup

### 🔍 Ricerca in tempo reale
- Cerca per indirizzo destinatario
- Cerca per nome/email account mittente
- Filtraggio istantaneo mentre digiti

### 🗑️ Eliminazione selettiva
- Pulsante "Elimina" per ogni associazione
- Conferma prima di eliminare
- Aggiornamento immediato della lista

### 🧹 Cancella tutto
- Pulsante rosso "Cancella tutto"
- Doppia conferma di sicurezza
- Reset completo del database

### 💾 Esporta dati
- Download file JSON
- Include tutte le associazioni
- Nome file con data (es: smart-sender-export-2026-02-13.json)
- Formato leggibile e reimportabile

### 📊 Statistiche live
- Conteggio associazioni totali
- Conteggio associazioni visualizzate (filtrate)
- Aggiornamento automatico

## Design

- **Colori**: Blu (#4A90E2) per UI principale, Rosso (#dc3545) per azioni pericolose
- **Font**: System font nativo per massima leggibilità
- **Dimensioni**: 450-600px di larghezza, max 400px di altezza per la lista
- **Scrollbar**: Personalizzata, minimalista
- **Hover effects**: Feedback visivo su tutti i pulsanti e liste
- **Responsive**: Si adatta alla finestra del browser

## Interazioni

1. **Click su pulsante toolbar** → Apre popup
2. **Digita nella ricerca** → Filtra lista in tempo reale
3. **Click su "Elimina"** → Conferma → Rimuove associazione
4. **Click su "Cancella tutto"** → Doppia conferma → Reset totale
5. **Click su "Esporta"** → Scarica file JSON

## File JSON esportato (esempio)

```json
{
  "version": "1.0.0",
  "exported": "2026-02-13T15:24:00.000Z",
  "associations": [
    {
      "recipient": "mario.rossi@azienda.com",
      "identityId": "id123",
      "identityName": "Tu Lavoro <tuo.lavoro@company.com>"
    },
    {
      "recipient": "amico@gmail.com",
      "identityId": "id456",
      "identityName": "Tu Personale <tu@gmail.com>"
    }
  ]
}
```

## Stato vuoto

Se non ci sono ancora associazioni, il popup mostra:

```
        📭
        
  Nessuna associazione ancora
  
  Smart Sender imparerà automaticamente
  mentre invii email.
  Le associazioni appariranno qui.
```
