+++
title = "Load program"
weight = 7
+++

## Download program from PC to PLC and HMI

<div class="shadow">
  {{< youtube _V39uCb8Kio >}}
</div>

To load the program from the TIA portal into the **PLC**. In a first step, click under devices on **Devices & networks**, where you can display the IP addresses.

* CPU 1512SP F-1 PN: `192.168.10.10`
* Touch panel KTP400 Comfort: `192.168.10.5`

In a second step you need to give the **laptop**, which is in the same network, a static IP address. In Windows in the adapter options choose the address `192.168.10.99` for the Ethernet port.

Select the symbol **Load in device** in the toolbar to load the program in the PLC.

Since we are using a Safety Integrated PLC, both **safety modules** `20KF5` (inputs) and `20KF6` (outputs) need to be identified. You need to assign a Profisafe address.

On the **HMI**, click **Settings** > **Transfer** > **PN/IE** > **Properties...** > **PN_X1** > **Specify an IP Address** > `192.168.10.5` to set the IP address. Additionally you need to click on **Load in device**.