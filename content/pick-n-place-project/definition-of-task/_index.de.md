+++
title = "Aufgabenstellung"
weight = 1
+++

## Beschreibung des Programmablaufes

![Festo Pick&Place Robot](./images/festo_pick_n_place.de.gif)

Wie in der Animation oben gezeigt, soll der Pick&Placer folgendermassen programmiert werden, inklusive Visualisierung am Bedienpanel.

1. Zu Beginn ist der Pick&Placer eingefahren und das Förderband steht.
2. Der Operator platziert einen Behälter auf dem Förderband bei der Einlauflichtschranke 100BG1 und drückt den Taster Start.
3. Der Behälter wird bis zum Vereinzeler gefördert und dort gestoppt.
4. Der Pick&Placer fährt nach unten, saugt einen Deckel an, fährt wieder nach oben, nach vorne und nach unten über den Behälter.
5. Vakuum wird gelöst und somit Deckel aufgesetzt.
6. Der Pick&Placer fährt wieder in die Startposition.
7. Der Vereinzeler lässt den Behälter mit aufgesetztem Deckel weiterfahren.
8. Kommt der Behälter an der Rückstau Lichtschranke 100BG3 an, stoppt das Förderband.

Die Positionen der wichtigsten Sensoren können folgender Grafik entnommen werden.

![Festo Pick&Place Robot](./images/festo_pick_n_place_overview.de.png)

{{% notice info %}}
Das Elektroschema des Steuerschranks kann [hier als PDF](./docs/Pick_and_Placer.de.pdf) heruntergeladen werden.
{{% /notice %}}