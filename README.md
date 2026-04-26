# PromptOS – Prompt Engineering Hub

Aggregatore open-source di 58 tecniche di prompt engineering per LLM e modelli generativi, basato sul *2024 Prompt Report (Schulhoff et al.)*.

## 🚀 Quick Start
1. **Scarica** `promptOS.html` da [Releases](https://github.com/yourusername/promptOS/releases) o clona la repo:
   ```bash
   git clone https://github.com/yourusername/promptOS.git
   ```
2. **Apri** `promptOS.html` in qualsiasi browser moderno (Chrome, Firefox, Edge).
3. Usa la **Modalità Demo** (default) per testare tutte le funzionalità senza API key.

## 🔍 Funzionalità
- **Libreria**: 58 tecniche classificate per categoria, difficoltà e modello supportato
- **Builder**: Genera prompt personalizzati selezionando tecniche e modello target
- **LLM Advisor**: Raccomanda il modello migliore per il tuo caso d'uso
- **Confronto**: Confronta output di diversi modelli per lo stesso prompt
- **Analizzatore**: Analizza e migliora i tuoi prompt esistenti
- **Academy**: Lezioni strutturate sul prompt engineering
- **Preferiti**: Salva le tue tecniche preferite (persiste in localStorage)

## ⚠️ Limitazione CORS per API Reali
Le chiamate API reali (Anthropic, OpenAI, Gemini) sono bloccate da CORS se fatte da file locale. Per abilitarle:
1. Deploya un serverless proxy (Vercel/Netlify/Cloudflare Workers)
2. Inserisci la tua API key nelle Impostazioni
3. Disattiva la Modalità Demo

## 🛠 Proxy Serverless (Opzionale)
Crea un file `vercel.json` nella root per un proxy Vercel leggero:
```json
{
  "rewrites": [
    { "source": "/api/anthropic", "destination": "https://api.anthropic.com/v1/messages" },
    { "source": "/api/openai", "destination": "https://api.openai.com/v1/chat/completions" }
  ]
}
```

## 📄 Licenza
MIT License – libero uso, modifica e distribuzione.