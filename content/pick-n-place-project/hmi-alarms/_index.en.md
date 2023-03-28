+++
title = "HMI alarms"
weight = 10
+++

## Displaying HMI messages on the touch panel

<div class="shadow">
  {{< youtube l-SyezS_op4 >}}
</div>

An error which illuminates the red lamp exists already in **Main [OB1]**, but we don't have a message for this error. The lamp acts as a centralised error. It gets generated in network 7, which has the following variables. 

Description                                  | Symbolic address           | Absolute address
-------------------------------------------- | -------------------------- | -----------------
Pick&Placer Carrier extended (120BG2)        | `PIPL_BG_CarrierExtended`  | E0.5
Pick&Placer Carrier retracted (120BG1)       | `PIPL_MB_CarrierRetracted` | E0.4
Pick&Placer Carrier extend (125MB1)          | `PIPL_MB_CarrierExtend`    | A0.4
Pick&Placer Carrier retract (125MB2)         | `PIPL_MB_CarrierRetract`   | A0.5
Error active                                 | `ErrorActive`              | M100.0

To give the operator specific information of a problem, Siemens has the function **HMI messages**. It handles the messages and the display of them on the touch panel.

To give the HMI messages, you need to create a **Data block DB** with the name `HMI_messages`, type `Global-DB` and number `120`. In a second step create a data structure which consists of 3 structs of 1 word each (1 word = 16 bit), while the structs stand for **Error**, **Warnings** and **Messages**.

* Static
  * Error (Struct)
    * `Hcyl_not_extended` (Bool)
    * `Hcyl_not_retracted` (Bool)
  * Warning (Struct)
  * Message (Struct)

In a next step click in the project navigation of 155PH1 on the menu **HMI messages**. Choose **Bit messages** in the tabs and type in the following mesaages. With this you link the messages on the HMI with the program.

ID | Message                                   | Class       | Trigger variable | Trigger bit | Trigger address
-- | ----------------------------------------- | ----------- | ---------------- | ----------- | --------------
1  | Horizontal cylinder not extended          | Errors      | Errors           | 8           | `%DB120.DBX0.0`
2  | Horizontal cylinder not retracted         | Errors      | Errors           | 9           | `%DB120.DBX0.1`

In the last step create an image with a **Message display**.