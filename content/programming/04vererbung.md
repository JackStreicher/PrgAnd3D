---
title: "04. Vererbung"
description: "Eine Einführung in OOP"
date: '05.03.2020'
screenshot: 'Skyrim_Hidden_Peak_Barrow'
layout: 'portfolio'
featured: true
categories: [ "C#", "Programming" ]
tags: ["C#", "OOP"]


---

![Inheritance](../inheritance.gif "https://media0.giphy.com/media/fTzgTmNrXWOY6ERKDU/giphy.gif")
## 01 Grundlagen der Vererbung
Für die OOP ist Vererbung ein sehr wichtiges Konzept. Die Vererbung ermöglicht es, dass child Klassen von parent Klassen Methoden und Eigenschaften erben und erweitern können.  
Auf Member mit dem Schlüsselwort **protected** können anderen Klassen nicht zugreifen, child Klassen jedoch haben Zugriff, insofern diese **protected** Member der parent Klasse angehören.  
Auf **private** Member können von child Klassen, die in der parent Klasse eingebettet sind, zugegriffen werden.
Durch das Schlüsselwort **base** kann auf Member der parent Instanz zugegriffen werden. **base** wird z.B. dazu verwendet, den Konstruktor der parent Class in der child Class aufzurufen.

    public class BaseClass{

      string word;

      //Default Constructor
      public BaseClass(){

      }

      public BaseClass(string _word){
        word = _word
      }
    }

    public class ChildClass : BaseClass{

      public ChildClass(string _word) : base(_word){
        //This Constructor calls the Constructor "BaseClass(string _word)" of the base class
        //Afterwards the code inside this Constructor is called (if there is any code)
      }
    }

*Anmerkung: Man kann das vererben einer Klasse durch den Modifizierer **sealed** verhindern.*
&ensp; 
  
## 02 Klassen ableiten und erweitern
![TeaserImage](../duality.png "Different, yet somewhat similar")  

Zurück zum Beispiel unserer Monster Klasse. Da es viele verschiedene Überkategorien von Monstersn gibt, werden wir nun ein child der Monster Klasse erstellen. Dieses child erbt alle eigenschaften der parent Klasse.  hierzu erstellen wir eine normale Klasse und schreiben hinter den Bezeichner   

    : Monster

um festzulegen, dass unsere neue Klasse von Monster erbt.

![Inheritance](../inheritance1.PNG "Erstellung der child Klasse" )  

Nun instanziieren wir ein Objekt vom Typ unserer neuen Klasse, also von **Relic** in unserer Main Methode.  

![Inheritance](../inheritance2.PNG "Instanziierung" )  

Um zum zeigen, dass unsere child Klasse genau die gleichen Methoden kennt, wie unsere parent Klasse, nutzen wir doch einfach eine der geerbten Methoden!

![Inheritance](../inheritance3.PNG "child - Methodenanwendung" )
![Inheritance](../inheritance4.PNG "Erstellung der child Klasse" )  

Und nun können wir unsere child Klasse erweitern und eine Methode hinzufügen.

![Inheritance](../inheritance4.PNG "Erstellung der child Klasse" )  

Nun rufen wir diese **Roar()** wieder in usnerer Main Methode auf.

![Inheritance](../inheritanceExtension.PNG "Erweiterung der child Klasse" )
![Inheritance](../roarMain.PNG "Aufrufen von Roar()" )
![Inheritance](../roarOutput.PNG "Roar Ouput" )




&ensp;  
&ensp;  
&ensp;  
&ensp;  
&ensp;  
&ensp;  
&ensp;  
#### **Quellen und weiterführende Links**
```
01 https://docs.microsoft.com/en-us/dotnet/csharp/tutorials/inheritance
   https://www.dotnetperls.com/base

02 https://docs.microsoft.com/de-de/dotnet/csharp/tutorials/inheritance
