+++
title = "Create a new project"
weight = 3
+++

## The PLC hardware configuration as a basis

<div class="shadow">
  {{< youtube uTUbFHpi8Xk >}}
</div>

As a first step a new PLC project will be created in the projec view. Afterwards you need to project the installed PLC from the control cabinet in the software. This will be done with the **hardware configuration**.

The Pick&Place robot is equipped with a **SIMATIC ET200 CPU**. Additionally input and ouptut modules will be added and configured.

### Articel no° of the CPU for the hardware config

* **Control** CPU 1512SP F-1 PN: `6ES7512-1SK01-0AB0`
* **Safety input** ET200SP F-DI 8x 24V DC HF: `6ES7136-6BA00-0CA0`
* **Safety output** ET200SP F-DQ 8x 24V DC/0.5A PP `6ES7136-6DC00-0CA0`
* **Digital input** ET200SP DI 16x 24V DC ST: `6ES7131-6BH01-0BA0`
* **Digital output** ET200SP DQ 16x 24V DC/0.5A ST: `6ES7132-6BH01-0BA0`
* **Analog input** ET200SP AI 2x U/I 2/4-Wire HS: `6ES7134-6HB00-0DA1`
* **Analog output** ET 200SP AQ 2xU ST: `6ES7135-6FB00-0BA1`