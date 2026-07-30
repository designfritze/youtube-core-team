# Decision Log

Jede Grundsatzentscheidung wird hier festgehalten: Datum, Entscheidung,
Begründung, ggf. verworfene Alternativen. Neue Einträge oben anfügen.
Format angelehnt an Architecture Decision Records (ADR).

---

## 2026-07-30 – Schlanker Start mit 3 Rollen statt 9 Agenten

**Entscheidung:** Die Produktion startet halb-manuell mit drei definierten
Rollen (Research, Skript, Qualität). Die volle Agenten-Architektur ist
Zielbild für Stufe 3, nicht Startpunkt.

**Begründung:** Neun Agenten vor dem ersten Video wäre Over-Engineering –
es würden Annahmen automatisiert statt erprobter Prozesse. Übergabeformate
werden trotzdem von Anfang an agentenfähig definiert, damit die spätere
Automatisierung ein Austausch des Ausführenden ist, kein Umbau.

**Verworfen:** Sofortiger Aufbau aller 9 Agenten inkl. Projektleiter-Agent.

---

## 2026-07-30 – Machbare Schritte als GitHub Issues + Roadmap

**Entscheidung:** Jeder konkrete Arbeitsschritt wird ein GitHub Issue mit
Akzeptanzkriterien und Meilenstein-Label (M1–M4); ROADMAP.md liefert den
Überblick.

**Begründung:** Issues sind abhakbar, kommentierbar und erzwingen die
Zerlegung in wirklich machbare Schritte. Vom Projektinhaber so gewählt.

---

## 2026-07-30 – Phase 1: genau ein YouTube-Kanal, sonst nichts

**Entscheidung:** In Phase 1 wird ausschließlich ein YouTube-Kanal
aufgebaut. Keine Landingpage, kein Funnel, keine Produkte, kein zweiter
Kanal.

**Begründung:** YouTube liefert Feedback, Daten, Reichweite und
Themenvalidierung. Ein Marketingapparat ohne Reichweite verbrennt Zeit und
Geld. Der größte Hebel liegt darin, zuerst ein einziges System erfolgreich
zu machen und erst dann zu skalieren (Kernerkenntnis der
Ursprungs-Strategie).

**Verworfen:** Paralleler Aufbau von Kanal, Landingpage, Newsletter,
Produkten und mehreren Kanälen.

---

## 2026-07-30 – Phase 1 bekommt schriftliche Erfolgs- und Abbruchkriterien

**Entscheidung:** Vor Produktionsbeginn werden messbare Go-/Pivot-/No-Go-
Kriterien festgelegt ([PHASE-1-KRITERIEN.md](PHASE-1-KRITERIEN.md)); die
ersten 10 Videos zählen als Kaltstart und nicht gegen das Projekt.

**Begründung:** Ohne vorab definierte Kriterien gibt es keinen definierten
Punkt zum Skalieren oder ehrlichen Abbrechen – das Projekt liefe sonst
zombiehaft weiter. Das Kaltstart-Problem neuer Kanäle ist ein bekanntes
Muster und wird als Erwartung eingeplant statt als Scheitern
fehlinterpretiert.

---

## Offene Grundsatzentscheidungen (fällig in M1)

- Nische (mit Bewertungsmatrix aus [STRATEGIE.md](STRATEGIE.md))
- Sprache: Deutsch oder Englisch
- Unkopierbarer Winkel
- Finale Werte der Phase-1-Kriterien inkl. Budget-Deckel
