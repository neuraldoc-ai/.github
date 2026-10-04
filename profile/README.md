## neuraldoc hält Produktdokumentation auf dem Stand des Codes

Ändert sich der Code, findet neuraldoc die Dokumente, die dadurch veralten, und schlägt belegte Textänderungen vor. Jeder Vorschlag zeigt seine Quelle im Code. Ein Mensch prüft und gibt frei.

| Repository | Wofür |
| --- | --- |
| [neuraldoc-dashboard](https://github.com/neuraldoc-ai/neuraldoc-dashboard) | Das Werkzeug. Lokal starten, das Beispiel ansehen oder ein eigenes Projekt prüfen. |
| [neuraldoc-landing](https://github.com/neuraldoc-ai/neuraldoc-landing) | Die Website. |
| [mobiq](https://github.com/neuraldoc-ai/mobiq) | Unser Beispiel- und Testdatensatz: ein erfundener ERP-Hersteller mit Release, Tickets und veralteter Doku. |
| [mobiq-code](https://github.com/neuraldoc-ai/mobiq-code) · [mobiq-docs](https://github.com/neuraldoc-ai/mobiq-docs) · [mobiq-db](https://github.com/neuraldoc-ai/mobiq-db) | Code, Dokumentation und Datenbank dieses Datensatzes. |

### Ausprobieren

Voraussetzungen: [Node.js 24](https://nodejs.org) und Git.

```bash
git -c core.autocrlf=false clone --recursive https://github.com/neuraldoc-ai/neuraldoc-dashboard.git
cd neuraldoc-dashboard/frontend
npm ci
npm run dev
```

Dann http://localhost:5174/app/ öffnen. Das Beispiel läuft ohne Schlüssel und ohne Kosten. Für ein eigenes Projekt braucht es einen Jev-Schlüssel und ein Sprachmodell nach Wahl, siehe [README](https://github.com/neuraldoc-ai/neuraldoc-dashboard#readme).

Alle Repositories stehen unter der MIT-Lizenz. Firmen, Personen und Inhalte im Beispiel sind erfunden.
