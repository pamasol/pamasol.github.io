+++
title = "Structure program"
weight = 11
+++

## Dividing OB1 in separate subprogrammes

<div class="shadow">
  {{< youtube UQWpMJmHEiQ >}}
</div>

The `OB1`, in which the program resides, can be divided into 3 `FB's`:

* `FB1` 01-General
* `FB2` 02-General_Pick&Placer
* `FB3` 03-Cycle_Pick&Placer

With this the programm can be divided into **small subtasks**, which makes the **program clearer**. Additionally recurring functions such as moving the axis can be programmed once and reused again and again - which corresponds to the [DRY principle](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).


| Blocktype          | Short | Features                                                                                                                                                                                                                   |
|--------------------|-------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Organization block | `OB`  | <ul><li>Link between OS and program</li><li>Graduated priorities (1 to 28)</li><li>i.e. OB1, OB120</li><ul>                                                                                                                |
| Function block     | `FB`  | <ul><li>Parametrable (with memory)</li><li>IN, OUT, INOUT, STAT, TEMP</li><li>Usage of instance-DB. Replace actual parameter [Formal parameter](https://en.wikipedia.org/wiki/Parameter_(computer_programming)).</li></ul> |
| Function           | `FC`  | <ul><li>Gives return value of calling functions</li><li>Parametrable, but no(!) memory</li><li>i.e. mathematical functions</li></ul>                                                                                       |
| Data block         | `DB`  | <ul><li>Global data storage</li><li>Local data storage (Instance-DB)</li></ul>                                                                                                                                             |