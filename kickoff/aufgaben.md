## Aufgaben zum Kickoff-Workshop
Node.js bietet hat das Modul _fs_ integriert, welches den Zugriff auf Dateien ermöglicht.

```javascript
var fs = require('fs');
```

Die Funktion `fs.readFile(__dirname+"/dateiname", function(err, data) { ... });` ermöglicht das auslesen von Dateien.

Die Variable `__dirname` enthält den Namen des Verzeichnisses, in dem das aktuelle Programm liegt. Der Parameter `data` ist normalerweise eine Buffer mit Binärdaten, der mittels `.toString()` in einen String umgewandelt werden kann.

Die Funktion `fs.writeFile(__dirname+"dateiname", data, function(err) { ... });` ermöglicht das schreiben von Dateien.

Mittels `JSON.stringify( ... )` und `JSON.parse( ... )` können Objekte in einen JSON-String umgewandelt werden und umgekehrt.

### Aufgabe 1
Schreiben sie ein Programm in Node.js, das die Datei [wolkenkratzer.json] ausliest und die Liste der Wolkenkratzer in folgender Form auf der Konsole ausgibt:

```
Name: Burj Khalifa
Stadt: Dubai
Höhe: 828m
--------------------
Name: Shanghai Tower
Stadt: Shanghai
Höhe: 632m
--------------------
...
```

### Aufgabe 2
Erweitern sie das Programm aus Aufgabe 2 so, dass die Namen, Städte und Höhenangaben jeweils **farbig** ausgegeben werden. Hierzu können sie das Modul ```chalk``` verwenden, welches auch im Workshop vorgestellt wurde. Erstellen zu ihrem Programm auch eine ```package.json```-Datei, welche unter anderem die Modulabhängigkeiten definiert.

### Aufgabe 3
Erweitern sie das Programm aus Aufgabe 2 so, dass es die Wolkenkratzer der Höhe nach sortiert, die sortierte Liste in der neuen Datei `wolkenkratzer_sortiert.json` speichert und sie erst danach auf der Konsole ausgibt.

**Aus ihrer Git-Historie sollte hervorgehen, dass die Aufgaben in der hier vorgegebenen Reihenfolge gelöst wurden.**
