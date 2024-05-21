---
title: "Lerneinheit 4: Funktion & Aufbau von Archivsystemen"
date: 2024-03-12
---

Der nachfolgende Blogpost bezieht sich auf die Unterrichtseinheiten vom 05.03.2024 & 12.03.2024. In diesen sechs Lektionen ging es um die Funktion & den Aufbau von Archivsystemen (siehe auch [gemeinsames Dokument Teil 1](https://pad.gwdg.de/FrI1nt2NSvuNOAyu_yk64A) & [gemeinsames Dokument Teil 2](https://pad.gwdg.de/JmDfo4JOSQuF12mGPmm7IA)). Dazu wurde erst ein kurzer Blick auf die Metadatenstandards ISAD(G) & EAD geworfen. Anschliessend haben wir uns ausführlicher mit der Software ArchivesSpace beschäftigt.

## Metadatenstandards in Archiven
Der Metadatenstandard [ISAD(G) (International Standard Archival Description (General))](https://de.wikipedia.org/wiki/ISAD(G)) wurde bereits in einem anderen Modul thematisiert. Da ich jedoch ausser den Pflichtmodulen im Studium ansonsten keine Berührungspunkte mit dem Archivwesen habe, ist bei mir dazu nicht viel hängengeblieben. ISAD(G) bildet den Entstehungszusammenhang mit einer mehrstufigen Verzeichnung im Provenienzprinzip ab. Besonders wichtig sind die Angaben 'Signatur', 'Titel', 'Provenienz', 'Entstehungszeitraum', 'Umfang' & 'Verzeichnungsstufe', weshalb es sich dabei auch um Pflichtfelder handelt. Nachteile von ISAD(G) sind die nicht enthaltenen Vorgaben zur Digitalisierung oder zur digitalen Langzeitarchivierung, die monodimensionale Tektonik sowie dass einzelne Datensätze teilweise nur im Kontext verständlich sind. Ein neuerer Standard namens [RIC (Records in Context)](https://de.wikipedia.org/wiki/Records_in_Contexts) bietet in dieser Hinsicht mehr: Er basiert auf Linked-Data-Prinzipien & soll polydimensionale Beziehungen ermöglichen. Der Standard befindet sich jedoch aktuell noch in Entwicklung. Klar ist jedoch jetzt schon, dass der Umstieg von ISAD(G) auf RIC mit grossem Aufwand verbunden ist.

Bei [EAD (Encoded Archival Description](https://de.wikipedia.org/wiki/Encoded_Archival_Description) handelt es sich um einen XML-Standard, welcher für die Beschreibung von archivischen Findmitteln genutzt wird. Der Standard ist relativ offen, weshalb teilweise noch genauer spezifiziert wird, welche Werte zugelassen sind. Dadurch, dass der Standard XML-basiert ist, ist er gut maschinenlesbar, was für die digitale Verarbeitung von Vorteil ist. <br>⚠️ Mehr zu EAD werden wir in späteren Lerneinheiten erfahren, denn dort werden wir praktisch mit EAD-Dateien arbeiten.

## ArchivesSpace
[ArchivesSpace](https://archivesspace.org) ist eine Open-Source-Software für Archivinformationssysteme mit einer grossen Community in den USA. Genau genommen ist ArchivesSpace nicht vollständig Open-Source, denn beispielsweise das Benutzerhandbuch ist nur für zahlende Mitglieder zugänglich, was als Anreiz für die Mitgliedschaft dient.

Um das System kennenzulernen haben wir nach einer kurzen Einführung noch eine Gruppenübung gemacht. Dafür sollten wir auf einem Demosystem einen eigenen Datensatz erstelle & diesen in der öffentlichen Ansicht sichtbar machen. Für die Erstellung des Datensatzes mussten verschiedene Pflichtfelder wie z. B. 'Title', 'Identifier' oder 'Level of Description' ausgefüllt werden. Zusätzlich konnten jedoch auch noch viele weitere, nicht obligatorische Angaben gemacht werden. In unserer Gruppe arbeitete zwar niemand im Archivwesen, die Aufgabe konnten wir jedoch trotzdem gut lösen.

Eine Alternative zu ArchivesSpace ist [Access to Memory (AtoM)](https://www.accesstomemory.org/de). Genaueres zu AtoM kann auch auf der Website von [docuteam](https://www.docuteam.ch/atom-access-to-memory) nachgelesen werden. Der Schweizer Markt wird jedoch von den Produkten [scopeArchiv](https://www.scope.ch/de/produkteuebersicht/scopearchiv) & [CMI AIS](https://cmiag.ch/akten-management/archivierung/ais) dominiert.

## Unterschiede zwischen Bibliotheks- & Archivsystemen
Nach dem Einblick in Bibliothekssyseme in [Lerneinheit 3](https://yara-wagner.github.io/lerntagebuch/2024/02/27/lerneinheit3.html) folgte nun mit dieser Lerneinheit ein Einblick in Archivsysteme.<br>💡 Dabei konnten folgende Hauptunterschiede erkannt werden:
- In Bibliotheken wird medienzentriert gearbeitet, wohingegen man sich in Archiven an analogen Findmitteln orientiert. Das ist auch in der jeweiligen Software sichtbar.
- In Bibliotheken spielt die Benutzerinteraktion (Ausleihe) eine zentrale Rolle. Das ist in Archiven nicht der Fall, da dort der Bestand im Gegensatz zum Bibliotheksbestand eher stehend & unikal ist, weshalb die Nutzung meist nur auf Anfrage möglich ist.
- Aufgrund der unterschiedlichen Ansprüche unterscheidet sich auch das gängige Metadatenformat:
  - Bibliothek: MARC21 (zukünftig BIBFRAME)
  - Archiv: EAD (zukünftig RiC)
