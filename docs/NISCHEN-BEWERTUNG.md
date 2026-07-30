# Nischen-Bewertung und Winkel-Gegentest (Issues #1 + #3)

> **Status: ERLEDIGT – Entscheidung gefallen (2026-07-30).** Der Projektinhaber
> hat **K3 „Rekonstruktion"** festgelegt. Verbindlich ist ab jetzt
> [WINKEL.md](WINKEL.md); dieses Dokument bleibt als Begründungsgrundlage und
> Risikoübersicht erhalten. **Abschnitt 8 ist ein Nachtrag, der die Bewertung
> nach oben korrigiert** – er verändert zwei Noten und die Policy-Lage.
> Entscheidung im [Decision Log](ENTSCHEIDUNGEN.md).

Bearbeitet: 2026-07-30 · Zuständig: KI-Projektleitung · Issues [#1](../../issues/1), [#3](../../issues/3)

Issue #1 und #3 werden gemeinsam bearbeitet, weil ein Nischen-Kandidat ohne
tragfähigen Winkel laut Bewertungsmatrix ohnehin ausscheidet ([STRATEGIE.md](STRATEGIE.md)).

---

## 1. Bewertungsregeln

Fünf Kriterien aus [STRATEGIE.md](STRATEGIE.md), Skala 1–5. Damit die Summen
vergleichbar sind, gilt für **alle** Kriterien: **höher = besser für das
Projekt**. Konkret heißt „Policy-Risiko 5" also *geringes* Risiko und
„Wettbewerbsdichte 5" *wenig* starker Wettbewerb.

**K.-o.-Regel:** „Unkopierbarer Winkel ≤ 2" scheidet aus, unabhängig von den
übrigen Werten. Die Summe ist Orientierung, nicht Automatik – ein einzelnes
Kriterium darf einen Kandidaten kippen, wenn das Risiko beim Projektinhaber
persönlich landet.

**Gegentest zu jedem Winkel** (Issue #3): „Könnte ein generischer KI-Kanal das
nächste Woche nachmachen?" Ein Winkel, der diesen Test nicht besteht, ist kein
Winkel – auch wenn er sich gut anhört.

---

## 2. Recherchegrundlage und ihre Grenzen

Drei Recherche-Zuarbeiten (Wettbewerbsdichte, RPM/Monetarisierung, Policy-Lage)
wurden an Sonnet-Klasse-Subagenten delegiert (Dokumentation in Abschnitt 7).
Die Bewertung, der Gegentest und die Empfehlung stammen von der Projektleitung
selbst.

**Diese Grenzen sind für die Belastbarkeit der Matrix wesentlich und werden
nicht weggeglättet:**

1. **Direkte Seitenaufrufe waren in dieser Umgebung blockiert** (Gateway
   antwortet 403 auf CONNECT, u. a. für `support.google.com`). Alle Angaben
   stammen aus Suchmaschinen-Treffern und Fachmedien, **kein einziges
   Richtlinienzitat wurde am Originaltext gegengelesen.**
2. **Öffentliche RPM-Zahlen nach Nische sind grundsätzlich schwach.** Praktisch
   alle kursierenden Tabellen sind Anbieter-Blogs ohne offengelegte Methodik
   und widersprechen sich. Die RPM-Spalte der Matrix ist die unsicherste.
   Für Technik/Unfallanalyse und Datenjournalismus wurden **überhaupt keine**
   belastbaren Zahlen gefunden.
3. **„Kein Kanal gefunden" ist kein Beweis für eine Marktlücke,** sondern ein
   Indiz für geringe Suchsichtbarkeit. Das betrifft besonders die Kandidaten
   K3 und K4, deren gute Wettbewerbsnote auf Negativbefunden beruht.
4. **Abonnentenzahlen** stammen aus Aggregatoren-Treffern (HypeAuditor u. ä.),
   nicht aus direkt geprüften Kanalseiten.

**Pflicht-Nacharbeit vor Produktionsbeginn** (unabhängig von der Entscheidung):
die drei Google-Hilfeseiten `1311392` (Monetarisierung), `14328491`
(KI-Offenlegung) und `2802008` (Gewaltdarstellung) manuell im Browser
gegenlesen, und die genannten Kanäle direkt auf YouTube prüfen.

### Für alle Kandidaten gleichermaßen relevante Policy-Befunde

Diese vier Befunde verändern die Ausgangslage gegenüber [STRATEGIE.md](STRATEGIE.md)
und gelten kandidatenunabhängig:

- **Januar 2026:** YouTube beendete 16 Kanäle mit zusammen ~35 Mio. Abonnenten
  und ~4,7 Mrd. Lifetime-Views unter der „inauthentic content"-Richtlinie.
  Gemeinsames Muster: massenhafte, templatebasierte Produktion nahezu
  identischer Videos mit KI-Erzählstimme ohne redaktionellen Kontext.
  Berichtet wird auch **Kollateralschaden bei Faceless-Kanälen ohne jede
  KI-Nutzung**. Reviewer bewerten laut Berichten den **gesamten Kanal**, nicht
  Einzelvideos.
- **Juli 2026:** YouTube (Matt Halprin, VP Trust & Safety) beschrieb drei
  Kategorien von inauthentic content. Kategorie 3 – für dieses Projekt der
  wichtigste einzelne Befund – sind **„KI-Personas, die sich als menschliche
  Experten zu sensiblen Themen ausgeben: Gesundheit, Finanzen, Recht,
  Politik."** Genau dieses Muster ist die naheliegendste Bauform eines
  Faceless-Kanals zu Rechts- oder Finanzthemen.
- **Zulässig** ist KI-gestützte Produktion laut YouTube dort, wo „original,
  authentic insights or perspective" erkennbar sind bzw. „significant original
  commentary, modifications, or educational value" hinzukommen.
- **KI-Offenlegungspflicht** greift bei „meaningfully altered or synthetically
  generated" und **realistisch wirkenden** Inhalten. Reine TTS-Sprachausgabe
  löst sie nach übereinstimmenden Sekundärquellen **nicht** aus, solange keine
  echte, identifizierbare Stimme geklont wird; stilisierte Grafiken ebenfalls
  nicht, realistisch wirkende KI-Bilder dagegen schon.

**Konsequenz:** Nicht die Automatisierung ist das Risiko, sondern die
**Behauptung von Expertenautorität durch eine anonyme KI-Stimme**. Wer diese
Behauptung nicht aufstellt, hat das größte Policy-Risiko des Projekts
strukturell entschärft. Dieser Gedanke ist der Grund für die Empfehlung in
Abschnitt 5.

### Was menschliche Kuratierung an dieser Lage ändert – und was nicht

Der Projektinhaber hat klargestellt: **Es geht nichts vollautomatisch raus, es
gibt stets menschliche Kontrolle.** Das ist bereits Projektvoraussetzung
(QS-Veto in [PIPELINE.md](PIPELINE.md), Upload-Freigabe als harte Grenze 3 in
[CLAUDE.md](../CLAUDE.md)) und in den Noten unten schon berücksichtigt. Damit
die Wirkung nicht überschätzt wird, hier die Trennung:

**Kuratierung entschärft** die Kategorien 1 und 2 der Juli-2026-Klarstellung –
generische Templatemassen und emotional manipulative Machart. Das ist genau
das Muster der 16 im Januar 2026 beendeten Kanäle, und dieses Muster können
wir durch Kuratierung tatsächlich vermeiden. Ohne diese Zusage lägen **alle**
Policy-Noten unten niedriger.

**Kuratierung entschärft Kategorie 3 nicht.** Dort geht es nicht um die
Herstellungsweise, sondern um die **Außendarstellung**: ob der Kanal zu einem
sensiblen Thema (Recht, Finanzen, Gesundheit, Politik) den Anschein eines
menschlichen Experten erzeugt. Ein sorgfältig geprüftes Skript, vorgelesen von
einer anonymen Stimme, die deutsches Verwaltungsrecht erklärt, sieht von außen
genauso aus wie ein ungeprüftes. Das trifft K2 und K4 unverändert und ist der
Grund, warum diese beiden Kandidaten in der Policy-Spalte schlecht abschneiden,
obwohl das Projekt kuratiert arbeitet.

**Die dritte Einschränkung ist unangenehm und bleibt bestehen:** Berichtet wird
Kollateralschaden bei Faceless-Kanälen, die **nie** KI genutzt haben. Das
Faceless-Format selbst zieht Prüfaufmerksamkeit an, unabhängig von unserer
Sorgfalt. Kuratierung ist die richtige Antwort darauf, aber keine Garantie –
weshalb das entsprechende Abbruchsignal in
[PHASE-1-KRITERIEN.md](PHASE-1-KRITERIEN.md) („Monetarisierungs-Ablehnung →
sofortiger Produktionsstopp") relevant bleibt und nicht als Formalie zu lesen ist.

---

## 3. Die fünf Kandidaten mit Winkel-Ideen und Gegentest

### K1 – „Alltagspsychologie, erzählt" · *Kontrollkandidat*

**Nische:** Psychologie der Alltagsentscheidungen als Erzählformat – warum
Menschen aufschieben, sich verschätzen, an Preisen hängenbleiben.

**Winkel-Idee:** „Dasselbe Thema, aber sauber recherchiert und mit
Studienquellen belegt."

**Gegentest:** **JA, nächste Woche kopierbar – und zwar bereits kopiert.** Die
Recherche fand für genau dieses Feld aktive deutschsprachige Anleitungen der
Form „Faceless-YouTube-Kanal mit KI automatisieren", die Psychologie/Trivia
als Standard-Einstiegsnische empfehlen. „Studienquellen" sind kein Winkel,
sondern eine Selbstverständlichkeit, die das Manifest ohnehin verlangt
([MANIFEST.md](MANIFEST.md), Grundsatz 3) – und ein Sprachmodell liefert
Quellenangaben genauso schnell wie wir.

**Zweck dieses Kandidaten:** Er ist absichtlich in der Liste. Er dokumentiert,
dass die K.-o.-Regel angewendet wurde und dass „interessante Fakten, aber von
uns" **nachweislich nicht** als Winkel akzeptiert wurde (Akzeptanzkriterium
Issue #3). Er scheidet aus.

---

### K2 – „Amtsdeutsch" · Verwaltungs- und Verfahrensmechanik

**Nische:** Nicht Rechtstipps, sondern **Mechanik**: Was passiert mit einem
Widerspruch *innerhalb* der Behörde? Warum dauert ein Bauantrag neun Monate?
Wie ist das Grundbuch tatsächlich aufgebaut? Zielgruppe sind Bürger, die nicht
Recht, sondern den Ablauf verstehen wollen.

**Winkel-Ideen:**
1. **Primärquellen-Prinzip:** Jedes Video wird aus dem tatsächlichen
   Gesetzestext, der Verwaltungsvorschrift oder der Entscheidung gebaut,
   Paragraf sichtbar im Bild, vollständige Quellenliste im öffentlichen Repo.
2. **Verfahrens-Rekonstruktion als Format:** Das Video folgt einem echten
   Verfahrensweg Schritt für Schritt, statt Regeln aufzuzählen.
3. **Öffentliches Korrektur-Changelog:** Fehler werden datiert korrigiert,
   nicht stillschweigend gelöscht.

**Gegentest:** **Teilweise.** Die *Form* ist in einer Woche imitierbar – ein
Sprachmodell kann Paragrafen einblenden. Die *Fehlerquote* ist es nicht: In
diesem Feld sitzt ein Publikum, das Falschaussagen sofort erkennt und
kommentiert, und Vertrauen entsteht erst über Monate belegbarer Korrektheit.
Der Winkel ist also echt, aber **er wird langsam sichtbar** – in Woche 1
unterscheidet uns nichts von einem Klon. Für einen Kanal, der in Phase 1 gegen
den Kaltstart antritt, ist das eine ernste Schwäche.

**Der eigentliche Killer ist nicht der Winkel, sondern die Bauform:** Ein
Faceless-Kanal mit KI-Stimme, der deutsches Verwaltungsrecht erklärt, ist
exakt die Kategorie 3, die YouTube im Juli 2026 benannt hat („KI-Persona als
vermeintlicher Rechtsexperte"). Dazu kommt das RDG: Allgemeine, abstrakte
Rechtsinformation ist nach § 2 Abs. 1 RDG **keine** Rechtsdienstleistung, weil
der Einzelfallbezug fehlt – das Format ist also zulässig. Riskant wird es in
**Kommentaren und Nachrichten**, sobald auf konkrete Zuschauerfälle eingegangen
wird. Das ist eine dauerhafte Betriebslast, kein einmaliges Problem.
*(Laien-Recherche, keine Rechtsberatung.)*

**Wettbewerb:** Das Oberthema ist stark besetzt – Kanzlei WBS ~1,04 Mio.
Abonnenten, GegenHartz(tv) ~240.000. Für die enge Verfahrensmechanik-Nische
wurde kein dedizierter Kanal gefunden; die großen Nachbarn können sie aber
jederzeit betreten, und zwar mit echter Anwaltsautorität.

---

### K3 – „Rekonstruktion" · Störfälle aus amtlichen Untersuchungsberichten

**Nische:** Ein reales technisches Versagen pro Video – Bahnunfall, Stromnetz-
Störung, Brückenschaden, Industriestörfall, IT-Großausfall, Flugunfall –
rekonstruiert **ausschließlich aus dem offiziellen Abschlussbericht** (BFU,
Bundesstelle für Eisenbahnunfalluntersuchung, BSI, Untersuchungsberichte der
Aufsichtsbehörden).

**Winkel-Ideen:**
1. **Ein Bericht = ein Video, und der Bericht ist im Bild.** Die Quelle ist
   ein benanntes, verlinktes öffentliches Dokument mit Seitenzahl. Die
   Autorität des Kanals liegt **nicht** bei einem behaupteten Experten,
   sondern bei der zitierten Untersuchungsbehörde. Der Kanal sagt ausdrücklich:
   „Wir haben das nicht untersucht – das hier ist, was die Untersuchung ergab,
   Seite 47."
2. **Fester forensischer Aufbau:** Zeitleiste → der Entscheidungspunkt, an dem
   es kippte → was der Bericht als Ursache benennt → **was die
   Berichterstattung damals behauptete und der Bericht nicht stützt.**
3. **Segment „was im Bericht nicht steht":** die offen benannten Grenzen der
   Untersuchung. Das ist die epistemische Ehrlichkeit, die generierte
   Massenware nie liefert, weil sie Sicherheit simulieren muss.
4. **Eigene Diagramm- und Animationssprache** statt Berichtsfotos – aus
   Rechtsgründen (siehe unten) und als wiedererkennbarer Hausstil.

**Gegentest:** **Die Idee ja, die Ausführung nein.** Ein generischer KI-Kanal
kann „Bahnunfall erklärt" nächste Woche veröffentlichen. Er kann nicht billig:
einen 60–200-seitigen deutschen Fachbericht korrekt lesen, technische
Kausalketten fehlerfrei wiedergeben, und das vor einem Publikum aus
Ingenieuren, Bahn- und IT-Leuten, das den Bericht selbst herunterladen kann.
In dieser Nische ist **Nachprüfbarkeit die Verteidigung**: Der Klon muss
entweder denselben Aufwand treiben – dann ist er kein billiger Klon mehr –
oder er produziert sichtbare Fehler. Kein exklusiver Datenzugang (die Berichte
sind öffentlich), deshalb 4 und nicht 5.

**Warum dieses Format policy-seitig ungewöhnlich gut liegt:**
- Die **„Sensitive Events"-Klausel** trifft vor allem *laufende* Ereignisse.
  Ein Abschlussbericht existiert erst Jahre nach dem Ereignis – die
  Formatregel „nur abgeschlossene Untersuchungen mit veröffentlichtem
  Bericht" ist damit gleichzeitig die Policy-Versicherung. Das ist kein
  Zusatzaufwand, sondern fällt mit dem Format zusammen.
- Sachlich-dokumentarischer Kontext ist in den Werberichtlinien **ausdrücklich
  der mildernde Faktor** bei Unglücksinhalten; reißerische Bebilderung und
  Opferdarstellung sind das Verbotene. Eigene Diagramme statt Unfallfotos
  treffen genau die zulässige Seite.
- **Es gibt keine Experten-Persona,** also greift Kategorie 3 nicht.

**Restrisiken, klar benannt:**
- **Bildrechte.** § 5 UrhG stellt den *Text* amtlicher Werke frei, **nicht
  automatisch Fotos und Grafiken darin** – die können eigenständigen
  Lichtbildschutz nach § 72 UrhG genießen. Die BFU beansprucht im Impressum
  ausdrücklich Rechte an ihren Inhalten: journalistische Nutzung kostenlos
  **mit Quellenangabe**, Bilder mit fremder Quellenangabe nur nach
  schriftlicher Zustimmung. Für die Eisenbahn-Unfalluntersuchung war die Lage
  nicht ermittelbar. → Deshalb ist Winkel-Idee 4 (eigene Grafiken) keine
  Kür, sondern Voraussetzung. *(Laien-Recherche, keine Rechtsberatung.)*
- **Werbetauglichkeit deckelt möglicherweise den RPM,** selbst bei
  Freischaltung durch YouTube: Werbekunden steuern Unfall-Themen über ihre
  eigenen „content suitability"-Einstellungen aus. Das ist in der RPM-Note
  berücksichtigt.

**Wettbewerb:** Für Flugunfälle gibt es im Deutschen zwei thematisch passende
Kanäle („Flugzeugkatastrophen", „Flugforensik" – letzterer arbeitet ebenfalls
mit Untersuchungsberichten), Abonnentenzahlen nicht ermittelbar. Für
**Bahn, Stromnetz, Industrie und IT-Ausfälle im Rekonstruktionsformat wurde
kein einziger dedizierter deutschsprachiger Kanal gefunden**; ein deutsches
Gegenstück zum englischen „Plainly Difficult" existiert offenbar nicht. Was
existiert, sind Sender-Dokus zu Einzelereignissen – teuer produziert,
unregelmäßig, kein Katalog. Wichtig: Das ist ein Negativbefund (siehe
Abschnitt 2, Grenze 3), keine bewiesene Marktlücke.

---

### K4 – „Aktenlage" · Wirtschaftsskandale aus Gerichts- und Aufsichtsdokumenten

**Nische:** Wirtschaftskriminalität rekonstruiert aus Gerichtsentscheidungen,
BaFin-Material und Untersuchungsausschuss-Dokumenten – der Wirecard-Typ Fall,
aber systematisch und aus den Akten.

**Winkel-Ideen:**
1. Dieselbe Primärquellendisziplin wie K3, angewandt auf Wirtschaftsdelikte.
2. „Was in der Akte steht und in der Berichterstattung nicht."
3. Aufarbeitung der **Aufsichtsversagen**, nicht der Personen – die Mechanik
   statt der Empörung.

**Gegentest:** **Grenzwertig.** Die Primärquellendisziplin ist echt, aber das
Genre (True Crime / Skandal) ist international das am stärksten mit
KI-Massenware bespielte Feld überhaupt. Der Winkel muss hier gegen sehr viel
Lärm ankommen.

**Warum ich diesen Kandidaten trotz der besten RPM-Aussichten nicht
empfehle:** Das Risiko landet persönlich beim Projektinhaber. Nach der
Rechtsprechung zur Verdachtsberichterstattung (BGH, Urteil vom 22.02.2022,
VI ZR 1175/20) ist **Namensnennung** nur zulässig, wenn das
Öffentlichkeitsinteresse an der Identität das Geheimhaltungsinteresse
überwiegt – bei nicht prominenten Beschuldigten regelmäßig **nicht**. Ein
Kanal in diesem Feld ohne anwaltliche Begleitung trägt ein reales
Abmahn- und Klagerisiko, und zwar bei jedem einzelnen Video. Dazu kommt
Kategorie 3 (Finanzthemen) und die Werbetauglichkeitsdämpfung von
Kriminalitätsinhalten. *(Laien-Recherche, keine Rechtsberatung.)*

**Wettbewerb:** Kein dedizierter deutschsprachiger Kanal gefunden; das Thema
ist medial hochpräsent (viele Sender-Dokus zu Wirecard), aber nicht als
serielles Format. Ein englisches Gegenstück existiert („Coffeezilla").

---

### K5 – „Deutschland in Daten" · reproduzierbarer Datenjournalismus

**Nische:** Eigene Auswertungen amtlicher Daten (Destatis, Eurostat,
Bundesbank) als wiederkehrendes Kernformat – Langzeitserien statt Tagesaktuelles.

**Winkel-Ideen:**
1. **Jede Analyse als lauffähiges öffentliches Repository** (Daten + Code).
   Wer will, reproduziert das Ergebnis selbst.
2. Eigene, strenge Diagrammsprache als visuelle Handschrift.
3. Öffentliche Korrekturen samt Auswirkung auf die Aussage.

**Gegentest:** **Nein – und das ist der strukturell härteste Winkel der
Liste.** Ein generischer KI-Kanal kann kein lauffähiges, reproduzierbares
Analyse-Repository fälschen; entweder der Code läuft und liefert die gezeigte
Zahl, oder er tut es nicht. Das ist Unkopierbarkeit im wörtlichen Sinn.

**Warum er trotzdem nicht die Empfehlung ist:** Reproduzierbarkeit ist ein
Graben gegen *Kopierer*, aber kein Grund für *Zuschauer* zu klicken – und
Phase 1 muss zuerst Reichweite und Retention beweisen. Dazu zwei harte
Einwände: Der Winkel setzt echte Datenkompetenz beim Ausführenden voraus (er
ist nicht an eine KI delegierbar), und die Nachbarschaft ist die stärkste im
ganzen Feld – Simplicissimus ~2,45 Mio., MrWissen2go ~2,39 Mio. Abonnenten,
beide mit Redaktion und Budget. RPM-Daten: keine gefunden; politiknahe
Analyse gilt tendenziell als schwächer monetarisierbar.

---

## 4. Die vollständige Bewertungsmatrix

Skala 1–5, **höher = besser für das Projekt** (Policy-Risiko 5 = geringes
Risiko; Wettbewerbsdichte 5 = wenig starker Wettbewerb).

| | **K1** Alltags­psychologie | **K2** Amtsdeutsch | **K3** Rekonstruktion | **K4** Aktenlage | **K5** Daten |
|---|---|---|---|---|---|
| **Unkopierbarer Winkel** | **1** | 3 | **4** | 3 | **4** |
| **Wettbewerbsdichte** | 1 | 3 | 4 | 4 | 2 |
| **Policy-Risiko** | 1 | 2 | 4 | 1 | 3 |
| **RPM / Monetarisierung** | 2 | 4 | 3 | **5** | 2 |
| **Evergreen-Faktor** | 3 | 2 | **5** | 4 | 3 |
| **Summe** | **8** | 14 | **20** | 17 | 14 |
| **Status** | **K.-o.** | – | **Empfehlung** | nicht empfohlen | – |

### Begründung je Zelle

**K1 – Alltagspsychologie**
- *Winkel 1:* „Sauber recherchiert" ist kein Winkel; das Feld wird in Faceless-Anleitungen aktiv als Standardnische empfohlen.
- *Wettbewerb 1:* Hohe Dichte an Trivia-Kurzformaten plus laufender Zustrom automatisierter Kanäle.
- *Policy 1:* Templatebasierte Faktenvideos mit KI-Stimme sind exakt das Muster der 16 im Januar 2026 beendeten Kanäle.
- *RPM 2:* Psychologie/Selbstoptimierung wird durchgehend unter Bildung/Lifestyle im unteren Mittelfeld verortet.
- *Evergreen 3:* Zeitlos, aber ohne Katalogwert, weil beliebig ersetzbar.

**K2 – Amtsdeutsch**
- *Winkel 3:* Primärquellendisziplin und Verfahrensrekonstruktion sind echt, wirken aber erst über Monate und sind in der Form imitierbar.
- *Wettbewerb 3:* Enge Nische unbesetzt, aber sehr starke Nachbarn (WBS ~1,04 Mio.) mit echter Anwaltsautorität können jederzeit einsteigen.
- *Policy 2:* Direkter Treffer auf Kategorie 3 („KI-Persona als Rechtsexperte"); dazu dauerhafte RDG-Einzelfallgrenze in Kommentaren. **Diese Note steigt auf 4, wenn ein namentlich erkennbarer Mensch mit einschlägiger Qualifikation als Autor auftritt** – dann ist es kein vorgetäuschter Experte. Menschliche Kuratierung allein genügt dafür nicht (siehe Abschnitt 2); nötig ist sichtbare Autorschaft. Deshalb Frage 2 in Abschnitt 6.
- *RPM 4:* Recht/Verbraucherrecht wird über alle (schwachen) Quellen konsistent als überdurchschnittlich beschrieben.
- *Evergreen 2:* Gesetzesänderungen entwerten den Katalog – der Widerspruch zur Blaupausen-These „Katalogwert vor Spike" ([MANIFEST.md](MANIFEST.md), Grundsatz 7).

**K3 – Rekonstruktion**
- *Winkel 4:* Idee kopierbar, Ausführung nicht billig; Nachprüfbarkeit durch ein fachlich wehrhaftes Publikum ist die Verteidigung. Kein exklusiver Zugang → nicht 5.
- *Wettbewerb 4:* Zwei Kanäle im Teilbereich Luftfahrt, für Bahn/Strom/Industrie/IT kein dedizierter deutschsprachiger Kanal gefunden. Negativbefund, kein Beweis.
- *Policy 4:* Formatregel „nur abgeschlossene Berichte" entschärft die Sensitive-Events-Klausel strukturell; dokumentarischer Kontext ist der ausdrücklich mildernde Faktor; keine Experten-Persona. Abzug für Bildrechte (§ 72 UrhG) und Werbetauglichkeit.
- *RPM 3:* Keine belastbaren Daten für dieses Feld gefunden; Technik gilt als solides Mittelfeld, Unfallthemen dämpfen die Werbenachfrage.
- *Evergreen 5:* Ein abgeschlossener Untersuchungsbericht veraltet nie. Ein Bericht von 1998 ist in drei Jahren genauso gültig und suchbar.

**K4 – Aktenlage**
- *Winkel 3:* Quellendisziplin echt, aber das Genre ist am stärksten mit Massenware besetzt.
- *Wettbewerb 4:* Kein dediziertes deutschsprachiges Format gefunden.
- *Policy 1:* Persönlichkeitsrecht bei Namensnennung (BGH VI ZR 1175/20) erzeugt ein Klagerisiko pro Video, das persönlich beim Projektinhaber liegt; dazu Kategorie 3 und Werbedämpfung.
- *RPM 5:* Finanzen/Wirtschaft ist der einzige über alle Quellen hinweg konsistent als teuerste Nische beschriebene Bereich.
- *Evergreen 4:* Abgeschlossene Fälle bleiben relevant, laufende Verfahren veralten.

**K5 – Deutschland in Daten**
- *Winkel 4:* Lauffähiges Analyse-Repo ist strukturell unfälschbar – stärkster Mechanismus der Liste, aber kein Zuschauertreiber, und nicht delegierbar.
- *Wettbewerb 2:* Die thematisch nächsten Kanäle sind die größten (~2,45 Mio. / ~2,39 Mio.) mit Redaktion und Budget.
- *Policy 3:* Inhaltlich unkritisch, die Lockerung für kontroverse Themen von Januar 2026 hilft; politiknahe Inhalte bleiben werbeseitig gedämpft.
- *RPM 2:* Keine Daten gefunden; politiknahe Analyse gilt als schwächer monetarisierbar.
- *Evergreen 3:* Daten altern, die Methodik und Langzeitserien halten.

**Ergebnis der K.-o.-Regel:** K1 scheidet mit Winkel 1 aus. Damit ist
Akzeptanzkriterium von Issue #3 erfüllt: „Interessante Fakten, aber von uns"
wurde geprüft und **nicht** als Winkel akzeptiert.

---

## 5. Empfehlung

**Empfehlung: K3 – „Rekonstruktion". Ein reales technisches Versagen pro
Video, ausschließlich aus dem veröffentlichten amtlichen Abschlussbericht,
mit eigener Diagrammsprache und dem Segment „was im Bericht nicht steht".**

Vier Gründe, in der Reihenfolge ihres Gewichts:

1. **Der Winkel und die Policy-Versicherung sind derselbe Mechanismus.**
   [STRATEGIE.md](STRATEGIE.md) fordert genau das („Der unkopierbare Winkel
   ist auch die Policy-Versicherung"), aber bei den anderen Kandidaten sind es
   zwei getrennte Aufgaben. Hier fällt es zusammen: Die Regel „nur
   abgeschlossene Berichte" erzeugt gleichzeitig die inhaltliche Tiefe, die
   Abgrenzung zur Tagesaktualität und die Distanz zur Sensitive-Events-Klausel.
   Und weil die Autorität ausdrücklich bei der zitierten Behörde liegt und
   nicht bei einer behaupteten Expertenfigur, greift die im Juli 2026 benannte
   Kategorie 3 nicht – die Kategorie, die K2 und K4 direkt trifft.

2. **Bester Evergreen-Wert der Liste, und der zählt hier doppelt.** Das
   Projektziel ist eine reproduzierbare Blaupause, nicht ein einzelner Hit.
   Ein Katalog aus abgeschlossenen Untersuchungsberichten wächst monoton und
   entwertet sich nicht – anders als K2, dessen Bestand mit jeder
   Gesetzesänderung erodiert.

3. **Die schwächste Konkurrenz bei belastbarem Themennachschub.** Für Bahn,
   Stromnetz, Industrie und IT-Ausfälle wurde kein deutschsprachiger Kanal in
   diesem Format gefunden, während die Berichte kostenlos, laufend neu und in
   großer Zahl verfügbar sind. Die Nachschubfrage – bei Nischenformaten
   regelmäßig das stille Scheitern – ist hier gelöst.

4. **Das Risiko bleibt beim Format, nicht bei der Person.** K4 hätte den
   besten RPM, aber jedes Video wäre ein presserechtliches Wagnis für den
   Projektinhaber. K2 verlangt dauerhafte Disziplin an der RDG-Grenze in jedem
   Kommentarfeld. K3 verlangt handwerkliche Sorgfalt – Berichte richtig lesen,
   eigene Grafiken erstellen. Das ist Arbeit, kein Haftungsrisiko, und Arbeit
   ist genau das, was ein billiger Klon nicht aufbringt.

**Was ich gegen die eigene Empfehlung einwende, damit es entschieden und nicht
übersehen wird:** Der RPM ist bei K3 nur mittel, und er ist die unsicherste
Zahl der Matrix – für dieses Feld wurden **überhaupt keine** belastbaren
RPM-Daten gefunden, und Unfallthemen können werbeseitig gedeckelt sein. Wer
Phase 2 vor allem über Werbeeinnahmen finanzieren will, hätte mit K2 die
bessere Wette. Meine Einschätzung: Für Phase 1 ist das zweitrangig, weil die
Erfolgskriterien Retention und CTR heißen, nicht Umsatz
([PHASE-1-KRITERIEN.md](PHASE-1-KRITERIEN.md)), und weil aus K3 gut ableitbare
Phase-2-Produkte entstehen (Fallsammlungen, Aufbereitungen für Lehre und
betriebliche Schulung).

**Rückfallkandidat, falls K3 abgelehnt wird:** K2 – höherer RPM, geringeres
Rechtsrisiko als K4, aber mit zwei bewusst zu akzeptierenden Lasten
(Kategorie-3-Nähe und Katalogerosion). **K4 empfehle ich trotz Platz 2 in der
Summe ausdrücklich nicht** – die Summe verdeckt hier, dass ein einzelnes
Kriterium persönliche Haftung bedeutet.

**Berührungspunkt zu Issue #2 (Sprache):** Die Wettbewerbsvorteile von K3
existieren so nur im **deutschsprachigen** Markt – im Englischen steht dort
etabliertes Angebot. Das ist ein Argument für Deutsch, aber die Sprachfrage
gehört in Issue #2 und wird hier nicht mitentschieden.

---

## 6. Konkrete Frage an den Projektinhaber

**Frage 1 (Entscheidung, blockiert alles Weitere):** Wird **K3 –
„Rekonstruktion"** als Nische für Phase 1 festgelegt, mit den vier
Winkel-Ideen aus Abschnitt 3 als Grundlage für die Winkel-Ausformulierung in
Issue #3? Antwortoptionen: **(a) ja, K3** · **(b) nein, stattdessen K2** ·
**(c) nein, keiner der Kandidaten überzeugt – neue Runde mit geänderten
Vorgaben.**

**Frage 2 (unabhängig von Frage 1 zu beantworten, verändert die Bewertung):**
Welche fachliche Vorbildung, berufliche Erfahrung oder besonderen Zugänge
bringst du persönlich mit? Das Repo enthält dazu nichts, und es ist die
einzige Lücke, die die Matrix substanziell verändern könnte:

- Technischer oder ingenieurwissenschaftlicher Hintergrund → **stärkt K3** um
  einen zweiten, personengebundenen Winkel.
- Juristische Qualifikation → **hebt K2 klar über K3**, weil damit die
  Kategorie-3-Schwäche entfällt: Dann ist es kein KI-Experte, sondern ein
  echter.
- Daten-/Statistikkompetenz → **hebt K5** von „interessantem Mechanismus" zu
  tragfähigem Winkel.
- Keiner davon → K3 bleibt die Empfehlung, weil sein Winkel als einziger
  allein auf Arbeitsdisziplin beruht und keine Qualifikation voraussetzt.

**Nach der Entscheidung übernimmt die Projektleitung ohne weitere Rückfrage:**
Winkel-Ausformulierung als Stil-Referenz für den Skript-Agenten (Issue #3),
Eintrag ins Decision Log, Datenlage für die Sprachentscheidung (Issue #2),
und die in Abschnitt 2 festgelegte Pflicht-Nacharbeit an den Originalquellen.

---

## 7. Modell-Delegation (Dokumentationspflicht laut PROJEKTPLAN.md)

| Arbeitsschritt | Modellklasse | Ausführung | Umfang |
|---|---|---|---|
| Kandidatenbildung, Winkel-Ideen, Gegentests, Bewertung, Empfehlung, dieses Dokument | Opus-Klasse | Projektleitung selbst | – |
| Zuarbeit 1: Wettbewerbsdichte der fünf Themenrichtungen (DE) | Sonnet-Klasse | Subagent | ~81 Tsd. Token, 45 Werkzeugaufrufe, ~5 min |
| Zuarbeit 2: RPM-/Monetarisierungsdaten und Werberichtlinien | Sonnet-Klasse | Subagent | ~59 Tsd. Token, 29 Werkzeugaufrufe, ~5 min |
| Zuarbeit 3: Policy-Lage „inauthentic content", KI-Offenlegung, § 5 UrhG, RDG | Sonnet-Klasse | Subagent | ~73 Tsd. Token, 36 Werkzeugaufrufe, ~5 min |

**Begründung der Wahl:** Recherche-Zuarbeit mit Urteilsvermögen entspricht der
mittleren Klasse laut Delegationsrichtlinie; Bewertung und Empfehlung fallen
unter „Strategie und Entscheidungsvorlagen" und wurden nicht delegiert. Alle
drei Subagenten waren beauftragt, belegte Angaben von eigenen Schätzungen zu
trennen und Nichtwissen auszuweisen – die Lücken in Abschnitt 2 sind das
Ergebnis dieser Auflage und ausdrücklich gewollt.

**Kosten in Euro:** nicht angegeben, weil dafür der Abrechnungssatz des Kontos
nötig wäre, der hier nicht vorliegt. Statt einer geschätzten Zahl steht oben
der tatsächliche Tokenverbrauch. Sobald der Budget-Deckel in Issue #4
beschlossen ist, wird die Umrechnung im Produktionsprotokoll verbindlich
mitgeführt.

---

## 8. Nachtrag nach der Entscheidung: das Profil des Projektinhabers

Die Bewertung oben entstand **ohne Kenntnis** des fachlichen Hintergrunds –
Frage 2 in Abschnitt 6 war genau deshalb gestellt. Die Antwort lautet:
**Künstler und Designer, Cutter, Sprecher.** Das ist keine Randnotiz, sondern
korrigiert die Bewertung von K3 an zwei Stellen nach oben. Der Nachtrag steht
hier statt in der Matrix, damit nachvollziehbar bleibt, was vor und was nach
der Entscheidung bekannt war.

### Was sich ändert

| Kriterium | vorher | jetzt | Grund |
|---|---|---|---|
| Unkopierbarer Winkel | 4 | **5** | Aus dem Winkel wird ein zweiter, **personengebundener** Mechanismus: eine selbst gestaltete Rekonstruktionssprache von einem Designer ist nicht mit Aufwand aufzuholen, sondern gar nicht – Gestaltungsqualität ist keine Fleißaufgabe. Der Gegentest („nächste Woche kopierbar?") fällt damit klar negativ aus. |
| Policy-Risiko | 4 | **5** | Kein TTS und keine generierten Bilder heißt: keine anonyme KI-Erzählstimme, die Autorität simuliert (Kategorie 3 entfällt vollständig), und kein Auslöser der KI-Offenlegungspflicht. Der Kanal ist nicht „KI-Produktion mit Sorgfalt", sondern handwerkliche Produktion mit KI-Zuarbeit. Das ist der Unterschied, den YouTubes Formulierung „original, authentic insights or perspective" beschreibt. |

**Neue Summe für K3: 22 von 25.** Die drei Kandidatenlücken bleiben, wo sie
waren – nur K3 profitiert von diesem Profil, weil K2/K4 ihre Schwäche im
Rechtsbereich haben und K5 Datenkompetenz verlangt.

### Was sich nicht ändert

- **Die RPM-Unsicherheit bleibt die größte offene Flanke.** Für dieses Feld
  wurden weiterhin keine belastbaren Zahlen gefunden; Unfallthemen können
  werbeseitig gedeckelt sein. Das Profil verbessert die Qualität, nicht die
  Werbenachfrage.
- **Die Pflicht-Nacharbeit aus Abschnitt 2 bleibt vollständig bestehen**
  (drei Google-Hilfeseiten am Originaltext gegenlesen, genannte Kanäle direkt
  prüfen). Ein gutes Profil ersetzt keine Quellenprüfung.
- **Der Negativbefund bleibt ein Negativbefund:** „kein deutschsprachiger
  Kanal gefunden" ist weiterhin kein Beweis für eine Marktlücke.
- **Bildrechte bleiben relevant** – eigene Grafiken sind jetzt Stärke *und*
  weiterhin rechtliche Voraussetzung (§ 72 UrhG).

### Die unangenehme Kehrseite, damit sie nicht untergeht

Eigene Stimme, eigener Schnitt und eigene Grafik sind der Grund für die
verbesserten Noten – und gleichzeitig **drei personengebundene Engpässe**. Der
Automatisierungsgrad in Phase 1 sinkt damit deutlich unter das, was das
Ursprungskonzept anvisierte: Automatisierbar bleiben Research, Skript-Rohbau,
Qualitätsprüfung, SEO und Statistik; Sprechen, Schneiden und Gestalten nicht.

Das ist die richtige Reihenfolge – erst Qualität beweisen, dann skalieren –
aber es heißt: **Die Blaupause hängt in Phase 1 an einer Person.** Wer daraus
in Phase 3 mehrere Kanäle ableiten will, muss diesen Engpass dann bewusst
lösen (siehe [WINKEL.md](WINKEL.md), „Bekannter Vorbehalt: Skalierung"). Nicht
jetzt, aber auch nicht vergessen.
