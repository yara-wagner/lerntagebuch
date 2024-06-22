---
title: "Lerneinheit 9: Suchmaschinen und Discovery-Systeme 2/2"
date: 2024-06-03
---

Der nachfolgende Blogpost bezieht sich auf die Unterrichtseinheit am Morgen vom 03.06.2024. In diesen vier Lektionen ging es wie bereits in der [vorherigen Lerneinheit](https://yara-wagner.github.io/lerntagebuch/2024/05/21/lerneinheit8.html) um Suchmaschinen und Discovery-Systeme (siehe auch [gemeinsames Dokument dieser Lerneinheit](https://pad.gwdg.de/5jn060c8RDC6WukTIuP5RQ)). Auch in dieser Unterrichtseinheit haben wir uns wieder mit VuFind beschäftigt. Zum Abschluss haben wir uns noch das Suchportal der HAAB angeschaut und einen Marktüberblick über Discovery-Systeme erhalten.

## Datenimport in VuFind
In einer ersten Gruppenübung haben wir die in vorherigen Unterrichtseinheiten exportierten und konvertierten Daten aus Koha, ArchivesSpace, DSpace und DOAJ in das System VuFind importiert. Dazu stand jeder Gruppe ein eigener Server zur Verfügung. Das Ganze haben wir via SSH-Zugriff gemacht.<br>
💭 Da ich auch bei der Arbeit ab und zu mit SSH in Berührung komme, war das für mich kein Problem.

Der Import der Daten aus Koha und OpenRefine hat problemlos geklappt. Der Import aus DSpace und ArchivesSpace war zuerst nicht erfolgreich, da bei diesen Daten ein Feld gefehlt hat, welches für den Import als ID verwendet wurde. Zu diesem Problem kam es, da das Marc21-Feld '001', bei welchem es sich nicht um ein obligatorisches Feld von Marc21 handelt, als ID verwendet wurde. Welches Feld als ID verwendet wird, kann im File marc.properties konfiguriert werden (siehe Screenshot). In diesem File können auch noch andere Anpassungen für den Import vorgenommen werden, wie beispielsweise die Änderung des Names der Institution, unter welcher die Daten importiert werden sollen.<br>
![image](https://github.com/yara-wagner/lerntagebuch/assets/160014711/60f69dad-eb12-403d-9843-07835ab9a881)<br>
Um das Import-Problem der DSpace- und ArchivesSpace-Daten zu lösen gibt es zwei verschiedene Möglichkeiten: Entweder kann die ID bei den Daten ergänzt werden oder es wird in der Konfiguration ein anderes Feld festgelegt, welches als ID verwendet werden soll.<br>
💡 Die manuelle Anpassung der Import-Datei ist jedoch sehr fehleranfällig und sollte deshalb möglichst vermieden werden.

## VuFind Konfiguration
In einer zweiten Gruppenübung haben wir Konfigurationsanpassungen zur Änderung der Benutzeroberfläche von VuFind vorgenommen. Bei VuFind existiert ein globales und ein lokales Konfigurationsverzeichnis. Die Konfigurationen aus dem lokalen Verzeichnis haben mehr Gewicht als die Konfigurationen aus dem globalen Verzeichnis.<br>
Hilfestellungen zur Konfiguration von VuFind fanden wir auf folgenden zwei Seiten:
- [VuFind Tutorial: Allgemeine Einstellungen](https://vufind.felixlohmeier.de/#/06_Konfiguration_Allgemein)
- [VuFind Tutorial: Konfiguration der Facetten](https://vufind.felixlohmeier.de/#/08_Konfiguration_Facetten)

⚠️ Weitere Information sowie auch Video-Tutorials zu VuFind sind in der [VuFind Dokumentation](https://vufind.org/wiki/) auffindbar.


Während der Übung haben wir folgendes angepasst (siehe auch nachfolgende Screenshots):
- Sidebar links anstatt rechts anzeigen lassen
- Gesamtdesign (Theme) ändern
- Tab-Titel und Seperator ändern

![image](https://github.com/yara-wagner/lerntagebuch/assets/160014711/a0a345f9-23c3-4daf-9625-981036d6aadc)
![image](https://github.com/yara-wagner/lerntagebuch/assets/160014711/7263980f-7f22-4fc2-aee0-6171ad2bdacf)

## Marktüberblick Discovery-Systeme
Die Funktionalität eines Discovery-Systems besteht aus mindestens zwei Komponenten: Der Software und den Daten. Ein gutes Discovery-System ist nicht nur im Discovery-Teil (Finden), sondern auch im Delivery-Teil (an Texte rankommen) gut.

Ein jährlicher Report über Library Systems von Marshall Breeding (Bsp.: [Library Systems Report von 2020](https://americanlibrariesmagazine.org/2020/05/01/2020-library-systems-report/)) liefert einen guten Überblick über die kommerziellen, internationalen Systeme. Auch interessant ist die Grafik von [librarytechnology.org](https://librarytechnology.org/mergers/), welche die Geschichte der Fusionen und Übernahmen in der internationalen Bibliothekstechnologiebranche aufzeigt.

In den wissenschaftlichen Bibliotheken in der Schweiz kommt durch die [SLSP (Swiss Library Service Platform)](https://slsp.ch/) Ex Libris Alma und das zugehörige Discovery-System Primo VE zum Einsatz.
