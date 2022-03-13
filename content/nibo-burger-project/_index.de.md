+++
chapter = false
title = "Elektronikprojekt"
weight = 2
+++

## Roboter programmieren für lernende Automatiker

![NIBO Burger Roboter](./images/nibo_group.de.jpg)

Neben Berufsschule, den überbetrieblichen [Swissmechanic](https://www.swissmechanic.ch/) Kursen und dem praktischen Arbeiten an Aerosol-Anlagen für Kunden aus der ganzen Welt, arbeiten Automatiker Lernende bei Pamasol auch an Projekten, welche den Fokus auf ein bestimmtes Ausbildungsthema setzen.

NIBO Burger repräsentiert das **Elektronikprojekt** der Ausbildung. Es handelt sich hierbei um einen kleinen Roboter, welcher von den Lernenden zusammengebaut, **gelötet** und in der [Hochsprache C](https://de.wikipedia.org/wiki/C_(Programmiersprache)) programmiert wird.

Die Aufgabenstellung, wie auch sämtliche Datenblätter und Wiki Beiträge sind in Englisch geschrieben. Nach dem Zusammenbau und den Funktionstests, erhalten die Lernenden eine Einführung in die **C-Programmierung**. Den Projekthöhepunt bilden die folgenden «Master-Tasks».

### A) Round trip
Der Roboter muss genau 1.5m nach vorne fahren, eine 180° Drehung machen und wieder an seinen Startpunkt zurückkehren. Damit das funktioniert, müssen die [Odometrie-Sensoren](https://de.wikipedia.org/wiki/Odometrie) der Räder ausgelesen und verglichen werden. Basierend darauf werden die [PID-geregelten](https://de.wikipedia.org/wiki/Regler#PID-Regler) Motoren angesteuert.

_TODO: Video einfügen_

### B) Fraidy cat
Frontseitig ist der Roboter mit IR-Bricks versehen. Das sind Infrarotsensoren, welche Hindernisse detektieren können. In dieser Aufgabe geht es darum, den Hindernissen auszuweichen.

_TODO: Video einfügen_

### C) Follow me
Im Gegensatz zu Aufgabe B, muss man in Aufgabe C den Hindernissen nicht ausweichen, sondern dem Hindernis folgen. In diesem Fall der menschlichen Hand.

_TODO: Video einfügen_

### D) Colour detection
Mit den [RGB](https://de.wikipedia.org/wiki/RGB-Farbraum) (Rot-Grün-Blau) Farbsensoren müssen die Bodenfarben Schwarz, Weiss, Rot, Gelb, Grün und Blau detektiert sowie auf dem Display angezeigt werden. Das Display läuft eigenständig mit eigenem [Microcontroller](https://de.wikipedia.org/wiki/Mikrocontroller). Der Microcontroller vom Roboter kommuniziert via [UART](https://de.wikipedia.org/wiki/Universal_Asynchronous_Receiver_Transmitter) mit dem Microcontroller des Displays.

_TODO: Video einfügen_

### E) Rabbit warren
In der Königsaufgabe muss der Roboter einer schwarzen Linie auf dem Boden folgen. Die Linie wird mittels Sensoren detektiert und basierend darauf werden die Motoren gesteuert.

_TODO: Video einfügen_

## Dokumentation

Die Arbeiten werden dokumentiert. Folgend können die PDFs heruntergeladen und nachgelesen werden.

| Name             | Lehrjahr  | Lehrberuf   | Dokumentation   |
| ---------------- | --------- | ----------- | --------------- |
| Marvin Büeler    | 2016-2020 | Automatiker | [Download PDF](./docs/2019-12-16_Nibo_Doku_MarvinBueeler.de.pdf)
| Joel Glaus       | 2017-2021 | Automatiker | [Download PDF](./docs/2020-04-28_Nibo_Doku_JoelGlaus.de.pdf)
| David Bernhard   | 2018-2022 | Automatiker |
| Jonas Bisig      | 2018-2022 | Automatiker | [Download PDF](./docs/2022-03-04_Nibo_Doku_JonasBisig.de.pdf)
| Stefan Feier     | 2019-2023 | Automatiker |
| Nicolas Diethelm | 2020-2024 | Automatiker |
| Flavio Knobel    | 2020-2024 | Automatiker |

{{% notice tip %}}
Die Projektbeschreibung in Englisch sowie alle Aufgaben und Hilfestellungen gibt es in folgendem GitHub Repository: https://github.com/pamasol/Lehrlingsprojekt-Nibo-Burger
{{% /notice %}}
