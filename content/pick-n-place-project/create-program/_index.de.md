+++
title = "Programm erstellen"
weight = 8
+++

## Erstes Programm für Pick&Place Roboter

<div class="shadow">
  {{< youtube n3mIfJFSIYE >}}
</div>

Im **Main [OB1]** wird ein Programm erstellt, um die horizontale Achse des Roboters aus- und einzufahren. Dazu wird die grafische Programmiersprache **KOP (Kontaktplan)** verwendet mit folgenden Ein- und Ausgängen.

Beschreibung                                 | Symbolische Adresse      | Absolute Adresse
-------------------------------------------- | ------------------------ | -----------------
Pick&Placer Bedienstelle Start (160SF3)      | `PIPL_Pa_SF_Start`       | E1.1
Pick&Placer Schlitten ausfahren (125MB1)     | `PIPL_MB_CarrierExtend`  | A0.4
Pick&Placer Schlitten einfahren (125MB2)     | `PIPL_MB_CarrierRetract` | A0.5
Pick&Placer Bedienstelle Stop (160SF4)       | `PIPL_Pa_SF_Stop`        | E1.2
PLC Clock 0.4s (2.5Hz)                       | `ME_PLC_Clock_0.4s`      | M0.2
Pick&Placer Bedienstelle LED Start (160SF3)  | `PIPL_Pa_PF_Start`       | A1.2
Pick&Placer Turmleuchte Grün (130PF1)        | `PIPL_SC_Green`          | A0.1
