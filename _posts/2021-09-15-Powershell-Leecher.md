---
layout: post
title: PowerShell Leecher - Bilder vom Internet in Word-Datei speichern
---

In diesem Portfolio erkläre ich mein PowerShell Projekt, welches ich mit meinem Kollegen Dion zusammen erarbeitet habe.
<!--break-->

## Aufgabenstellung

Für das Auftrag 1306 im Lernatelier wurde wieder eine grosse Auswahl an Projekten gegeben. 
Ich und mein Kollege Dion haben uns zu zweit entschieden, einen Leecher in PowerShell zu schreiben. 
Die genaue Aufgabenstellung des Leechers war:

"Schreiben Sie ein Power-Shell-Script, das rekursiv alle oder nur bestimmte Bilder von einer gegebenen URL herunterlädt und in einer eigenen HTML-Seite oder Word-Dokument ablegt. Eine Anwendung wäre zum Beispiel das Herunterladen von Comics."

## Ziele

Meine eigenen Ziele waren:

1. Das Skript speichert die Bilder Lokal

2. Die Bilder werden in einer HTML Datei oder in einem Word Dokument gespeichert.

## Produkt

Der Leecher speichert also Bilder aus dem Internet ab und fügt de dann in ein Word oder HTML Dokument. 
Wir haben uns dafür entschieden, die Bilder schlussendlich in einem Word Dokument zu speichern, das Klang für uns einfacher, als es in einer HTML Seite zu speichern.

Das Skript hat 2 Hauptaufgaben. Im ersten Teil werden die Bilder gespeichert, und im zweiten Teilwerden sie in ein Word Dokument gespeichert. 
Natürlich haben beide diese Schritte noch Unteraufgaben. Zuerst wird der Benutzer gefragt, wie viele Bilder er haben will, dann müssen die Bilder Links auch noch eingegeben werden. 
Dieser Schritt sowie das Speichern passieren beide über eine "for" Iteration damit man auch mehrere Bilder automatisiert herunterladen kann. 
Die Bilder werden dann von PowerShell aus einem Lokalen Speicherpfad ausgesucht und ein Worddokument eingefügt. 
Die Word Datei wird dabei auch automatisch erstellt, benennt und gespeichert. schlussendlich wird die Word-Datei noch geschlossen.

## Problem

Unser einziges Problem, welches wir noch nicht lösen konnten, ist, dass nur 1 Bild gespeichert werden kann. Auch wenn man eingibt, dass man mehrere speichern will, geht das Skript direkt nach der Eingabe des ersten Links weiter.
![Leecher Powershell log](images/leecherCode.png)

Wir haben nicht viel zeit mit der Behebung dieses Problems verbracht, da wir das Skript erstens mal mit einem Bild zum laufen bringen wollten. Gegen Schluss kamen wir noch ein bisschen unter Zeitdruck mit dem IPERKA und diesem Portfolio also entschieden wir, es so zu lassen.


## Reflexion

Dieses Projekt fand ich sehr informativ. Ich denke ich habe abgesehen vom meinem neuen wissen auch den Umgang mit PowerShell verbessert, was code Struktur und Problemlösung bei Fehlermeldungen angeht.

Die Arbeitsaufteilung mit Dion fand ich auch gut und gerecht. Wir arbeiteten oft separat aber haben uns immer wieder abgesprochen und den Stand unseres Projekts angeschaut.

Anfangs ging es ein bisschen lang bis wir angefangen haben zu Coden. Wir haben uns viele Beispiele und Fragen anderer angeschaut, um herauszufinden wie wir am besten zu einer Lösung unseres Problems kommen.

## Zeilerfüllung

Meine eigenen Ziele waren:

1. Das Skript speichert die Bilder Lokal ✓

Ein Bild wird im gleichen Ordner wie die Word-Datei als "1.jpg" gespeichert.
![Leecher Verifizierung](images/leecherProof.png)

2. Die Bilder werden in einer HTML Datei oder in einem Word Dokument gespeichert. ✓

In der vom Skript erstellten Word-Datei, wird das Bild "1.jpg" eingefügt und gespeichert.


## Code download

Sie können mein Powershell-Skript <a href="files/Leecher.ps1" download>hier</a> herunterladen.

Sie können meine IPERKA-Dokumentation <a href="files/IPERKA_1306.docx" download>hier</a> herunterladen.
