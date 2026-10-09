Rotorflight Log Analyzer - Windows
============================================
Eigenstaendige Windows-App ohne Server, Python oder Decoder: die Auswertung laeuft komplett in der App (WebView2, bei Win10/11 vorinstalliert).

Bauen ueber GitHub (ohne Installation):
 1. Neues Repository, INHALT dieses Ordners hochladen. Der versteckte Ordner .github wird im Browser oft nicht mit hochgeladen:
    dann "Add file > Create new file", Name  .github/workflows/windows.yml  und den Inhalt der Datei einfuegen.
    Ebenso muss  www/index.html  und  src-tauri/...  mit der Ordnerstruktur im Repo liegen (Ordner ueber den Dateinamen mit / anlegen).
    Am einfachsten: GitHub Desktop oder "git push" nutzen, dann bleibt alles erhalten.
 2. Actions > "Build Windows" laeuft automatisch (ca. 8-12 Min beim ersten Mal).
 3. Unter Artifacts "RFLogAnalyzer-windows" laden: darin rf-log-analyzer.exe (portabel) und das Setup (nsis).

Lokal bauen: Node 18+, Rust (rustup), dann  npm install ; npx tauri icon icon.png ; npx tauri build

<img width="1557" height="873" alt="screenshot" src="https://github.com/user-attachments/assets/37b9d3ac-a0c2-4283-9b89-03a864380463" />

