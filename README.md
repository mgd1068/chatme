# chatme

Das **Chatme Project** ist eine Webanwendung, die verschiedene Funktionen zur Interaktion mit OpenAI-APIs bietet. Ziel ist es, eine benutzerfreundliche Oberfläche bereitzustellen, über die Skripte generiert, getestet, iterativ verbessert und direkt über die Chat-Funktion kommuniziert werden kann. Die Entwicklung erfolgt iterativ.

## Projektübersicht

### Funktionen
1. **Codegenerierung**:
   - Beschreibungen eingeben und Python-Skripte generieren lassen.
   - Nutzung von `code-davinci-002` (OpenAI Codex) über die API.

2. **Code testen**:
   - Generierte Skripte können getestet werden.
   - Ergebnisse werden analysiert und in einer Logdatei protokolliert.

3. **Iterative Verbesserung**:
   - Generierte oder vorhandene Skripte können iterativ durch die API verbessert werden.

4. **Chat-Funktion**:
   - Direkte Kommunikation mit OpenAI (z. B. `gpt-3.5-turbo` oder `gpt-4`).
   - Benutzer können natürliche Sprache eingeben und eine Antwort erhalten.

5. **Weboberfläche**:
   - Flask-basierte Oberfläche für einfache Bedienung.
   - Anzeigen und Bearbeiten von Dateien, Logs und Konfigurationen.

6. **Konfigurationsverwaltung**:
   - `config.yaml` zur Speicherung von API-Informationen und anderen Einstellungen.

7. **Logging**:
   - Alle Aktionen werden protokolliert (z. B. Codegenerierung, Tests, Chat).

---

### Verzeichnisstruktur
```plaintext
/scripts/chatme/
├── main.py           # Hauptskript
├── config/
│   └── config.yaml   # Konfigurationsdatei
├── templates/
│   ├── index.html    # Startseite
│   ├── chat_form.html # Eingabe für den Chat
│   ├── chat.html     # Ausgabe der Chat-Antwort
├── log/              # Verzeichnis für Logs
├── scripts/          # Verzeichnis für generierte Skripte
