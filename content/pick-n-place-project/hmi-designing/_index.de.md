+++
title = "Visualisierung erstellen"
weight = 9
+++

## Bindeglied zwischen Mensch und Maschine entwerfen

<div class="shadow">
  {{< youtube 7MDUunpy3hg >}}
</div>

Als HMI (Human Machine Interface) **155PH1** kommt ein [KTP400 Comfort](https://mall.industry.siemens.com/mall/en/de/Catalog/Product/6AV2124-2DC01-0AX0) Panel von Siemens zum Einsatz. 400 steht für die Bidschirmgrösse, was in diesem Fall 4.3" ist. Die Auflösung beträgt **480 auf 272 Pixels**.

> Zum Vergleich: ein [Samsung Galaxy S22](https://en.wikipedia.org/wiki/Samsung_Galaxy_S22) Smartphone mit einem 6.1" Display hat eine Auflösung von 1080 x 2340 Pixels. Bezüglich Design ist man somit etwas eingeschränkt, dennoch kann ein schönes und übersichtliches Design erstellt werden, welches dem Operator die Bedienung des Pick&Place Rotobers erleichtert.

In der **Projektnavigation** klickt man auf das HMI 155PH1. Unter **Bildverwaltung > Vorlagen** wird eine Vorlage erstellt. Im Laufe des Tutorials werden basierend auf der Vorlage folgende drei Bilder erstellt:

* `Bild_1 - Uebersicht`
* `Bild_2 - Meldungen`
* `Bild_3 - Schalter Etc`

Mittels **Schaltflächen** können die Bilder und somit die Anzeigen gewechselt werden (Klicken > Ereignis). Der Datenaustausch zwischen PLC und HMI wird mittels Datenbaustein `DB122` realisiert.

Neben einer Meldelampe mit **Textliste** wird eine Meldelampe mit **Grafikliste** erstellt.
