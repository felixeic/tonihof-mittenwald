# tonihof-mittenwald.de

Bürgerinformationsseite zum vorhabenbezogenen Bebauungsplan
„Sondergebiet Hotel Tonihof“, Markt Mittenwald.

Statische Website, keine Build-Tools, keine Abhängigkeiten.

## Struktur

```
index.html         Startseite
impressum.html     Impressum        (Platzhalter — vor Livegang ausfüllen)
datenschutz.html   Datenschutz      (Platzhalter — vor Livegang ausfüllen)
styles.css         gesamtes Styling
assets/            Visualisierungen, Logo, Social-Preview
CNAME              Custom Domain für GitHub Pages
.nojekyll          Jekyll-Verarbeitung deaktivieren
```

## Lokal ansehen

```bash
python3 -m http.server 8000
# http://localhost:8000
```

## Deployment

GitHub Pages, Branch `main`, Ordner `/` (root).
Pages ist derzeit **deaktiviert**, bis Impressum und Datenschutzerklärung
vollständig sind.

### DNS für tonihof-mittenwald.de

Apex-Domain — vier A-Records:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

Und vier AAAA-Records:

```
2606:50c0:8000::153
2606:50c0:8001::153
2606:50c0:8002::153
2606:50c0:8003::153
```

Zusätzlich `www` als CNAME auf `felixeic.github.io`.

Nach der DNS-Propagierung in den Pages-Einstellungen
„Enforce HTTPS“ aktivieren.

## Hinweise zum Inhalt

- Zahlen und Aussagen stammen aus den zur 1. Offenlage ausgelegten Unterlagen
  (Stand 30. Juli 2026). Maßgeblich sind die Originalunterlagen beim Markt Mittenwald.
- Das Kontaktformular sendet keine Daten an einen Server, sondern öffnet das
  E-Mail-Programm des Besuchers (`mailto:` an Tonihof@kvlgroup.com).
- Keine Cookies, kein Tracking, keine extern geladenen Schriftarten.
