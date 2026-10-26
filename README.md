# Size Sense
Touch-first Größenratespiel für Handy und iPad. Statische Website ohne Build-Schritt.

## Veröffentlichung
GitHub Settings → Pages → Deploy from a branch → main → / (root) → Save. Nach erfolgreicher Veröffentlichung erscheint Visit site. Die Website ist auf relative Pfade ausgelegt.

## Spiel
100 Supabase-Objekte im Solo-Modus, 10 Runden pro Duell. Beide Spieler öffnen die Website und sichern unterschiedliche Namen. Gegnernamen eingeben, einladen und auf dem zweiten Gerät beitreten. Einladungen werden alle fünf Sekunden abgefragt. Punkte: 100 × min(Schätzung, Spielwert) / max(Schätzung, Spielwert). Maximale Duellsumme: 1000 Prozentpunkte.

## Technik und Grenzen
Verwendet das vorhandene Supabase-Projekt Size und dessen sg_-RPCs. Nur der öffentliche Publishable-Key steht im Frontend. Spieler-Tokens werden lokal gespeichert; kein Passwort-Login und keine Wiederherstellung bei Verlust. Objektzeichnungen sind stilisierte Modelle, keine exakten wissenschaftlichen Silhouetten. Nur die gespeicherte Hauptdimension wird gewertet. Solo lädt den öffentlichen Katalog; daher ist dies kein manipulationssicheres Wettbewerbssystem. Einladungen erfordern eine geöffnete Website, keine Push-Nachrichten.

## Manuelle Prüfung vor Freigabe
Solo-Katalogzugriff und 100 Runden; Slider und Zahleneingabe; Hoch-/Querformat auf iPhone und iPad; drei Designs; zwei Browser mit unterschiedlichen Namen; Einladung annehmen/ablehnen; zehn Abgaben pro Spieler; Endstand; erneutes Öffnen eines laufenden Duells; abgelaufene Einladungen und Netzwerkausfälle. Diese Browserprüfungen sind noch nicht durchgeführt.
