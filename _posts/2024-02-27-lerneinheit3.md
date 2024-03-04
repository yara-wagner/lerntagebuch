---
title: "Lerneinheit 3: Funktion und Aufbau von Bibliothekssystemen"
date: 2024-02-27
---

Ein Entwurf für meine Erfahrungen in der dritten Lehreinheit "..."

Heute sind wir nach den letzten beiden eher organisatorischen Einheiten ins eigentliche Thema des Moduls eingestiegen (siehe auch [gemeinsames Dokument dieser Lerneinheit](https://pad.gwdg.de/EC9WU7DITxiK1ciMll3ZOw)). Dazu haben wir uns die Metadatenstandards MARC21 und Dublin Core sowie den Unterschied zwischen Regelwerk und Datenformat angeschaut. Zum Abschluss haben wir uns ausserdem noch mit dem Open Source Bibliothekssystem 'Koha' befasst. Von Dublin Core habe ich bereits vor längerer Zeit in einem anderen Modul gehört, habe jedoch dazu kein vertieftes Wissen. Der restliche Inhalt dieser Lerneinheit war für mich gänzlich neu, deshalb nachfolgend eine grobe Zusammenfassung.

## Metadatenstandards in Bibliotheken
### MARC21
Zu Beginn haben wir uns **den** Metadatenstandard für Bibliotheken schlechthin angeschaut: MARC21. MARC21 wurde 1999 von der [Library of Congress](https://www.loc.gov) begründet und kann entweder als XML oder im eigenen Binärformat (.mrc) kodiert werden. Der Standard ist international verbreitet und wird von grossen Bibliothekssystemen als Basis genutzt oder als Austauschformat unterstützt. Aber trotz der internationalen Verbreitung kann es in der praktischen Anwendung grössere Abweichungen zwischen den Anwendenden geben. Das ist auf unterschiedliche Katalogisierungsregeln der Institutionen und die Möglichkeit eigene Felder zu belegen zurückzuführen. Weitere Abweichungen kommen zudem nocht durch Anwendungsfehler oder technische Fehler zustande. Um dem entgegenzuwirken gibt es Assessment-Software, die die Verwendung des Standards auf Fehler prüft.

Ein MARC21-Datensetz besteht aus 3 Elementen: Datensatzstruktur, Inhaltsbezeichnung und Dateninhalt. Für die Inhaltsbezeichnung der Felder werden explizit festgelegte Codes, bestehend aus Buchstaben und Zahlen, verwendet (siehe auch [Summary Statement of Content Designators](https://www.loc.gov/marc/bibliographic/bdsummary.html)) [^1]. Da die Inhaltsbezeichnungen aus Codes bestehen, sind sie weniger gut menschenlesbar als es Inhaltsbezeichnungen mit sprechende Namen wären.
-> ToDo: Beispiel aufzeigen und erklären

MARC21 soll voraussichtlich in Zukunft durch das auf RDF basierende Datenmodell BIBFRAME abgelöst werden, welches Inkonsistenzen verhindern soll. MARC21 orientiert sich am Medium, wodurch pro Werk ein Eintrag erstellt wird, welcher mit allen notwendigen Angeben befüllt wird. Das kann dazu führen, dass derselbe Autor je nach Werk auf verschiedene Arten aufgeführt wird. Bei BIBFRAME hingegen wird pro Autor ein Eintrag erstellt, welcher dann bei den zugehörigen Werken verlinkt werden kann.

### Dublin Core
Dublin Core ist im Gegensatz zu MARC21 ein Standard, welcher über die Bibliothekswelt hinaus genutzt wird.
-> ToDo: noch mehr beschreiben 

### Vergleich MARC21 und Dublin Core
siehe https://pad.gwdg.de/EC9WU7DITxiK1ciMll3ZOw#Erkenntnisse-Fragen

## Regelwerk vs. Datenformat
Nebst den Standards gibt es auch noch ergänzende Regelwerke. Darin wird definiert, wie eine Ressource beschrieben werden soll (theoretische Grundlage für Katalogisierung). Zu den Regelwerken gehören normalerweise normierte Vokabularien und inhaltliche Kategorien. Ein Beispiel für ein Regelwerk ist 'Resource Description and Access' kurz RDA.

Anders als Regelwerke dienen Datenformate der praktischen Repräsentation von Katalogisaten. Datenformate legen mit Hilfe von Datenstrukturen und Datentypen fest, wie Daten zu kodieren sind. MARC21 und BIBFRAME zählen zu den Datenformaten, wobei BIBFRAME auch Aspekte eines Regelwerks beinhaltet.

💡 Regelwerke und Datenformate sind nicht immer trennscharf und ergänzen sich gegenseitig. Bei einer Kombinatoin von beidem wird von einem Datenmodell gesprochen.


## Koha
Was ist Koha?
basiert auch auf MARC21
praktische Übung
gelernt: open source software gesundheit



[^1]: https://www.loc.gov/marc/bibliographic/bdintro.html
