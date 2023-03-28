+++
title = "PLC simulation"
weight = 6
+++

## Emulate CPU and HMI for tests without hardware

<div class="shadow">
  {{< youtube qJF1XHB1Bmo >}}
</div>

With the help of SIMATIC **S7-PLCSIM** the Pick&Place control can be simulated and tested without any hardware components added.

The video shows the simulation of the PLC and the touch panel. Emulating means recreating the functions of a computer with another device.

To be able to emulate a PLC or an HMI, you need to select the component in the **Project navigator** under **Devices** and click on the icon **Start simulation** in the smybol menu.

Afterwards the preferred blocks get loaded. These can be tested almost in the same fashion as with a hardware-based PLC. For example with the **Monitor on/off** function or with a **SIM table**.

Not that important here, but for other projects: You can't load **protected blocks** in the simulation. If they exist in your project, you first need to enable the access for them.