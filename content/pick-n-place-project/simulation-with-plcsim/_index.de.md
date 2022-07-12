+++
title = "SPS simulieren"
weight = 6
+++

## CPU und HMI emulieren für Tests ohne Hardware

<div class="shadow">
  {{< youtube qJF1XHB1Bmo >}}
</div>

Mit Hilfe von SIMATIC **S7-PLCSIM** kann die Pick&Place Steuerung simuliert und somit getestet werden, ohne dass irgendwelche Hardwarekomponenten benötigt werden.

Im Video wird die PLC und das Touch-Panel emuliert. Emulieren bedeutet die Funkionen eines Computers auf einem anderen Gerät nachbilden.

Um eine SPS oder ein HMI zu simulieren, muss man das Bauteil im **Projektnavigator** unter **Geräte** anwählen und anschliessend in der Symbolleiste auf das Icon **Simulation starten** klicken.

Anschliessend werden die gewünschten Bausteine geladen. Diese können fast im selben Umfang wie bei einer hardwaremässig angeschlossenen SPS getestet werden. Beispielsweise mit **Beobachten ein/aus** Funktion oder mit einer **SIM-Tabelle**.

Hier nicht entscheidend, aber für andere Projekte: Es können keine **geschützten Bausteine** in die Simulation geladen werden. Falls es diese im Projekt gibt, müssen sie zuerst freigegeben werden.
