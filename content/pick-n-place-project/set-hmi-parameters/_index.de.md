+++
title = "HMI parametrieren"
weight = 5
+++

## 4-Zoll Touch-Panel Siemens KTP400 Comfort

<div class="shadow">
  {{< youtube BCkbDmbao6w >}}
</div>

HMI steht für Human-Machine Interface oder in Deutsch für Mensch-Maschine-Schnittstelle. Es ist das Touch-Panel, mit dessen Hilfe der Operator die Maschine bedient.

Unter **Geräte > Geräte und Netze** wird das HMI hinzugefügt. Es handelt sich um ein [KTP400 Comfort](https://mall.industry.siemens.com/mall/de/ch/Catalog/Product/6AV2124-2DC01-0AX0) Panel von Siemens mit der Typennummer `6AV2124-2DC01-0AX0`.

**Profinet** steht für Process Field Network. Es ist ein **Kommunikationsprotokoll**, welches in der Industrie oft zum Einsatz kommt und [TCP/IP Standards](https://www.elektronik-kompendium.de/sites/net/0606251.htm) verwendet. Die Kommunikation zwischen SPS und HMI funktioniert somit ähnlich, wie das Internet (IP steht für Internet Protocol). Jeder Teilnehmer kriegt eine **eindeutige IP-Adresse** – die Profinet-Adresse. Jede Adresse darf im Projekt nur einmal vorkommen.

* Profinet-Adresse von HMI **155PH1**: `192.168.10.5`
* Profinet-Adresse von SPS **20KF3**: `192.168.10.10`
