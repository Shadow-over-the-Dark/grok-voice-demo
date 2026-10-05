# grok-voice-demo
Grok Bot Safari Web Speech demo

Eine Seite, kein Server, keine Schlüssel. Läuft im Browser über die Web Speech API.

- **Sprechen → Text:** `webkitSpeechRecognition` (Safari ab iOS 14.5 / macOS), Deutsch oder Englisch, Live-Zwischentext.
- **Text → Sprache:** `speechSynthesis` mit Stimmenwahl und Tempo.
- Optional liest die Seite jeden erkannten Satz sofort vor. Während des Vorlesens pausiert das Mikrofon.

## Starten
Das Mikrofon geht nur über **https**. Am einfachsten: GitHub → Settings → Pages → Branch `main`, Ordner `/`. Dann die Pages-Adresse in Safari öffnen.

Lokal zum Testen am Mac: `python3 -m http.server 8000` und `http://localhost:8000` öffnen (localhost zählt als sicher).

## iPhone
- Diktieren muss an sein (Einstellungen → Allgemein → Tastatur → Diktieren).
- Beim ersten Tippen auf „Zuhören starten“ fragt Safari nach dem Mikrofon → Erlauben.
