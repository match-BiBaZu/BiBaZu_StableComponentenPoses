# Rf3a: 10.000 ungruppierte Fallversuche bei statischem Band (0 mm/s)

Simulator-Commit: `72b1ba08aa9b317804cd60e1e2ae6e636910f3fd`; Seed: 42; Gruppierung: aus. 9993 von 10.000 Abwürfen erfüllen das jeweilige Ruhekriterium.

Jeder eingependelte Abwurf besitzt seine eigene Orientierung und Versuch-ID. Die Einträge in der archivierten frequencies.csv sind deshalb einzelne Versuche, keine gruppierten Pose-Klassen.

Das verlustfreie TAR.XZ-Archiv enthält sämtliche Originaldateien des Laufs einschließlich der Einzelversuche, Rauheitsereignisse, Bandstopp-Beobachtungen, Originalkonfiguration und des Manifests. Die Konfiguration daneben verwendet relative Pfade zum bereits vorhandenen STL.

- [Vollständige Simulationsdaten mit allen CSV-/JSONL-Dateien und der vollständigen summary.json](simulation_results.tar.xz)
- [Kompakte Zusammenfassung](summary.json)
- [Konfiguration](config.json), [Manifest](manifest.json)
- [Prüfung](validation.json), [Ausführung und Vergleich](execution.json)

Die Parameter entsprechen den archivierten Referenzvorgaben mit den angeforderten Änderungen für Bandmodus, Geschwindigkeit, 10.000 Versuche und deaktivierte Gruppierung. Die zusätzliche Bandstopp-Beobachtung bleibt im bewegten Fall aktiviert.

Entpacken: `python -m tarfile -e simulation_results.tar.xz extracted`.
