+++
title = "Set HMI parameters"
weight = 5
+++

## 4 inch touch panel Siemens KTP400 Comfort

<div class="shadow">
  {{< youtube BCkbDmbao6w >}}
</div>

HMI stands for Human-Machine Interface. This is the touch panel, with which the operator controls the machine.

Add the HMI under **Devices > Devices and networks**. It is the [KTP400 Comfort](https://mall.industry.siemens.com/mall/en/ww/Catalog/Product/6AV2124-2DC01-0AX0) panel from Siemens with the type number `6AV2124-2DC01-0AX0`.

**Profinet** stands for Process Field Network. It is a common protocol in the industry which uses [TCP/IP Standards](https://www.techtarget.com/searchnetworking/definition/TCP-IP#:~:text=TCP%2FIP%20stands%20for%20Transmission,(an%20intranet%20or%20extranet).) As such, the communication between PLC and HMI works similar to the internet (IP stands for Internet Protocol). Each member of the network gets a **unique IP address** - the Profinet address. Each address in the projetc can only show up once.

* Profinet address HMI **155PH1**: `192.168.10.5`
* Profinet address PLC **20KF3**: `192.168.10.10`
