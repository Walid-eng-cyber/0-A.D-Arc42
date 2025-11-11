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


## 5.1 Ebene 1 – Überblick über die Subsysteme

Dieser Abschnitt beschreibt die wichtigsten Subsysteme von 0 A.D. auf oberster Ebene.
Die Architektur trennt den technischen Kern (Engine) von der Darstellung, den Spieldaten und der Benutzeroberfläche.
Jedes Subsystem erfüllt eine klar definierte Aufgabe und kommuniziert über wohlstrukturierte Schnittstellen mit anderen Modulen.


# Laufzeitsicht {#section-runtime-view}

:::::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Diese Sicht erklärt konkrete Abläufe und Beziehungen zwischen Bausteinen
in Form von Szenarien aus den folgenden Bereichen:
::::

- Wichtige Abläufe oder *Features*: Wie führen die Bausteine der
  Architektur die wichtigsten Abläufe durch?

- Interaktionen an kritischen externen Schnittstellen: Wie arbeiten
  Bausteine mit Nutzern und Nachbarsystemen zusammen?

- Betrieb und Administration: Inbetriebnahme, Start, Stop.

- Fehler- und Ausnahmeszenarien

Anmerkung: Das Kriterium für die Auswahl der möglichen Szenarien (d.h.
Abläufe) des Systems ist deren Architekturrelevanz. Es geht nicht darum,
möglichst viele Abläufe darzustellen, sondern eine angemessene Auswahl
zu dokumentieren.

:::: formalpara
::: title
Motivation
:::

Sie sollten verstehen, wie (Instanzen von) Bausteine(n) Ihres Systems
ihre jeweiligen Aufgaben erfüllen und zur Laufzeit miteinander
kommunizieren.
::::

Nutzen Sie diese Szenarien in der Dokumentation hauptsächlich für eine
verständlichere Kommunikation mit denjenigen Stakeholdern, die die
statischen Modelle (z.B. Bausteinsicht, Verteilungssicht) weniger
verständlich finden.

:::: formalpara
::: title
Form
:::

Für die Beschreibung von Szenarien gibt es zahlreiche
Ausdrucksmöglichkeiten. Nutzen Sie beispielsweise:
::::

- Nummerierte Schrittfolgen oder Aufzählungen in Umgangssprache

- Aktivitäts- oder Flussdiagramme

- Sequenzdiagramme

- BPMN (Geschäftsprozessmodell und -notation) oder EPKs
  (Ereignis-Prozessketten)

- Zustandsautomaten

- ...​

:::: formalpara
::: title
Weiterführende Informationen
:::

Siehe [Laufzeitsicht](https://docs.arc42.org/section-6/) in der
online-Dokumentation (auf Englisch!).
::::
::::::::::::

## *\<Bezeichnung Laufzeitszenario 1\>* {#_bezeichnung_laufzeitszenario_1}

- \<hier Laufzeitdiagramm oder Ablaufbeschreibung einfügen\>

- \<hier Besonderheiten bei dem Zusammenspiel der Bausteine in diesem
  Szenario erläutern\>

## *\<Bezeichnung Laufzeitszenario 2\>* {#_bezeichnung_laufzeitszenario_2}

...​

## *\<Bezeichnung Laufzeitszenario n\>* {#_bezeichnung_laufzeitszenario_n}

...​

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

# Qualitätsanforderungen {#section-quality-scenarios}

:::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Dieser Abschnitt enthält alle relevanten Qualitätsanforderungen.
::::

Die wichtigsten davon haben Sie bereits in Abschnitt 1.2
(Qualitätsziele) hervorgehoben, daher soll hier nur auf sie verwiesen
werden. In diesem Abschnitt 10 sollten Sie auch Qualitätsanforderungen
mit geringerer Bedeutung erfassen, deren Nichterfüllung keine großen
Risiken birgt (die aber *nice-to-have* sein könnten).

:::: formalpara
::: title
Motivation
:::

Weil Qualitätsanforderungen die Architekturentscheidungen oft maßgeblich
beeinflussen, sollten Sie die für Ihre Stakeholder relevanten
Qualitätsanforderungen kennen, möglichst konkret und operationalisiert.
::::

<div>

::: title
Weiterführende Informationen
:::

- Siehe [Qualitätsanforderungen](https://docs.arc42.org/section-10/) in
  der online-Dokumentation (auf Englisch!).

- Siehe auch das ausführliche [Q42 Qualitätsmodell auf
  https://quality.arc42.org](https://quality.arc42.org).

</div>
::::::::::

## Übersicht der Qualitätsanforderungen {#_übersicht_der_qualitätsanforderungen}

:::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Eine Übersicht oder Zusammenfassung der Qualitätsanforderungen.
::::

:::: formalpara
::: title
Motivation
:::

Oft stößt man auf Dutzende (oder sogar Hunderte) von detaillierten
Qualitätsanforderungen für ein System. In diesem Abschnitt sollten Sie
versuchen, sie zusammenzufassen, z. B. durch die Beschreibung von
Kategorien oder Themen (wie z.B. von [ISO
25010:2023](https://www.iso.org/obp/ui/#iso:std:iso-iec:25010:ed-2:v1:en)
oder [Q42](https://quality.arc42.org) vorgeschlagen).
::::

Wenn diese Kurzbeschreibungen oder Zusammenfassungen bereits präzise,
spezifisch und messbar sind, können Sie Abschnitt 10.2 auslassen.

:::: formalpara
::: title
Form
:::

Verwenden Sie eine einfache Tabelle, in der jede Zeile eine Kategorie
oder ein Thema und eine kurze Beschreibung der Qualitätsanforderung
enthält. Alternativ können Sie auch eine Mindmap verwenden, um diese
Qualitätsanforderungen zu strukturieren. In der Literatur (insb.
\[Bass+21\]) ist die Idee eines *Quality Attribute Utility Tree* (auf
Deutsch manchmal kurz als *Qualitätsbaum* bezeichnet) beschrieben
worden, der den Oberbegriff „Qualität" als Wurzel hat und eine
baumartige Verfeinerung des Begriffs „Qualität" verwendet.
::::
::::::::::

## Qualitätsszenarien {#_qualitätsszenarien}

:::::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Qualitätsszenarien konkretisieren Qualitätsanforderungen und ermöglichen
es zu entscheiden, ob sie erfüllt sind (im Sinne von
Akzeptanzkriterien). Stellen Sie sicher, dass Ihre Szenarien spezifisch
und messbar sind.
::::

Zwei Arten von Szenarien finden wir besonders nützlich:

- Nutzungsszenarien (auch bekannt als Anwendungs- oder
  Anwendungsfallszenarien) beschreiben, wie das System zur Laufzeit auf
  einen bestimmten Auslöser reagieren soll. Hierunter fallen auch
  Szenarien zur Beschreibung von Effizienz oder Performance. Beispiel:
  Das System beantwortet eine Benutzeranfrage innerhalb einer Sekunde.

- Änderungsszenarien\_ beschreiben die gewünschte Wirkung einer Änderung
  oder Erweiterung des Systems oder seiner unmittelbaren Umgebung.
  Beispiel: Zusätzliche Funktionalität wird implementiert oder
  Anforderungen an ein Qualitätsmerkmal ändern sich, und der Aufwand
  oder die Dauer der Änderung wird gemessen.

:::: formalpara
::: title
Form
:::

Typische Informationen für detaillierte Szenarien sind die folgenden:
::::

In Kurzform (bevorzugt im Q42-Modell):

- K**ontext/Hintergrund**: Um welche Art von System oder Komponente
  handelt es sich, wie sieht die Umgebung oder Situation aus?

- **Quelle/Stimulus**: Wer oder was initiiert oder löst ein Verhalten,
  eine Reaktion oder eine Aktion aus.

- **Metrik/Akzeptanzkriterien**: Eine Reaktion einschließlich einer
  *Maßnahme* oder *Metrik*

Die Langform von Szenarien (die von der SEI und \[Bass+21\] bevorzugt
wird) ist detaillierter und enthält die folgenden Informationen:

- **Szenario-ID**: Ein eindeutiger Bezeichner für das Szenario.

- **Szenario-Name**: Ein kurzer, beschreibender Name für das Szenario.

- **Quelle**: Die Entität (Benutzer, System oder Ereignis), die das
  Szenario auslöst.

- **Stimulus**: Das auslösende Ereignis oder die Bedingung, auf die das
  System reagieren muss.

- **Umgebung**: Der betriebliche Kontext oder die Bedingungen, unter
  denen das System den Stimulus erlebt.

- **Artefakt**: Die Bausteine oder anderen Elemente des Systems, die von
  dem Stimulus betroffen sind.

- **Reaktion**: Das Ergebnis oder Verhalten, das das System als Reaktion
  auf den Stimulus zeigt.

- **Antwortmaß**: Das Kriterium oder die Metrik, nach der die Antwort
  des Systems bewertet wird.

:::: formalpara
::: title
Beispiele
:::

Ausführliche Beispiele für Qualitätsanforderungen finden Sie auf [der
Website zum Qualitätsmodell Q42](https://quality.arc42.org).
::::

<div>

::: title
Weitere Informationen
:::

- Len Bass, Paul Clements, Rick Kazman: „Software Architecture in
  Practice", 4. Auflage, Addison-Wesley, 2021.

</div>
::::::::::::

# Risiken und technische Schulden {#section-technical-risks}

:::::::::::: sidebar
::: title
:::

:::: formalpara
::: title
Inhalt
:::

Eine nach Prioritäten geordnete Liste der erkannten Architekturrisiken
und/oder technischen Schulden.
::::

<div>

::: title
Motivation
:::

> Risikomanagement ist Projektmanagement für Erwachsene.
>
> ---  Tim Lister Atlantic Systems Guild

</div>

Unter diesem Motto sollten Sie Architekturrisiken und/oder technische
Schulden gezielt ermitteln, bewerten und Ihren Management-Stakeholdern
(z.B. Projektleitung, Product-Owner) transparent machen.

:::: formalpara
::: title
Form
:::

Liste oder Tabelle von Risiken und/oder technischen Schulden, eventuell
mit vorgeschlagenen Maßnahmen zur Risikovermeidung, Risikominimierung
oder dem Abbau der technischen Schulden.
::::

:::: formalpara
::: title
Weiterführende Informationen
:::

Siehe [Risiken und technische
Schulden](https://docs.arc42.org/section-11/) in der
online-Dokumentation (auf Englisch!).
::::
::::::::::::

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
