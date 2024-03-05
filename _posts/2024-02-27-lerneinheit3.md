---
title: "Lerneinheit 3: Funktion und Aufbau von Bibliothekssystemen"
date: 2024-02-27
---

Heute sind wir nach den letzten beiden eher organisatorischen Einheiten ins eigentliche Thema des Moduls eingestiegen (siehe auch [gemeinsames Dokument dieser Lerneinheit](https://pad.gwdg.de/EC9WU7DITxiK1ciMll3ZOw)). Dazu haben wir uns die Metadatenstandards MARC21 und Dublin Core sowie den Unterschied zwischen Regelwerk und Datenformat angeschaut. Zum Abschluss haben wir uns ausserdem noch mit dem Open Source Bibliothekssystem 'Koha' befasst. Von Dublin Core habe ich bereits vor längerer Zeit in einem anderen Modul gehört, habe jedoch dazu kein vertieftes Wissen. Der restliche Inhalt dieser Lerneinheit war für mich gänzlich neu, deshalb nachfolgend eine grobe Zusammenfassung.

## Metadatenstandards in Bibliotheken
### MARC21
Zu Beginn haben wir uns **den** Metadatenstandard für Bibliotheken schlechthin angeschaut: MARC21. MARC21 wurde 1999 von der [Library of Congress](https://www.loc.gov) begründet und kann entweder als XML oder im eigenen Binärformat (.mrc) kodiert werden. Der Standard ist international verbreitet und wird von grossen Bibliothekssystemen als Basis genutzt oder als Austauschformat unterstützt. Aber trotz der internationalen Verbreitung kann es in der praktischen Anwendung grössere Abweichungen zwischen den Anwendenden geben. Das ist auf unterschiedliche Katalogisierungsregeln der Institutionen und die Möglichkeit eigene Felder zu belegen zurückzuführen. Weitere Abweichungen kommen zudem nocht durch Anwendungsfehler oder technische Fehler zustande. Um letzterem entgegenzuwirken gibt es Assessment-Software, die die Verwendung des Standards auf Fehler prüft.

Ein MARC21-Datensetz besteht aus 3 Elementen: Datensatzstruktur, Inhaltsbezeichnung und Dateninhalt. Für die Inhaltsbezeichnung der Felder werden explizit festgelegte Codes, bestehend aus Buchstaben und Zahlen, verwendet (siehe auch [Summary Statement of Content Designators](https://www.loc.gov/marc/bibliographic/bdsummary.html)) [^1]. Da die Inhaltsbezeichnungen aus Codes bestehen, sind sie weniger gut menschenlesbar als es Inhaltsbezeichnungen mit sprechende Namen wären.

MARC21 soll voraussichtlich in Zukunft durch das auf RDF basierende Datenmodell BIBFRAME abgelöst werden, welches Inkonsistenzen verhindern soll. MARC21 orientiert sich am Medium, wodurch pro Werk ein Eintrag erstellt wird, welcher mit allen notwendigen Angeben befüllt wird. Das kann dazu führen, dass derselbe Autor je nach Werk auf verschiedene Arten aufgeführt wird. Bei BIBFRAME hingegen wird pro Autor ein Eintrag erstellt, welcher dann bei den zugehörigen Werken verlinkt werden kann.

### Dublin Core
Dublin Core ist im Gegensatz zu MARC21 ein Standard, welcher über die Bibliothekswelt hinaus genutzt wird. Im Kern setzt sich der Standard aus 15 Basiselementen zusammen, welche sprechende Namen wie z. B. "title" tragen.  

### Vergleich MARC21 und Dublin Core
In einer kurzen Übung haben wir MARC21 mit Dublin Core verglichen und unsere Erkenntnisse im [gemeinsemen Dokument](https://pad.gwdg.de/EC9WU7DITxiK1ciMll3ZOw#Erkenntnisse-Fragen) festgehalten. Kurz zusammengefasst ist der Dublin Core kompakter und durch die sprechenden Feldnamen besser menschenlesbar wohingegen MARC21 spezifischere Angaben ermöglicht und für Maschinen besser verwertbar ist.

## Regelwerk vs. Datenformat
Nebst den Standards gibt es auch noch ergänzende Regelwerke. Darin wird definiert, wie eine Ressource beschrieben werden soll (theoretische Grundlage für Katalogisierung). Zu den Regelwerken gehören normalerweise normierte Vokabularien und inhaltliche Kategorien. Ein Beispiel für ein Regelwerk ist 'Resource Description and Access' kurz RDA.

Anders als Regelwerke dienen Datenformate der praktischen Repräsentation von Katalogisaten. Datenformate legen mit Hilfe von Datenstrukturen und Datentypen fest, wie Daten zu kodieren sind. MARC21 und BIBFRAME zählen zu den Datenformaten, wobei BIBFRAME auch Aspekte eines Regelwerks beinhaltet (-> Datenmodell). In der Praxis werden die Begriffe 'Standard' und 'Datenformat' teilweise auch Synonym verwendet.

💡 Regelwerke und Datenformate sind nicht immer trennscharf und ergänzen sich gegenseitig. Bei einer Kombinatoin von beidem wird von einem Datenmodell gesprochen.

## Koha
Zum Schluss der Lerneinheit haben wir uns noch mit [Koha](https://koha-community.org/), dem auf MARC21-basierenden, skalierbaren Open Source Bibliotheksverwaltungssstem beschäftigt. Um besser zu verstehen, wie ein solches System im Hintergrund funktioniert, haben wir zuerst gemeinsam die Grundkonfiguration angeschaut. Anschliessend haben wir noch einzeln das System erforscht, indem wir auf dem Demo-System verschiedene Use Cases durchgespielt haben (z. B. Buch erfassen oder Benutzer anlegen).

Die Software steht unter der GNU General Public License (GPL). Das heisst, dass die Software frei genutzt und weiterentwickelt werden darf, die Weiterentwicklungen müssen jedoch auch wieder unter derselben Lizenz veröffentlicht werden und dürfen nicht verkauft werden.

### Gesundheit von Open Source Software
Nicht jedes Open Source Projekt ist ein solches Vorzeige-Projekt wie Koha. Aus diesem Grund ist es besonders wichtig, vor der Nutzung von Open Source Software den Gesundheitsstatus zu überprüfen (dazu gibt es verschiedene Internetseiten).

💡 Der Gesundheitsstatus sagt aus wie stabil eine Software ist und dementsprechen auch wie wahrscheinlich es ist, dass die Sotware noch lange besteht und auch weiterentwickelt wird.



[^1]: https://www.loc.gov/marc/bibliographic/bdintro.html
