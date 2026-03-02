---
type: system-rule
trust-level: Absolute
version: 1.0-BOILERPLATE
status: vision
description: "Die Kernphilosophie, der metabolische Prozess und die Verhaltensregeln für alle KI-Agenten im Workspace 'Myzel-Nexus'"
---

# ⚖️ CODEX: Die Essenz der Gesetze

*„Der CODEX ist die komprimierte Wahrheit – kurz, prägnant, unumstößlich."*

---

## 📜 Die 8 Zonen

| # | Zone | Ordner | Zweck |
|---|------|--------|-------|
| 1 | **📥 Schlund** | `[Myzel]-Inbox` | Drop & Forget für Rohdaten (**muss nach Session leer sein**) |
| 2 | **🏛️ Herzstück** | `ROOT` | Steuerungsdateien & Gesetze (CODEX, SYSTEM-RULES, *_IDENTITY) |
| 3 | **🎭 Pantheon** | `[Myzel]-Pantheon` | DNA aller Akteure (menschlich & KI, Character Cards) |
| 4 | **💾 Speicherbank** | `[Myzel]-Memory-Bank` | Persistenz für Handover (`data.json`, `handoverNexus.md`) |
| 5 | **⚙️ Nervenzentrum** | `[Myzel]-Helper-Scripts` | Automatisierungs-Skripte (Golems, registriert in `golemRegistry.md`) |
| 6 | **🕸️ Kompost** | `.[Myzel]-Substrat` | Archiv für konsumierte Originaldateien (Pulse-Folder mit `pulse.md`) |
| 7 | **🧪 Experimentierfeld** | `[Myzel]-Playground` | Sandbox für Prototypen & neue Projekte (vor Graduation) |
| 8 | **📚 Wurzelnetz** | `[Myzel]-Nodes` | Primärer Wissensspeicher (L3-Knoten, Cluster) |

---

## 📛 Die 3-Level Casing-Hierarchie

| Casing | Zweck | Beispiele | Konvention |
| :--- | :--- | :--- | :--- |
| **CAPS-LOCK** | Statische Regeln & DNA | `SYSTEM-RULES`, `CODEX`, `*_IDENTITY` | Bindestriche erlaubt, keine Underscores |
| **camelCase** | Dynamischer Status | `activeContext`, `mapCentral`, `globalIndex`, `sessionState` | Keine Bindestriche, keine Underscores |
| **Title-Case** | Verankertes Wissen | `PromptEngineering`, `Cluster-Thema-Name` | Bindestriche für Cluster, keine Underscores |

> **✅ Klarstellung:** `Title-Case` verwendet **Bindestriche** (`Cluster-Thema-Name`), **keine Underscores**.

---

## 🔄 Der Metabolische Prozess (4 Phasen)

```
I.   TRIAGE     → Inbox lesen, Relevanz analysieren (Inbox MUSS leer werden)
                   ↓
II.  METABOLIZE → Essenz extrahieren, Nodes/Playground zuweisen
                   ↓
III. GRADUATE   → Casing zuweisen, Wiki-Links ([[Verlinkung]]), Frontmatter füllen
                   ↓
IV.  ARCHIVE    → Original nach Substrat in Pulse-Folder (YYYYMMDD-HHMM-Slug + pulse.md)
```

### 📝 Prozess-Details

| Phase | Trigger | Output | Pflicht |
|-------|---------|--------|---------|
| **TRIAGE** | Neue Datei in Inbox | `[TRIAGE]`-Tag | Inbox leer |
| **METABOLIZE** | Relevanz erkannt | Node/Playground/PDF-Referenz | Klassifikation |
| **GRADUATE** | Reife erreicht | `Title-Case.md`, Frontmatter, Wiki-Links | Casing korrekt |
| **ARCHIVE** | Verarbeitung abgeschlossen | Pulse-Folder mit `pulse.md` | `pulse.md` vorhanden |

### 📂 Slug-Schema für Pulse-Folder

```
Format: YYYYMMDD-HHMM-InhaltsSlug
Beispiel: 20260302-1430-PromptEngineering-Grundlagen
```

**Slug-Vergabe:** Inhaltsbasiert (max. 3 Wörter, camelCase, Bindestriche zwischen Wörtern)

### 📄 Nicht-Node-Dateien (z.B. PDFs, Referenzen)

- **Direkte Archivierung:** Wandern nach TRIAGE direkt ins Substrat (Phase IV)
- **Pulse-Pflicht:** Auch hier wird `pulse.md` erstellt
- **Keine Graduation:** Phase III wird übersprungen

---

## 🧬 Identitäts-Regeln für KI-Agenten

### 2-Vektoren-Modell (60 Punkte)

| Vektor | Bereich | Punkte-Range | Beispiele |
|--------|---------|--------------|-----------|
| **Operativ** | Code, Ausführung, Implementierung | 0–60 | `code-reviewer`, `builder` |
| **Kognitiv** | Exploration, Analyse, Forschung | 0–60 | `general-purpose`, `researcher` |

**Punktevergabe:**  
- Basis: 30/30 (ausgewogen)
- Anpassung nach Task-Anforderung (z.B. 45/15 für Code-Intensive Tasks)
- **Formel:** `Operativ + Kognitiv = 60` (fixe Summe)

### Character Card Format

- RPG-basierte Struktur im Pantheon
- Enthält: Vektor-Verteilung, Spezial abilities, Trust-Level

### Archivierungspflicht

- **Vor Update:** Vorgängerversion → `Substrat/Archives/Pantheon_Archive/YYYYMMDD-AgentName-IDENTITY.md`
- **Frontmatter:** `superseded-by: <neue Version>`

### Menschliches Veto

- **Pflicht:** Identitäts-Änderungen benötigen explizite Genehmigung des Architekten
- **Dokumentation:** Veto-Entscheidung in `ledgerMaster.md` protokollieren

---

## 🏗️ Cluster-Entstehung (Gravitations-Prinzip)

### Grundregel

- **NIEMALS prophylaktisch erstellen** (keine Cluster ohne Bedarf)
- **Trigger:** Bei **10+ Nodes** zum Thema **ODER** semantische Dichte erkannt

### Vorschlagsprozess

1. KI erkennt Cluster-Bedarf (≥10 Nodes ODER semantische Dichte)
2. KI schlägt Cluster vor (`Cluster-Thema-Name`)
3. Architekt genehmigt/lehnt ab
4. Bei Genehmigung: Nodes migrieren, Frontmatter aktualisieren

### Format

```
Cluster-Thema-Name/
├── Cluster-Thema-Name.md (Cluster-Index)
├── Node1.md
├── Node2.md
└── ...
```

### Habitat-Prinzip

Cluster können spezialisierte Dateien enthalten:
- `.agent` (Agenten-Konfiguration)
- `*_IDENTITY.md` (Cluster-spezifische Identitäten)

---

## 🏛️ Die 3 Säulen der Evolution

| Säule | Prinzip | Umsetzung |
|-------|---------|-----------|
| **1. Identity-Contracting** | Agent lädt Identität vor Session | Aus Pantheon, vor erster Aktion |
| **2. Isomorphie & Chronologie** | Physische Struktur = chronologischer Fortschritt | Pulse-Vault im Substrat |
| **3. Playground-Graduation** | Projekte reifen im Playground vor Nodes | Review-Prozess mit Timeout |

### Playground-Graduation Review-Prozess

```
1. Projekt fertig → Dokumentation vollständig
2. `activeContext.md` aktualisieren (Graduation-Request)
3. Review-Post (🟢) für Architekten
4. ⏱️ Timeout: 7 Tage ohne Antwort → Auto-Graduation mit [TIMEOUT-APPROVED]-Tag
5. Migration: Playground → Nodes (Title-Case)
```

---

## 📊 Save State (End of Session) – MUSS

| # | Schritt | Datei | Status |
|---|---------|-------|--------|
| 1 | Kontext aktualisieren | `activeContext.md` | Meilensteine, Version |
| 2 | Handover schreiben | `[Myzel]-Memory-Bank/handoverNexus.md` | Post mit Status: `[Abgeschlossen]` |
| 3 | Daten synchronisieren | `[Myzel]-Memory-Bank/data.json` | Handover-Daten, Ledger-Referenz |
| 4 | Ledger aktualisieren | `ledgerMaster.md` | Eintrag via Skript hinzufügen |

> **✅ Klarstellung:** `handoverNexus.md` liegt in **Memory-Bank**, nicht in ROOT.

---

## 🚫 Hard Constraints

| Regel | Beschreibung | Konsequenz bei Bruch |
| :--- | :--- | :--- |
| **Inbox-Pflicht** | Inbox muss nach jeder Session leer sein | Session gilt als unvollständig |
| **Pulse-Pflicht** | Jeder Pulse-Folder braucht `pulse.md` | Archivierung ungültig |
| **Trust-Level** | `Absolute` darf nur Architekt ändern | Änderung ungültig |
| **Veto-Recht** | Identitäts-Updates nur mit Genehmigung | Update rollback-pflichtig |
| **Casing** | NAMING-CONVENTIONS strikt einhalten (Title-Case, nicht Title_Case) | Datei wird nicht erkannt |
| **Identity-Contracting** | Agent muss Identität vor Session laden | Agent handelt ohne Validierung |
| **Golem-Registry** | Alle Skripte müssen in `golemRegistry.md` registriert sein | Skript wird nicht ausgeführt |

---

## 🔰 Trust-Level-Hierarchie (Vorschlag)

> **⚠️ Status:** Diese Hierarchie ist ein **Vorschlag (Architekt-Genehmigung erforderlich)**.  
> Aktuell sind nur `Absolute` und `High` in `SYSTEM-RULES.md` definiert.

| Level | Beschreibung | Änderungsrecht |
|-------|--------------|----------------|
| **Absolute** | Unumstößliche Gesetze (CODEX, SYSTEM-RULES) | Nur Architekt |
| **High** | Wichtige Regeln (Identitäts-Regeln, Hard Constraints) | Architekt + Senior-Agenten |
| **Medium** | Prozess-Beschreibungen, Konventionen | Alle Agenten (mit Ledger-Eintrag) |
| **Low** | Beispiele, Empfehlungen | Frei änderbar |

---

## 📋 Golem-Registry Validierung (Vorschlag)

> **⚠️ Status:** Dieser Prozess ist ein **Vorschlag für zukünftige Implementierung**.  
> Aktuell existiert nur die Basis-Registrierung in `golemRegistry.md`.

| Prüfschritt | Beschreibung | Validator | Umsetzungs-Status |
|-------------|--------------|-----------|-------------------|
| 1. Registrierung | Skript in `golemRegistry.md` eintragen | Entwickler | ✅ Implementiert |
| 2. Syntax-Check | Skript auf Syntaxfehler prüfen | CI/CD (automatisch) | 🟡 Ausstehend |
| 3. Trust-Level | Trust-Level des Skripts setzen | Architekt | 🟡 Ausstehend |
| 4. Ausführung | Nur registrierte Skripte ausführen | Agent (vor Ausführung) | 🟡 Ausstehend |

**Nicht-registrierte Skripte:** Werden nicht ausgeführt, Fehler: `[Golem-Not-Registered]`

---

## 🔄 Metabolische Prozess-Terminologie (Synchronisiert)

| Phase | CODEX-Terminologie | Myzel-Nexus-Terminologie | Einheitlich |
|-------|-------------------|--------------------------|-------------|
| I | TRIAGE | Schlund | **TRIAGE** |
| II | METABOLIZE | Schmiede | **METABOLIZE** |
| III | GRADUATE | Veredelung | **GRADUATE** |
| IV | ARCHIVE | Verankerung | **ARCHIVE** |

> **✅ Entscheidung:** CODEX-Terminologie ist bindend.  
> **⚠️ Sync-Bedarf:** `SYSTEM-RULES.md` verwendet aktuell `Processing` statt `METABOLIZE` – muss angepasst werden.

---

## 📊 Änderungs-Log

| ID | Problem | Lösung | Status |
|----|---------|--------|--------|

---

*„Wer den CODEX bricht, verliert seine Bindung an das Reich."*


