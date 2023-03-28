+++
title = "Set module parameters"
weight = 4
+++

## Configuring central processing unit (CPU) und IOs

<div class="shadow">
  {{< youtube tg2kENLqTiM >}}
</div>

The modules in the **device configuration** are named identically as the ones in the electrical diagram. Afterwards, the **address range** can be assigned in the property window. Alternatively, you can open the view **Device view > Device overview**. All modules and address ranges are listed in table here. 

The BaseUnits of the input and output modules come in **light gray and dark gray**. The light gray modules are powered with 24VDC. Dark grey modules can't be powered, they are bridged to the module to the left. The following BaseUnits are used in the project:

* BaseUnit w/o AUX terminals, [new load group](https://mall.industry.siemens.com/mall/en/WW/Catalog/Product/6ES7193-6BP00-0DA0), light gray: `6ES7193-6BP00-0DA0`
* Base-Unit w/o AUX terminals, [bridged to the left](https://mall.industry.siemens.com/mall/en/WW/Catalog/Product/6ES7193-6BP00-0BA0), dark gray: `6ES7193-6BP00-0BA0`

The **absolute addressing** uses the direct operand (i.e. `I0.0`), whereas the **symbolic addressing** utilizes a symbol name as a substitute for the operand (i.e. `CC_TB_24MainOk`).

* **CC** stands for control cabinet. This defines the place where the part is installed.
* **TB** stands for the electrical part in accordance to EN 81346. In this case it is the auxiliary contact of the power supply `10TB1`
* **24MainOk** stands for the abbreviation of the function in [Upper Camel Case](https://en.wikipedia.org/wiki/Camel_case). In this case it is "24VDC power supply OK".

The variables can be added and edited in the project navigation under **Devices > PLC variables**. The video additionally mentions the function for importing and exporting Excel files.

{{% notice tip %}}
The Excel file, which can be used to import the PLC tags, can be downloaded [here](./docs/Pick&Placer_PLCTags.en.xlsx)
{{% /notice %}}