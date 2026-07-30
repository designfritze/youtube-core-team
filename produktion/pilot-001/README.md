# Pilot 001 – Erste Version zum Testen

Ein vollständiger Durchlauf der Welle-1-Pipeline an einem echten Fall, damit
das System **benutzt** und nicht nur gelesen werden kann.

**Fall:** Nordamerikanischer Stromausfall vom 14. August 2003
**Bericht:** U.S.–Canada Power System Outage Task Force, Final Report, April 2004
**Warum dieser Fall:** Stromnetz – eines der Teilgebiete, die im englischsprachigen
Raum dünner besetzt sind als Luftfahrt und Seefahrt ([WINKEL.md](../../docs/WINKEL.md)).
Untersuchung abgeschlossen, Bericht öffentlich, US-Bundeswerk und damit
gemeinfrei.

## Was hier liegt

| Datei | Rolle | Sprache |
|---|---|---|
| [`research-brief.md`](research-brief.md) | Ausgabe des [Research-Agenten](../../agents/research.md) | Englisch |
| [`script.md`](script.md) | Ausgabe des [Skript-Agenten](../../agents/skript.md) | Englisch |
| [`qs-protokoll.md`](qs-protokoll.md) | Ausgabe des [Qualitäts-Agenten](../../agents/qualitaet.md) | Deutsch (intern) |
| [`narration-test.md`](narration-test.md) | Der 60-Sekunden-Text für die Probeaufnahme (Issue #7) | Englisch |

## Wie du das testest

**1. Probeaufnahme (wichtigster Test, 15 Minuten).**
[`narration-test.md`](narration-test.md) öffnen, den Text laut aufnehmen, in
Zielqualität. Das prüft die letzte Annahme, auf der alles andere steht: ob
deine englische Sprecherstimme dieses Format trägt. Ergebnis als Kommentar in
Issue #7.

**2. Skript lesen (30 Minuten).**
Trägt der Aufbau? Ist der Hook stark genug? Ist die Bildregie (`[VISUAL: …]`)
umsetzbar oder verlangt sie Dinge, die in vertretbarer Zeit nicht zu bauen
sind? Deine Antwort auf die Bildregie ist der wertvollste Input – du bist der
Einzige, der weiß, was ein Video an Gestaltungsarbeit wirklich kostet.

**3. QS-Protokoll lesen (10 Minuten).**
Es endet mit **RÜCKGABE**. Prüf, ob die Strenge stimmt: zu hart, zu lasch, oder
richtig? Diese Kalibrierung entscheidet später über jedes Video.

## Das Ergebnis vorweg: der Pilot ist durchgefallen – absichtlich ehrlich

Der Qualitäts-Agent gibt das Skript zurück, und zwar aus einem Grund, der für
das ganze Projekt zentral ist: **Keine einzige Seitenzahl konnte am
Originalbericht geprüft werden.** Diese Arbeitsumgebung blockiert direkte
Dokumentenaufrufe (403 auf CONNECT, dieselbe Sperre wie bei der
Policy-Recherche in [NISCHEN-BEWERTUNG.md](../../docs/NISCHEN-BEWERTUNG.md),
Abschnitt 2).

Damit ist der Pilot als *Format-* und *Prozesstest* vollständig – und als
Produktionsvorlage bewusst unfertig. Genau diese Trennung soll die Pipeline
leisten: Sie produziert nichts Veröffentlichungsfähiges, solange die Belege
fehlen, egal wie gut der Text klingt.

**Was du tun musst, um den Piloten produktionsreif zu machen:** den
[Abschlussbericht](https://www.energy.gov/sites/prod/files/oeprod/DocumentsandMedia/BlackoutFinal-Web.pdf)
herunterladen und die mit `[VERIFY p. __]` markierten Stellen füllen. Jede
Markierung nennt, was zu belegen ist.

## Kosten dieses Durchlaufs

| Posten | Modellklasse | Aufwand |
|---|---|---|
| Research-Brief, Skript, QS-Protokoll, Sichtung | Opus-Klasse | Projektleitung selbst |
| Fallrecherche | – | 4 Websuchen |

Kein Delegationsaufwand an günstigere Modelle, weil der Pilot als Referenz für
die spätere Qualitätsmessung dient – hier soll die obere Grenze sichtbar sein,
nicht der Sparfall. Ab Video 1 gilt die Delegationsrichtlinie aus
[PROJEKTPLAN.md](../../PROJEKTPLAN.md).
