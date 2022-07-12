+++
title = "Programm laden"
weight = 7
+++

## Download des Programms vom PC auf SPS und HMI

<div class="shadow">
  {{< youtube _V39uCb8Kio >}}
</div>

Um das Programm aus dem TIA Portal auf die **SPS zu laden**. In einem ersten Schritt klickt man unter Geräte auf **Geräte & Netze**, wo man sich die IP-Adressen einblenden lassen kann.

* CPU 1512SP F-1 PN: `192.168.10.10`
* Touch-Panel KTP400 Comfort: `192.168.10.5`

In einem zweiten Schritt muss man dem **Laptop**, welcher sich im gleichen Netzwerk befindet, eine statische IP-Adresse vergeben. In Windows bei den Adapteroptionen wählt man für den Ethernet-Port die Adresse `192.168.10.99`.

In der Symbolleiste wählt man das Symbol **Laden in Gerät**, um das Programm auf die SPS zu laden.

Da eine Safety Integrated SPS zum Einsatz kommt, müssen die beiden **Safety Karten** `20KF5` (Eingänge) und `20KF6` (Ausgänge) identifiziert werden. Man muss eine Profisafe-Adresse zuweisen.

Auf dem **HMI** klickt man auf **Settings** > **Transfer** > **PN/IE** > **Properties...** > **PN_X1** > **Specify an IP Address** > `192.168.10.5` um die IP-Adresse einzustellen. Ebenfalls muss man im Anschluss auf **Laden in Gerät** klicken.
