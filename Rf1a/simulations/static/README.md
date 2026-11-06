# Rf1a: 1.000 ungruppierte Fallversuche bei statischem Band (0 mm/s)

Simulator-Commit: `643b0e1ac5020602a4846eba96baaacef255a332`; Seed: 42; Gruppierung: aus. 940 von 1.000 Abwürfen erfüllen das jeweilige Ruhekriterium.

Jeder eingependelte Abwurf besitzt seine eigene Orientierung und Versuch-ID. Die Einträge in frequencies.csv sind deshalb einzelne Versuche, keine gruppierten Pose-Klassen.

Das ZIP enthält sämtliche CSV- und JSONL-Dateien des Laufs einschließlich der Einzelversuche, Rauheitsereignisse, Bandstopp-Beobachtungen, Originalkonfiguration und des Manifests. Die Konfiguration daneben verwendet relative Pfade zum bereits vorhandenen STL.

- [Vollständige Simulationsdaten](simulation_results.zip)
- [Zusammenfassung](summary.json), [Einzelorientierungen](frequencies.csv)
- [Konfiguration](config.json), [Manifest](manifest.json)
- [Prüfung](validation.json), [Ausführung und Vergleich](execution.json)

Die Parameter entsprechen den aktuellen GUI-Vorgaben mit den angeforderten Änderungen für Bandmodus, Geschwindigkeit, 1.000 Versuche und deaktivierte Gruppierung. Die zusätzliche Bandstopp-Beobachtung bleibt im bewegten Fall aktiviert.
