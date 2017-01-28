# Visitenkarte für Wetterstationen
Die digitale "Visitenkarte" für die Wetterstationen ist eine offene Schnittstelle, die es ermöglicht Informationen über Wetterstationen strukturiert zu beschreiben und weiterzugeben. Die Entwicklung fing zusammen mit der Erstellung der [Wetterstationen](http://wetterstationen.biz) - Liste an.

## Verwendung
Die Verwendung ist recht einfach:

- die Vorlage [template.xml](https://raw.githubusercontent.com/wetterstation/metadata/master/template.xml) herunterladen und lokal speichern
- die xml-Datei mit einem einfachen Texteditor öffnen
- Informationen, die man über die Wetterstation veröffentlichen will, in den entsprechenden Felder (wie in dieser Anleitung beschrieben) eintragen
- die geänderte Datei lokal speichern
- dann sie auf der eigenen Webspace hochladen. Dateiname und Speicherort auf dem Server kann frei festgelegt werden


## Format (Beispiel)
```xml
<station>
    <name>Erste Wetterstation aus Braunschweig</name>
    <description>Hier findet man eine kurze Beschreibung der Station (max. 350 Buchstaben)</description>
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
    <images>
        <banner>http://example.com/mybanner.jpg</banner>
        <symbol>http://example.com/symbol.png</symbol>
    </images>
    <links>
        <website>http://example.com</website>
        <rss>http://example.com/myfeed.rss</rss>
        <facebook>@Wetterstationen</facebook>
        <twitter>@Twitter</twitter>
    </links>
    <contact>
        <name>Max Mustermann</name>
        <email>example@example.com</email>
        <ref>http://www.example.com/info.html</ref>
    </contact>
</station>
```


## Felder der XML-Datei
* `name` Kurze Bezeichnung der Wetterstation
* `description` Kurze Beschreibung der Station (max. 300 Buchstaben)
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
* `images` Abschnitt mit Bilder für die an­der­wei­tig Station-Vorstellung. Durch diese Angabe, bestätigen Sie, dass der Urheberrechtsinhaber dieser Datei ein unbeschränktes Nutzungsrecht ohne jegliche Bedingungen für jedermann eingeräumt hat. Dieses Nutzungsrecht gilt unabhängig von Ort und Zeit und ist unwiderruflich. Das Nutzungsrecht wurde ausdrücklich oder – aufgrund einer noch weiter gehenden, im deutschen Sprachraum aber rechtlich nicht möglichen Übergabe in die „public domain“ oder der rechtlich ebenfalls nicht möglichen Deklarierung eigener Werke als „gemeinfrei“ – konkludent eingeräumt.
    * `banner` URL-Verweis auf Banner-Bild (468x60, jpg, png, gif, max: 30KB)
    * `symbol` URL-Verweis auf Symbol-Bild (64x64, jpg, png, gif)
* `links` Abschnitt mit Angaben über die Internetpräsenz der Wetterstation
    * `website` Website-URL der Wetterstation
    * `rss` URL des RSS-Feeds
    * `facebook` Username oder Fan-Seite-ID (z.B. 338845646476760)
    * `twitter` Twitter-Username
* `contact` Abschnitt mit Angaben zum Betreiber der Wetterstation
    * `name` Name und/oder Vorname der Kontaktperson bei Fragen oder Problemen
    * `email` Emailadresse für die Kontaktaufnahme
    * `ref` alternative URL mit Formular oder Zusatzinformationen zwecks Kontaktaufnahme

## Informationen
Das Format der Wetterstation-"Visitenkarte" wird laufend erweitert, für mehr Informationen besuchen Sie immer wieder diese Projektseite. Dieses Projekt ist Open Source, Lizenz CC BY-SA 4.0 https://creativecommons.org/licenses/by-sa/4.0/deed.de

