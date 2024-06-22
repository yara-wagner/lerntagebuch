---
title: "Lerneinheit 6: Metadaten modellieren und Schnittstellen nutzen 1/2"
date: 2024-04-30
---

Der nachfolgende Blogpost bezieht sich auf die Unterrichtseinheiten vom 23.04.2024 und 30.04.2024. In diesen vier Lektionen ging es um die Modellierung von Metadaten (siehe auch [gemeinsames Dokument Teil 1](https://pad.gwdg.de/NY1-soGUSsim-sttsoHNXw) und [gemeinsames Dokument Teil 2](https://pad.gwdg.de/GDKAQMKwT3u-VP6hZ6NtOA)). Das Thema wurde am Beispiel von OpenRefine angeschaut. Nach dem Theorieinput zu OpenRefine haben wir uns die Software auch noch praktisch angeschaut und kleinere Übungen gemacht.

## OpenRefine
[OpenRefine](https://openrefine.org/) ist eine Open Source Software, welche dabei hilft Rohdaten aufzubereiten und zu bereinigen. Genauer gesagt wird die Software für die Analyse, die Bereinigung, die Konvertierung und die Anreicherung von Daten eingesetzt.

⚠️ Falls ich mal im Arbeitsalltag mit OpenRefine in Berührung kommen sollte, kann ich mein Wissen über die Software mit Hilfe einer [Library Carpentry Lesson zu OpenRefine](https://librarycarpentry.org/lc-open-refine/) wieder auffrischen. Ausserdem bietet OpenRefine selbst eine ausführliche Dokumentation: [OpenRefine User Manual](https://openrefine.org/docs).

💭 Sidenote: Als Logo für die Software wurde das Bild eines Diamanten gewählt, da bei diesem bzw. bei dessen Ausgangszustand, gleich wie bei Daten auch, erst eine Aufbereitung und Reinigung notwendig ist, um zum vollen Wert zu gelangen.

### Hauptfunktionen
Die Hauptfunktionen von OpenRefine sind laut ihrer Website folgende:
* Faceting → hilft dabei Muster und Trends in den Daten zu erkennen und die Daten besser untersuchen zu können
* Clustering → schneller und einfacher Weg Inkonsistenzen zu finden und zu beheben
* Reconciliation → halbautomatisierte Reconciliation mit einem externen Datensatz via Reconciliation Service API
* Infinite undo/redo → Änderungsverlauf der Daten über das gesamte Projekt hinweg, welcher es ermöglicht auf einen beliebigen Stand zuzugreifen
* Privacy → mit OpenRefine transformierte Daten werden lokal gespeichert und nicht auf einem Server
* Wikibase → Integration, die es ermöglicht Daten der Wikibase zu beziehen und ihr Daten hinzuzufügen

### Unterstütze Formate
Am einfachsten ist die Nutzung von OpenRefine mit tabelleraische Daten (z. B. CSV, XLS oder auch TXT mit Trennzeichen oder festen Spaltenbreiten). Etwas schwieriger wird es bereits mit flachen XML (wie z. B. MARCXML) oder JSON, doch auch das gelingt mit ein wenig Übung gut. Richtig schwierig wird es erst bei komplexen XML-Daten mit Hierarchien (wie z. B. EAD). Für solche Daten sind zusätzliche Tools notwendig.

## Übungen zu OpenRefine
Wie bereits bei vorherigen Übungen stand uns auch hierfür wieder ein Codespace zur Verfügung, über welchen wir auf eine Testversion von OpenRefine zugreifen konnten. <br>
In der ersten Unterrichtseinheit haben wir Beispieldaten in OpenRefine importiert, mit welchen wir danach selbstständig Basisfunktionen (Faceting, Zellen-Split, Clustering, Zellen-Join) ausprobiert haben. <br>
In der zweiten Unterrichtseinheit haben wir eine weitere Basisfunktion, die Reconciliation, angeschaut aber jedoch nicht selbst ausprobiert. Stattdessen haben wir noch eine Übung zur Konvertierung von CSV nach MARCXML gemacht. Dazu haben wir die Funktion "Templating Exporter" genutzt. Mit dieser Funktion kann das Template, anhand dessen die Konvertierung gemacht wird, direkt bearbeitet werden. So kann beispielsweise selbst gewählt werden, welches Trennzeichen verwendet werden soll. Die Möglichkeit, das Template direkt bearbeiten zu können, kann beispielsweise nützlich sein, wenn ein Format gewünscht ist, welches (noch) nicht von OpenRefine unterstützt wird.

![image](https://github.com/yara-wagner/lerntagebuch/assets/160014711/7c8ffb24-1037-4a27-98be-6c8a8626985d)
<br>(Bildquelle: [OpenRefine](https://openrefine.org/docs/manual/exporting#templating-exporter))
