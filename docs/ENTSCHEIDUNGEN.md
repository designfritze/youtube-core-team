# Decision Log

Jede Grundsatzentscheidung wird hier festgehalten: Datum, Entscheidung,
Begründung, ggf. verworfene Alternativen. Neue Einträge oben anfügen.
Format angelehnt an Architecture Decision Records (ADR).

---

## 2026-07-30 – Sprache: Englisch

**Entscheidung:** Der Kanal wird **englischsprachig**. Skripte, Research-Briefs,
Titel und Beschreibungen werden auf Englisch erstellt – keine
Übersetzungsschicht zwischen Recherche und Skript.

**Begründung des Projektinhabers:** größerer Markt, direkte internationale
Reichweite.

**Gegen die Empfehlung der Projektleitung entschieden.** Die Empfehlung lautete
Deutsch, weil der Wettbewerbsvorteil von K3 auf einem *deutschsprachigen*
Negativbefund beruhte. Die Entscheidung ist getroffen; die Konsequenzen sind
eingearbeitet statt weggeglättet (Nachtrag 9 in
[NISCHEN-BEWERTUNG.md](NISCHEN-BEWERTUNG.md)):

**Was schlechter wird:**
- **Wettbewerbsdichte 4 → 2.** Das Format existiert im Englischen etabliert:
  Plainly Difficult, Brick Immortar (~393 Tsd. Abonnenten), Fascinating Horror,
  Scary Interesting, Military Expert (arbeitet ausdrücklich mit NTSB-, AAIB- und
  BEA-Berichten) – dazu der offizielle CSB-Kanal mit ~417 Tsd. Abonnenten. Der
  Winkel muss jetzt gegen sichtbare Konkurrenz bestehen, nicht gegen eine Lücke.
- **Neues Risiko: Sprecherqualität.** Die Konkurrenz sind Muttersprachler mit
  wiedererkennbaren Stimmen. Ein hörbarer Akzent untergräbt ein Format, dessen
  Kern Präzision ist. Vor Video 1 zu testen (Issue #7).

**Was besser wird:**
- **Bildrechte entspannen sich deutlich.** NTSB- und CSB-Berichte sind Werke der
  US-Bundesregierung und damit in den USA gemeinfrei; britische Berichte (RAIB,
  AAIB, MAIB) stehen unter der Open Government Licence, nutzbar mit
  Quellenangabe. Das deutsche Problem – § 5 UrhG befreit den Text, nicht die
  Fotos (§ 72 UrhG) – entfällt weitgehend. *(Laien-Recherche, keine
  Rechtsberatung; vor Produktionsbeginn zu prüfen.)*
- **Größerer und besser erschlossener Quellenkorpus:** NTSB, CSB, RAIB, AAIB,
  MAIB veröffentlichen umfangreich, durchsuchbar und in der Arbeitssprache.

**Folgeempfehlung (keine Entscheidung, aber dringend):** Innerhalb von K3 auf
die Teilgebiete zielen, die im Englischen dünn besetzt sind – **Stromnetz,
IT-/Infrastrukturausfälle, Bahn** – statt auf Luftfahrt und Seefahrt, die von
den etablierten Kanälen bedient werden. Details in [WINKEL.md](WINKEL.md).

---

## 2026-07-30 – Budget-Deckel Phase 1: 600 €

**Entscheidung:** Der Budget-Deckel für Phase 1 beträgt **600 € gesamt**
(Richtwert ~30 € pro Video), gerechnet auf 20 Videos. Umfasst KI-Modellnutzung,
Software-Abos, Musik- und Assetlizenzen. Nicht enthalten: die Arbeitszeit des
Projektinhabers.

**Begründung:** Weil Stimme, Schnitt und Grafik selbst erbracht werden,
entfallen die größten üblichen Kostenblöcke. Der Deckel ist eine harte Grenze –
bei Erreichen ohne Sicht auf die Erfolgskriterien greift „Stopp und Review"
laut [PHASE-1-KRITERIEN.md](PHASE-1-KRITERIEN.md).

---

## 2026-07-30 – Phase-1-Kriterien beschlossen (Zeitrahmen 9 Monate)

**Entscheidung:** Die Vorschlagswerte werden übernommen – Ø-Retention ≥ 40 %,
Ø-CTR ≥ 4 %, ≥ 1.000 Abonnenten, steigende Tendenz, gemessen an den **letzten
10** von 20 Videos. **Abweichung vom Vorschlag: Der Zeitrahmen beträgt 9 statt
6 Monate.**

**Begründung der Verlängerung:** realistischere Taktung neben anderer Arbeit;
die Produktion bleibt qualitätsgetrieben statt terminfixiert. Preis: Die
Go/No-Go-Entscheidung verschiebt sich entsprechend nach hinten.

**Ab jetzt gilt:** Diese Werte werden nicht mehr angepasst – auch nicht mit
guter Begründung ([CLAUDE.md](../CLAUDE.md), harte Grenze 4).

**Erledigt damit:** Issues #2 und #4. **M1 ist abgeschlossen bis auf das
Kanal-Setup (#5).**

---

## 2026-07-30 – Nische und Winkel beschlossen: K3 „Rekonstruktion"

**Entscheidung:** Phase 1 wird mit der Nische **K3 „Rekonstruktion"** gebaut –
ein reales technisches Versagen pro Video, rekonstruiert ausschließlich aus
dem veröffentlichten amtlichen Abschlussbericht. Der ausformulierte Winkel und
die Stil-Referenz stehen in [WINKEL.md](WINKEL.md).

**Begründung:** Empfehlung der Bewertungsmatrix
([NISCHEN-BEWERTUNG.md](NISCHEN-BEWERTUNG.md), Summe 20 von 25, höchster Wert
der fünf Kandidaten). Ausschlaggebend: Winkel und Policy-Versicherung sind
derselbe Mechanismus, bester Evergreen-Wert, schwächste Konkurrenz bei
gesichertem Themennachschub, und das Risiko liegt beim Format statt bei der
Person des Projektinhabers.

**Verworfen:** K1 (K.-o. wegen Winkel 1), K4 „Aktenlage" (bester RPM, aber
presserechtliches Risiko pro Video), K2 „Amtsdeutsch" (Rückfallkandidat),
K5 „Daten" (stärkster Kopierschutz, aber kein Zuschauertreiber und stärkste
Konkurrenz).

**Erledigt damit:** Issues #1 und #3.

---

## 2026-07-30 – Profil des Projektinhabers: eigene Stimme, eigener Schnitt, eigene Grafik

**Sachverhalt:** Der Projektinhaber ist Künstler und Designer, Cutter und
Sprecher. Das war bei der Bewertung nicht bekannt und verändert sie
substanziell (Nachtrag in [NISCHEN-BEWERTUNG.md](NISCHEN-BEWERTUNG.md),
Abschnitt 8).

**Entscheidung:** Sprecherstimme, Schnitt und die gesamte visuelle Sprache
werden **vom Projektinhaber selbst** verantwortet – kein TTS, keine
Bildgeneratoren für die Rekonstruktionsgrafiken. Das sind die
personengebundenen Winkel-Bausteine 5 und 6 in [WINKEL.md](WINKEL.md).

**Begründung:** Damit entfällt das größte Policy-Risiko des Ursprungskonzepts
strukturell statt durch Sorgfalt: Es gibt keine anonyme KI-Erzählstimme, die
Expertenautorität simuliert (die im Juli 2026 benannte Kategorie 3), und keine
generierten Bilder, die unter die KI-Offenlegungspflicht fallen könnten.
Gleichzeitig entsteht der Wiedererkennungswert, den eine generische Pipeline
nicht erreicht – gestaltete Erklärgrafik statt Stockbild mit Zoomeffekt.

**Bewusst akzeptierte Folge:** Der Automatisierungsgrad in Phase 1 sinkt.
Stimme und Schnitt bleiben menschlich; automatisiert werden Research,
Skript-Rohbau, Qualitätsprüfung, SEO und Statistik. Die Blaupause hängt damit
in Phase 1 an einer Person – ein Phase-3-Problem, das in
[WINKEL.md](WINKEL.md) („Bekannter Vorbehalt: Skalierung") festgehalten ist
und nicht jetzt gelöst wird.

---

## 2026-07-30 – KI-Projektleitung durch Opus 5 mit Modell-Delegationsrecht

**Entscheidung:** Die operative Projektleitung übernimmt eine Claude-Session
(Opus 5) auf diesem Repository. Onboarding und Autonomie-Grenzen stehen in
[CLAUDE.md](../CLAUDE.md). Die Projektleitung darf selbstständig Agenten aus
dem geplanten Wellen-Plan ins Leben rufen und je Aufgabe entscheiden, welches
Modell (Opus-/Sonnet-/Haiku-Klasse) sie ausführt – dokumentationspflichtig
(Modell + Kosten je Arbeitsergebnis).

**Begründung:** Setzt die Modellstrategie des Ursprungskonzepts (teure Modelle
für Strategie/Qualität, günstige für Routine) auf Betriebsebene um und macht
das Projekt session-unabhängig: Alles Wissen liegt im Repo, nicht im Chat.

**Harte Grenzen (unverändert beim Projektinhaber):** Grundsatzentscheidungen,
Geld/Budget-Deckel, Veröffentlichungs-Freigaben, Kriterien-Änderungen,
Phasengrenzen.

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

- ~~Nische~~ → beschlossen: K3 „Rekonstruktion" (2026-07-30)
- ~~Unkopierbarer Winkel~~ → beschlossen und ausformuliert: [WINKEL.md](WINKEL.md) (2026-07-30)
- ~~Sprache~~ → beschlossen: Englisch (2026-07-30)
- ~~Phase-1-Kriterien und Budget-Deckel~~ → beschlossen: 600 €, 9 Monate (2026-07-30)

**Alle M1-Grundsatzentscheidungen sind gefallen.** Offen bleibt nur die
operative Umsetzung: Kanal-Setup (#5).

### Verschoben (bewusst nicht jetzt)

- Teilgebiets-Schärfung innerhalb von K3 (Stromnetz/IT/Bahn statt Luftfahrt) –
  Empfehlung liegt in [WINKEL.md](WINKEL.md), Entscheidung sinnvoll nach den
  ersten Research-Briefs statt vorab am Reißbrett.
- Ablösung des Sprecher-Engpasses (Stimmklon, weitere Sprecher) → Phase 3.

## Verschoben / für später notiert

- **Euro-Umrechnung der Modellkosten:** Solange der Abrechnungssatz nicht
  vorliegt, werden Delegationen in Token dokumentiert. Verbindliche
  €-Erfassung ab Beschluss des Budget-Deckels (Issue #4).
