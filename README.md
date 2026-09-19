# Chris Storm Horror Festival – GitHub Pages

## Schnellste Variante

Der Ordner `site/` im ZIP ist bereits für GitHub Pages gebaut. Lade den Inhalt
von `site/` in das Root-Verzeichnis deines GitHub-Repositories und aktiviere
unter **Settings → Pages** die Veröffentlichung aus dem Haupt-Branch.

## Mit dem Quellcode neu bauen

Der Ordner `source/` enthält die React/Vite-Quelldateien, das Poster und die
Festivalinhalte. Für eine Veröffentlichung unter
`https://USERNAME.github.io/REPOSITORY/` muss der Vite-Basispfad dem
Repository-Namen entsprechen:

```bash
pnpm install
PORT=4173 BASE_PATH=/REPOSITORY/ pnpm --filter @workspace/chris-storm-festival run build
```

Danach den Inhalt von `artifacts/chris-storm-festival/dist/public/` als
GitHub-Pages-Dateien veröffentlichen.

Die Standardsprache beim Öffnen ist Englisch. Deutsch kann jederzeit über den
Sprachumschalter aktiviert werden.