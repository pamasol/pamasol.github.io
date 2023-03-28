+++
title = "HMI Alarmmeldungen"
weight = 10
+++

## HMI-Bitmeldungen auf Touch-Panel anzeigen

<div class="shadow">
  {{< youtube l-SyezS_op4 >}}
</div>

Eine Störung, welche die rote Lampe aufleuchten lässt, ist bereiets vorhanden im **Main [OB1]**, jedoch gibt es zu dieser Leuchte keine Fehlermeldung. Die Leuchte waltet als **Sammelfehler**. Sie wird in Netzwerk 7 generiert, wo es folgende Variabeln gibt.

Beschreibung                                 | Symbolische Adresse        | Absolute Addresse
-------------------------------------------- | -------------------------- | -----------------
Pick&Placer Schlitten ausgefahren (120BG2)   | `PIPL_BG_CarrierExtended`  | E0.5
Pick&Placer Schlitten eingefahren (120BG1)   | `PIPL_MB_CarrierRetracted` | E0.4
Pick&Placer Schlitten ausfahren (125MB1)     | `PIPL_MB_CarrierExtend`    | A0.4
Pick&Placer Schlitten einfahren (125MB2)     | `PIPL_MB_CarrierRetract`   | A0.5
Störung aktiv                                | `StoerungAktiv`            | M100.0

Um dem Operator spezifische Informationen zum Problem bereitstellen zu können, gibt es bei Siemens die Funktion **HMI-Meldungen**. Sie übernimmt das Handling der Meldungen und deren Anzeige auf dem Touch-Panel.

Damit man dem HMI Fehlermeldungen übergeben kann, muss man einen **Datenbaustein DB** erstellen mit Name `HMI_Meldungen`, Typ `Global-DB` und Nummer `120`. In einem zweiten Schritt erstellt man die Datenstruktur, welche aus 3 Struct von je einem Wort (1 Wort = 16 Bit) besteht, wovon je ein Struct für **Fehler**, **Warnungen** und **Meldungen** reserviert ist.

* Static
  * Fehler (Struct)
    * `Hzyl_nicht_ausfefahren` (Bool)
    * `Hzyl_nicht_einfefahren` (Bool)
  * Warnungen (Struct)
  * Meldungen (Struct)

In einem weiteren Schritt klickt man in der Projektnavigation unter 155PH1 das Menü **HMI-Meldungen**. Bei den Tabs wählt man **Bitmeldungen** und fügt folgende Bitmeldungen ein. Damit verknüpft man die Meldungen auf dem HMI mit dem Programm.

ID | Meldetext                                 | Meldeklasse | Triggervariable | Triggerbit | Triggeradresse
-- | ----------------------------------------- | ----------- | --------------- | ---------- | --------------
1  | Horizontalzylinder ist nicht ausgefahren  | Errors      | Fehler          | 8          | `%DB120.DBX0.0`
2  | Horizontalzylinder ist nicht eingefahren  | Errors      | Fehler          | 9          | `%DB120.DBX0.1`

Im letzten Schritt wird ein Bild erstellt mit einer **Meldeanzeige**.
