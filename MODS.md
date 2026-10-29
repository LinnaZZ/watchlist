<p align="center"><img src="assets/mods/mods-banner.svg" width="100%" alt="Mods-Katalog – geprüfte Mods, Skills &amp; MCP-Server mit Ampel und Herkunft"></p>

# 🧩 Mods-Katalog

<p align="center"><a href="README.md"><img src="assets/mods/back-button.svg" width="300" alt="← Zur Watchlist"></a></p>

Ergänzung zur [Watchlist](README.md): Plugins, Skills, Hooks, Mods und MCP-Server – jeweils mit **Herkunft** (offiziell oder Community) und **Sicherheits-Ampel**.

**Stand: 2026-10-29** · **138 Einträge** in 14 Gruppen · 14 × 🏛️ offiziell · 124 × 👥 Community · 20 × 🟢 · 97 × 🟡 · 21 × 🔴

> [!CAUTION]
> Plugins, Skills, Hooks und „Mods“ laufen **mit deinen Rechten** (Claude-Code-Mods laut offizieller Doku ohne Sandbox): Sie können Dateien lesen/schreiben, Befehle starten und Daten senden. Bewertet wurde nur durch Lesen von Code und Doku – **nichts wurde ausgeführt**. Keine Garantie: vor der Installation selbst prüfen, z. B. mit `claude plugin validate ./plugin`, Version pinnen, nichts per `curl | bash` installieren.

## 📚 Inhalt

| | |
| --- | --- |
| [**🏛️ Offizielle Mods**](#offiziell)<br><sub>14 Einträge · Übersicht</sub> | [**🛡️ 1. Sicherheit & Kontrolle**](#sicherheit)<br><sub>27 Einträge</sub> |
| [**💰 2. Kosten & Usage**](#kosten)<br><sub>15 Einträge</sub> | [**🖥️ 3. Anzeige & UI**](#anzeige)<br><sub>20 Einträge</sub> |
| [**🧠 4. Lernen & Regeln**](#lernen)<br><sub>9 Einträge</sub> | [**🤝 5. Multi-Agent & Fremdmodelle**](#multi-agent)<br><sub>9 Einträge</sub> |
| [**🎨 6. Frontend & Animation**](#frontend)<br><sub>11 Einträge</sub> | [**🧩 7. Skills: Denken & Recherche**](#skills)<br><sub>14 Einträge</sub> |
| [**🎬 8. MCP & Kreativ-Tools**](#mcp-kreativ)<br><sub>10 Einträge</sub> | [**🗺️ 9. Visualisierung**](#visualisierung)<br><sub>5 Einträge</sub> |
| [**🔌 10. MCP: SaaS-Anbindungen**](#mcp-saas)<br><sub>3 Einträge</sub> | [**🏛️ 11. Offizielle Anthropic-Skills**](#anthropic-skills)<br><sub>9 Einträge</sub> |
| [**📦 12. Sammlungen**](#sammlungen)<br><sub>2 Einträge</sub> | [**🔍 13. Prüfwerkzeuge**](#pruefwerkzeuge)<br><sub>2 Einträge</sub> |
| [**🔎 Weitere Funde**](#nebenfund)<br><sub>2 Einträge</sub> | [**🧭 Legende**](#legende)<br><sub>Ampel &amp; Herkunft</sub> |

<a id="legende"></a>

> [!TIP]
> **Legende**
> - Ampel: ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) Code gelesen und unauffällig, bekannte Herkunft oder rein lesend/anzeigend, kein Netz, keine Zusatzkosten · ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) unbedenklich mit Auflagen (z. B. junges Einzel-Repo: Version pinnen; Token-Kosten; schreibt in Konfiguration; startet Prozesse) · ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) vorerst nicht einrichten bzw. nur in einer Wegwerf-Umgebung (z. B. `curl | bash`-Installer, Telemetrie standardmäßig an, Daten gehen an fremde Server).
> - Herkunft: ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) = direkt von Anthropic (GitHub-Orgs `anthropics`/`anthropic-ai` oder in Claude Code eingebaut) · ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) = alles von Dritten, auch Hersteller wie Cloudflare oder NVIDIA.
> - Herkunft sagt nichts über Sicherheit: auch offizielle Einträge haben eine eigene Ampel.

**Abschalten & Prüfen:** Offizielle Doku zu Mods: <https://code.claude.com/docs/en/plugins/mods/overview> · Mods sind ab Claude Code 2.1.287 standardmäßig an · einzeln abschalten über `/plugin`, für eine Sitzung mit `--safe-mode`, alle eigenen Hooks mit `"disableAllHooks": true` · ohne Ausführen prüfen mit `claude plugin validate ./mod`.

**Quellen:** Verzeichnisse wie claude-mods.com, claudemods.ai und claudemod.com sind 👥 Community-Seiten ohne Impressum und nur Hinweisquellen – ihr „verified“ oder „checked by hand“ ist kein Sicherheits-Audit. Jeder Eintrag hier wurde am Primär-Repo geprüft.

---

<a id="offiziell"></a>

## 🏛️ Offizielle Mods (Übersicht)

<img src="assets/mods/cat-offiziell.svg" width="100%" alt="Offizielle Mods">

Alle 14 Einträge mit ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb), also direkt von Anthropic. Einige davon (z. B. Blast Radius, Replay Theater, Token Weather) sind laut README Beispiele aus `anthropics/claude-code-playground` und kein unterstütztes Produkt – die Ampel gilt deshalb wie bei Community-Code.

| Name | Ampel | Abschnitt |
| :-- | :-: | :-- |
| [Blast Radius](https://github.com/anthropics/claude-code-playground/tree/main/claude-code/mods/blast-radius) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) | [🛡️ 1. Sicherheit & Kontrolle](#sicherheit) |
| [Replay Theater](https://github.com/anthropics/claude-code-playground/tree/main/claude-code/mods/replay-theater) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) | [🛡️ 1. Sicherheit & Kontrolle](#sicherheit) |
| [You Should Know](https://code.claude.com/docs/en/plugins/mods/overview#mods-built-into-claude-code) (`cc-plugin-you-should-know`) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) | [🛡️ 1. Sicherheit & Kontrolle](#sicherheit) |
| [frontend-design](https://github.com/anthropics/skills/tree/main/skills/frontend-design) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) | [🏛️ 11. Offizielle Anthropic-Skills](#anthropic-skills) |
| [canvas-design · theme-factory · brand-guidelines](https://github.com/anthropics/skills/tree/main/skills/canvas-design) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) | [🏛️ 11. Offizielle Anthropic-Skills](#anthropic-skills) |
| [internal-comms · doc-coauthoring · discernment-nudge](https://github.com/anthropics/skills/tree/main/skills/doc-coauthoring) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) | [🏛️ 11. Offizielle Anthropic-Skills](#anthropic-skills) |
| [academy-guide · algorithmic-art · claude-api · mcp-builder · slack-gif-creator](https://github.com/anthropics/skills/tree/main/skills/claude-api) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) | [🏛️ 11. Offizielle Anthropic-Skills](#anthropic-skills) |
| [docx · pdf · pptx · xlsx](https://github.com/anthropics/skills/tree/main/skills/docx) | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) | [🏛️ 11. Offizielle Anthropic-Skills](#anthropic-skills) |
| [skill-creator](https://github.com/anthropics/skills/tree/main/skills/skill-creator) | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) | [🏛️ 11. Offizielle Anthropic-Skills](#anthropic-skills) |
| [web-artifacts-builder](https://github.com/anthropics/skills/tree/main/skills/web-artifacts-builder) | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) | [🏛️ 11. Offizielle Anthropic-Skills](#anthropic-skills) |
| [webapp-testing](https://github.com/anthropics/skills/tree/main/skills/webapp-testing) | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) | [🏛️ 11. Offizielle Anthropic-Skills](#anthropic-skills) |
| [template-skill](https://github.com/anthropics/skills/tree/main/template) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) | [🏛️ 11. Offizielle Anthropic-Skills](#anthropic-skills) |
| [Token Weather](https://github.com/anthropics/claude-code-playground/tree/main/claude-code/mods/token-weather) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) | [🔎 Weitere Funde](#nebenfund) |
| [plugin-authoring](https://code.claude.com/docs/en/plugins/mods/overview#mods-built-into-claude-code) (`cc-plugin-plugin-authoring`) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) | [🔎 Weitere Funde](#nebenfund) |

---

<a id="sicherheit"></a>

## 1. Sicherheit & Kontrolle (Guards, Review)

<img src="assets/mods/cat-01-sicherheit.svg" width="100%" alt="1. Sicherheit &amp; Kontrolle (Guards, Review)">

| Name | Herkunft | Typ | Wofür | Ampel |
| :-- | :-: | :-- | :-- | :-: |
| [Blast Radius](https://github.com/anthropics/claude-code-playground/tree/main/claude-code/mods/blast-radius) | ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) | Mod (tool.call-Guard + Pane) | Hält riskante Bash-Befehle an (`rm -r/-f`, `git reset --hard`, `git clean`, Force-Push, Migrationen), zeigt, was betroffen wäre, und verlangt Proceed oder Cancel | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [Replay Theater](https://github.com/anthropics/claude-code-playground/tree/main/claude-code/mods/replay-theater) | ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) | Mod (Recorder + `/replay`-Pane) | Spielt nach jedem Turn die Datei-Edits von Claude Schritt für Schritt als Diff ab | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [You Should Know](https://code.claude.com/docs/en/plugins/mods/overview#mods-built-into-claude-code) (`cc-plugin-you-should-know`) | ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) | Eingebauter Mod (Side-Agent) | Ein zweiter Agent liest Claudes Ausgaben mit und blendet Wichtiges über dem Prompt ein, z. B. Kostenhinweise | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [launch-codes](https://github.com/OneWave-AI/claude-code-mods/tree/main/launch-codes) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (tool.call-Guard Bash + Alarm-Pane) | Riskante Bash-Befehle (`rm -rf` auf riskante Pfade, Force-Push, `git reset --hard`, DROP/TRUNCATE, `supabase db reset`, `vercel --prod`, `chmod -R 777`, curl/wget in eine Shell) brauchen einen Einmal-Code | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [security-audit-skill](https://github.com/cloudflare/security-audit-skill) (Skill `security-audit`) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill (Markdown + 2 Node-Validatoren ohne Abhängigkeiten) | Sicherheits-Audit eines Repos: viele parallele Subagents suchen Schwachstellen, belegen sie und schreiben einen Bericht | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [reverse-skill](https://github.com/zhaoxuya520/reverse-skill) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill-Sammlung (599 Dateien) + Bootstrap-Skript | Router für Reverse Engineering und Pentests: Payload-Bibliotheken, Burp-MCP-Brücke, Kali-Werkzeuge | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) |
| [secret-redactor (davila7)](https://github.com/davila7/claude-code-templates/tree/main/cli-tool/components/mods/security/secret-redactor) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (`tool.call`-Hook nach dem Tool) | Schwärzt bekannte Key-/Token-Formate (AWS, Anthropic, OpenAI, GitHub, Google, Stripe, Slack, JWT, PEM, DB-URLs mit Passwort) in Tool-Ausgaben, bevor Claude sie sieht | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [large-edit-confirmation](https://github.com/davila7/claude-code-templates/tree/main/cli-tool/components/mods/security/large-edit-confirmation) (davila7) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (`tool.call`-Guard auf Edit/Write) | Fragt nach, bevor Claude eine Datei mit mehr als 1.000 Zeilen (einstellbar) per Edit oder Write ändert | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [jev-auto-mode](https://github.com/davila7/claude-code-templates/tree/main/cli-tool/components/mods/security/jev-auto-mode) (davila7) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Permission-Layer) | JSON-Policy plus KI-Richter (TypeSafe „Jev“), der entscheidet, ob Tool-Calls laufen dürfen | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) |
| [ash / claude-skills](https://github.com/randommonicle/claude-skills) (Reddit „43 Claude Code guardrails“) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Plugin: 56 Guardrail-Skills + 13 Hook-Aufrufe (Node) + Normen beim Sessionstart | Leitplanken aus echten Fehlern: push-gate fragt vor Push/Merge, Warnungen bei SQL, Secrets und kill, Linter nach jedem Edit | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [Probity](https://github.com/nizos/probity) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Claude-Code-Plugin (PreToolUse-Hook) + npm-Paket `@nizos/probity` | Prüft vor jedem Bash/Write/Edit/NotebookEdit-Call Regeln aus `probity.config.ts` (z. B. TDD erzwingen, Befehle sperren) und blockt bei Verstoß | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [anchorwatch-mod](https://github.com/anchorwatch-dev/anchorwatch/tree/main/plugins/anchorwatch-mod) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (tool.call-Guard) | Blockt `rm -rf` auf riskante Pfade, Force-Push, `DROP TABLE`, Pipe-in-Shell-Downloads und `cat .env`, bevor sie laufen | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [guardrails (arasovic)](https://github.com/arasovic/claude-code-mods/tree/main/guardrails) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (tool.call-Guard Bash) | Verweigert `cf deploy/migrate/init`, Attribution-Zeilen in Commits/PRs und Branches mit Präfix `claude/`, je per Schalter | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [loop-guard](https://github.com/arasovic/claude-code-mods/tree/main/loop-guard) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Fehler-Zähler + versteckte Notiz) | Scheitert derselbe Schritt zweimal, bekommt Claude eine versteckte Notiz, den Ansatz zu wechseln | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [secret-guard](https://github.com/arasovic/claude-code-mods/tree/main/secret-guard) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Redaction + Lese-Sperre) | Maskiert Schlüssel in Tool-Ausgaben, blockt `.env`-Lesen und Befehle, die Geheimnisse ausgeben | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [assertion-guardian](https://github.com/ccdwyer/claude-mods) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Edit-Guard für Tests) | Verweigert Test-Edits, die Assertions entfernen, Tests überspringen oder Erwartungswerte ändern | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [collision-guard](https://github.com/nateherkai/claude-code-mods/tree/main/collision-guard) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Edit-Guard + Abfrage) | Fragt nach, bevor Claude eine Datei ändert, die ein anderer offener Chat gerade geändert hat | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [recording-mode](https://github.com/nateherkai/claude-code-mods/tree/main/recording-mode) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Anzeige-Maske) | Maskiert Schlüssel, Namen und Geldbeträge auf dem Bildschirm und hält private Dateien zu, solange man aufnimmt | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [env (davekiss)](https://github.com/davekiss/env) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (eigene Tools + Eingabe-Pane) | Claude sieht nur die Namen der `.env`-Schlüssel und fragt Werte über ein Pane ab, das es selbst nicht lesen kann | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (strenge Auflagen) |
| [git-gates](https://github.com/bahaospanov/skills) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (tool.call-Guard git) | Blockt Commit, Push und Merge, solange die letzte Nachricht es nicht verlangt, und prüft Commit-Messages | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [harness-mods](https://github.com/ucsandman/Agnostic-AI/tree/main/engine/mods) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod-Paar (Runtime-Adapter + Guards) | Routing der Subagent-Modelle, Geheimnis-Redaction, Lese-Cache und Subagent-Abrechnung, je Guard im Modus classic/shadow/mod | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (strenge Auflagen) |
| [honmoon-redact](https://github.com/pleaseai/honmoon/tree/main/packages/claude-plugin) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Redaction + Lese-Sperre) für ein lokales Gateway | Schwärzt Geheimnisse und PII in Tool-Ausgaben und Prompts und blockt das Lesen von Schlüsseldateien | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [pii-guard](https://github.com/danyuchn/pii-guard) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod + lokaler Python-Dienst | Reversible PII-Schwärzung (auf Taiwan-Daten ausgelegt) für Tool-Ergebnisse, Prompts und Writes, alles über Loopback | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [secret-redactor (ray-amjad)](https://github.com/ray-amjad/claude-code-mods) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Redaction), laut Seite | Ersetzt Geheimnisse, Mails und IPs durch Platzhalter, bevor das Modell sie sieht | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst, nicht prüfbar) |
| [taxi-speedcam](https://github.com/devbrother2024/devbrothers-mods) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (tool.call-Guard + Abfrage) | Fängt Force-Push, `rm -rf`, DB-Wipes und Prod-Deploys ab und fragt nach | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [toolgate](https://github.com/RiskAverseTech/toolgate) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod / PreToolUse-Hook / MCP-Proxy | Fragt TypeSafes Modell „Jev“ pro Tool-Aufruf sieben Risikofragen und erlaubt, fragt nach oder blockt | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst) |
| [wp-credential-guard](https://github.com/nathanonn/agent-skills) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Redaction + Rückersetzung) | Maskiert WordPress-Logins für das Modell und setzt die echten Werte erst in Bash-Befehle wieder ein | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |

<sub>[↑ Inhalt](#-inhalt)</sub>

---

<a id="kosten"></a>

## 2. Kosten & Usage

<img src="assets/mods/cat-02-kosten.svg" width="100%" alt="2. Kosten &amp; Usage">

| Name | Herkunft | Typ | Wofür | Ampel |
| :-- | :-: | :-- | :-- | :-: |
| [Cache Tax](https://github.com/karanb192/cache-tax) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (prompt.submit-Guard + `/keepwarm`, `/cache-tax`) | Warnt vor einem „kalten“ Prompt-Cache, zeigt die geschätzten Kosten für das erneute Einlesen und kann den Cache mit Pings warmhalten | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [burn-meter](https://github.com/OneWave-AI/claude-code-mods/tree/main/burn-meter) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Band über dem Prompt + Pane) | Live-Feuerbalken für die Session-Kosten, Plan-Limits mit Reset-Zeit, Kosten in Burritos umgerechnet | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [session-wrapped](https://github.com/OneWave-AI/claude-code-mods/tree/main/session-wrapped) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (`/wrapped`-Pane + PNG) + 2 Python-Skripte | „Spotify Wrapped“ für Session, Woche und Monat (Tool-Calls, Tests, Kosten), dazu eine teilbare PNG-Karte | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [context-lens](https://github.com/Arunjay4213/claude-mods/tree/main/plugins/context-lens) (+ quota-meter, token-ledger, budget-guard) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | 4 Mods aus einer Sammlung (Statuszeilen + Panes, `/context-lens`, `/quota`, `/ledger`, `/guard`) | context-lens: Kontextfüllung und Wachstum pro Turn mit Balken je Kategorie. quota-meter: Plan-Fenster mit Reset-Countdown. token-ledger: Kosten und Tokens pro Turn. budget-guard: stoppt die Session über einem Dollar- oder Plan-Limit | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [effort-cycle](https://github.com/Anerco/claude-code-effort-cycle) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Tasten Ctrl+↑/↓, Effort-Anzeige im Footer und in den Subagent-Zeilen) | Stellt den Reasoning-Effort pro Agent um und zeigt ihn als farbige Skala | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [rtk](https://github.com/rtk-ai/rtk) („Rust Token Killer“) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Rust-Binary + PreToolUse-Hook (`rtk init -g`) | Kürzt die Ausgabe von Shell-Befehlen (git, Tests, Build), damit weniger Tokens im Kontext landen | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [prompt-cache-control](https://github.com/davila7/claude-code-templates/tree/main/cli-tool/components/mods/observability/prompt-cache-control) (davila7) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Band + Pane `/cache`, Toasts) | Zeigt live Cache-Treffer, Cache-Ablauf (TTL) und Compaction-Einstellungen | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [claude-code-templates-CLI](https://github.com/davila7/claude-code-templates) (`npx claude-code-templates`) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Installer-CLI (npm 1.30.0) für 45 Mods und weitere Komponenten | Installiert Mods per `--mod <kategorie>/<name>` nach `.claude/skills/<name>/` | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) im Default / 🟡 mit Auflagen |
| [context-mode](https://github.com/mksglu/context-mode) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | MCP-Server + Hooks (Plugin, npm `context-mode`) | Hält rohe Tool-Ausgaben aus dem Kontext: führt Befehle in Sandbox-Prozessen aus, indiziert Ergebnisse in SQLite-FTS5 und gibt nur Auszüge zurück | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [caveman](https://github.com/JuliusBrussee/caveman) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill + Plugin, dazu CLI, Proxy, MCP und Cloud („six rocks“) | Lässt den Agenten in extrem knapper „Höhlenmenschen“-Sprache antworten und komprimiert Ein- und Ausgaben, um Tokens zu sparen | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst; nur Plugin 🟡) |
| [Chisle](https://github.com/JayPokale/Chisle) (Schreibweise so korrekt, npm `chisle`; nicht „Chisel“) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Plugin (Skills, Hooks, MCP-Proxy), Installer für 13 Agenten | Spart Tokens auf drei Wegen: knappe Prosa, YAGNI-Code, Kompression von Tool-Ausgaben | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [context-bar](https://github.com/hamzafer/claude-code-mods/tree/main/mods/context-bar) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Band über dem Prompt) | Zeigt das Kontextfenster als gestapelten Balken, eine Farbe je Kategorie | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [fast-jev-compaction](https://github.com/tamaratran/fast-jev-compaction) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (ersetzt Compaction) | Löscht bei der Compaction veraltete Tool-Aufrufe statt zusammenzufassen, der Rest bleibt wörtlich | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst) |
| [effortless](https://github.com/HeyCubit/effortless) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (prompt.submit + Bänder) | Wählt je Prompt die Effort-Stufe und zeigt, wie lange der Prompt-Cache warm bleibt | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (strenge Auflagen) |
| [context-attachment-manager](https://github.com/chipfighter/context-attachment-manager) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod + lokaler Proxy | Wählt aus, welche früheren Bilder mit der nächsten Nachricht mitgehen, der Rest wird zu Platzhaltern | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst) |

<sub>[↑ Inhalt](#-inhalt)</sub>

---

<a id="anzeige"></a>

## 3. Anzeige & UI (Panels, Themes, Dateibaum)

<img src="assets/mods/cat-03-anzeige.svg" width="100%" alt="3. Anzeige &amp; UI (Panels, Themes, Dateibaum)">

| Name | Herkunft | Typ | Wofür | Ampel |
| :-- | :-: | :-- | :-- | :-: |
| [Claude Skins](https://github.com/hellosverre/claude-skins) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (UI-Reskin) + Skill `skin-designer` | Themes für Tool-Zeilen, Spinner und Antwort-Gutter, wechselbar mit `/skin` | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [Filetree](https://github.com/data-goblin/claude-code-filetree) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Seitenpane) | Dateibaum rechts. Zeigt, welche Dateien Claude liest, schreibt oder committet, dazu Git-Status und Zeilen-Diffs | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [Savvy Progress](https://github.com/JohnnyVizz/claude-kit/tree/main/plugins/savvy-progress) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Band + Agents-Panel) + 2 MCP-Tools | Fortschrittsbalken über dem Prompt und Live-Panel aller Subagents mit Modell, Fortschritt, Kontext und geschätzten Kosten | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [Terminal Browser](https://github.com/zenbu-labs/terminal-browser) (Plugin unter [`claude-code-plugin/`](https://github.com/zenbu-labs/terminal-browser/tree/main/claude-code-plugin)) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod + **externe Electron-App** + Skill | Echter Browser im Terminal neben dem Chat (`/browser`), über das Kitty-Grafikprotokoll | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst) |
| [Flightdeck](https://github.com/scasella/claude-flightdeck) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Live-Pane + Statuszeile, `/flightdeck`) | Dashboard: Modell-Vitals (ttft, tok/s), „Architect“-Konsultationen, jede Permission-Prüfung (Gate), Subagent-Karten und Swimlanes, Turn-Beleg, Session-Log | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [agent-narrator](https://github.com/OneWave-AI/claude-code-mods/tree/main/agent-narrator) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Pane, `/narrate`) | Übersetzt jeden Agenten-Schritt in einen Satz in Alltagssprache und schätzt die gesparte Zeit | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [inner-monologue](https://github.com/OneWave-AI/claude-code-mods/tree/main/inner-monologue) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Pane) | Schreibt trockene „innere Gedanken“ von Claude zu dem, was es gerade tut | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [sportscaster](https://github.com/OneWave-AI/claude-code-mods/tree/main/sportscaster) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Pane + Ticker + Audio) | Kommentiert die Session wie eine Live-Sportübertragung, laut per TTS und mit generiertem Publikumsjubel | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [code-pet](https://github.com/OneWave-AI/claude-code-mods/tree/main/code-pet) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Statuszeile + Pane) | Pixel-Haustier: frisst bei Tool-Calls, wird bei Fehlern krank, gerät bei destruktiven Befehlen in Panik | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [boss-fight](https://github.com/OneWave-AI/claude-code-mods/tree/main/boss-fight) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Pane) | Fehlschlagende Tests erzeugen einen Pixel-Boss, jeder Testlauf mit Fixes trifft ihn | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [inbox-alerts](https://github.com/OneWave-AI/claude-code-mods/tree/main/inbox-alerts) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Toasts + Statuszeile + Pane, `/alerts`) | Holt Gmail, Slack und Google Calendar über die claude.ai-Connectoren und zeigt neue Einträge im Terminal; `/alerts triage` übergibt sie an Claude | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst) |
| [agent-flow](https://github.com/Charlie0113-T/claude-agent-flow) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Pane, `/flow`, `/flow text`) | Live-Baum der Subagents einer Session neben dem Transkript | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [cctop](https://github.com/tomstagl/cctop) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Rust-Programm (TUI-Dashboard) + Plugin (`/cctop`, Skills `cctop`, `cctop-insights`) | „btop“ für Claude Code: Kontext, Tokens, Kosten, Limits, Tools, Agents, Cache und Coach-Hinweise in einem Pane oder Terminal-Split | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [statuspane](https://github.com/xuanji86/claude-statuspane) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (schwebende Statuskarte + Progress-API) | Karte mit Modell, Kontext, Rate-Limits, Kosten, Verzeichnis/Branch, optional CI-Status, plus Fortschrittszeilen, die Skripte über JSON-Dateien melden | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [firstmate-calm](https://github.com/kunchenguid/firstmate/tree/main/.claude/mods/firstmate-calm) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (UI) | Blendet Tool-Zeilen aus und ersetzt den Spinner durch ein Segelboot, Umschalten mit `/calm` | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [textfold](https://github.com/chenxiachan/textfold) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (UI) | Zeigt jede Antwort in fünf Stufen, vom ganzen Text bis zu einem Satz, je eine Taste | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [cc-stretch](https://github.com/pro-vi/cc-stretch) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (UI) | Antworten kommen kurz, ein Klick auf eine Phrase klappt sie aus | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [Habblaud](https://github.com/marmottajr/habblaud) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod + lokale Web-App (Node/Docker) | Ein Pixel-Büro, in dem jeder Claude-Code-Agent live zeigt, was er tut, mit Usage-Anzeige | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (strenge Auflagen) |
| [remctl](https://github.com/viticci/remctl) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod + CLI/MCP (macOS) | Zeigt die heutigen Apple-Erinnerungen über dem Prompt, dazu Tools, mit denen Claude sie verwaltet | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [Storybloq](https://github.com/Storybloq/storybloq) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Pane) + npm-CLI | Board der Tickets und Issues aus `.story/` in einem Pane neben dem Transkript | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |

<sub>[↑ Inhalt](#-inhalt)</sub>

---

<a id="lernen"></a>

## 4. Lernen & Regeln (Memory/Workflow)

<img src="assets/mods/cat-04-lernen.svg" width="100%" alt="4. Lernen &amp; Regeln (Memory/Workflow)">

| Name | Herkunft | Typ | Wofür | Ampel |
| :-- | :-: | :-- | :-- | :-: |
| [Reflect](https://github.com/BayramAnnakov/claude-reflect) (Mod: [`mod/`](https://github.com/BayramAnnakov/claude-reflect/tree/main/mod) = `reflect-mod`) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Band) · alternativ Python-Plugin mit Settings-Hooks, Commands und Skill | Erkennt Korrekturen („nein, so nicht …“) und bietet per Button an, sie als Regel in `./CLAUDE.md` oder `~/.claude/CLAUDE.md` zu speichern | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [i-have-adhd](https://github.com/ayghri/i-have-adhd) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Plugin (Output-Style-Skill + optionaler SessionStart-Hook) | Antworten kurz, klar und in Schritten, bis „stop adhd mode“ | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [ponytail](https://github.com/DietrichGebert/ponytail) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Plugin (Regeln, 3 Hooks) + Mod „band“ | Bringt Claude zu minimalem Code mit wenigen Änderungen, mit Modus-Umschalter und Statistik | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [book-to-skill](https://github.com/virgiliojr94/book-to-skill) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill (879 Zeilen) + Python-Extraktor | Macht aus einem Buch (PDF/EPUB) einen eigenen Skill mit Kernideen und Regeln | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [GSD Core](https://github.com/open-gsd/gsd-core) (Nachfolger von gsd-build/get-shit-done) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Framework (Commands, Agents, Skills, rund 32 Hooks, MCP-Server), npm `@opengsd/gsd-core` | Spec-getriebene Entwicklung: Projekt in Phasen planen, ausführen und prüfen lassen | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [Claude Auto Handoff](https://github.com/alexknowshtml/claude-auto-handoff) (alexknowshtml) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Function Hooks), `--plugin-dir` | Ersetzt Auto-Compact: kurz vor vollem Kontext schreibt Haiku eine Übergabe-Notiz, dann `/clear` und eine frische Session liest sie | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [unlazy](https://github.com/Leonxlnx/unlazy) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill + Node-Checker, optionaler Stop-Hook | „Anti-Faulheit“: zwingt den Agenten, vorab Abnahme-Kriterien mit prüfbaren Checks festzulegen und erst bei bestandenen Checks „fertig“ zu melden | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [time-machine](https://github.com/YeonwooSung/my-claude-code-mods) (agent-time-machine) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Timeline-Pane) | Jeder Tool-Aufruf auf einer verzweigten Zeitleiste mit Snapshots: ansehen, zurückholen, verzweigen, neu ausführen | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [after](https://github.com/midudev/better-claude) (midudev) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Warteschlange) | Reiht Aufgaben für nach dem aktuellen Turn ein, ohne Claude mitten im Turn umzulenken | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |

<sub>[↑ Inhalt](#-inhalt)</sub>

---

<a id="multi-agent"></a>

## 5. Multi-Agent & Fremdmodelle (Subagents anderer Anbieter)

<img src="assets/mods/cat-05-multi-agent.svg" width="100%" alt="5. Multi-Agent &amp; Fremdmodelle (Subagents anderer Anbieter)">

| Name | Herkunft | Typ | Wofür | Ampel |
| :-- | :-: | :-- | :-- | :-: |
| [BitFrost](https://github.com/SavaSoftworks/BitFrost) (Plugin unter [`plugins/bitfrost/`](https://github.com/SavaSoftworks/BitFrost/tree/main/plugins/bitfrost)) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Function Hooks `register.js`) + lokaler Daemon `bitfrostd` + CLI `bitfrost` + optionale ZCode-Bridge | Claude Code startet Subagents mit Modellen anderer Anbieter über deren eigene Apps: Codex (GPT), ZCode (GLM), experimentell opencode, Oh My Pi, Gemini CLI. Claude kann Status abfragen, Nachrichten schicken, stoppen und fortsetzen | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (Richtung 🔴 für sensible Repos) |
| [swarm](https://github.com/OneWave-AI/claude-code-mods/tree/main/swarm) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Pane) | Live-Ansicht eines Agent-Teams: Agenten, Nachrichten zwischen ihnen, Ereignisse | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [agent-race](https://github.com/OneWave-AI/claude-code-mods/tree/main/agent-race) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Pane, `/race`) | Mehrere Sessions treten auf derselben Aufgabe gegeneinander an (Vergleich von Modellen oder Prompts) | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [oh-my-claudecode](https://github.com/Yeachan-Heo/oh-my-claudecode) (OMC) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Plugin-Sammlung (~30 Hooks, Agents, Skills, Team-Modus) + npm `oh-my-claude-sisyphus` | Orchestrierung mehrerer Agents (Claude, Codex, Gemini) mit Keyword-Modi, Persistenz und Teams | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (strenge Auflagen) |
| [Orgtree](https://github.com/Maurdekye/orgtree) (v2, „Now an App“; aktuell v4.4.3) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Desktop-App (Electron mit Rust-Engine, Python, Node), steuert Claude Code, Codex, Gemini, OpenCode | Visueller Multi-Agent-Orchestrator: Agenten-Hierarchie auf einer Leinwand, Work Docket (Tickets), geteiltes Gedächtnis, mehrere Konten pro Anbieter | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [Ouroboros](https://github.com/Q00/ouroboros) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | „Agent OS“: Python-Paket `ouroboros-ai` + Claude-Plugin mit Hooks | Zerlegt Ziele per Interview in Specs und lässt Agenten sie in Schleifen umsetzen und prüfen | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst) im Default / 🟡 mit Auflagen |
| [Ruflo](https://github.com/ruvnet/ruflo) (früher Claude Flow, `ruvnet/claude-flow` leitet per 301 auf dieselbe Repo-ID 995029641 um; npm `ruflo` 3.59.17, intern `@claude-flow/cli`) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Agent-Harness: CLI + MCP-Server (README: 314 Tools), Hooks, Daemon, Hive-Mind/Swarm, Plugin-Marktplatz mit über 40 Plugins | Orchestriert viele Agenten (Swarm, Hive-Mind) mit Vektor-Gedächtnis, automatischem Routing und Hintergrund-Workern | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst; Plugin `ruflo-core` mit lokal gepinnter CLI 🟡) |
| [Shared Sessions](https://github.com/Paradigm-Study/claude-share) (`shared-session`) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Live-Sitzung teilen) | Teilt eine Sitzung per Link, andere treten aus ihrem Claude Code bei und prompten live mit | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst) |
| [shunt](https://github.com/pleaseai/shunt) (Mod) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Mod (Band) zu einem LLM-Gateway | Zeigt Restkontingent und Reset-Zeiten des Account-Pools aus dem shunt-Gateway | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |

<sub>[↑ Inhalt](#-inhalt)</sub>

---

<a id="frontend"></a>

## 6. Frontend & Animation (Skills)

<img src="assets/mods/cat-06-frontend.svg" width="100%" alt="6. Frontend &amp; Animation (Skills)">

| Name | Herkunft | Typ | Wofür | Ampel |
| :-- | :-: | :-- | :-- | :-: |
| [gsap-skills](https://github.com/greensock/gsap-skills) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | 8 Skills (Markdown) + Claude-/Cursor-Plugin-Manifest | GSAP korrekt nutzen: core, timeline, scrolltrigger, plugins, utils, react, performance, frameworks (Vue/Nuxt/Svelte) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [threejs-skills](https://github.com/CloudAI-X/threejs-skills) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | 13 Skills (Markdown) | three.js r186 + React Three Fiber 9.8/drei 10.7 + gltf-transform 4.5: Grundlagen, Geometrie, Materialien, Licht, Texturen, Animation, Loader, Shader/TSL, Postprocessing, Interaktion, Performance, R3F, Asset-Pipeline | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [web-design-guidelines](https://github.com/vercel-labs/agent-skills/tree/main/skills/web-design-guidelines) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill (Markdown) | Prüft UI-Code gegen Vercels Web-Interface- und Barrierefreiheitsregeln | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [vercel-composition-patterns](https://github.com/vercel-labs/agent-skills/tree/main/skills/composition-patterns) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill (Markdown) | React-Kompositionsmuster (Compound Components, keine Boolean-Prop-Flut) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [ui-ux-pro-max](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill + Plugin, lokales Python-Suchskript, optional CLI `uipro` | Design-Datenbank (Stile, Paletten, Schriftpaare, UX-Regeln) für Claude | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [sleek-design-mobile-apps](https://github.com/sleekdotdesign/agent-skills) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill für kommerzielle Cloud-API | Mobile-App-Designs über sleek.design erzeugen | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [ui-skills](https://github.com/ibelick/ui-skills) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | 9 eigene Skills (Markdown) + Registry ui-skills.com, CLI `npx ui-skills`, Remote-MCP | Regeln für bessere UI (Typografie, Abstände, Animation, Barrierefreiheit). Primär-Repo ist ibelick/ui-skills | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (eigene Skills fast grün) |
| [img2threejs](https://github.com/img2threejs/img2threejs) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill + Python-Werkzeug „Forge“, Installer `npx img2threejs` | Baut aus einem Bild eine Three.js-3D-Szene | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [fwc-swiftui-skills](https://github.com/FloWritesCode/fwc-swiftui-skills) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | 2 Skills (Markdown) | SwiftUI-Hilfen für Liquid Glass und das iPhone-Duo-Layout (iOS 27.1 SDK) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [shadcn MCP](https://ui.shadcn.com/docs/mcp) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Lokaler MCP-Server in der offiziellen CLI (`npx shadcn@latest mcp`) | Claude sucht und installiert shadcn/ui-Komponenten aus Registries | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [html-anything](https://github.com/nexu-io/html-anything) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Lokale Web-App (Next.js) + 81 Template-Skills | Lokaler Agent macht aus Markdown fertige HTML-Seiten (Slides, Berichte, Poster) | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst) App / 🟡 Templates |

<sub>[↑ Inhalt](#-inhalt)</sub>

---

<a id="skills"></a>

## 7. Skills: Denken, Recherche & Skill-Verwaltung

<img src="assets/mods/cat-07-skills.svg" width="100%" alt="7. Skills: Denken, Recherche &amp; Skill-Verwaltung">

| Name | Herkunft | Typ | Wofür | Ampel |
| :-- | :-: | :-- | :-- | :-: |
| [RedTeam](https://github.com/danielmiessler/LifeOS/tree/main/LifeOS/install/skills/RedTeam) (LifeOS) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill (Markdown, 2 Workflows), v1.1.17 | Stresstest für **Ideen, Pläne und Argumente**: zerlegt sie in Einzelthesen, lässt viele parallele Experten-Agenten angreifen und liefert Steelman plus stärkstes Gegenargument | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [ArXiv](https://github.com/danielmiessler/LifeOS/tree/main/LifeOS/install/skills/ArXiv) (LifeOS) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill (Markdown, 3 Workflows), v1.0.9 | Sucht arXiv-Paper nach Thema, Kategorie oder ID und holt KI-Zusammenfassungen von AlphaXiv | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [LifeOS](https://github.com/danielmiessler/LifeOS) (gesamt, früher „Personal AI Infrastructure“/PAI) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Kompletter Harness: 57 Skills, 60 Settings-Hooks, Agents, Statusline, Dashboard „Pulse“, Voice-Server | Persönliches KI-Betriebssystem rund um Claude Code (Gedächtnis, Ziele, Workflows, Dashboards) | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst) |
| [find-skills](https://github.com/vercel-labs/skills/tree/main/skills/find-skills) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill (Markdown) für die Skills-CLI `npx skills` | Sucht passende Skills über skills.sh bzw. `npx skills find` und schlägt Install-Befehle vor | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst) |
| [Skill Manager](https://github.com/abubakarsiddik31/skill-manager) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Desktop-App (Tauri/Rust), kein Skill | Ein Dashboard für die Skills von Claude Code, Codex, Cursor und OpenCode: anzeigen, suchen, (de)aktivieren, bearbeiten, löschen, aus Sammlungen installieren | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [the-fool](https://github.com/Jeffallan/claude-skills/tree/main/skills/the-fool) (Jeffallan/claude-skills) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill (Markdown, 6 Referenzen), v1.0.0 | Advocatus Diaboli: prüft Pläne und Entscheidungen in 5 Modi (sokratische Fragen, Gegenthese, Pre-Mortem, Red Team, Evidenz-Check) und baut daraus eine stärkere Fassung | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [CreateCLI](https://github.com/danielmiessler/LifeOS/tree/main/LifeOS/install/skills/CreateCLI) (LifeOS) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill (Markdown, 3 Workflows), v1.1.25 | Erzeugt fertige TypeScript-Kommandozeilen-Tools in drei Ausbaustufen, mit Doku und Konfiguration | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [skillselion-mcp](https://github.com/skillselion/skillselion-mcp) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | MCP-Server (npm, `npx -y skillselion-mcp`) + optionaler SessionStart-Hook | Sucht Skills auf skillselion.com und lädt sie **mitten in der Aufgabe** samt Skripten in die Session | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) |
| [agent-teams-lite](https://github.com/Gentleman-Programming/agent-teams-lite) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | 16 Skills (Markdown, SDD-Phasen als Subagents) + Install-Skripte | Spec-Driven Development: erkunden → vorschlagen → spezifizieren → entwerfen → Aufgaben → umsetzen → prüfen → archivieren | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [academic-research-skills](https://github.com/Imbad0202/academic-research-skills) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Plugin: 5 Skills, 16 Commands, Agents, 2 Hooks | Forschungs-Pipeline: Recherche, Paper schreiben, simuliertes Peer-Review, Revision, Zitat-Prüfung | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [academic-paper-skills](https://github.com/lishix520/academic-paper-skills) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | 2 Skills (strategist, composer) + 4 lokale Python-Skripte | Fachartikel planen und schreiben mit Qualitäts-Checkpoints (v. a. Philosophie) | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [tieline](https://github.com/knoxgraeme/tieline) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill + lokaler MCP-Server (npm `tieline` 0.2.2) | Verknüpft Produkt-Absicht (Fähigkeiten, User Stories, Akzeptanzkriterien) mit Code und Tests als Beleg | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [no-ai-slop](https://github.com/petergyang/no-ai-slop) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill (Markdown, 97 Zeilen) + Codex-Plugin-Metadaten | Entfernt über 20 typische KI-Schreibmuster aus Texten | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [humanizer](https://github.com/blader/humanizer) (WL-184) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill (Markdown, 1 `SKILL.md`, 397 Zeilen) als Claude-Plugin, v3.1.0 | Schreibt KI-klingende Texte natürlicher um (26 Muster nach Wikipedias „Signs of AI writing“), ohne den Inhalt zu ändern. Modi: eingefügter Text, Datei, eingebettet (PR/Commit-Text) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |

<sub>[↑ Inhalt](#-inhalt)</sub>

---

<a id="mcp-kreativ"></a>

## 8. MCP-Server & Kreativ-Tools (Video, 3D, Reverse Engineering)

<img src="assets/mods/cat-08-mcp-kreativ.svg" width="100%" alt="8. MCP-Server &amp; Kreativ-Tools (Video, 3D, Reverse Engineering)">

| Name | Herkunft | Typ | Wofür | Ampel |
| :-- | :-: | :-- | :-- | :-: |
| [HyperFrames](https://github.com/heygen-com/hyperframes) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Plugin (7 Skills) + npm-CLI `hyperframes` | Claude baut Videos aus HTML/CSS/Animationen und rendert sie lokal zu MP4 (headless Chrome + FFmpeg), optional mit HeyGen-Stimmen, -Avataren und -Musik | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst) |
| [MCP for Blender](https://github.com/ahujasid/mcp-for-blender) (ex blender-mcp) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | MCP-Server (uvx) + Blender-Addon | Claude baut 3D-Modelle und Szenen in Blender per Chat | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) (vorerst) |
| [ghidra-mcp](https://github.com/bethington/ghidra-mcp) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | MCP-Server (Ghidra-Extension + Python-Bridge), 200+ Tools | Claude bedient Ghidra (NSA-Reverse-Engineering): analysieren, umbenennen, typisieren, debuggen | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [IDA MCP](https://github.com/HexRaysSA/ida-mcp) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | MCP-Server + Claude-Plugin (offiziell Hex-Rays) | Claude arbeitet im kommerziellen Disassembler IDA Pro (≥ 9.4) | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [universal-modder](https://github.com/rehan-remade/universal-modder) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Plugin (Skills + SessionStart-Hook + fal-Remote-MCP + `um`-CLI) | Claude modded PC-Spiele: Analyse, Reverse Engineering, KI-generierte Assets über fal, Tests im Spiel | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) |
| [ElevenLabs MCP](https://elevenlabs.io/mcp) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Gehosteter MCP-Server (`https://api.elevenlabs.io/v1/mcp`) | Stimmen, Sprache, Musik und Voice-Agents aus Claude heraus | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [Higgsfield MCP](https://higgsfield.ai/mcp) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Gehosteter MCP-Server (`https://mcp.higgsfield.ai/mcp`) | KI-Bilder, Videos, Upscaling, Stimmen und Ad-Workflows | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [claude-video](https://github.com/bradautomates/claude-video) („Watch“, `/watch`) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Plugin (Skill + Python-Skripte, SessionStart-Hook) | Claude „schaut“ Videos: Download per yt-dlp, Einzelbilder per ffmpeg, Untertitel bzw. Transkript, optional Gemini schaut das ganze Video | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [Brag](https://github.com/latent-spaces/brag) (`/brag`) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill bzw. Plugin (Markdown, Musik- und SFX-Assets, Python-Analyse) | Macht aus dem aktuellen Projekt ein kurzes Launch-Video mit Musik und Share-Text, gerendert mit HyperFrames | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [Brag Slim](https://github.com/latent-spaces/brag/tree/main/skills/brag-slim) (`/brag-slim`) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill (eine Markdown-Datei, 105 Zeilen) | Wie Brag, aber ohne HyperFrames: rendert lokal mit FFmpeg, Playwright und TTS | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |

<sub>[↑ Inhalt](#-inhalt)</sub>

---

<a id="visualisierung"></a>

## 9. Visualisierung & Code-Verständnis

<img src="assets/mods/cat-09-visualisierung.svg" width="100%" alt="9. Visualisierung &amp; Code-Verständnis">

| Name | Herkunft | Typ | Wofür | Ampel |
| :-- | :-: | :-- | :-- | :-: |
| [archify](https://github.com/tt-a1i/archify) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill + lokaler Node-Renderer (CLI) | Architektur- und Ablaufdiagramme aus Beschreibung oder Code als HTML/SVG | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [Architecture Dissector / Blueprint](https://github.com/flaviocopes/architecture-dissector) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | macOS-App (ab macOS 15) + Skill (32 Zeilen) + CLI `blueprint` | Zerlegt ein Repo in eine interaktive Architekturkarte | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | MCP-Server (natives Binary, Hintergrund-Daemon) + Skill, 3 Agents, Hooks | Indexiert den Code als Graph, damit Claude schneller und mit weniger Tokens sucht | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [mermaid-diagrams](https://github.com/DZunke/dotfiles/tree/master/.claude/skills/mermaid) (DZunke/dotfiles) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Skill (Markdown, 23 Beispiele, 1 Vorlage) | Erzeugt Mermaid-Diagramme (Flussdiagramm, Sequenz, Klassen, C4, Gantt usw.) aus Beschreibung oder Code, prüft sie mit `mmdc` und rendert auf Wunsch SVG, PNG oder PDF | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [Context Timeline](https://github.com/davila7/claude-code-templates/blob/main/cli-tool/components/hooks/monitoring/context-timeline.py) (aitmpl.com, davila7) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Settings-Hook (Python, SessionStart/PreToolUse/PostToolUse/Stop) + lokaler HTTP-Daemon | Zeitleiste aller Tool-Calls und Subagents plus Kontext-Füllstand im Browser (localhost:7878) | ![🔴 rot](https://img.shields.io/badge/-%F0%9F%94%B4_rot-cf222e) wie ausgeliefert |

<sub>[↑ Inhalt](#-inhalt)</sub>

---

<a id="mcp-saas"></a>

## 10. MCP-Server: SaaS-Anbindungen (Automatisierung, Analytics)

<img src="assets/mods/cat-10-mcp-saas.svg" width="100%" alt="10. MCP-Server: SaaS-Anbindungen (Automatisierung, Analytics)">

| Name | Herkunft | Typ | Wofür | Ampel |
| :-- | :-: | :-- | :-- | :-: |
| [Zapier MCP](https://zapier.com/mcp) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Gehosteter MCP-Server (`https://mcp.zapier.com/api/v1/connect`) | Claude bedient über Zapier über 9.000 Apps (Gmail, Slack, CRM …) | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [PostHog MCP](https://posthog.com/docs/model-context-protocol) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Gehosteter MCP-Server (`https://mcp.posthog.com/mcp`) | Analytics, Feature-Flags, Fehler und SQL in PostHog per Chat | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [ToolJet MCP](https://github.com/ToolJet/tooljet-mcp) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | MCP-Server + Plugin (Skill `tooljet-app-builder`) | Claude baut und pflegt ToolJet-Apps (Seiten, Queries, ToolJet-DB) über ToolJets APIs | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |

<sub>[↑ Inhalt](#-inhalt)</sub>

---

<a id="anthropic-skills"></a>

## 11. Offizielle Anthropic-Skills

<img src="assets/mods/cat-11-anthropic-skills.svg" width="100%" alt="11. Offizielle Anthropic-Skills">

| Name | Herkunft | Typ | Wofür | Ampel |
| :-- | :-: | :-- | :-- | :-: |
| [frontend-design](https://github.com/anthropics/skills/tree/main/skills/frontend-design) | ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) | Skill (Markdown) | Eigenständige, nicht generische Web-Oberflächen bauen | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [canvas-design · theme-factory · brand-guidelines](https://github.com/anthropics/skills/tree/main/skills/canvas-design) | ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) | 3 Skills (Markdown, Fonts) | Poster/Grafiken, 10 fertige Themes, Anthropic-Markenstil | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [internal-comms · doc-coauthoring · discernment-nudge](https://github.com/anthropics/skills/tree/main/skills/doc-coauthoring) | ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) | 3 Skills (Markdown) | Interne Mitteilungen, gemeinsames Schreiben von Specs, kritische Rückfragen | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [academy-guide · algorithmic-art · claude-api · mcp-builder · slack-gif-creator](https://github.com/anthropics/skills/tree/main/skills/claude-api) | ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) | 5 Skills, teils mit Skripten | Academy-Kurse, p5.js-Kunst, Claude-API/Agent-SDK, MCP-Server bauen, Slack-GIFs | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [docx · pdf · pptx · xlsx](https://github.com/anthropics/skills/tree/main/skills/docx) | ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) | 4 Skills mit 50 Skript-Dateien (Plugin `document-skills`) | Office-Dateien und PDFs erstellen, bearbeiten, umrechnen | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [skill-creator](https://github.com/anthropics/skills/tree/main/skills/skill-creator) | ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) | Skill + 10 Skripte | Eigene Skills bauen, testen und per Messlauf verbessern | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [web-artifacts-builder](https://github.com/anthropics/skills/tree/main/skills/web-artifacts-builder) | ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) | Skill + 2 Shell-Skripte | Komplexe React-Artefakte bauen und zu einer HTML-Datei bündeln | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [webapp-testing](https://github.com/anthropics/skills/tree/main/skills/webapp-testing) | ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) | Skill + 4 Python-Skripte (Playwright) | Lokale Web-Apps im Browser testen | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [template-skill](https://github.com/anthropics/skills/tree/main/template) | ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) | Vorlage (nur Frontmatter) | Gerüst für eigene Skills | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |

<sub>[↑ Inhalt](#-inhalt)</sub>

---

<a id="sammlungen"></a>

## 12. Subagents & Plugin-Sammlungen

<img src="assets/mods/cat-12-sammlungen.svg" width="100%" alt="12. Subagents &amp; Plugin-Sammlungen">

| Name | Herkunft | Typ | Wofür | Ampel |
| :-- | :-: | :-- | :-- | :-: |
| [wshobson/agents](https://github.com/wshobson/agents) (Marketplace `claude-code-workflows`) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Plugin-Marketplace: 94 Plugins, 202 Subagents, 185 Skills, 105 Commands (gegen Repo geprüft) | Kein einzelner Skill, sondern ein Regal: Man installiert einzelne Themen-Plugins (z. B. `python-development` = 3 Agents, 1 Command, 16 Skills) | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |
| [claude_subagents](https://github.com/davila7/claude_subagents) (davila7) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Demo-Repo: 7 Subagents (`.claude/agents/`) + Mini-Web-App | Übungsplatz zum Artikel „Keep your Claude Code context clean with Subagents“: sauberer vs. geforkter Kontext, Ketten bis Tiefe 5 | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) zum Lernen / 🟡 zum Übernehmen |

<sub>[↑ Inhalt](#-inhalt)</sub>

---

<a id="pruefwerkzeuge"></a>

## 13. Prüfwerkzeuge (Hilfen, keine Mods)

<img src="assets/mods/cat-13-pruefwerkzeuge.svg" width="100%" alt="13. Prüfwerkzeuge (Hilfen, keine Mods)">

| Name | Herkunft | Typ | Wofür | Ampel |
| :-- | :-: | :-- | :-- | :-: |
| [SkillSpector](https://github.com/NVIDIA/SkillSpector) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Security-Scanner (Python-CLI, optional MCP/Docker) | Prüft Skills vor der Installation auf 71 Risikomuster (Prompt Injection, Datenabfluss, Lieferkette …) und gibt einen Risiko-Score 0–100 | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) (fast grün) |
| [Caliper](https://github.com/edonadei/caliper) | ![👥 Community](https://img.shields.io/badge/-%F0%9F%91%A5_Community-6e7781) | Eval-Werkzeug (PyPI `caliper-eval` 0.19.0) + Skill `grill-skill` | Misst, ob ein Skill wirklich hilft: echte Agent-Läufe mit und ohne Skill (Ablation), Trefferquote, Tokens, Zeit | ![🟡 gelb](https://img.shields.io/badge/-%F0%9F%9F%A1_gelb-bf8700) |

<sub>[↑ Inhalt](#-inhalt)</sub>

---

<a id="nebenfund"></a>

## Weitere Funde

<img src="assets/mods/cat-nebenfund.svg" width="100%" alt="Weitere Funde">

| Name | Herkunft | Typ | Wofür | Ampel |
| :-- | :-: | :-- | :-- | :-: |
| [Token Weather](https://github.com/anthropics/claude-code-playground/tree/main/claude-code/mods/token-weather) | ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) | Mod (Band) | Live-„Wettervorhersage“ für das Kontextfenster | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |
| [plugin-authoring](https://code.claude.com/docs/en/plugins/mods/overview#mods-built-into-claude-code) (`cc-plugin-plugin-authoring`) | ![🏛️ offiziell](https://img.shields.io/badge/-%F0%9F%8F%9B%EF%B8%8F_offiziell-1f6feb) | Eingebauter Skill | Damit baut Claude Mods auf Zuruf („Build your own mod“ im Video) | ![🟢 grün](https://img.shields.io/badge/-%F0%9F%9F%A2_gr%C3%BCn-2ea44f) |

<sub>[↑ Inhalt](#-inhalt)</sub>


---

<sub>Inhalt der Liste (Texte, Bewertungen, Banner): [CC BY 4.0](LICENSE). Die verlinkten Projekte haben ihre eigenen Lizenzen. Markennamen gehören ihren Inhabern.</sub>

