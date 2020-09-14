# Paritätsberechnung

## Gerade Parität
Bei der geraden Parität muss an jeder Stelle eine gerade Anzahl an Eins-Bits vorhanden sein.

|Eingabe|7|6|5|4|3|2|1|0|
|-|-|-|-|-|-|-|-|-|
|1.|1|1|0|0|1|0|1|0|
|2.|0|1|0|1|0|1|0|1|
|Parität|1|0|0|1|1|1|1|1|

## RAID 5
Für einen RAID-5-Verbund wird eine weitere Festplatte benötigt. Auf dieser werden die Paritätsinformationen des Verbundes abgelegt. Dadurch kann jede Festplatte ausfallen (inkl. der Paritätsplatte) ohne dass es zu Datenverlust kommt.

|Festplatte|Aufgabe|7|6|5|4|3|2|1|0|
|-|-|-|-|-|-|-|-|-|-|
|1|Daten|1|1|0|0|1|1|1|1|
|2|Daten|0|1|0|1|0|1|0|1|
|3|Parität|1|0|0|1|1|0|1|0|
