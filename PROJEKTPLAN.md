# Projektplan MAD42 – YouTube Core Team

> Der vollständige Arbeitsplan für Phase 1. Überblick in [ROADMAP.md](ROADMAP.md),
> Arbeitseinheiten als GitHub Issues (#1–#13). Dieses Dokument verbindet beides:
> Arbeitspakete, Abhängigkeiten, Verantwortlichkeiten, Zeitplan, Risiken, Governance.

## 1. Projektziel

Einen einzigen YouTube-Kanal exzellent aufbauen und dabei eine **reproduzierbare,
weitgehend automatisierte Produktions-Blaupause** entwickeln. Erfolg ist definiert
in [docs/PHASE-1-KRITERIEN.md](docs/PHASE-1-KRITERIEN.md) – nicht verhandelbar,
sobald in Issue #4 beschlossen.

## 2. Projektorganisation

| Rolle | Besetzung | Verantwortung |
|---|---|---|
| **Projektinhaber** | Mensch (mad@mad42.de) | Alle Grundsatzentscheidungen: Nische, Sprache, Winkel, Budget, Veröffentlichungen. Letzte Instanz. |
| **Projektleitung (KI)** | Opus 5 (Claude-Code-Session auf diesem Repo) | Operative Führung: Arbeitspakete vorantreiben, Agenten erstellen und betreiben, Modelle delegieren, Dokumente pflegen, Entscheidungsvorlagen liefern. |
| **Agenten** | Welle 1–3 laut [agents/README.md](agents/README.md) | Ausführung in klar definierten Rollen mit definierten Übergabeformaten. |

Details zur Zusammenarbeit und den Autonomie-Grenzen: [CLAUDE.md](CLAUDE.md).

### Modell-Delegationsrichtlinie

Die Projektleitung entscheidet **selbstständig**, welches Modell welche Aufgabe
ausführt, und dokumentiert die Wahl (Modell + Kosten) im jeweiligen
Arbeitsergebnis. Richtschnur:

| Aufgabentyp | Modellklasse | Beispiele |
|---|---|---|
| Strategie, Skript-Kreation, Qualitätskontrolle, Entscheidungsvorlagen | Stärkste verfügbare Modelle (Opus-Klasse) | Nischen-Analyse, Skripte, QS-Protokolle, Reviews |
| Solide Zuarbeit mit Urteilsvermögen | Mittlere Modelle (Sonnet-Klasse) | Research-Briefs, Konkurrenzanalysen, Beschreibungstexte |
| Routine & Fleißarbeit | Günstigste Modelle (Haiku-Klasse) | Tag-Listen, Kapitelmarken, Umformatierung, Varianten, Batch-Jobs |

Regel: Im Zweifel eine Klasse höher bei allem, was veröffentlicht wird –
eine Klasse tiefer bei allem, was intern bleibt.

## 3. Arbeitspakete

Abhängigkeiten: Ein AP startet erst, wenn seine Vorgänger abgeschlossen sind.
„Entscheidet" = Projektinhaber, „liefert zu" = Projektleitung/Agenten.

### M1 – Fundament & Entscheidungen (Ziel: Woche 1–2)

| AP | Issue | Inhalt | Hängt ab von | Verantwortung |
|---|---|---|---|---|
| 1.1 | [#1](../../issues/1) | Nische final entscheiden (Bewertungsmatrix) | – | KI liefert Matrix + Empfehlung, Mensch entscheidet |
| 1.2 | [#3](../../issues/3) | Unkopierbaren Winkel definieren | 1.1 (parallel sinnvoll) | KI liefert Kandidaten + Gegentests, Mensch entscheidet |
| 1.3 | [#2](../../issues/2) | Sprache DE/EN entscheiden | 1.1 | KI liefert Datenlage, Mensch entscheidet |
| 1.4 | [#4](../../issues/4) | Phase-1-Kriterien + Budget-Deckel beschließen | 1.1–1.3 | KI prüft Plausibilität, Mensch beschließt |
| 1.5 | [#5](../../issues/5) | Kanal-Branding & YouTube-Setup | 1.1–1.4 | KI entwirft, Mensch wählt aus und legt Kanal an |

**Meilenstein-Abschluss M1:** Alle vier Entscheidungen im Decision Log, Kanal live.

### M2 – Erste Videos, halb-manuell (Ziel: Woche 3–8)

| AP | Issue | Inhalt | Hängt ab von | Verantwortung |
|---|---|---|---|---|
| 2.1 | [#6](../../issues/6) | Skript-Template & Hook-Formate | M1 | KI, Mensch gibt frei |
| 2.2 | [#7](../../issues/7) | TTS-/Sprecher-Lösung | M1, parallel zu 2.1 | KI vergleicht, Mensch entscheidet (Kosten!) |
| 2.3 | [#8](../../issues/8) | Thumbnail- & Titel-Prozess | 1.5, parallel zu 2.1 | KI, Mensch gibt Stil frei |
| 2.4 | [#9](../../issues/9) | Videos 1–3 produzieren + Protokolle | 2.1–2.3 | Pipeline (Welle-1-Agenten + Mensch), Mensch gibt jeden Upload frei |
| 2.5 | [#10](../../issues/10) | Videos 4–5 + erstes Daten-Review | 2.4 | Pipeline; Review durch KI, Konsequenzen entscheidet Mensch |

**Meilenstein-Abschluss M2:** 5 Videos live, 5 vollständige Produktionsprotokolle,
schriftliches Review mit ≥ 3 Verbesserungen.

### M3 – Automatisierung (Ziel: Woche 9–12, parallel zur laufenden Produktion)

| AP | Issue | Inhalt | Hängt ab von | Verantwortung |
|---|---|---|---|---|
| 3.1 | [#11](../../issues/11) | Automatisierungs-Kandidaten priorisieren | M2 | KI, Mensch bestätigt Prioritäten |
| 3.2 | [#12](../../issues/12) | Welle-2-Agenten bauen + 1 Video vollautomatisierter produzieren | 3.1 | KI autonom (inkl. Modellwahl), Mensch prüft Stichprobe |

**Wichtig:** Während M3 läuft die Wochenproduktion weiter (Videos 6–20) –
Automatisierung ersetzt Schritte schrittweise, nie die QS-Freigabe und nie die
Upload-Freigabe durch den Menschen.

**Meilenstein-Abschluss M3:** Manueller Aufwand pro Video messbar gesunken,
Qualität gehalten.

### M4 – Phase-1-Review (Ziel: Monat 6 oder nach Video 20)

| AP | Issue | Inhalt | Hängt ab von | Verantwortung |
|---|---|---|---|---|
| 4.1 | [#13](../../issues/13) | Halbzeit-Review (Video 10), finaler Review, Go/Pivot/No-Go | laufend / M3 | KI misst und legt vor, Mensch entscheidet |

**Bei Go:** Phase-2-Arbeitspakete werden als neue Issues (M5) angelegt:
Landingpage → Newsletter → Leadmagnet → erstes Produkt aus dem erfolgreichsten
Video. **Bei Pivot:** Bewertungsmatrix erneut durchlaufen (Meditations-Kanal =
erster Alternativkandidat). **Bei No-Go:** Lessons-Learned-Dokument, sauberer Abschluss.

## 4. Laufender Betriebsrhythmus (ab M2)

- **Wöchentlich:** 1 Video durch die Pipeline (Research → Skript → QS → Produktion
  → Upload-Freigabe durch Mensch). Produktionsprotokoll ist Pflichtteil.
- **Nach jedem Video:** Kosten und Zeitaufwand ins Protokoll; Auffälligkeiten in
  den Statistiken als Issue-Kommentar.
- **Nach Video 5, 10, 20:** Review-Ritual laut [docs/PHASE-1-KRITERIEN.md](docs/PHASE-1-KRITERIEN.md).
- **Bei jeder Grundsatzfrage:** Entscheidungsvorlage der KI → Entscheidung des
  Menschen → Eintrag ins [Decision Log](docs/ENTSCHEIDUNGEN.md).

## 5. Risikoregister

| Risiko | Wahrscheinlichkeit | Wirkung | Gegenmaßnahme |
|---|---|---|---|
| YouTube-Policy „inauthentic content" trifft das Format | mittel | hoch | Unkopierbarer Winkel als K.-o.-Kriterium (#3), menschliche Kuratierung + Upload-Freigabe, kein Volumen-Spiel; bei Monetarisierungs-Ablehnung: sofortiger Produktionsstopp (Kriterien-Doc) |
| Nischen-Sättigung, Kanal bleibt unsichtbar | hoch | hoch | Winkel-Gegentest in #3; Kaltstart eingeplant (erste 10 Videos zählen nicht); Pivot-Kriterien greifen automatisch |
| Kostenexplosion durch Modell-/Tool-Nutzung | mittel | mittel | Budget-Deckel (#4) als harte Grenze; Kosten-Pflichtfeld je Video; Modell-Delegationsrichtlinie |
| Qualitätsdrift bei zunehmender Automatisierung | mittel | hoch | QS-Veto bleibt immer aktiv; menschliche Stichprobe je Video; M3-Abschluss verlangt „Qualität gehalten" |
| Planungs-Prokrastination (am System bauen statt produzieren) | mittel | mittel | M1 ist auf 2 Wochen begrenzt; „Ist das jetzt notwendig?"-Regel; Video 1 ist wichtiger als jedes weitere Dokument |
| Wissensverlust zwischen Chat-Sessions | sicher (by design) | mittel | Alles Projektwissen lebt im Repo, nie im Chat; [CLAUDE.md](CLAUDE.md) als Onboarding; Decision Log als Gedächtnis |
| Abhängigkeit von YouTube als einziger Plattform | niedrig (Phase 1) | hoch (langfristig) | Phase 2 (Newsletter, Produkte) ist genau dafür da – aber erst nach Go |

## 6. Was dieser Plan bewusst NICHT enthält

Landingpage, Funnel, Produkte, zweiter Kanal, Meditations-Kanal, Membership,
Projektleiter-Agent, Produkt-Agent. Alles davon hat seinen definierten Platz
(Phase 2/3) und wartet auf den Phase-1-Beweis. Neue Ideen während des Projekts:
aufschreiben (Decision Log, Abschnitt „Verschoben"), verschieben, weiterarbeiten.
