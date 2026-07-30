# MAD42 – YouTube Core Team

Dieses Repository ist die zentrale Arbeitsbasis für **Phase 1 von MAD42**: den Aufbau
eines einzigen, exzellenten YouTube-Kanals als Fundament einer später reproduzierbaren
Content-Maschine.

## Worum es geht

MAD42 ist der Aufbau einer weitgehend automatisierten Content- und Produktpipeline.
Das Ziel ist **nicht**, möglichst viele Projekte zu starten – das Ziel ist eine
**reproduzierbare Blaupause**: ein System, das einmal exzellent gebaut wird und
später beliebig kopiert werden kann.

## Kernprinzipien

1. **Qualität vor Geschwindigkeit.** Lieber ein Kanal exzellent als fünf halbfertig.
2. **„Ist das jetzt notwendig?"** Jede neue Idee muss diese Frage bestehen –
   wenn nein, wird sie auf eine spätere Phase verschoben und im
   [Decision Log](docs/ENTSCHEIDUNGEN.md) dokumentiert.
3. **Prozess vor Einzelergebnis.** Jede Verbesserung soll allen zukünftigen
   Projekten helfen, nicht nur dem nächsten Video.
4. **Erst manuell verstehen, dann automatisieren.** Automatisiert wird nur, was
   sich nachweislich wiederholt – nicht, was sich wiederholen könnte.
5. **Messbar oder nicht passiert.** Phase 1 hat schriftliche Erfolgs- und
   Abbruchkriterien ([PHASE-1-KRITERIEN](docs/PHASE-1-KRITERIEN.md)).

## Navigation

| Dokument | Inhalt |
|---|---|
| [PROJEKTPLAN.md](PROJEKTPLAN.md) | Der vollständige Arbeitsplan: Arbeitspakete, Abhängigkeiten, Zeitplan, Risiken, Governance |
| [CLAUDE.md](CLAUDE.md) | Betriebsanleitung der KI-Projektleitung (wird von Claude-Sessions automatisch geladen) |
| [ROADMAP.md](ROADMAP.md) | Meilensteine M1–M4 mit Verweis auf die GitHub Issues |
| [docs/STRATEGIE.md](docs/STRATEGIE.md) | Phasenmodell, Nischen-Entscheidungsframework, Plattformrisiken |
| [docs/PIPELINE.md](docs/PIPELINE.md) | Die schlanke Start-Pipeline (3 Rollen) und ihre Ausbaustufen |
| [docs/PHASE-1-KRITERIEN.md](docs/PHASE-1-KRITERIEN.md) | Messbare Erfolgs- und Abbruchkriterien für Phase 1 |
| [docs/MANIFEST.md](docs/MANIFEST.md) | Das gemeinsame Manifest – die Verfassung aller Beteiligten und Agenten |
| [docs/ENTSCHEIDUNGEN.md](docs/ENTSCHEIDUNGEN.md) | Decision Log: jede Grundsatzentscheidung mit Begründung |
| [agents/](agents/README.md) | Die Agenten-Definitionen – Welle 1 (Research, Skript, Qualität) einsatzbereit |

## Arbeitsweise in diesem Repo

- **Machbare Schritte = GitHub Issues.** Jeder konkrete Arbeitsschritt ist ein
  Issue mit Akzeptanzkriterien, zugeordnet zu einem Meilenstein-Label (`M1`–`M4`).
- **Grundsatzentscheidungen** (Nische, Sprache, Kriterienwerte) werden im
  jeweiligen Issue diskutiert und nach der Entscheidung im Decision Log festgehalten.
- **Dokumente sind lebendig.** Wenn Daten aus echten Videos einer Annahme
  widersprechen, wird das Dokument geändert – mit Eintrag im Decision Log.

## Eine neue Arbeits-Session starten

Das Projekt ist session-unabhängig: Kein Wissen steckt in einem Chat-Verlauf,
alles liegt in diesem Repo. Eine neue Claude-Code-Session auf diesem
Repository lädt [CLAUDE.md](CLAUDE.md) automatisch und findet dort ihre Rolle,
ihre Befugnisse und den aktuellen Projektstand.

Startprompt, der genügt:

> Du bist die KI-Projektleitung dieses Projekts. Lies CLAUDE.md und arbeite
> nach dem dort beschriebenen Stand weiter.

Der Abschnitt „Aktueller Stand" in CLAUDE.md sagt, was als Nächstes ansteht
und welche Entscheidungen beim Projektinhaber offen sind.
