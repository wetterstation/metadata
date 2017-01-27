# Visitenkarte für Wetterstationen
Die digitale "Visitenkarte" für die Wetterstationen ist eine offene Schnittstelle, die es ermöglicht Informationen über Wetterstationen strukturiert zu beschreiben und weiterzugeben. Die Entwicklung fing zusammen mit der Erstellung der [Wetterstationen - Liste](http://wetterstationen.biz) an.

## Verwendung
Die Verwendung ist recht einfach:

- die Vorlage (template.xml) herunterladen
- die xml-Datei mit einem einfachen Texteditor öffnen
- Informationen, die man über die Wetterstation veröffentlichen will, in den entsprechenden Felder (wie in dieser Anleitung beschrieben) eintragen
- die geänderte Datei lokal speichern
- dann sie auf der eigenen Webspace hochladen. Dateiname und Speicherort auf dem Server kann frei festgelegt werden


## Format
```xml
<station>
    <name>Erste Wetterstation aus Braunschweig</name>
    <position>
        <lat>52.269167</lat>
        <lng>10.521111</lng>
        <alt>75</alt>
    </position>
    <location>
        <country>Deutschland</country>
        <region>Niedersachsen</region>
        <place>Braunschweig</place>
        <zipcode>38104</zipcode>
        <area>Tierparknähe, direkt an der Straßenkreuzung</area>
    </location>
    <contact>
        <name>Max Mustermann</name>
        <email>example@example.com</email>
        <ref>http://www.example.com/info.html</ref>
    </contact>
</station>
```


## Felder der XML-Datei
* `name` Kurze Bezeichnung der Wetterstation
* `position` Abschnitt mit Angaben zum Standort der Wetterstation
    * `lat` die geographische Breite der Wetterstation in Dezimalgrad angegeben (z.B. hat Braunschweig die Latitude 52.269167°)
    * `lng` die geographische Länge der Wetterstation in Dezimalgrad angegeben (z.B. hat Braunschweig die Longitude 10.521111°)
    * `alt` die Höhe der Wetterstation über dem Meeresspiegel in Meter (z.B. hat die Braunschweig etwa 70 Meter Höhe üNN)
* `location` Abschnitt mit Angaben zum Standort der Wetterstation in einem für Menschen lesbaren Format
    * `country` Land
    * `region` Bundesland
    * `place` Ortsname, wo sich die Wetterstation befindet
    * `zipcode` Postleitzahl
    * `area` detaillierte Informationen zum Standort
* `contact` Abschnitt mit Angaben zum Betreiber der Wetterstation
    * `name` Name und/oder Vorname der Kontaktperson bei Fragen oder Problemen
    * `email` Emailadresse für die Kontaktaufnahme
    * `ref` alternative URL mit Formular oder Zusatzinformationen zwecks Kontaktaufnahme


## Informationen
Das Format der Wetterstation-"Visitenkarte" wird laufend erweitert, für mehr Informationen besuchen Sie immer wieder diese Projektseite. Dieses Projekt ist Open Source, Lizenz CC BY-SA 4.0 https://creativecommons.org/licenses/by-sa/4.0/deed.de

