# ShopDemo Kundenservice Bot

Ein Kundenservice-Chatbot für einen fiktiven Online-Shop, gebaut mit Dialogflow CX.

**[Live Demo hier](https://raphael-werner.github.io/shopdemo-kundenservice)**

> **Hinweis:** Der Bot läuft auf dem kostenlosen Google Cloud Tier. 
> Bitte zwischen den Nachrichten 2-3 Sekunden warten, 
> da sonst das Rate Limit erreicht wird.

## Funktionen

- Bestellstatus-Auskunft
- Rückgabeprozess Schritt für Schritt
- FAQ (Zahlung, Kontakt, Stornierung)
- Automatische Eskalation bei Frustration
- Ehrliche Antwort bei unbekannten Themen

## Architektur

Root Agent erkennt den Nutzer-Intent und leitet an spezialisierte Sub-Agents weiter:

- `bestellstatus-agent` – Lieferzeiten, Bestellnummer
- `rueckgabe-agent` – 3-stufiger Rückgabeprozess
- `faq-agent` – Allgemeine Fragen, Öffnungszeiten, Kontakt

## Tech Stack

- Dialogflow CX / Conversational Agents (Google Cloud)
- Multi-Agent Architektur
- Gemini 2.5 Flash
- GitHub Pages
