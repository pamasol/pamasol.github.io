+++
title = "Fernwartung"
weight = 2
+++

## Fehleranalyse und Support via Fernwartung

Die meisten Anlagen sind mit einem **Fernwartungsmodul** ausgestattet, welches eine sichere Verbindung via Internet von der Anlage zum Pamasol Techniker herstellt.

Es handelt sich grösstenteils um ein blau gefärbtes Gerät von den Herstellern «EWON» oder «VIPA», welches im Hauptschaltschrank eingebaut ist. Das folgende Bild zeigt ein EWON Gateway.

![Fernwartungsmodul im Schaltschrank](images/ewon_industrial_modem.de.png?width=100%)

**Suchen Sie nach dem Fernwartungsmodul** im Schaltschrank und verbinden Sie das Ethernet Kabel, welches eine **Internetverbindung** bereitstellt mit **Port Nummer 4**, wie folgend gezeigt.

![Frontseite des Modems](images/ewon_front_side.de.png?width=100%)

Bei einigen Modems ist zusätzlich ein Drehschalter eingebaut, mit welchem der Internetzugang des Modems hardwaremässig abgeschaltet werden kann. Prüfen Sie, ob dieser Schalter eingeschaltet ist.

Folgende Status LEDs müssen leuchten, damit das Modem korrekt arbeiten kann:

* **PWR** = Dauerhaft grün
* **USR** = Langsam blinkend grün
* **T2M** = Dauerhaft grün
* **@**   = Dauerhaft grün

Siehe dazu auch folgende Illustration.

![Status LEDs Legende](images/ewon_status_leds_general.de.png?width=100%)

{{% notice info %}}
Normalerweise muss **Ihre IT-Abteilung** nichts tun, damit sich das Modem mit dem Server verbinden kann. Der VPN-Tunnel wird vom Modem initiiert. Es gibt nur eine ausgehende Verbindung (HTTPS-Port 443 oder UDP-Port 1194) und keine eingehenden Verbindungen. Deshalb müssen in der Firewall keine Ports freigegeben werden.
{{% /notice %}}

{{% notice tip %}}
Wenn die IT-Abteilung keine Internetverbindung über das Firmennetzwerk zulässt, kann alternativ ein **GSM-Modem** verwendet werden. In diesem Fall sind Firmennetzwerk und Anlage strikt getrennt.
{{% /notice %}}
