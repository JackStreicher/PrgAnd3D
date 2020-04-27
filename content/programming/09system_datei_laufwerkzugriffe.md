---
title: "09. System-, Datei- und Laufwerkzugriffe"
description: "Eine Einführung in OOP"
date: '05.03.2020'
screenshot: 'Skyrim_Hidden_Peak_Barrow'
layout: 'portfolio'
featured: true
categories: [ "C#", "Programming" ]
tags: ["C#", "OOP"]


---

## 01 Klassen für den Dateizugriff
Im Folgenden eine Liste der Klassen für den Dateizugriff
- System.IO.FileInfo
- System.IO.DirectoryInfo
- System.IO.DriveInfo
- System.IO.Directory
- System.IO.File

Diese können als Objekt intanziiert werden, damit man Zugriff auf deren Member und Methoden erhält.
Über DriveInfo erhält man z.B. Zugriff auf *Directory*, *GetFiles* und *RootDirectory*.



## 02 Mit Laufwerken, Ordnern und Dateien arbeiten
Hier einige Code Beispiele, mit denen man allgemeine Informationen des Laufwerks ausgeben kann.


![KomplexeDatentypen](../09_MitLaufwerkenUndDateienArbeiten.PNG "Drive Infos & Change Path")  


Im folgenden Beispiel versuchen wir den Pfad einer Datei zu verändert und Dateien zu löschen (mit Exception Handling!).


![KomplexeDatentypen](../09_MitLaufwerkenUndDateienArbeiten2.PNG "Deletions")  


War gar nicht mal so schwer, oder?
![KomplexeDatentypen](../easyAsThat.gif "https://media.giphy.com/media/3o7btNa0RUYa5E7iiQ/giphy.gif")  

## 03 Mit Textdatei arbeiten
In den folgenen Beispielen wird gezeigt, wie man strings in eine Txt-Datei schreibt. Die benötigte Datei wird hierbei von selbst angelegt, sollte Sie noch nicht exisitieren.
Zunächst schreiben wir ein Array aus strings in eine .txt Datei.
![KomplexeDatentypen](../WriteToTxt.PNG "Write an Array of Strings")

Anschließend schreiben wir eine string Variable in eine .txt (wer bis hierhin glaubte, es würde kein Witcher Beispiel verwendet werden lag falsch!).
![KomplexeDatentypen](../WriteToTxt2.PNG "Write a string")

Wir können auch einzelne strings eines string Arrays ausschließen
![KomplexeDatentypen](../WriteToTxt3.PNG "Write an Array of Strings with exlusions")

Abschließend wird gezeigt, wie man einen string zu einer bereits bestehenden Txt-Datei hinzufügt.
![KomplexeDatentypen](../WriteToTxt4.PNG "add a strng to an exisiting .txt")


Abschließend wollen wir den Inhalt einer .txt auslesen und zur prüfung in der Console ausgeben.
![KomplexeDatentypen](../ReadTxtFile.PNG "Read the txt file")

Als nächstes wird der Inhalt einer .txt in ein string array eingelesen.
![KomplexeDatentypen](../ReadTxtFile2.PNG "Read the txt file")

Zu guter letzt geben wir den inhalt des zweiten Txt-Files Zeilenweise aus:
![KomplexeDatentypen](../ReadTxtFile3.PNG "Read the txt file")



Das war unerwartet...
![KomplexeDatentypen](../batmanEating.gif "https://coubsecure-s.akamaihd.net/get/b107/p/coub/simple/cw_image/cc641dc6970/9b09e962cb4f34804c885/med_1540544315_00032.jpg")

...einfach!

#### **Quellen und weiterführende Links**
```
01  https://docs.microsoft.com/de-de/dotnet/csharp/programming-guide/file-system/how-to-get-information-about-files-folders-and-drives

02 https://docs.microsoft.com/de-de/dotnet/csharp/programming-guide/file-system/how-to-copy-delete-and-move-files-and-folders

03 https://docs.microsoft.com/de-de/dotnet/csharp/programming-guide/file-system/how-to-write-to-a-text-file
https://docs.microsoft.com/de-de/dotnet/csharp/programming-guide/file-system/how-to-read-from-a-text-file
https://docs.microsoft.com/en-gb/dotnet/csharp/programming-guide/file-system/how-to-read-a-text-file-one-line-at-a-time
