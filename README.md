# ShopDemo Kundenservice Bot

Ein Kundenservice-Chatbot für einen fiktiven Online-Shop, gebaut mit Dialogflow CX.

**[Live Demo hier](https://raphael-werner.github.io/shopdemo-kundenservice)**

> **Hinweis:** Der Bot läuft auf dem kostenlosen Google Cloud Tier mit einem Rate Limit. 
> Bitte zwischen den Nachrichten 2-3 Minuten warten, da sonst ein Fehler erscheint.
> Die Begrüßung ist aus diesem Grund als statischer Text umgesetzt, so bleibt das gesamte Rate Limit für die eigentlichen Konversationsanfragen verfügbar.

## Funktionen

- Bestellstatus-Auskunft
- Rückgabeprozess Schritt für Schritt
- FAQ (Zahlung, Kontakt, Stornierung)
- Automatische Eskalation bei Frustration
- Ehrliche Antwort bei unbekannten Themen

## Aufbau

Root Agent erkennt den Nutzer-Intent und leitet an spezialisierte Sub-Agents weiter:

- `bestellstatus-agent`: Lieferzeiten, Bestellnummer
- `rueckgabe-agent`: 3-stufiger Rückgabeprozess
- `faq-agent`: Allgemeine Fragen, Öffnungszeiten, Kontakt; bezieht sich auf FAQ-Dokument
