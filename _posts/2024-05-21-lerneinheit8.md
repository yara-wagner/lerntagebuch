---
title: "Lerneinheit 8: Suchmaschinen und Discovery-Systeme 1/2"
date: 2024-05-21
---

Der nachfolgende Blogpost bezieht sich auf die Unterrichtseinheit vom 21.05.2024. In diesen vier Lektionen ging es um Suchmaschinen und Discovery-Systeme (siehe auch [gemeinsames Dokument dieser Lerneinheit](https://pad.gwdg.de/HW9D520ORJu79RoIEueNCw)). Zu diesem Zweck haben wir uns VuFind näher angeschaut und ausprobiert. Zu Beginn der Unterrichtseinheit wurde uns gezeigt, wie VuFind installiert und konfiguriert werden kann. Anschliessend haben wir Testdaten im MARC21-Format in das System geladen, damit wir die Software ausprobieren konnten.

## Discovery-Systeme
Ein Discovery-System bezeichnet ein auf Suchmaschinentechnologie basierendes bibliothekarisches Suchsystem. Sie dienen als moderne Alternative zum klassischen Online-Katalog. Während eine Suche in klassischen Bibliothekskataloge möglichst genaue Ergebnisse ergibt, liefern Discovery-Systeme viele Suchergebnisse, welche mit Hilfe eines Algorithmus nach Relevanz sortiert werden (wie bei Suchmaschinen)[^1]. Ein Beispiel für ein soches Discovery-System ist Solr.<br>
💭 Der Begriff Discovery-System ist kein offizieller IT-Begriff, hat sich in der Bibliothekswelt jedoch durchgesetzt. 

## Apache Solr
[Solr](https://solr.apache.org/) ist eine weit verbreitete Volltextsuche, die im Hintergrund verschiedener Software läuft. Bei der Suche handelt es sich um eine lexikalische Suche, d. h. es wir nicht ein reiner Zeichenabgleich für exakte Resultate gemacht wie das beispielsweise bei Datenbanken der Fall ist, sondern Wörter werden auf ihre Grundform zurückgesetzt, damit auch Varianten der Wörter und somit auch mehr Ergebnisse gefunden werden.<br>
Es existiert zwar eine Demo-Umgebung mit Frontend, grundsätzlich liefert Solr jedoch nur das Backend, um das Frontend muss man sich selber kümmern. Ein berühmtes Beispiel, welches Apache Solr für die Suche verwendet, ist Netflix.

Mehr zu Solr im [Apache Solr Reference Guide](https://solr.apache.org/guide/8_7/solr-tutorial.html)

## VuFind
[VuFind](https://vufind.org/vufind/) ist ein Open-Source Discovery-System, welches in PHP geschrieben wurde und Apache Solr für die Suche verwendet. VuFind erhält dabei die Resultate einer Suche von Solr im JSON-Format und stellt sie nutzerfreundlich dar.

## Vergleich Apache Solr und VuFind
In der Übung während der Vorlesung haben wir die Demo-Benutzeroberflächen von Solr und VuFind verglichen, um herauszufinden, was bereits von Solr gemacht wird und was VuFind noch zusätzlich bietet. Die Demo-Benutzeroberfläche von Solr entspricht dabei einer relativ technisch gestalteten Admin-Oberfläche (mit technischer Syntax) wohingegen VuFind eine benutzerfreundliche(re) Oberfläche (mit natürlicher Sprache) für Endnutzende bietet.<br>
Im nachfolgenden Screenshot sieht man die Oberflächen der beiden Demosysteme (links Solr, rechts VuFind):<br>
![image](https://github.com/yara-wagner/lerntagebuch/assets/160014711/e6d5a8b4-6ff6-4709-8a26-4a75c76be4e0)
<br>
Beim Vergleich fiel auf, dass VuFind zusätzlich zur Suche noch einige weitere nützliche Funktionen bietet, wie beispielsweise 'Zitieren' oder verschiedene Arten den Datensatz zu teilen/exportieren. Auch wird bei VuFind vieles verlinkt (z. B. ähnliche Einträge), wodurch man schnell zu weiteren Inhalten gelangen kann. VuFind zeigt ausserdem bereits während der Eingabe eines Suchstrings Vorschläge an, was bedeutet, dass bereits dort erste Abfragen gemacht werden. Hinter einer Suchanfrage in der VuFind-Oberfläche stekcken folglich mehr Abfragen als für Nutzende direkt sichtbar ist.<br>
Alle Erkenntnisse des Vergleichs sind im [gemeinsamen Dokument der Lerneinheit](https://pad.gwdg.de/HW9D520ORJu79RoIEueNCw#%C3%9Cbung-Suche-in-VuFind-vs-Suche-in-Solr) aufgeführt.

<hr>


[^1]: Quelle: [https://felixlohmeier.gitbooks.io/seminar-wir-bauen-uns-einen-bibliothekskatalog/content/01_1_opac_vs_discovery-system.html](https://felixlohmeier.gitbooks.io/seminar-wir-bauen-uns-einen-bibliothekskatalog/content/01_1_opac_vs_discovery-system.html)
