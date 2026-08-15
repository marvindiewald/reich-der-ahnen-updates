# Reich der Ahnen — Update-Kanal

Dieses Repository beliefert die installierte App mit neuen Spielstaenden.

- **`version.json`** auf `main` nennt die neueste Versionsnummer und die
  Adresse des zugehoerigen Buendels. Die App liest genau diese Datei.
- **Releases** tragen das jeweilige `bundle.zip` als Anhang.

Die Abfrage laeuft ueber `raw.githubusercontent.com`, weil GitHub fuer
Release-Anhaenge keine CORS-Freigabe sendet und die App-WebView die Antwort
sonst verwirft. Das Buendel selbst laedt die App nativ herunter, dort spielt
CORS keine Rolle.

Der Spielcode liegt im Hauptprojekt, nicht hier.