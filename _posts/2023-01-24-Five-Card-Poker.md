---
layout: post
title: Five Card Poker
---

Ich habe in zusmmen mit einem Klassenkameraden mittels JSF ein mehrspieler Five Card Poker in Form einer Webapplikation realisiert.
<!--break-->

## Aufgabenstellung
Wir durften für das Lernatelier slebst ein Projekt wählen. Wir haben uns dafür entschieden, ein Five Card Poker zu realisieren, dies mittels JSF.
Die Regeln des Five Card Pokers sind ähnlich zum traditionellen Poker. Man bekommt 5 Karten. Mit diesen Karten will man die bestmögliche Kombination haben, wobei diese Kombinationen die üblichen aus dem Poker sind (Pair, Full House, Straight, usw.).
Wenn man mit den Karten, die man von Beginn bekommt, nicht zufrieden ist, kann man sie für neue eintauschen (nur begrenzt). Der mit der besten Kartenkombination gewinnt den Pot.

## Ziele

**Meine Ziele waren:**

- Die Verteilung der Karten ist korrekt (Keine dopelten Karten).
- Das Spiel erkennt die aktuelle Kombination in der Hand.
- Man kann gewinnen oder verlieren. 

## Produkt

Bei der eigentlichen Realisierung haben wir uns von Anfang an mit überlegt, was wahrscheinlich der schwierigste oder aufwändigste Teil sein wird. Das Spiel funktioniert grundsätzlich so.

Als erste kommt man auf die menu.xhtml Seite, dort stellt man ein, wie viele Spieler man haben will und wie viele Spielzüge es geben sollte. Als Nächstes kommt man auf die eigentliche Spielseite. Dort kann man seine Karten, die einem nicht gefallen, eintauschen. Wenn man seinen Spielzug beendet hat, wird das wiederholt für jeden Spieler. 
Danach kommt man weiter auf noch eine Seite, wo die Kartenkombos überprüft werden, und Gewinner und Verlierer bestimmt werden, Unentschieden ist auch möglich. Die Informationen des Siegers werden auch dort ausgegeben. Zusätzlich hat man die Option das Spiel zu beenden oder Neuzustarten. Bei einem Neustart werden die Einstellungen des vorherigen Spiels übernommen. 

Die Evaluierung funktioniert so:

![determineWinner](images/determineWinner.png)

Die Scores aller Spieler werden durchitereirt, bis der mit dem Höchsten Score dem "winner" zugewiesen wird, wenn dies nicht machbar ist wird ein Gleichstant zurückgegeben. 

## Reflexion

Dieses Projekt ist ziemlich gut gegangen, meiner Meinung nach. Wir sind in der gegebenen Zeitgut vorangekommen. Gegen Schluss waren wir doch ein bisschen in Stress gekommen, was uns aber nur weitergeholfen hat, weil wir unter Zeitdruck effizienter gearbeitet haben. 
Wir konnten zu zweit die Arbeit gut einteilen, sodass wir nicht aneinander vorbeiarbeiteten. Dazu haben wir Git verwendet.

![commitverlauf](images/commitverlaufFCP.png)

Ich habe oft von zuhause aus auf mienem Pc gearbeitet, worauf ich aus unbekannten Gründen meinen Fortschritt nicht auf Git pushen konnte, also habe ih die geänderten Datein jeweils Mikhail geschickt, der hatte sie dann gepusht. Ich würde nicht sagen, dass ich konkret etwas Neues gelernt habe, aber mehr mein bereits bestehendes Wissen gefestigt habe.

Für nächstes Mal würde ich mich mehr mit dem Planen der ganzen Applikation auseinandersetzen, und nicht nur mit den Schlüsselstellen beschäftigen.

## Zielerfüllung

- Die Verteilung der Karten ist korrekt (Keine dopelten Karten). ✓

Das Spiel erzeugt ein vollständiges Deck mit 52 KArten, wovon jede nur ein mal gezogen werden kann.

- Das Spiel erkennt die aktuelle Kombination in der Hand. ✓

Die bestmögliche Kombination in der Hand wird angezeigt.

- Man kann gewinnen oder verlieren. ✓

Man kann im mehrspieler modus spielen und somit einen Gewinner, Verlierer oder Gleichstand erreichen.

## Projekt Download

Sie können Das Five Card Poker  <a href="files/fivecardpoker.zip" download>hier</a> herunterladen.

