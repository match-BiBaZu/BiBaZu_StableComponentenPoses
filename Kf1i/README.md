# Kf1i

10000 Fallversuche auf 500 mm Strecke; 0 eingependelte Endlagen. Prozentangaben beziehen sich auf alle Fallversuche.

Dies sind beobachtete Simulationslagen unter den dokumentierten Parametern; Reibung und Unebenheitsmodell sind noch nicht an realen Häufigkeiten kalibriert.

| Pose | Bild | Anzahl | Anteil | 95-%-Intervall | Anteil eingependelt |
| --- | --- | ---: | ---: | ---: | ---: |

Zusätzliche Ruheprüfung nach Bandstopp: 9445 von 9529 beobachteten Teilen ruhig. Fahrhäufigkeiten oben bleiben davon getrennt. Ruheposen stehen als stop_observation in trials.csv.

Ergebnisstatus: unsettled: 9529, stalled: 456, timeout: 15

Details und Erkennung: [JSON](poses.json), [YAML](poses.yaml). Quaternionen: xyzw, Bauteil → Rutsche. Symmetrieoperationen werden rechts an die Bauteilrotation multipliziert. Die kontinuierliche Symmetrieachse wird gerichtet verglichen. Orientierungsabstand ≤5°; bei konkurrierenden Treffern innerhalb 1° bleibt die Zuordnung mehrdeutig.

Die Pose-IDs bleiben über Läufe erhalten. Der Registereintrag einer früher beobachteten, aktuell nicht aufgetretenen Pose bleibt zur Wiedererkennung reserviert.


## 10.000 Fallversuche mit anschließender Ruheprüfung

Berechnet mit 16 parallelen Prozessen und je einer Rutsche; Simulationscode: [82f8bd4](https://github.com/match-BiBaZu/Dashas_drop_sim/commit/82f8bd43c70a0eb160d27dc0f7232849842efe9c).

Während der Fahrt: 456 stalled, 15 timeout, 9529 unsettled.

Nach Bandstopp: **9445 von 9529 beobachteten Teilen ruhig** (99.12 %). Die übrigen Fallversuche ohne Erreichen der virtuellen Messlinie werden in der Fahrstatistik separat gezählt.

Das Band bremst nach der Fahrmessung in 0,2 s auf null; anschließend folgen 2 s Beobachtung ohne Störimpulse. Die Anfangsanregung ist auf 1 s begrenzt. Fahrhäufigkeiten und Ruheprüfung sind getrennte Ergebnisse.

- [Zusammenfassung aller Ergebnisse](summary.json)
- [Einzelergebnisse nach Bandstopp](stop_observations.csv)
- [Versuche einschließlich Fahr- und Ruhepose](trials.csv)
- [Vollständige Laufdaten als ZIP](simulation_results.zip) (CSV, JSONL, Impulsprotokolle und Originalkonfiguration)
- [Ausführungsnachweis](execution.json) und [Datenprüfung](validation.json)

Die 10.000 Versuchsnummern und Seeds wurden geprüft. Die ersten 100 Versuche einschließlich der Ruheprüfung reproduzieren den vorherigen Kontrolllauf exakt.
