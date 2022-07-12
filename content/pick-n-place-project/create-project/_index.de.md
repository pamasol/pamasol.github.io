+++
title = "Neues Projekt erstellen"
weight = 3
+++

## Die SPS Hardwarekonfiguration als Basis

<div class="shadow">
  {{< youtube uTUbFHpi8Xk >}}
</div>

In einem ersten Schritt wird in der Projektansicht ein neues SPS Projekt erstellt. Anschliessend muss man die im Schaltschrank verbaute SPS in der Software abbilden. Das wird mittels **Hardwarekonfiguration** gemacht.

Der Pick&Place Roboter ist mit einer **SIMATIC ET200 CPU** ausgestattet. Zusätzlich werden die Ein- und Ausgangsmodule hinzugefügt und konfiguriert.

### Artikelnummern der SPS für Hardwarekonfig

* **Steuerung** CPU 1512SP F-1 PN: `6ES7512-1SK01-0AB0`
* **Safety Eingangskarte** ET200SP F-DI 8x 24V DC HF: `6ES7136-6BA00-0CA0`
* **Safety Ausgangskarte** ET200SP F-DQ 8x 24V DC/0.5A PP `6ES7136-6DC00-0CA0`
* **Digitale Eingangskarte** ET200SP DI 16x 24V DC ST: `6ES7131-6BH01-0BA0`
* **Digitale Ausgangskarte** ET200SP DQ 16x 24V DC/0.5A ST: `6ES7132-6BH01-0BA0`
* **Analoge Eingangskarte** ET200SP AI 2x U/I 2/4-Wire HS: `6ES7134-6HB00-0DA1`
* **Analoge Ausgangskarte** ET 200SP, AQ 2xU ST: `6ES7135-6FB00-0BA1`
