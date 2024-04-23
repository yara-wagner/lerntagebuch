---
title: "Lerneinheit 5: Repository-Software für Publikationen und Forschungsdaten"
date: 2024-03-26
---

Der nachfolgende Blogpost enthält bezieht sich auf die Unterrichtseinheiten vom 26.03.2024 & 09.04.2024. In diesen vier Lektionen ging es um Repository-Software für Publikationen und Forschungsdaten (siehe auch [gemeinsames Dokument Teil 1](https://pad.gwdg.de/ycs5WlX8R_6aiNDebpvJoA) & [gemeinsames Dokument Teil 2](https://pad.gwdg.de/suv2C7XsSrWtf9O7VRFJXg)). In der Vorlesung haben wir uns zuerst mit Open Access und Open Data im Allgemeinen beschäftigt und anschliessend die Software DSpace näher kennengelernt. Zum Abschluss gab es dann noch einen Marktüberblick über Repository-Software.

In diesem Lerntagebuch möchte ich mich auf einen bestimmten Aspekt, der mich interessiert, fokussieren und zwar auf die Suchmaschinenoptimierung (SEO) im Kontext von DSpace.

## DSpace
[DSpace](https://dspace.lyrasis.org/about) ist eine Open Source Software für Publikationen und Forschungsdaten, die sich zum Ziel gesetzt hat Wissen offen zugänglich und einfach verwaltbar zu machen.

## SEO von DSpace Seiten
Mit Hilfe von Suchmaschinenoptimierung sollen Websiten und ihre Inhalte besser auffindbar gemacht werden.

Zu diesem Thema findet man in der DSpace Dokumentation einige Tipps spezifisch für den eigenen DSpace. Damit soll sichergestellt werden, dass der eigene DSpace von Suchmaschinen indexiert ist, da viele Besucher über Suchmaschinen zu Inhalten im Internet gelangen. DSpace verfügt über Tools, die dafür sorgen, dass die wichtigsten Suchmaschinen die Inhalte einfach und effektiv indizieren können. Für die meisten dieser Tools müssen jedoch gewisse Grundeinstellungen vorgenommen werden. Es soll sichergestellt werden, dass:

1. die DSpace-Software stets auf dem neusten Stand ist, damit auch die neusten Verbesserungen und Bug Fixes für die Indizierung zur Verfügung stehen.
2. der DSpace für Suchmaschinen überhaupt sichtbar ist.<br>
💡 Nicht indizierte Seiten können bei Suchmaschinen via URL hinzugefügt werden, sodass zukünftig indexiert sind.
3. der Proxy X-Forwarded-Headers an die Benutzeroberfläche weiterleitet.
4. die Benutzeroberfläche serverseitiges Rendering verwendet. Das ist standardmässig aktiviert.
5. die Sitemaps-Funktion aktiviert ist. Das ist bereits standardmässig so.
6. robots.txt-Datei soll Zugriff auf die Splash-Seiten und den Volltext zulassen.<br>
💡 Eine Splash-Seiten ist eine Art Pop-up oder Overlay, welches beim Aufruf einer Website angezeigt wird bevor die eigentliche Website angezeigt wird. [^1]
7. die Metadaten der Items korrekt in der HTML-Kopfzeile angezeigt werden.
8. die Umleitung von Dateidownloads auf Item-Landingpages vermieden wird.

Ausserdem wird darauf hingewiesen, dass OAI-PMH (Open Archives Initiative Protocol for Metadata Harvesting) für Suchmaschinen grundsätzlich nicht von Nutzen ist. [^2]

❓ Was ist der Unterschied zwischen 'indexiert' und 'indiziert' und wann wird welcher Begriff verwendet? Ich habe nicht wirklich eine Antwort darauf gefunden bzw. die Antworten widersprechen sich zum Teil oder sind schwammig formuliert oder es ist nicht ersichtlich, woher die Definition stammt:
- "Bei Suchmaschinen heißt es so: Bestehende Informationen, welche nur Sortiert werden (beispielsweise eine Liste von 100 Wörter nach Beliebtheit) wird indexiert. Werden dann nachträglich neue Einträge in die Liste aufgenommen, werden diese neuen Begriffe indiziert." [^3] -> Unklar, woher die Definition stammt und ob sie korrekt ist.
- Im wird der jeweils andere Begriff im Abschnitt 'Bedeutung' aufgeführt, nicht jedoch bei den Synonymen. [^4] -> Unklar, ob die Begriffe nun gleichbedeutend sind oder nicht
- Antwort von Microsoft Copilot: ![image](https://github.com/yara-wagner/lerntagebuch/assets/160014711/ae797dcd-b636-4f71-984f-a5c6162619cb)
-> Schwammige Antwort, aufgeführte Quellen geben auch nicht weiter Aufschluss (widersprüchliche Aussagen)


[^1]: Quelle: https://unbounce.com/website-optimization/what-is-a-splash-page
[^2]: Quelle: https://wiki.lyrasis.org/display/DSDOC7x/Search+Engine+Optimization
[^3]: https://www.lima-city.de/thread/indexierung-oder-indizierung#:~:text=Bestehende%20Informationen%2C%20welche%20nur%20Sortiert,werden%20diese%20neuen%20Begriffe%20indiziert.
[^4]: https://www.duden.de/rechtschreibung/indexieren und https://www.duden.de/rechtschreibung/indizieren
