---
title: "Lerneinheit 4: Funktion und Aufbau von Archivsystemen"
date: 2024-03-12
---

Der nachfolgende Blogpost enthält beinhaltet die Unterrichtseinheiten vom 05.03.2024 und vom 12.03.2024. In diesen sechs Lektionen ging es um die Funktion und den Aufbau von Archivsystemen (siehe auch [gemeinsames Dokument Teil 1](https://pad.gwdg.de/FrI1nt2NSvuNOAyu_yk64A) und [gemeinsames Dokument Teil 2](https://pad.gwdg.de/JmDfo4JOSQuF12mGPmm7IA)). Dazu wurde erst ein kurzer Blick auf die Metadatenstandards ISAD(G) und EAD. Anschliessend haben wir uns ausführlicher mit der Software ArchivesSpace beschäftigt.

## Metadatenstandards in Archiven
Der Metadatenstandard [ISAD(G) (International Standard Archival Description (General))](https://de.wikipedia.org/wiki/ISAD(G)) wurde bereits in einem anderen Modul thematisiert. Da ich jedoch ausser den Pflichtmodulen im Studium ansonsten keine Berührungspunkte mit dem Archivwesen habe, ist bei mir dazu nicht viel hängengeblieben. ISAD(G) bildet den Entstehungszusammenhang mit einer mehrstufigen Verzeichnung im Provenienzprinzip ab. Besonders wichtig sind die Angaben 'Signatur', 'Titel', 'Provenienz', 'Entstehungszeitraum', 'Umfang' und 'Verzeichnungsstufe', weshalb es sich dabei auch um Pflichtfelder handelt. Nachteile von ISAD(G) sind die nicht enthaltenen Vorgaben zur Digitalisierung oder zur digitalen Langzeitarchivierung, die monodimensionale Tektonik sowie dass einzelne Datensätze teilweise nur im Kontext verständlich sind. Ein neuerer Standard namens [RIC (Records in Context)](https://de.wikipedia.org/wiki/Records_in_Contexts) bietet in dieser Hinsicht mehr: Er basiert auf Linked-Data-Prinzipien und soll polydimensionale Beziehungen ermöglichen. Der Standard befindet sich jedoch aktuell noch in Entwicklung. Klar ist jedoch jetzt schon, dass der Umstieg von ISAD(G) auf RIC mit grossem Aufwand verbunden ist.

Bei [EAD (Encoded Archival Description](https://de.wikipedia.org/wiki/Encoded_Archival_Description) handelt es sich um einen XML-Standard, welcher für die Beschreibung von archivischen Findmitteln genutzt wird. Der Standard ist relativ offen, weshalb teilweise noch genauer spezifiziert wird, welche Werte zugelassen sind. Dadurch, dass der Standard XML-basiert ist, ist er gut maschinenlesbar, was für die digitale Verarbeitung von Vorteil ist. <br>⚠️ Mehr zu EAD werden wir in späteren Lerneinheiten erfahren, denn dort werden wir praktisch mit EAD-Dateien arbeiten.

## ArchivesSpace
[ArchivesSpace](https://archivesspace.org) ist eine Open-Source-Software für Archivinformationssysteme. Genau genommen ist ArchivesSpace nicht vollständig Open-Source, denn beispielsweise das Benutzerhandbuch ist nur für zahlende Mitglieder zugänglich. 

...
- Demo-Umgebung: selbst ausprobiert, Übung
- basierend auf ... / unterstützt Import/Export in ...
- begrifflichkeiten (accession, resource, archival object)
- unterschiede zwischen bibliotheks- und archivsystemen
