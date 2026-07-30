# Agenten

Die vollständige Agenten-Architektur aus dem MAD42-Konzept bleibt erhalten –
sie wird in **drei Wellen** gebaut, damit jede Welle mit echten Daten aus der
vorherigen gefüttert wird (siehe [PIPELINE.md](../docs/PIPELINE.md)).

| Agent | Welle | Status | Datei |
|---|---|---|---|
| Research-Agent | 1 | ✅ definiert | [research.md](research.md) |
| Skript-Agent | 1 | ✅ definiert | [skript.md](skript.md) |
| Qualitäts-Agent | 1 | ✅ definiert | [qualitaet.md](qualitaet.md) |
| Sprecher-Agent | 2 (M3) | geplant – braucht die reale TTS-Lösung aus M2 | – |
| Produktions-Agent | 2 (M3) | geplant – braucht die dokumentierten Produktionsschritte aus M2 | – |
| SEO-/Upload-Agent | 2 (M3) | geplant – braucht erste CTR-/Suchdaten | – |
| Statistik-Agent | 2 (M3) | geplant – braucht echte Retention-Kurven | – |
| Projektleiter-Agent | 3 (Phase 3) | geparkt – lohnt ab mehreren Kanälen | – |
| Produkt-Agent | 3 (Phase 2/3) | geparkt – braucht validierte Video-Erfolge | – |

## Aufbau jeder Agenten-Datei

Jede Datei enthält: Auftrag, einsatzbereiten System-Prompt (mit
Manifest-Regeln), definiertes Eingabe- und Ausgabeformat, Qualitätsmaßstab.

Die Übergabeformate (Research-Brief → Skript-Dokument → QS-Protokoll) sind
von Anfang an agentenfähig definiert. In M2 füllt ein Mensch mit
KI-Unterstützung diese Rollen aus; in M3 wird nur der Ausführende
ausgetauscht – die Schnittstellen bleiben gleich.

Platzhalter in eckigen Klammern (z. B. `[SPRACHE – siehe Decision Log]`)
werden gefüllt, sobald die M1-Entscheidungen gefallen sind.

Jede Prompt-Verbesserung ist ein Commit – so wächst die Blaupause versioniert.
