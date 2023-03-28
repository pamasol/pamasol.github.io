+++
title = "Designing HMI"
weight = 9
+++

## Designing a link between human and machine

<div class="shadow">
  {{< youtube 7MDUunpy3hg >}}
</div>

The HMI (Human Machine Interface) **155PH1** consists of a [KTP400 Comfort](https://mall.industry.siemens.com/mall/en/ww/Catalog/Product/6AV2124-2DC01-0AX0) panel from Siemens. 400 stands for the screen size, which in this case is 4.3". The resolution is **480 by 272 pixels**.

> For comparison: a [Samsung Galaxy S22](https://en.wikipedia.org/wiki/Samsung_Galaxy_S22) smartphone with a 6.1" display has a resolution of 1080 x 2340 pixels. Regarding the design we are a bit restricted, but you can create a nice and clear design nevertheless, to facilitate the usage of the robot for the operator.

Click on the HMI 155PH1 in the **Project navigation** to create a template with **Image management > Templates**. In the course of the tutorial 3 images based off the templates will be created:

* `Image_1 - Overview`
* `Image_2 - Messages`
* `Image_3 - Switches etc`

The images and displays can be switched with **buttons** (click > action). The data exchange between PLC and HMI is managed by the data block `DB122`.

Next to the signal lamp **text list**, create a signal lamp called **graphics list**.