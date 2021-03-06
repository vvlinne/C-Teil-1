# C++ Teil_1

Semesterarbeit des C++ Kurses (Teil 1) an der Universität zu Köln, von Viviane Linne (#5966540)
Link zum Github-Repository: https://github.com/vvlinne/CPlusPlus-Teil-1

Was, Wie , und Wieso?

Im Folgenden werde ich einen kurze Dokumentation meines Projektes darlegen, in der ich aufzeigen werde was ich gemacht habe (welche Funktionalitäten sind umgesetzt worden), wie ich das gemacht habe, und wieso ich es auf diese Art und Weise gemacht habe.

Das Programm erfüllt den Funktionsumfang der Stufe II. Man hat eine Menüführung, in der man eine XML- und TXT-Datei einlesen sowie konvertieren kann, als auch die Daten nach Klasseneigenschaften samt Suchbegriff durchsuchen kann. Diese wurden in den Menüpunkten (K)onvertieren und (S)uchen realisiert. Das Programm kann mit (E)xit beendet werden.

Die XML Datei (mit zugehöriger DTD) enthält Informationen zu ausgewählten Funko Pop Figuren, zum Zwecke eines Sammlungsarchivs zu privaten oder geschäftlichen Nutzen. Die Tags enthalten Informationen zu: Name, Herkunft, Größe, und Preis. Im Tag Figur, der die Informationen umschließt, ist eine ID enthalten die auch in der TXT widerzufinden ist und die Dateien verbindet. In der TXT ist nämlich der Lagerplatz sowie die Stückzahl der Figuren verzeichnet.

Kurze Zusammenfassung der Funktionalitäten:
Eine Klasse Base enthält die grundsätzlichen Funktionen zum Laden, Konvertieren und Durchsuchen der vom User angegebenen Dateien (XML und TXT). Eine Klasse Figure hält für ein Figure-Tag der XML-Datei alle notwendigen Informationen im Zwischenspeicher, weshalb die XML-und TXT-Datei nur beim Starten des Programms abgefragt werden. Ein Vektor wird in der Base.cpp zum Halten von allen gelesenen Figure-Objekten benutzt und kann durch Iteration später ausgelesen werden, wodurch Figure-Eigenschaften abgefragt und verglichen werden können. Ich habe mich grundlegend an dem Lehrmaterial aus der Vorlesung orientiert und dieses Grundwissen in diesem Programm angewandt. Es gibt sicherlich elegantere Lösung für solch ein Programm, die vermutlich allerdings erst mit erweitertem Kenntnisstand problemlos anzuwenden sind.
Weitere Kommentare innerhalb des Codes erklären die Funkitonen zusätzlich.

Probleme/Änderungen zwischendurch:
Da ich Token und Attribut Klassen aus den Vorlesungsfolien verwendet habe musste ich die XML Deklarationen sowie den DTD Verweis
in den von mir erstellten Dateien entfernen, da diese nicht sauber ausgegeben, wenn auch verarbeitet wurden. Diese liegen im Ordner Final Project. Diese sollten auch zur Überprüfung der Funktionen genutzt werden.
Weiterhin, sind in diesen Dateien keine weiteren Kommentare zu finden, da wir diese schon zu genüge in den Vorlesungen besprochen haben, kommentiert ist also eigentlich nur das, was ich selbst geschrieben habe.

Post Mortem:
Da ich die Semesterarbeit schnell und effektiv erledigen wollte (da ich nebenher schon mit meiner Bachelorarbeit angefangen habe), habe ich mich die vergangene Tage konstant mit der Programmierung beschäftigt und kontinuierlich dran gearbeitet. Daraus resultierend entstanden weniger Updates in diesem Repository.
