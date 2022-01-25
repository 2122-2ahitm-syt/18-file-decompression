# File Decompression

Der Inhalt der Datei `zipped.txt` liegt in verpackter Form vor: "A5" steht für "AAAAA", "B3" für "BBB" etc.

## Task 1: Read File
Erstellen Sie das Modul `decompress.ts`. Lesen Sie darin in der Funktion `decompressFile()` die übergebene Datei `inputFile` ein und geben Sie den (verpackten) Inhalt auf der Konsole aus:

```javascript
function decompressFile(inputFile: string, outputFile: string): void {
	    
}
```

Exportieren Sie die Funktion und rufen Sie diese in `app.ts` mit dem Argument `"zipped.txt"` auf:

![img](./images/console1.png)

## Task 2: Decompress Data

Implementieren Sie im Modul `decompress.ts` die Funktion `decompressLine(line: string): string`.
  - Der Parameter `line` ist eine verpackte Zeile (z. B. `"A5"`).
  - Der Rückgabewert der Funktion ist die entpackte Zeile (z. B. `"AAAAA"`).

Verwenden Sie `decompressLine()` in der Funktion `decompressFile()` um den Dateiinhalt zeilenweise zu entpacken und anschließend auf der Konsole auszugeben.

![img](./images/console2.png)

## Task 3: Write File

Entwickeln Sie in `decompress.ts` die Funktion `writeLinesToFile(file: string, lines: string[])`.
  - Der Parameter `file` ist der Name der Datei, die erstellt werden soll.
  - Der Parameter `lines` ist ein String-Array, dessen Inhalt in die Datei geschrieben werden soll.

Rufen Sie `writeLinesToFile()` in `decompressFile()` mit dem übergebenen `outputFile` auf. Führen Sie anschließend das Programm aus und prüfen Sie ob die entpackte Datei erstellt wurde.

![img](./images/console3.png)

## Task 4: Handle Errors

Stellen Sie sicher, dass sowohl beim Lesen als auch beim Schreiben der Dateien im Fehlerfall eine Meldung ausgegeben wird. Ihre App darf keinesfalls abstürzen.

![img](./images/console4.png)
