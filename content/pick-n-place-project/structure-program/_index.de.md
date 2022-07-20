+++
title = "Programm strukturieren"
weight = 11
+++

## OB1 in verschiedene Teilprogramme zerlegen

<div class="shadow">
  {{< youtube UQWpMJmHEiQ >}}
</div>

Der `OB1`, in welchem sich das Programm befindet, wird in folgende drei `FB's` aufgeteilt:

* `FB1` 01-Allgemein
* `FB2` 02-Allgemein_Pick&Placer
* `FB3` 03-Ablauf_Pick&Placer

So kann man das Programm in **kleine Teilaufgaben** zerstückeln, was das **Programm übersichtlicher** macht. Zudem kann man wiederkehrende Funktionen wie das Bewegen einer Achse einmal programmieren und dann immer wieder verwenden – was dem [DRY-Prinzip](https://de.wikipedia.org/wiki/Don%E2%80%99t_repeat_yourself) entspricht.

Bausteintyp           | Kurzform | Merkmale
--------------------- | -------- | --------------------------------------
Organisationsbaustein | `OB`     | <ul><li>Schnittstelle zwischen Betriebssystem und Programm</li><li>Gestaffelte Prioritäten (1 bis 28)</li><li>zum Beispiel OB1, OB120</li><ul>
Funktionsbaustein     | `FB`     | <ul><li>Parametrierbar (mit Gedächtnis)</li><li>IN, OUT, INOUT, STAT, TEMP</li><li>Verwendung von Instanz-Datenbaustein. Aktualparameter ersetzen [Formalparameter](https://de.wikipedia.org/wiki/Parameter_(Informatik)#Ersetzen_der_formalen_durch_tats%C3%A4chliche_Parameter).</li></ul>
Funktion              | `FC`     | <ul><li>Liefert Rückgabewert an aufrufende Funktion</li><li>Parametrierbar, aber nicht(!) speichernd</li><li>zum Beispiel für mathematische Funktionen</li></ul>
Datenbaustein         | `DB`     | <ul><li>Globale Datenspeicherung</li><li>Lokale Datenspeicherung (Instanz-DB)</li></ul>
