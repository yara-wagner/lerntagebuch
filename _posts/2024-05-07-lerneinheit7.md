---
title: "Lerneinheit 7: Metadaten modellieren und Schnittstellen nutzen 2/2"
date: 2024-05-07
---

Der nachfolgende Blogpost enthält bezieht sich auf die Unterrichtseinheit vom 07.05.2024. In diesen vier Lektionen ging es um die Modellierung von Metadaten und die Nutzung von Schnittstellen (siehe auch [gemeinsames Dokumnet dieser Lerneinheit](https://pad.gwdg.de/vv-Q4RDnQ22Gqc-EEgbewA)). Nachdem wir uns in den vorherigen Lerneinheiten mit OpenRefine beschäftigt haben, widmet sich diese Lerneinheit nun den Schnittstellen im Allgemeinen sowie der Konvertierung zwischen Metadatenstandards. In dieser zentralen Lerneinheit fliessen folglich viele der zuvor gelernten Themen zusammen, wie auch im Schaubild des Moduls ersichtlich wird:
![image](https://github.com/yara-wagner/lerntagebuch/assets/160014711/2c392a8d-2d52-4863-81e7-651c716cfc8d)

## Schnittstellen
Schnittstellen dienen dem Austausch von Daten zwischen verschiedenen Systemen. Der Austausch findet mit Hilfe von Austauschprotokollen statt. Im Bibliotheks- und Archivbereich gibt es viele solcher Protokolle. Wir haben uns OAI-PMH (Open Archives Initiative Protocol for Metadata Harvesting) näher angeschaut. Dazu haben wir in Codespace mit einem vorbereiteten Repository Daten mit VuFindHarvest (Software) aus den in vorherigen Lerneinheiten angeschauten Systemen ([Koha](https://yara-wagner.github.io/lerntagebuch/2024/02/27/lerneinheit3.html), [ArchivesSpace](https://yara-wagner.github.io/lerntagebuch/2024/03/12/lerneinheit4.html) & [DSpace](https://yara-wagner.github.io/lerntagebuch/2024/03/26/lerneinheit5.html)) über deren angebotene Schnittstellen abgerufen. Die Daten aus Koha wurden im Format MARC21, die Daten aus ArchivesSpace in EAD und die Daten aus DSpace in OAI-DC abgerufen. Die auf den Systemen verfügbaren Metadatenformate können in den Systemen nachgeschaut werden (für URL siehe [gemeinsames Dokument](https://pad.gwdg.de/vv-Q4RDnQ22Gqc-EEgbewA))
<br><br>
💡 Metadata Harvesting = automatisierte Sammlung von Metadatenbeschreibungen aus verschiedenen Quellen, um nützliche Aggregationen von Metadaten und zugehörigen Diensten zu erstellen [^1]<br>
💡 VuFindHarvest = OAI Harvester von [VuFind](https://vufind.org/vufind) (= Discovery-System)<br>
💡 Je nach System sind die Daten bereits im gewünschten Format vorhanden (in unserem Fall MARC21) und können direkt in diesem Format anstatt im Ausgansformat heruntergeladen werden. Teilweise sind diese Angebote aber auch nicht vorhanden oder relativ schlecht. In diesen Fällen ist es sinnvoller, die Daten im Ausgangsformat abzufragen und dann noch selbst zu konvertieren.

## Konvertierung



[^1]: Quelle: https://guides.lib.utexas.edu/metadata-basics/harvesting
