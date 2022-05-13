+++
title = "Modulkarten parametrieren"
weight = 3
+++

## SPS CPU und IOs konfigurieren

<div class="shadow">
  {{< youtube tg2kENLqTiM >}}
</div>

In der **Gerätekonfiguration** werden die Module so benannt, dass sie dieselben Namen wie im Elektroschema haben. Anschliessend wird der **Adressbereich** vergeben über das Eigenschaftsfenster. Alternativ kann man die Ansicht **Gerätesicht > Geräteübersicht** anwählen. Dort sind alle Karten und die Adressbereiche in Tabellenform gelistet.

Die BaseUnits der Eingangs und Ausgangsmodule gibt es in **Hell- und Dunkelgrau**. Hellgraue Module werden mit 24VDC gespiesen. Dunkelgraue Module werden nicht gespiesen, sie greifen die Spannung von Links ab. Im Projekt werden folgende BaseUnits verwendet:

* BaseUnit ohne AUX-Klemmen, [neue Lastgruppe](https://mall.industry.siemens.com/mall/de/WW/Catalog/Product/6ES7193-6BP00-0DA0), hellgrau: `6ES7193-6BP00-0DA0`
* Base-Unit ohne AUX-Klemmen, [nach links gebrückt](https://mall.industry.siemens.com/mall/de/WW/Catalog/Product/6ES7193-6BP00-0BA0), dunkelgrau: `6ES7193-6BP00-0BA0`

Bei der **absoluten Adressierung** wird direkt der Operand (z.B. `I0.0`) eingegeben. Bei der **symbolischen Programmierung** wird nicht der Operand, sondern stellvertretend ein Symbolname (z.B. `CC_TB_24VMainOk`) anstelle des Operanden eingegeben.

* **CC** steht für Control Cabinet oder in Deutsch Schaltschrank.
* **TB** steht für das elektrische Bauteil. In diesem Fall der Hilfskontakt des Netzgerätes `10TB1`.
* **24VMainOk** steht für die Kurzbeschreibung der Funktion in [Upper Camel Case](https://en.wikipedia.org/wiki/Camel_case). In diesem Fall "24VDC Versorgung OK".

Die Variabeln können in der Projektnavigation unter **Geräte > PLC-Variabeln** eingegeben und editiert werden. Im Video wird zusätlich auf die Excel Import und Export Funktion eingeganen.
