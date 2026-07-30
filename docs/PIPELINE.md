# Pipeline

## Grundsatz

Das ursprüngliche Konzept sah neun spezialisierte Agenten vor. Das ist die
**Zielarchitektur**, nicht der Startpunkt. Agenten werden erst gebaut, wenn
ein Schritt sich in der halb-manuellen Produktion nachweislich wiederholt hat
– sonst automatisieren wir Annahmen statt Prozesse.

## Stufe 1: Halb-manuelle Pipeline (M2) – drei Rollen

Für die Videos 1–5 gibt es genau drei definierte Rollen. Jede Rolle kann von
einem Menschen mit KI-Unterstützung ausgefüllt werden; die Übergabeformate
sind aber von Anfang an so definiert, als wären es Agenten – so wird die
spätere Automatisierung ein Austausch des Ausführenden, kein Umbau.

### Rolle 1: Research

**Auftrag:** Themen finden und absichern.

- Evergreen-Themen mit Suchpotenzial identifizieren
- Konkurrenzanalyse: Wer bedient das Thema, was fehlt dort?
- Quellen sammeln, Fakten mit Beleg notieren

**Übergabeformat (Research-Brief):** Thema, Kernfrage, 5–10 belegte
Kernfakten mit Quelle, Konkurrenz-Lücke, geschätztes Suchpotenzial.

### Rolle 2: Skript

**Auftrag:** Aus dem Research-Brief ein Skript mit Spannungsbogen machen.

- Hook (erste 30 Sekunden) nach den definierten Hook-Formaten
- Retention-orientierte Struktur (offene Schleifen, Kapitel, Payoff)
- Verständlichkeit vor Vollständigkeit; TTS-tauglich formuliert
  (Betonung, Pausen, Aussprache-Hinweise direkt im Skript)

**Übergabeformat (Skript-Dokument):** Hook, Kapitelstruktur mit Zeitzielen,
Volltext mit Sprechanweisungen, Thumbnail-/Titel-Vorschläge (3 Varianten).

### Rolle 3: Qualität

**Auftrag:** Letzte Instanz vor der Produktion. Prüft gegen das
[Manifest](MANIFEST.md):

- Faktencheck gegen die Quellen des Research-Briefs
- Logik, Dopplungen, Verständlichkeit, Stil-Konsistenz
- Löst der Inhalt das Versprechen von Titel/Thumbnail ein?
- **Veto-Recht:** Ein Skript, das durchfällt, geht zurück – nicht weiter.

**Übergabeformat (QS-Protokoll):** Befund je Prüfpunkt, Freigabe oder
Rückgabe mit konkreten Änderungsauflagen.

### Produktion, Upload, Analyse (Stufe 1: bewusst manuell)

Voiceover (TTS), Schnitt, Assets, Thumbnail, Titel/Beschreibung/Kapitel,
Upload und die Auswertung der Statistiken macht in Stufe 1 ein Mensch – und
**dokumentiert dabei jeden Schritt** (Dauer, Werkzeug, Kosten, Schmerzpunkte).
Diese Dokumentation ist das Anforderungsdokument für Stufe 2.

## Stufe 2: Automatisierung (M3)

Nach Video 5 wird priorisiert: Welche dokumentierten Schritte kosten am
meisten Zeit und sind am klarsten regelbasiert? Diese werden zuerst
automatisiert – typischerweise in dieser Reihenfolge:

1. Research- und Skript-Rolle als Agenten (klare Ein-/Ausgabeformate existieren bereits)
2. Qualitäts-Rolle als Agent (mit menschlicher Stichprobe als Backstop)
3. SEO-Paket (Titel, Beschreibung, Kapitel, Tags) als Routineaufgabe
4. Statistik-Auswertung als wiederkehrender Report

## Stufe 3: Zielarchitektur (erst bei bewiesener Blaupause)

Die volle Agenten-Riege aus dem Ursprungskonzept – Projektleiter, Research,
Skript, Qualität, Sprecher, Produktion, SEO/Upload, Statistik, Produkt –
wird erst aufgebaut, wenn Phase 1 bestanden ist und mehrere Kanäle die
Koordination tatsächlich erfordern. Ein Projektleiter-Agent für einen
einzelnen Kanal ist Verwaltung ohne Gegenwert.

## Modellstrategie

Gilt ab Stufe 1 für jede KI-Nutzung, auch die manuelle:

| Aufgabentyp | Modellklasse | Beispiele |
|---|---|---|
| Strategie, Kreativität, Qualitätskontrolle | Teuerste/intelligenteste Modelle | Nischen-Analyse, Skript-Erstellung, Hook-Varianten, Faktencheck |
| Routine und Fleißarbeit | Günstige Modelle | Umformatierung, Tag-Listen, Kapitel-Marken, Beschreibungs-Varianten, Batch-Aufgaben |

Kosten pro Video werden von Anfang an erfasst (Pflichtfeld in der
Produktionsdokumentation) – die Blaupause muss wirtschaftlich kopierbar sein.
