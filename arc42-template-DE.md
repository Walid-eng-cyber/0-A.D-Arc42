# 

**Über arc42**

arc42, das Template zur Dokumentation von Software- und
Systemarchitekturen.

Template Version 9.0-DE. (basiert auf der AsciiDoc Version), Juli 2025

Created, maintained and © by Dr. Peter Hruschka, Dr. Gernot Starke and
contributors. Siehe <https://arc42.org>.

:::::: sidebar
::: title
:::

:::: note
::: title
:::

Diese Version des Templates enthält Hilfen und Erläuterungen. Sie dient
der Einarbeitung in arc42 sowie dem Verständnis der Konzepte. Für die
Dokumentation eigener System verwenden Sie besser die *plain* Version.
::::
::::::

# Einführung und Ziele {#section-introduction-and-goals}

:::: sidebar
::: title
:::

Beschreibt die wesentlichen Anforderungen und treibenden Kräfte, die bei
der Umsetzung der Softwarearchitektur und Entwicklung des Systems
berücksichtigt werden müssen.

Dazu gehören:

- zugrunde liegende Geschäftsziele,

- wesentliche Aufgabenstellungen,

- wesentliche funktionale Anforderungen,

- Qualitätsziele für die Architektur und

- relevante Stakeholder und deren Erwartungshaltung.
::::

## Aufgabenstellung {#_aufgabenstellung}

:::::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Kurzbeschreibung der fachlichen Aufgabenstellung, treibenden Kräfte,
Extrakt (oder Abstract) der Anforderungen. Verweis auf (hoffentlich
vorliegende) Anforderungsdokumente (mit Versionsbezeichnungen und
Ablageorten).
::::

:::: formalpara
::: title
Motivation
:::

Aus Sicht der späteren Nutzung ist die Unterstützung einer fachlichen
Aufgabe oder Verbesserung der Qualität der eigentliche Beweggrund, ein
neues System zu schaffen oder ein bestehendes zu modifizieren.
::::

:::: formalpara
::: title
Form
:::

Kurze textuelle Beschreibung, eventuell in tabellarischer Use-Case Form.
Sofern vorhanden, sollte die Aufgabenstellung Verweise auf die
entsprechenden Anforderungsdokumente enthalten.
::::

Halten Sie diese Auszüge so knapp wie möglich und wägen Sie Lesbarkeit
und Redundanzfreiheit gegeneinander ab.

:::: formalpara
::: title
Weiterführende Informationen
:::

Siehe [Anforderungen und Ziele](https://docs.arc42.org/section-1/) in
der online-Dokumentation (auf Englisch!).
::::
::::::::::::

## Qualitätsziele {#_qualitätsziele}

:::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Die Top-3 bis Top-5 der Qualitätsanforderungen für die Architektur,
deren Erfüllung oder Einhaltung den maßgeblichen Stakeholdern besonders
wichtig sind. Gemeint sind hier wirklich Qualitätsziele, die nicht
unbedingt mit den Zielen des Projekts übereinstimmen. Beachten Sie den
Unterschied.
::::

Hier ein Überblick möglicher Themen (basierend auf dem ISO 25010
Standard):

![Kategorien von
Qualitätsanforderungen](images/01_2_iso-25010-topics-EN-2023.drawio.png)

:::: formalpara
::: title
Motivation
:::

Weil Qualitätsziele grundlegende Architekturentscheidungen oft
maßgeblich beeinflussen, sollten Sie die für Ihre Stakeholder relevanten
Qualitätsziele kennen, möglichst konkret und operationalisierbar.
::::

:::: formalpara
::: title
Form
:::

Tabellarische Darstellung der Qualitätsziele mit möglichst konkreten
Szenarien, geordnet nach Prioritäten.
::::
::::::::::

## Stakeholder {#_stakeholder}

:::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Expliziter Überblick über die Stakeholder des Systems -- über alle
Personen, Rollen oder Organisationen --, die
::::

- die Architektur kennen sollten oder

- von der Architektur überzeugt werden müssen,

- mit der Architektur oder dem Code arbeiten (z.B. Schnittstellen
  nutzen),

- die Dokumentation der Architektur für ihre eigene Arbeit benötigen,

- Entscheidungen über das System und dessen Entwicklung treffen.

:::: formalpara
::: title
Motivation
:::

Sie sollten die Projektbeteiligten und -betroffenen kennen, sonst
erleben Sie später im Entwicklungsprozess Überraschungen. Diese
Stakeholder bestimmen unter anderem Umfang und Detaillierungsgrad der
von Ihnen zu leistenden Arbeit und Ergebnisse.
::::

:::: formalpara
::: title
Form
:::

Tabelle mit Rollen- oder Personennamen, sowie deren Erwartungshaltung
bezüglich der Architektur und deren Dokumentation.
::::
::::::::::

+-----------------+-----------------+-----------------------------------+
| Rolle           | Kontakt         | Erwartungshaltung                 |
+=================+=================+===================================+
| *\<Rolle-1\>*   | *\<Kontakt-1\>* | *\<Erwartung-1\>*                 |
+-----------------+-----------------+-----------------------------------+
| *\<Rolle-2\>*   | *\<Kontakt-2\>* | *\<Erwartung-2\>*                 |
+-----------------+-----------------+-----------------------------------+

# Randbedingungen {#section-architecture-constraints}

:::::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Randbedingungen und Vorgaben, die ihre Freiheiten bezüglich Entwurf,
Implementierung oder Ihres Entwicklungsprozesses einschränken. Diese
Randbedingungen gelten manchmal organisations- oder firmenweit über die
Grenzen einzelner Systeme hinweg.
::::

:::: formalpara
::: title
Motivation
:::

Für eine tragfähige Architektur sollten Sie genau wissen, wo Ihre
Freiheitsgrade bezüglich der Entwurfsentscheidungen liegen und wo Sie
Randbedingungen beachten müssen. Sie können Randbedingungen vielleicht
noch verhandeln, zunächst sind sie aber da.
::::

:::: formalpara
::: title
Form
:::

Einfache Tabellen der Randbedingungen mit Erläuterungen. Bei Bedarf
unterscheiden Sie technische, organisatorische und politische
Randbedingungen oder übergreifende Konventionen (beispielsweise
Programmier- oder Versionierungsrichtlinien, Dokumentations- oder
Namenskonvention).
::::

:::: formalpara
::: title
Weiterführende Informationen
:::

Siehe [Randbedingungen](https://docs.arc42.org/section-2/) in der
online-Dokumentation (auf Englisch!).
::::
::::::::::::

# Kontextabgrenzung {#section-context-and-scope}

:::::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Die Kontextabgrenzung grenzt das System gegen alle Kommunikationspartner
(Nachbarsysteme und Benutzerrollen) ab. Sie legt damit die externen
Schnittstellen fest und zeigt damit auch die Verantwortlichkeit (scope)
Ihres Systems: Welche Verantwortung trägt das System und welche
Verantwortung übernehmen die Nachbarsysteme?
::::

Differenzieren Sie fachlichen (Ein- und Ausgaben) und technischen
Kontext (Kanäle, Protokolle, Hardware), falls nötig.

:::: formalpara
::: title
Motivation
:::

Die fachlichen und technischen Schnittstellen zur Kommunikation gehören
zu den kritischsten Aspekten eines Systems. Stellen Sie sicher, dass Sie
diese komplett verstanden haben.
::::

:::: formalpara
::: title
Form
:::

Verschiedene Optionen:
::::

- Diverse Kontextdiagramme

- Listen von Kommunikationsbeziehungen mit deren Schnittstellen

:::: formalpara
::: title
Weiterführende Informationen
:::

Siehe [Kontextabgrenzung](https://docs.arc42.org/section-3/) in der
online-Dokumentation (auf Englisch!).
::::
::::::::::::

## Fachlicher Kontext {#_fachlicher_kontext}

:::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Festlegung **aller** Kommunikationsbeziehungen (Nutzer, IT-Systeme, ...​)
mit Erklärung der fachlichen Ein- und Ausgabedaten oder Schnittstellen.
Zusätzlich (bei Bedarf) fachliche Datenformate oder Protokolle der
Kommunikation mit den Nachbarsystemen.
::::

:::: formalpara
::: title
Motivation
:::

Alle Beteiligten müssen verstehen, welche fachlichen Informationen mit
der Umwelt ausgetauscht werden.
::::

:::: formalpara
::: title
Form
:::

Alle Diagrammarten, die das System als Blackbox darstellen und die
fachlichen Schnittstellen zu den Nachbarsystemen beschreiben.
::::

Alternativ oder ergänzend können Sie eine Tabelle verwenden. Der Titel
gibt den Namen Ihres Systems wieder; die drei Spalten sind:
Kommunikationsbeziehung, Eingabe, Ausgabe.
::::::::::

**\<Diagramm und/oder Tabelle\>**

**\<optional: Erläuterung der externen fachlichen Schnittstellen\>**

## Technischer Kontext {#_technischer_kontext}

:::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Technische Schnittstellen (Kanäle, Übertragungsmedien) zwischen dem
System und seiner Umwelt. Zusätzlich eine Erklärung (*mapping*), welche
fachlichen Ein- und Ausgaben über welche technischen Kanäle fließen.
::::

:::: formalpara
::: title
Motivation
:::

Viele Stakeholder treffen Architekturentscheidungen auf Basis der
technischen Schnittstellen des Systems zu seinem Kontext.
::::

Insbesondere bei der Entwicklung von Infrastruktur oder Hardware sind
diese technischen Schnittstellen durchaus entscheidend.

:::: formalpara
::: title
Form
:::

Beispielsweise UML Deployment-Diagramme mit den Kanälen zu
Nachbarsystemen, begleitet von einer Tabelle, die Kanäle auf
Ein-/Ausgaben abbildet.
::::
::::::::::

**\<Diagramm oder Tabelle\>**

**\<optional: Erläuterung der externen technischen Schnittstellen\>**

**\<Mapping fachliche auf technische Schnittstellen\>**

# 4. Lösungsstrategie 

#### Dieser Abschnitt enthält einen stark verdichteten Architekturüberblick. Eine Gegenüberstellung der wichtigsten Ziele und Lösungsansätze.

## 4.1. Einstieg


| **Qualitätsziel**                                            | **Architektonische Ansätze zur Unterstützung**                                                                                                                                                                                                     |
| ------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Erweiterbarkeit** (neue Einheiten, Zivilisationen, Karten) | • Datengetriebenes Design: Spieleinhalte werden in XML / JSON beschrieben<br>• Klare Trennung zwischen Engine-Kern und Game-Content<br>• Modularer Asset-Loader und Skriptsystem<br>• Offene Modding-Schnittstelle für Community-Erweiterungen     |
| **Performance** (viele Einheiten gleichzeitig)               | • Entity-Component-System (ECS) für effiziente Datenverarbeitung<br>• Engine in C++ implementiert<br>• Deterministische Simulation für stabile Synchronisation<br>• Level-of-Detail-Rendering (LOD) zur Entlastung der Grafikebene                 |
| **Portabilität** (Windows, Linux, macOS)                     | • Nutzung plattformübergreifender Bibliotheken (OpenGL, SDL, Boost)<br>• Abstraktionsschichten für Grafik, Audio und Eingabe<br>• Minimale Betriebssystem-abhängigkeiten                                                                           |
| **Wartbarkeit** (klare Struktur und leichte Änderbarkeit)    | • Schichtenarchitektur (Rendering / Simulation / Netzwerk klar getrennt)<br>• Modularer C++-Code mit definierten Schnittstellen<br>• Spiel-Logik (JavaScript) getrennt vom Engine-Kern<br>• Strukturierte Code-Reviews durch Open-Source-Community |
| **Multiplayer-Zuverlässigkeit**                              | • Deterministische Simulation für alle Clients<br>• Synchronisation über Befehle statt Zustände<br>• Replay-System zur Fehleranalyse bei Desynchronisation                                                                                         |
| **Modding-Freundlichkeit**                                   | • Separate „Mods“-Verzeichnisse überlagern Basisdaten<br>• Automatisches Laden von Benutzer-Inhalten beim Start<br>• Einfache Anpassbarkeit durch XML / JSON-Struktur                                                                              |
| **Internationalisierung und Zugänglichkeit**                 | • Unicode-Unterstützung und Übersetzungsdateien (.po)<br>• Lokalisierte Benutzeroberfläche und Texte<br>• Layout-System unabhängig von Sprache und Schriftart                                                                                      |
| **Sicherheit und Stabilität**                                | • Sandboxed Scripting über JavaScript-Engine<br>• Versionskontrolle und Community-Überprüfung von Beiträge<br>• Deterministische Netzwerkarchitektur reduziert Cheating-Risiken                                                                    |


## 4.2. Aufbau 

0 A.D ist als plattformuabhängige (cross-platform) C++/JavaScript-Anwendung realisiert.Es zerfällt grob in folgende Teile:

- **1. Game-/Simulation-Engine**
  
  Verantwortlich für Spielschleife, deteminitische Simulation, Entity-Component-System (ECS), Pathfinding, Kampf- und Wirtschaftlogik.

- **2. Rendering und Audio Subsysteme**
  
  Zuständig für Darstellung der Spielwelt (Terrain, Einheiten, Effekte) sowie Wirdergabe von Sound und Musik, über plattformunabhängige Bibliotheken (z.B. OpenGL, OpenAL).

- **3. Daten und Content Layer**

  Beschreibt alles Spielinhalte (z.B. Einheiten, Gebäude, Karten, Items, etc.) in XML/JSON-Dateien sowie skriptbare Spiellogik in JavaScript, dient zugleicht als Grundlage für Modding.

- **4. Multiplayer / Networking Module**

  Implementiert  die deterministische, befehlsbasierte Synchronisation zwichen mehreren Spielern (Lockstep-Modell = alle Spieler führen die gleiche Simulation aus) sowie Replay-/Desync-Unterstützung.

- **5.  Graphical User Interface (GUI)**


    Menüsystem, Ingame-HUD, Auswahl und Befehlsoberfläche.
    Die GUI interagiert über Skripte mut der Engine und präsentiert dem Spieler Daten.

- **6.Mod-/Ressourcen-Loader**

  Lädt beim Start die Basisdaten und zusätzliche Mods aus getrennten Verzeichnissen und überlagert sie nach Priorität.


## 4.3 Spielstrategie / Integration  

Die Architektur von 0 A.D. folgt einer klaren Spielstrategie, die auf einem **deterministischen Simulationsmodell** und einer **datengetriebenen Trennung von  Engine und Spielinhalt** basiert.

Das System arbeitet in einem **kontinuerlichen Game Loop**, in dem Eingaber verarbeitet, Spielzustände aktualisiert und anschließend visualisiert werden.

- **1. Eingabe und Steuerung**

  - Spielerinteraktion über Tastatur und Maus werden vom input-System erfasst und in Befehle übersetzt.
  - In Single-Player mode werder Befehle direkt an  die Simulation gesendet, im Multiplayer mode werden sie zwischen allen Peers synschronisiert.

- **2. Simulation und Logik**

  - Die deterministische Simulation verarbeitet alle Befehle im nächsten Tick.

  - Das Entity-Component-System aktualisiert Positionen, Zustände, Ressourcen und Einheitenverhalten.

  - Skripte in JavaScript steuern KI, Wirtschaft und Kampflogik.

- **3. Rendering und Audio**

  - Nach der Simulation werden die aktualisierten Spielobjekte vom Rendering-System (OpenGL) dargestellt.

  - Das Audiosystem (OpenAL) spielt passende Geräusche und Musik ab.

- **4. Multiplayer-Synchronisation**

  - Alle Spieler führen dieselbe Simulation aus; nur Befehle werden über das Netzwerk ausgetauscht (Lockstep-Modell).

  - Dies garantiert identische Ergebnisse auf allen Rechnern.

- **5. Modulare Datenfluss**

  - Inhalte (Units, Gebäude, Karten) werden beim Start aus XML- und Skriptdateien geladen.

  - Das Mod-System kann zusätzliche Daten überlagern und zur Laufzeit erweitern.


## 4.4 Integration 

0 A.D. verbindet seine internen Systeme mit der Außenwelt über drei zentrale Schnittstellen: das Betriebssystem, das Mehrspieler-Netzwerk und das dateibasierte Daten- und Mod-System.
Die Spiel-Engine interagiert mit der Host-Plattform über plattformunabhängige Bibliotheken wie **SDL**, **OpenGL** und **OpenAL**, welche Eingabe, Darstellung und Audio einheitlich und betriebssystemübergreifend verarbeiten.
Für die Mehrspielerkommunikation verwendet 0 A.D. die **ENet( ***ENet ist eine kleine, schnelle und Open-Source-Netzwerkbibliothek, die in C geschrieben wurde und eine zuverlässige Kommunikation über das UDP-Protokoll ermöglicht***)**-Netzwerkbibliothek, um Spielerbefehle zwischen den Teilnehmern im **Lockstep-Synchronisationsmodell** auszutauschen. Dieser Ansatz reduziert die Netzwerklast und stellt sicher, dass bei allen Clients identische Simulationsergebnisse entstehen.
Alle Spieldaten und von der Community erstellten Erweiterungen werden über ein modulares Dateisystem verwaltet. Der **Mod-Loader** kombiniert beim Start des Spiels die Basisdaten dynamisch mit benutzerdefinierten Inhalten und Skripten, sodass neue Zivilisationen, Karten oder Spielmechaniken integriert werden können, ohne den Engine-Code zu verändern.

Durch diese Architektur besitzt 0 A.D. klar definierte Schnittstellen zum Betriebssystem, zum Netzwerk und zu benutzererstellten Inhalten. Dadurch bleibt der Kern der Engine unabhängig, stabil und leicht erweiterbar.








<br> 
<br> 
<br>
 
***High-level Integration Overview***

```

                                +-------------------------+
                                |     Player (User)       |
                                |  Mouse / Keyboard Input |
                                +-----------+-------------+
                                            |
                                            v
                                +-----------+-----------+
                                |       0 A.D. Engine    |
                                |------------------------|
                                |   Input Manager        |
                                |   Simulation Core      |
                                |   Rendering / Audio    |
                                +-----------+------------+
                                            |
                          +----------------+----------------+
                          |                                 |
                          v                                 v
                        +----------+                  +-------------+
                        |  Network | <--- Commands --->| Other Peers |
                        | (ENet)   |                  |   (Players)  |
                        +----------+                  +-------------+
                                            |
                                            v
                                    +--------------+
                                    |  Mod / Data  |
                                    |  File System |
                                    +--------------+

```


# Bausteinsicht 

Dieser Abschnitt beschreibt die Zerlegung von ***0 A.D.*** in seine Hauptmodule, wie sie sich auch in der Struktur des Quellcodes widerspiegelt.
Module der ersten Zerlegungsebene werden in ***0 A.D.*** als Subsysteme bezeichnet.
Die → Bausteinsicht, Ebene 1 stellt diese Subsysteme einschließlich ihrer Hauptaufgaben und Schnittstellen dar.

Für einige Subsysteme, insbesondere das → Simulationssystem (***Entity-Component-System***), enthält dieser Abschnitt zusätzlich eine detailliertere Zerlegung in → Ebene 2.


## 5.1 Überblick über die Subsysteme

Dieser Abschnitt beschreibt die wichtigsten Subsysteme von 0 A.D. auf oberster Ebene.
Die Architektur trennt den technischen Kern (Engine) von der Darstellung, den Spieldaten und der Benutzeroberfläche.
Jedes Subsystem erfüllt eine klar definierte Aufgabe und kommuniziert über wohlstrukturierte Schnittstellen mit anderen Modulen.

| **Subsystem**                | **Kurzbeschreibung**                                                                                                                                                                                               |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Game Engine Core**         | Steuert die Hauptspielschleife, verwaltet Ereignisse und Ressourcen. Stellt grundlegende Dienste wie Logging, Konfiguration und Initialisierung bereit.                                                            |
| **Simulationssystem (ECS)**  | Das zentrale Logiksystem des Spiels. Verwendet das **Entity-Component-System**-Prinzip, um Einheiten, Gebäude und Ressourcen zu verwalten. Beinhaltet Bewegungs-, Kampf-, Wirtschafts- und KI-Logik.               |
| **Rendering-Subsystem**      | Verantwortlich für die visuelle Darstellung der Spielwelt. Rendert Gelände, Einheiten und Effekte mithilfe von **OpenGL**. Aktualisiert die Szene basierend auf dem Simulationszustand.                            |
| **Audio-Subsystem**          | Steuert Soundeffekte und Hintergrundmusik. Nutzt **OpenAL** für räumliche Audiowiedergabe und sorgt für immersives Sounddesign.                                                                                    |
| **Netzwerkmodul**            | Ermöglicht Mehrspieler-Partien über eine **deterministische Simulation** mit **Befehlssynchronisation (Lockstep-Modell)**. Zuständig für Sitzungsverwaltung, Replays und Fehlerbehandlung bei Desynchronisationen. |
| **Benutzeroberfläche (GUI)** | Umfasst Menüs, das In-Game-HUD und Eingabeverarbeitung (Maus, Tastatur). Basierend auf **XML-Layouts** und **JavaScript-Logik**. Übersetzt Benutzereingaben in Simulationsbefehle.                                 |
| **Daten- und Mod-System**    | Lädt alle Spieldaten wie Einheiten, Karten, Zivilisationen, Skripte und Texturen. Unterstützt ein modulares Dateisystem, das das einfache Hinzufügen und Aktivieren von Mods ermöglicht.                           |
| **KI- und Scripting-Ebene**  | Implementiert computergesteuerte Gegner (z. B. Petra Bot) und Spielereignisse. Nutzt **JavaScript**, um KI-Verhalten, Strategien und Skripte für Gameplay zu definieren.                                           |
| *Tabelle: Überblick über Subsysteme von 0 A.D.*     |                                            |


![Sequence Diagram](./SequenceDiagramSystemundSubsystem.png)
*Dieses Sequenzdiagramm repräsentiert den kompletten Architekturfluss.*

##  5.2  Game Engine 

Der Game Engine Core bildet das zentrale Steuersystem von *0 A.D.* und ist die Grundlage, auf der alle anderen Subsysteme aufbauen.
Er koordiniert die **Ausführung der Hauptspielschleife**, verwaltet **Ressourcen und Ereignisse** und stellt **gemeinsame Dienste** für Simulation, Rendering, Audio, Netzwerk und GUI bereit.
Darüber hinaus stellt der Engine-Kern eine umfangreiche **Skript-Schnittstelle (Engine API)** zur Verfügung, über die JavaScript-Code (z. B. aus der GUI, KI oder Simulation) direkt mit der C++-Engine interagieren kann.


### 5.2.1 Verantwortlichkeiten

1. **Hauptspielschleife**

    Der Engine-Kern steuert die kontinuierlich laufende Hauptschleife des Spiels.
    Jeder Schleifendurchlauf (Frame) führt mehrere Schritte aus:

    - Verarbeitung von Eingaben aus GUI und Netzwerk
    - Aktualisierung des Simulationssystems (Spielzustand und Logik)
    - Weitergabe aktualisierter Daten an Rendering- und Audio-Subsysteme
    - Verwaltung der Zeitschritte und Synchronisierung aller Subsysteme
    - Hintergrundaufgaben wie Laden von Assets oder Empfang von Netzwerkbefehlen

    Dadurch werden gleichmäßige Bildraten und eine stabile Ausführung des Spiels gewährleistet.

2. **Initialisierung und Beendigung**

    Beim Start initialisiert der Engine-Kern alle Subsysteme, lädt Konfigurationsdateien und Ressourcen,
    und richtet Rendering (OpenGL), Audio (OpenAL), Netzwerk (ENet) sowie Mod-Verzeichnisse ein.
    Beim Beenden werden alle Ressourcen sauber freigegeben, um Speicherlecks oder Datenverluste zu vermeiden.

3. **Ressourcen- und Ereignisverwaltung**

    Der Engine-Kern fungiert als zentrale Ereignis- und Ressourcenverwaltung.
    Subsysteme kommunizieren über Ereignisse anstatt direkter Aufrufe.
    Beispiel:

    - Die Simulation löst ein Ereignis „Einheit zerstört“ aus → das Rendering zeigt eine Explosion → das Audio-System spielt den passenden Sound.
    Zusätzlich verwaltet der Engine-Kern Caching und Zugriff auf Texturen, Modelle, Sounds und Skripte, um Ladezeiten zu reduzieren.

4. **Plattform-Abstraktionsschicht**

    Um 0 A.D. auf verschiedenen Betriebssystemen lauffähig zu machen, abstrahiert der Engine-Kern plattformspezifische Funktionen über Bibliotheken wie SDL oder Boost.
    Dadurch werden Dateizugriffe, Eingabegeräte, Threads und Fenstererstellung unabhängig vom Betriebssystem gehandhabt.

5. **Zeit- und Synchronisationsmanagement**

    Der Engine-Kern verwaltet konsistente Zeitwerte (Frame-Zeit, Simulationszeit, Delta-Zeit),
    um sicherzustellen, dass Simulation, Rendering und Netzwerk-Ticks synchron laufen.
    Das ist besonders wichtig für die Konsistenz im Mehrspielermodus.

6. **Logging, Debugging und Profiling**
Der Engine-Kern stellt Infrastruktur zum Protokollieren, Debuggen und Profilieren bereit.
Entwickler können während der Laufzeit Frame-Rate, Speicherverbrauch oder Simulationszeiten beobachten.
Über Funktionen wie ProfileStart() und ProfileStop() kann auch aus JavaScript heraus Performance gemessen werden.

### 5.2.2 Engine-API
Die API besteht aus Hunderten von Funktionen, die sich in mehrere Gruppen einteilen lassen:

| **Kategorie**                    | **Beispielfunktionen**                                                      | **Zweck**                                                          |
| -------------------------------- | --------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| **Systemsteuerung**              | `Exit()`, `Crash()`, `GetEngineInfo()`, `GetBuildVersion()`                 | Kontrolle über Laufzeit, Debug-Informationen und Version           |
| **Datei- und Datenzugriff**      | `FileExists()`, `ReadJSONFile()`, `ListDirectoryFiles()`                    | Zugriff auf Spieldaten und Konfigurationsdateien                   |
| **Simulation & Gameplay**        | `PostCommand()`, `AddEntity()`, `DestroyEntity()`, `GetTemplate()`          | Senden und Verwalten von Spielbefehlen aus Skripten                |
| **GUI-Steuerung**                | `GetGUIObjectByName()`, `OpenChildPage()`, `SetGUIScale()`, `PlayUISound()` | Kontrolle der Benutzeroberfläche und Anzeigeelemente               |
| **Netzwerk**                     | `StartNetworkGame()`, `SendNetworkChat()`, `AssignNetworkPlayer()`          | Steuerung und Synchronisierung von Mehrspieler-Sitzungen           |
| **Konfiguration & Mods**         | `ConfigDB_SaveValue()`, `GetAvailableMods()`, `SetModsAndRestartEngine()`   | Verwaltung von Konfigurationen und aktivierten Mods                |
| **Internationalisierung (i18n)** | `Translate()`, `GetAllLocales()`, `SaveLocale()`                            | Übersetzungs- und Sprachunterstützung für GUI und Spieltexte       |
| **Debugging & Profiling**        | `ProfileStart()`, `ProfileStop()`, `DumpSimState()`                         | Messung und Analyse von Laufzeitverhalten und Simulationszuständen |

### 5.2.3 Beziehungen zu anderen Subsystemen
| **Subsystem**           | **Beschreibung der Interaktion**                                                       |
| ----------------------- | -------------------------------------------------------------------------------------- |
| **Simulation (ECS)**    | Der Engine-Kern ruft regelmäßig Simulations-Updates auf und empfängt Statusänderungen. |
| **Rendering**           | Erhält vom Engine-Kern aktuelle Simulationsdaten zur Darstellung.                      |
| **Audio**               | Spielt Sounds basierend auf Ereignissen aus Simulation oder GUI ab.                    |
| **Netzwerk**            | Tauscht Befehle und Synchronisations-Informationen über den Hauptloop aus.             |
| **GUI**                 | Nutzt die Engine-API, um Eingaben zu verarbeiten und Oberflächenelemente zu steuern.   |
| **Daten- & Mod-System** | Liefert Konfigurations- und Inhaltsdaten beim Start.                                   |
## 5.3 Simulationssystem (ECS)

Simulationssystem ist für die gesamte Logik und den Zustand der Spielwelt verantwortlich — also für Einheiten, Gebäude, Ressourcen, Bewegungen, Kämpfe und wirtschaftliche Abläufe.
Die Architektur des Systems basiert auf dem modernen Entwurfsmuster **Entity-Component-System (ECS)**, das hohe Flexibilität, Wiederverwendbarkeit und Performance ermöglicht.

### 5.3.1 Verantwortlichkeiten

1. **Verwaltung des Spielzustands**

    Das Simulationssystem speichert und aktualisiert alle Informationen über die Spielwelt:
    Positionen, Zustände, Eigentümer, Ressourcen, Trefferpunkte, Sichtweite usw.
    Es bestimmt, wie sich Einheiten bewegen, wie sie interagieren, kämpfen oder produzieren.

2. **Echtzeit-Logik**

    In jeder Simulations-Tick (Logik-Frame) werden alle relevanten Komponenten aktualisiert.
    Dadurch wird das Verhalten der Spielobjekte bestimmt, z. B. Pfadfindung, Kampfentscheidungen, Baufortschritt oder Ressourcenabbau.

3. **Synchronisation mit Netzwerk und Engine**

    Die Simulation erhält Befehle von der Benutzeroberfläche oder vom Netzwerkmodul
    und überträgt den aktualisierten Spielzustand an das Rendering- und Audio-Subsystem.
    Im Mehrspielermodus sorgt eine deterministische Simulation dafür, dass alle Clients denselben Spielverlauf haben.

4. **Ereignissteuerung und Messaging**

    Die Kommunikation innerhalb der Simulation erfolgt über Nachrichten (Events).
    Beispiel: Eine Einheit stirbt → das System sendet eine Nachricht „EntityDestroyed“ → andere Komponenten reagieren darauf (z. B. Soundeffekt oder Punktestand-Update).

5. **Erweiterbarkeit durch Daten und Skripte**

    Spielinhalte (z. B. Einheiten oder Gebäude) sind datengetrieben in XML/JSON beschrieben
    und können mit JavaScript-Skripten um spezifische Logik erweitert werden,
    ohne den C++-Code zu verändern.

### 5.3.2 ECS
Das Simulationssystem folgt dem ECS-Prinzip und ist in drei zentrale Strukturen gegliedert:
| **Element**                | **Beschreibung**                                                                                                                                                                                                                       |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Entity (Entität)**       | Repräsentiert ein einzelnes Spielobjekt – z. B. eine Einheit, ein Gebäude oder ein Projektil. Jede Entität besitzt eine eindeutige ID und besteht aus einer Menge von Komponenten.                                                     |
| **Component (Komponente)** | Kapselt Daten, die eine bestimmte Eigenschaft oder Fähigkeit beschreiben, z. B. Position, Gesundheit, Angriffskraft, Produktion oder Sichtweite. Komponenten enthalten **keine Logik**, nur Zustand.                                   |
| **System**                 | Implementiert die Logik, die auf Komponenten angewendet wird. Jedes System ist für einen bestimmten Aspekt zuständig, z. B. Bewegung, Kampf, Produktion, KI oder Sichtberechnung. Systeme werden in jedem Simulations-Tick ausgeführt. |

### 5.3.3 Komponenten und Systeme

| **Komponenten**                       | **Beispielhafte Systeme**                                       |
| ------------------------------------- | --------------------------------------------------------------- |
| `Position`, `Velocity`, `Orientation` | Bewegungssystem (aktualisiert Position und Richtung)            |
| `Health`, `Attack`, `Armor`           | Kampfsystem (führt Angriffe aus und berechnet Schaden)          |
| `ResourceGatherer`, `Storage`         | Wirtschaftssystem (sammelt Ressourcen, verwaltet Lagerbestände) |
| `ProductionQueue`, `Technology`       | Produktions-/Forschungssystem                                   |
| `Vision`, `Ownership`, `Formation`    | KI- und Sichtsysteme                                            |
| `Decay`, `Obstruction`, `Projectile`  | Umwelt- und Kollisionssysteme                                   |

## 5.4 Rendering Subsystem

Das **Rendering-Subsystem** ist für **grafische Darstellung der Spielwelt** verantwortlich.
Es bildet die Schnittstelle zwischen der Simulationslogik und der visuellen Ausgabe auf dem Bildschirm. Das System verarbeit die von der Simulatiuon bereitgestellten Datem (z.b Position, Animationen uzw.) und rendert daraus eine realistische , dynamische 3D-Spielwelt.
Das Rendering erfolgt plattformübergreifend über **OpenGl** und nutzt moderne Techsniken wie Schader , LOD(Leveld of Detail) und Culling.

### 5.4.1 Verantwortlichkeiten

- 1. **Darstellung der Spielwelt**

      Das Rendering-System übersetzt den abstrakten Spielzustand aus der Simulation (z. B. Einheiten, Gebäude, Gelände, Effekte) in sichtbare 3D-Objekte.
      Es verwaltet die Szenegraph-Struktur, in der alle darzustellenden Elemente organisiert sind.

- 2. **Kamerasteuerung und Sichtfeld**

      Die Kamera kann frei bewegt, rotiert und gezoomt werden.
      Das Rendering-System berechnet, welche Objekte im aktuellen Sichtfeld (Frustum) liegen, und rendert nur diese (Frustum Culling).

- 3. **Beleuchtung, Schatten und Effekte**

      Das System nutzt Shader-basierte Beleuchtung, dynamische Schatten und Partikeleffekte, um eine realistische Spielumgebung zu erzeugen.
      Wetter-, Feuer- und Explosionseffekte werden ebenfalls hier gesteuert.

- 4. **Level of Detail (LOD)**

      Abhängig von der Entfernung zur Kamera rendert das System Modelle mit unterschiedlicher Detailtiefe, um Performance zu optimieren.

- 5. **UI-Overlay**

      Neben der 3D-Welt rendert das Subsystem auch 2D-Overlays (z. B. Auswahlrahmen, Lebensbalken oder Minimap) über der Hauptszene.

- 6. **Performance und Optimierung**

      Das Rendering ist auf hohe Performance ausgelegt und nutzt Techniken wie Instancing, Textur-Atlas, Batch-Rendering und Occlusion Culling.
      Frame-Timing und GPU-Performance werden über das Engine-Profiling-System überwacht.


### 5.4.2 Aufbau 

Das Rendering-Subsystem besteht aus mehreren logischen Komponenten beispielweise :

| **Komponente**        | **Beschreibung**                                                                                |
| --------------------- | ----------------------------------------------------------------------------------------------- |
| **Scene Graph**       | Hierarchische Datenstruktur, die alle sichtbaren Objekte (Modelle, Effekte, Gelände) verwaltet. |
| **Terrain Renderer**  | Zeichnet Gelände, Höhenkarten, Texturen und Übergänge zwischen Biomen.                          |
| **Model Renderer**    | Rendert Einheiten, Gebäude und Objekte mit Animationen.                                         |
| **Water Renderer**    | Simuliert Wasser, Reflexionen und Wellenbewegungen.                                             |
| **Particle Renderer** | Verantwortlich für Effekte wie Rauch, Feuer, Staub oder Projektilspuren.                        |
| **Shader Manager**    | Lädt und verwaltet GPU-Shader (Beleuchtung, Transparenz, Texturen).                             |
| **Post-Processing**   | Fügt Nachbearbeitungseffekte hinzu (z. B. Bloom, Tiefenschärfe, Farbkorrektur).                 |

## 5.5 Audio Subsystem

Das **Audio-Subsystem** ist für die gesamte akustische Darstellung in 0 A.D verantwortlich.
Es verarbeitet Soundeffekte, Umgebungsgeräusche und Hintergrundmusik und sorgt dafür, dass akustische Ereignisse synchron zur Simulation und Darstellung ausgefürht werden.
Das System basiert auf der plattformübergreifenden Audio-Bibliothek **OpenAL**, welche 3D-Sound, Positionsberechnung und räumliche Audioeffekte unterstützt.

### 5.5.1 Verantwortlichkeiten

- 1. **Abspielen von Soundeffekten**

      Das Audio-System spielt Ereignissounds ab, wie Angriffe, Treffer, Gebäudefertigstellungen oder das Fällen eines Baumes.
      Diese Sounds werden durch Nachrichten aus der Simulation ausgelöst.

- 2. **Wiedergabe von Musik und Ambient-Sounds**

      Hintergrundmusik und Umgebungsgeräusche (Wind, Wasser, Tiere) laufen parallel zum Spielgeschehen und werden im Audio-Subsystem verwaltet.
      Es steuert Lautstärke, Übergänge und Wiedergabelisten.

- 3. **Räumliches (3D-)Audio**

      Die Position der Kamera und der Entitäten bestimmt, wie laut und aus welcher Richtung ein Sound abgespielt wird.
      Das System berechnet hierfür Lautstärkeabfälle, Panning und Filter, um ein realistisches Raumgefühl zu erzeugen.

- 4. **Audio-Mixing und Lautstärkekontrolle**

      Das System mischt unterschiedliche Audiokanäle (Effekte, Musik, Interface-Sounds) und bietet globale Regler für Spieler und Entwickler.

- 5. **Synchronisierung mit Simulation und Rendering**

      Die Audioausgabe reagiert auf Änderungen im Spielzustand, z. B.:

      - Einheit stirbt → Todesgeräusch
      - Projektil trifft → Aufprallsound
      - Gebäude startet Produktion → akustischer Hinweis

- 6. **Performance-Verwaltung**

      Das Audio-System arbeitet größtenteils asynchron und nutzt eigene Puffer, damit es die Framerate oder den Simulationsfluss nicht beeinflusst.

### 5.5.2 Aufbau

Das Audio-Subsystem besteht aus mehreren Komponenten :

| **Komponente**              | **Beschreibung**                                                                           |
| --------------------------- | ------------------------------------------------------------------------------------------ |
| **Sound Manager**           | Verwalten aller Soundquellen; steuert das Laden, Abspielen und Stoppen von Sounds.         |
| **Music Manager**           | Verwaltung von Hintergrundmusik, Wiedergabelisten und Übergängen.                          |
| **Audio Source Controller** | Repräsentiert eine einzelne Tonquelle (z. B. eine Einheit, Explosion oder Umgebungssound). |
| **Listener**                | Entspricht der Kamera; bestimmt, wie der Spieler den Ton wahrnimmt.                        |
| **OpenAL Backend**          | Bindings zu OpenAL für räumliches Audio und Hardwarebeschleunigung.                        |

## 5.6 Benutzeroberfläche

Die **Benutzeroberfläche (GUI)** von 0 A.D. ist für alle Interaktionen zwischen Spieler und Spiel zuständig.
Sie umfasst sowohl das **Hauptmenü**, die **Spielkonfiguration**, die **Lobby**, als auch das **In-Game-HUD**, über das der Spieler Einheiten auswählt, Befehle erteilt und Informationen über den Spielzustand erhält.
Die GUI wird überwiegend über **XML-Layout-Dateien und JavaScript-Skripte** definiert und ist somit vollständig daten- und skriptabhängig aufgebaut.
Dadurch ist sie besonders flexibel, leicht modifizierbar und gut erweiterbar.


### 5.6.1 verantwortlichkeiten

- 1. **Verarbeitung von Benutzereingaben**

      Die GUI interpretiert alle Eingaben des Spielers:

      - Mausaktionen (Klicken, Ziehen, Auswahlrechtecke)

      - Tastatureingaben (Hotkeys, Kamerasteuerung)

      - Menüinteraktionen

      - Diese Eingaben werden in Simulationsbefehle übersetzt, die an die ECS-Simulation weitergeleitet werden.

- 2. **Anzeige von Spielinformationen**

      Die GUI zeigt alle relevanten Daten an, wie:

      - Ressourcen und Spielstatistiken

      - Ausgewählte Einheiten und deren Attribute

      - Minimap

      - Bau- und Produktionsmenüs

      - Tooltips, Befehlsleisten und Einheitenaktionstasten
      Diese Informationen werden dynamisch aus der Simulation und dem Engine-Kern abgerufen.
    
- 3. **Navigieren durch Menüs und Spielmodi**

      Die GUI verwaltet Menülogik, z. B.:

      - Startmenü

      - Optionen (Audio, Grafik, Steuerung)

      - Kampagnen- und Szenariomenüs

      - Multiplayer-Lobby

      - Lade-/Speichermodi

- 4. **Kommunikation mit der Engine über die Engine-API**

      Die GUI nutzt viele Funktionen der Engine-API (z. B. Engine.GetGUIObjectByName, Engine.PickEntityAtPoint, Engine.PostCommand).
      Dadurch ruft sie sowohl Simulationsbefehle als auch Engine-Funktionen ab, ohne C++-Code zu berühren.

- 5. **Darstellung von Statusänderungen**

      Die GUI reagiert auf Spielereignisse:

      - Eine Einheit wird verletzt → Gesundheitsbalken ändern sich

      - Ein Gebäude wird fertiggestellt → Icons aktualisieren sich

      - Eine neue Technologie wird erforscht → Tooltip + Effekte
      Die GUI ist eng mit dem Event-System des Engine-Kerns verbunden.


### 5.6.2 Aufbau

Die GUI besteht aus meheren klar abgegrenzten Komponenten:

| **Komponente**             | **Beschreibung**                                                                            |
| -------------------------- | ------------------------------------------------------------------------------------------- |
| **XML-Layout-Dateien**     | Definieren die Struktur aller GUI-Elemente: Buttons, Panels, Tooltips, Frames.              |
| **JavaScript-Logik**       | Steuert dynamische Inhalte, reagiert auf Eingaben und führt Engine-API-Aufrufe aus.         |
| **GUI Renderer**           | Rendert 2D-Overlays und HUD-Elemente über der 3D-Spielszene.                                |
| **GUI Objekte / Controls** | Standard-Steuerelemente wie Buttons, Listen, Rahmen, Anzeigen.                              |
| **Interface Manager**      | Verwaltet GUI-Seiten (z. B. Menü → Spiel → Pausemenü) und sorgt für reibungslose Übergänge. |


# Laufzeitsicht 

Diese Sicht beschreibt im Gegensatz zur statischen Bausteinsicht die dynamischen Abläufe zur Laufzeit des Systems.Im Fokus steht nicht, aus welchen Modulen 0 A.D. besteht, sondern wie diese Module in typischen Szenarien zusammenarbeiten.

## 6.1 Beispiele für Szenarien

### 6.1.1 Beispiel 1: Spieler gibt einer Einheit einen Bewegungsbefehl (Move Command)


Dieses Diagramm zeigt das Zusammenspiel von **GUI** → **Engine Core** → **Simulation (ECS)** → **Rendering**.

![Move Command](GUI-Engine-Sim.png)

Der Benutzer löst eine Aktion aus, die GUI erzeugt einen passenden Command, dieser wird durch den Engine Core an die Simulation übergeben und nach Ausführung visuell dargestellt.
### 6.1.2 Beispiel 2: Multiplayer Lockstep – alle Clients synchronisieren Kommandos

![Lockstep](MultiplayerLockstep.png)

Hier wird gezeigt, wie 0 A.D. das deterministische Lockstep-Netzwerkmodell umsetzt:
Nach einem Spielbefehl werden die Commands über das Netzwerk an alle Clients verteilt.
Erst wenn alle Spieler denselben Befehl empfangen haben, wird der Simulations-Tick ausgeführt.

### 6.1.3 Beispiel 3: Start eine Spiels - Map laden

![StartGame](Startthegame.png)

Dieses Diagramm beschreibt, wie beim Start eines Spiels die GUI den Engine Core anweist,
die notwendigen Ressourcen zu laden, die Simulation zu initialisieren und anschließend die Darstellung einzuleiten.

# Verteilungssicht {#section-deployment-view}

:::::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Die Verteilungssicht beschreibt:
::::

1.  die technische Infrastruktur, auf der Ihr System ausgeführt wird,
    mit Infrastrukturelementen wie Standorten, Umgebungen, Rechnern,
    Prozessoren, Kanälen und Netztopologien sowie sonstigen
    Bestandteilen, und

2.  die Abbildung von (Software-)Bausteinen auf diese Infrastruktur.

Häufig laufen Systeme in unterschiedlichen Umgebungen, beispielsweise
Entwicklung-/Test- oder Produktionsumgebungen. In solchen Fällen sollten
Sie alle relevanten Umgebungen aufzeigen.

Nutzen Sie die Verteilungssicht insbesondere dann, wenn Ihre Software
auf mehr als einem Rechner, Prozessor, Server oder Container abläuft
oder Sie Ihre Hardware sogar selbst konstruieren.

Aus Softwaresicht genügt es, auf die Aspekte zu achten, die für die
Softwareverteilung relevant sind. Insbesondere bei der
Hardwareentwicklung kann es notwendig sein, die Infrastruktur mit
beliebigen Details zu beschreiben.

:::: formalpara
::: title
Motivation
:::

Software läuft nicht ohne Infrastruktur. Diese zugrundeliegende
Infrastruktur beeinflusst Ihr System und/oder querschnittliche
Lösungskonzepte, daher müssen Sie diese Infrastruktur kennen.
::::

:::: formalpara
::: title
Form
:::

Das oberste Verteilungsdiagramm könnte bereits in Ihrem technischen
Kontext enthalten sein, mit Ihrer Infrastruktur als EINE Blackbox. Jetzt
zoomen Sie in diese Infrastruktur mit weiteren Verteilungsdiagrammen
hinein:
::::

- Die UML stellt mit Verteilungsdiagrammen (Deployment diagrams) eine
  Diagrammart zur Verfügung, um diese Sicht auszudrücken. Nutzen Sie
  diese, evtl. auch geschachtelt, wenn Ihre Verteilungsstruktur es
  verlangt.

- Falls Ihre Infrastruktur-Stakeholder andere Diagrammarten bevorzugen,
  die beispielsweise Prozessoren und Kanäle zeigen, sind diese hier
  ebenfalls einsetzbar.

:::: formalpara
::: title
Weiterführende Informationen
:::

Siehe [Verteilungssicht](https://docs.arc42.org/section-7/) in der
online-Dokumentation (auf Englisch!).
::::
::::::::::::

## Infrastruktur Ebene 1 {#_infrastruktur_ebene_1}

:::: sidebar
::: title
:::

An dieser Stelle beschreiben Sie (als Kombination von Diagrammen mit
Tabellen oder Texten):

- die Verteilung des Gesamtsystems auf mehrere Standorte, Umgebungen,
  Rechner, Prozessoren o. Ä., sowie die physischen Verbindungskanäle
  zwischen diesen,

- wichtige Begründungen für diese Verteilungsstruktur,

- Qualitäts- und/oder Leistungsmerkmale dieser Infrastruktur,

- Zuordnung von Softwareartefakten zu Bestandteilen der Infrastruktur

Für mehrere Umgebungen oder alternative Deployments kopieren Sie diesen
Teil von arc42 für alle wichtigen Umgebungen/Varianten.
::::

***\<Übersichtsdiagramm\>***

Begründung

:   *\<Erläuternder Text\>*

Qualitäts- und/oder Leistungsmerkmale

:   *\<Erläuternder Text\>*

Zuordnung von Bausteinen zu Infrastruktur

:   *\<Beschreibung der Zuordnung\>*

## Infrastruktur Ebene 2 {#_infrastruktur_ebene_2}

:::: sidebar
::: title
:::

An dieser Stelle können Sie den inneren Aufbau (einiger)
Infrastrukturelemente aus Ebene 1 beschreiben.

Für jedes Infrastrukturelement kopieren Sie die Struktur aus Ebene 1.
::::

### *\<Infrastrukturelement 1\>* {#_infrastrukturelement_1}

*\<Diagramm + Erläuterungen\>*

### *\<Infrastrukturelement 2\>* {#_infrastrukturelement_2}

*\<Diagramm + Erläuterungen\>*

...​

### *\<Infrastrukturelement n\>* {#_infrastrukturelement_n}

*\<Diagramm + Erläuterungen\>*

# Querschnittliche Konzepte {#section-concepts}

:::::::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Dieser Abschnitt beschreibt übergreifende, prinzipielle Regelungen und
Lösungsansätze, die an mehreren Stellen (=*querschnittlich*) relevant
sind.
::::

Solche Konzepte betreffen oft mehrere Bausteine. Dazu können vielerlei
Themen gehören, wie beispielsweise die Themen aus dem nachfolgenden
Diagramm:

![Mögliche Themen für querschnittliche
Konzepte](images/08-concepts-DE.drawio.png)

:::: formalpara
::: title
Motivation
:::

Konzepte bilden die Grundlage für *konzeptionelle Integrität*
(Konsistenz, Homogenität) der Architektur und damit eine wesentliche
Grundlage für die innere Qualität Ihrer Systeme.
::::

Dieser Abschnitt im Template ist der richtige Ort für die konsistente
Behandlung solcher Themen.

Viele solche Konzepte beeinflussen oder beziehen sich auf mehrerer Ihrer
Bausteine.

:::: formalpara
::: title
Form
:::

Kann vielfältig sein:
::::

- Konzeptpapiere mit beliebiger Gliederung,

- beispielhafte Implementierung speziell für technische Konzepte,

- übergreifende Modelle/Szenarien mit Notationen, die Sie auch in den
  Architektursichten nutzen,

:::: formalpara
::: title
Struktur
:::

Wählen Sie **nur** die wichtigsten Themen für Ihr System und erklären
das jeweilige Konzept dann unter einer Level-2 Überschrift dieser
Sektion (z.B. 8.1, 8.2 etc).
::::

Beschränken Sie sich auf die wichtigen, und versuchen **auf keinen
Fall** alle oben dargestellten Themen zu bearbeiten.

:::: formalpara
::: title
Weiterführende Informationen
:::

Einige Themen innerhalb von Systemen betreffen oft mehrere Bausteine,
Hardwareelemente oder Prozesse. Es könnte einfacher sein, solche
*Querschnittsthemen* an einer zentralen Stelle zu kommunizieren oder zu
dokumentieren, anstatt sie in der Beschreibung der betreffenden
Bausteine, Hardwareelemente oder Entwicklungsprozesse zu wiederholen.
::::

Bestimmte Konzepte können **alle** Elemente eines Systems betreffen,
andere sind vielleicht nur für einige wenige relevant.

Siehe [Querschnittliche Konzepte](https://docs.arc42.org/section-8/) in
der online-Dokumentation (auf Englisch).
::::::::::::::

## *\<Konzept 1\>* {#_konzept_1}

*\<Erklärung\>*

## *\<Konzept 2\>* {#_konzept_2}

*\<Erklärung\>*

...​

## *\<Konzept n\>* {#_konzept_n}

*\<Erklärung\>*

# Architekturentscheidungen {#section-design-decisions}

:::::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Wichtige, teure, große oder riskante Architektur- oder
Entwurfsentscheidungen inklusive der jeweiligen Begründungen. Mit
\"Entscheidungen\" meinen wir hier die Auswahl einer von mehreren
Alternativen unter vorgegebenen Kriterien.
::::

Wägen Sie ab, inwiefern Sie Entscheidungen hier zentral beschreiben,
oder wo eine lokale Beschreibung (z.B. in der Whitebox-Sicht von
Bausteinen) sinnvoller ist. Vermeiden Sie Redundanz. Verweisen Sie evtl.
auf Abschnitt 4, wo schon grundlegende strategische Entscheidungen
beschrieben wurden.

:::: formalpara
::: title
Motivation
:::

Stakeholder des Systems sollten wichtige Entscheidungen verstehen und
nachvollziehen können.
::::

:::: formalpara
::: title
Form
:::

Verschiedene Möglichkeiten:
::::

- ADR ([Documenting Architecture
  Decisions](https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions))
  für jede wichtige Entscheidung

- Liste oder Tabelle, nach Wichtigkeit und Tragweite der Entscheidungen
  geordnet

- ausführlicher in Form einzelner Unterkapitel je Entscheidung

:::: formalpara
::: title
Weiterführende Informationen
:::

Siehe [Architekturentscheidungen](https://docs.arc42.org/section-9/) in
der arc42 Dokumentation (auf Englisch!). Dort finden Sie Links und
Beispiele zum Thema ADR.
::::
::::::::::::

# Qualitätsanforderungen 

## 10.1 Qualitätsbaum

Das folgende Bild gibt in Form eines sogenannten Qualitätsbaumes  einen Überblick über die relevanten Qualitätsmerkmale und ordnet ihnen Szenarien als Beispiele zu. Die Qualitätsziele sind in der Abbildung ebenfalls enthalten und verweisen jeweils auf die Szenarien, welche sie illustrieren.

![Qualitätsbaum](Qualitätanforderungen.png)
## 10.2 Qualitätsszenarien

Die Anfangsbuchstaben der Bezeichner (IDs) der Szenarien in der folgenden Tabelle stehen jeweils für das übergeordnete Qualitätsmerkmal,  M beispielsweise für Erweiterbarkeit. Die Bezeichner finden auch im Qualitätsbaum Verwendung. Nicht immer lassen sich die Szenarien eindeutig einem Merkmal zuordnen. Sie treten daher mitunter mehrmals im Qualitätsbaum auf.


| **Qualitätsbereich**             | **ID**  | **Qualitätsszenario (Stimulus, Kontext, Reaktion, Messkriterium)**                                                                                                                               |
| -------------------------------- | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Erweiterbarkeit / Modding**    | **M01** | *Stimulus:* Modder fügt eine neue Zivilisation hinzu. *Kontext:* Keine Engine-Codeänderung. *Reaktion:* Engine lädt Templates. *Messkriterium:* Zivilisation erscheint im Menü und ist spielbar. |
|                                  | **M02** | *Stimulus:* Neue XML/JSON-Datei wird erstellt. *Kontext:* Spielstart. *Reaktion:* Engine liest Datei korrekt. *Messkriterium:* Einheit erscheint ohne Codeänderung im Spiel.                     |
|                                  | **M03** | *Stimulus:* Neues JavaScript-Script wird hinzugefügt. *Kontext:* Engine startet. *Reaktion:* Script läuft in Sandbox. *Messkriterium:* Funktioniert ohne Engine-Modifikation.                    |
| **Performance / Effizienz**      | **P01** | *Stimulus:* 400 Einheiten aktiv. *Kontext:* Standard-Hardware. *Reaktion:* Simulation verarbeitet alle. *Messkriterium:* Mindestens 30 FPS.                                                      |
|                                  | **P02** | *Stimulus:* Große Massenschlacht. *Kontext:* Viele Effekte. *Reaktion:* Rendering optimiert. *Messkriterium:* FPS bleibt > 25 FPS.                                                               |
|                                  | **P03** | *Stimulus:* Spielerbefehl wird ausgeführt. *Kontext:* Hochlastphase. *Reaktion:* Engine verarbeitet sofort. *Messkriterium:* < 150 ms Verzögerung.                                               |
|                                  | **P04** | *Stimulus:* Viele ECS-Komponenten verändern sich. *Kontext:* Simulations-Tick. *Reaktion:* ECS verarbeitet effizient. *Messkriterium:* Tick < 60 ms.                                             |
| **Multiplayer-Zuverlässigkeit**  | **N01** | *Stimulus:* Spieler senden gleichzeitig Befehle. *Kontext:* Lockstep. *Reaktion:* Gleichzeitige Tick-Ausführung. *Messkriterium:* GameState identisch bei allen Clients.                         |
|                                  | **N02** | *Stimulus:* Netzwerk-Lag. *Kontext:* Multiplayer-Spiel. *Reaktion:* Engine puffert Befehle. *Messkriterium:* Kein Desync.                                                                        |
|                                  | **N03** | *Stimulus:* Replay wird geladen. *Kontext:* Gespeicherte Befehle. *Reaktion:* Simulation rekonstruiert Match. *Messkriterium:* 100% Identisch zur Originalpartie.                                |
| **Wartbarkeit**                  | **W01** | *Stimulus:* Neues Subsystem wird hinzugefügt. *Kontext:* Modulare Architektur. *Reaktion:* Engine integriert über Interfaces. *Messkriterium:* Keine Änderungen an anderen Subsystemen nötig.    |
|                                  | **W02** | *Stimulus:* Entwickler schreibt Unit-Test. *Kontext:* Subsystem-isolierung. *Reaktion:* Test läuft ohne Abhängigkeiten. *Messkriterium:* Komponente isoliert testbar.                            |
|                                  | **W03** | *Stimulus:* Entwickler liest ECS-Komponenten. *Kontext:* Neue Fähigkeit. *Reaktion:* Leicht verständlich. *Messkriterium:* < 10 Minuten Einlernzeit.                                             |
| **Portabilität**                 | **T01** | *Stimulus:* Spielstart auf verschiedenen OS. *Kontext:* Gleiches Build. *Reaktion:* Engine initialisiert erfolgreich. *Messkriterium:* Keine OS-spezifischen Fehler.                             |
|                                  | **T02** | *Stimulus:* Update von OpenGL/SDL. *Kontext:* Engine nutzt abstrahierte APIs. *Reaktion:* Läuft ohne Änderungen. *Messkriterium:* Keine Inkompatibilitäten.                                      |
|                                  | **T03** | *Stimulus:* OS hat andere Datei-API. *Kontext:* Engine nutzt FS-Abstraktion. *Reaktion:* Einheitliches Verhalten. *Messkriterium:* Keine Plattformbugs.                                          |
| **Internationalisierung (I18N)** | **I01** | *Stimulus:* Sprachwechsel im Menü. *Kontext:* Spiel läuft. *Reaktion:* Texte laden neu. *Messkriterium:* < 1 Sekunde Reaktionszeit.                                                              |
|                                  | **I02** | *Stimulus:* Anzeige chinesischer Schrift. *Kontext:* GUI aktiv. *Reaktion:* Engine rendert Unicode korrekt. *Messkriterium:* Keine Darstellungsfehler.                                           |
|                                  | **I03** | *Stimulus:* Mod liefert neue .po-Dateien. *Kontext:* Spielstart. *Reaktion:* Engine lädt neue Strings. *Messkriterium:* Alle Texte korrekt sichtbar.                                             |
| **Benutzbarkeit**                | **U01** | *Stimulus:* Spieler wählt Einheit im Kampf. *Kontext:* Viele Entities. *Reaktion:* HUD aktualisiert schnell. *Messkriterium:* < 200 ms.                                                          |
|                                  | **U02** | *Stimulus:* Ressourcen ändern sich. *Kontext:* HUD aktiv. *Reaktion:* GUI aktualisiert Anzeige. *Messkriterium:* < 100 ms.                                                                       |
|                                  | **U03** | *Stimulus:* Neuer Spieler startet Tutorial. *Kontext:* Standard-GUI. *Reaktion:* Eindeutige Anleitungen. *Messkriterium:* Spieler versteht Grundlagen in < 5 Minuten.                            |
| **Stabilität & Sicherheit**      | **S01** | *Stimulus:* JavaScript-Mod enthält Fehler. *Kontext:* Engine lädt Mods. *Reaktion:* Sandbox blockiert fehlerhaften Code. *Messkriterium:* Kein Absturz.                                          |
|                                  | **S02** | *Stimulus:* Textur fehlt. *Kontext:* Map-Ladevorgang. *Reaktion:* Engine loggt Warnung. *Messkriterium:* Spiel läuft weiter.                                                                     |
|                                  | **S03** | *Stimulus:* XML ist ungültig. *Kontext:* Spielstart. *Reaktion:* Engine meldet Fehler. *Messkriterium:* Engine bleibt stabil.                                                                    |


# Risiken und technische Schulden 

Die folgende Tabelle gibt einen strukturierten Überblick über die zentralen technischen und architektonischen Risiken von 0 A.D.

| **Risiko-ID** | **Beschreibung**                                                                                              |
| ------------- | ------------------------------------------------------------------------------------------------------------- |
| **R01**       | Hohe Komplexität des ECS-Systems erschwert Debugging und führt zu potenziell unerwarteten Logikfehlern.       |
| **R02**       | Gefahr von Desynchronisationen im Multiplayer aufgrund des deterministischen Lockstep-Modells.                |
| **R03**       | Performance-Probleme bei großen Massenschlachten durch hohe CPU-Last (Pathfinding, Kampf, Sichtweite).        |
| **R04**       | Abhängigkeit von älteren Technologien wie OpenGL oder SpiderMonkey kann zukünftige Wartung erschweren.        |
| **R05**       | Fehlerhafte oder inkompatible Mods können Instabilität verursachen oder Spielabläufe stören.                  |
| **R06**       | Große und komplexe Codebasis (C++ + JS) führt zu hoher Einarbeitungszeit für neue Entwickler.                 |
| **R07**       | Plattformabhängige Unterschiede zwischen Windows, Linux und macOS können OS-spezifische Bugs verursachen.     |
| **R08**       | Große Asset-Dateien führen zu langen Ladezeiten und hohem Speicherverbrauch.                                  |
| **R09**       | KI (Petra Bot) benötigt viel CPU-Leistung, was im Spiel zu FPS-Einbrüchen führen kann.                        |
| **R10**       | Komplexität der deterministischen Simulation macht bestimmte Bugs schwer reproduzierbar und schwer zu finden. |


| **Technische Schuld** | **Beschreibung**                                     |
| --------------------- | ---------------------------------------------------- |
| **TS01**              | Veraltete SpiderMonkey JS-Engine → erschwert Updates |
| **TS02**              | Viele Legacy-C++-Module ohne klare Abgrenzung        |
| **TS03**              | Fehlende vollständige Testabdeckung                  |
| **TS04**              | Inkompatible oder alte Assets im Modding-System      |
| **TS05**              | Nicht vollständig dokumentierte ECS-Komponenten      |


# Glossar {#section-glossary}

:::::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Die wesentlichen fachlichen und technischen Begriffe, die Stakeholder im
Zusammenhang mit dem System verwenden.
::::

Nutzen Sie das Glossar ebenfalls als Übersetzungsreferenz, falls Sie in
mehrsprachigen Teams arbeiten.

:::: formalpara
::: title
Motivation
:::

Sie sollten relevante Begriffe klar definieren, so dass alle Beteiligten
::::

- diese Begriffe identisch verstehen, und

- vermeiden, mehrere Begriffe für die gleiche Sache zu haben.

:::: formalpara
::: title
Form
:::

Zweispaltige Tabelle mit \<Begriff\> und \<Definition\>.
::::

Eventuell weitere Spalten mit Übersetzungen, falls notwendig.

:::: formalpara
::: title
Weiterführende Informationen
:::

Siehe [Glossar](https://docs.arc42.org/section-12/) in der
online-Dokumentation (auf Englisch!).
::::
::::::::::::

+----------------------+-----------------------------------------------+
| Begriff              | Definition                                    |
+======================+===============================================+
| *\<Begriff-1\>*      | *\<Definition-1\>*                            |
+----------------------+-----------------------------------------------+
| *\<Begriff-2*        | *\<Definition-2\>*                            |
+----------------------+-----------------------------------------------+
