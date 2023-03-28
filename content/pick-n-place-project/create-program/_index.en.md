+++
title = "Create program"
weight = 8
+++

## First program for Pick&Place robot

<div class="shadow">
  {{< youtube n3mIfJFSIYE >}}
</div>

To move the horizontal axis of the robot, creat a program in **Main [OB1]**. Use ladder logic with the following in- and outputs.

Description                                  | Symbolic address         | Absolute address
-------------------------------------------- | ------------------------ | -----------------
Pick&Placer HMI Start (160SF3)               | `PIPL_Pa_SF_Start`       | E1.1
Pick&Placer extend carrier (125MB1)          | `PIPL_MB_CarrierExtend`  | A0.4
Pick&Placer retract carrier (125MB2)         | `PIPL_MB_CarrierRetract` | A0.5
Pick&Placer HMI Stop (160SF4)                | `PIPL_Pa_SF_Stop`        | E1.2
PLC Clock 0.4s (2.5Hz)                       | `ME_PLC_Clock_0.4s`      | M0.2
Pick&Placer HMI LED Start (160SF3)           | `PIPL_Pa_PF_Start`       | A1.2
Pick&Placer signaling column green (130PF1)  | `PIPL_SC_Green`          | A0.1