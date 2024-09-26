---
tags:
  - FISI
  - Ausbildung
  - Virtualisierung
  - VM
---
# Virtualisierung
Unter Virtualisierung versteht man das Vereinen oder aufteilen von Ressourcen. Das heißt das die Hardware Komponenten die im Physischen Gerät eingebaut ist, wird von Virtualisierungssoftware aufgeteilt oder mit eine Physischen Gerät verbunden und vereint wird.

## Visualisierte Anwendungen 
Hier ist eine Reihe von Sachen die Formen der Virtualisierung sind mit Beispielen:

| Komponente        | Beispiel                                                                                               |
| ----------------- | ------------------------------------------------------------------------------------------------------ |
| Prozessor         | Intel-VT (Intel Virtualization Technology)<br>AMD-VT (AMD Virtualization Technology)<br>Hyperthreading |
| System / Hardware | Emulatoren<br>Virtuelle Machine (VMs)                                                                  |
| Betriebssystem    | Container<br>Zoning<br>Jails                                                                           |
| Anwendungen       | Laufzeitumgebungen<br>Sandboxed Applikationen                                                          |
| Desktop           | Terminalserver                                                                                         |
| Rechenzentrum     | SDDC (Software Defined Datacenter)<br>Cloud-Computing                                                  |
| RAM               | Auslagerungsdateien                                                                                    |
| Festplatten       | Partitionierung<br>Logical Volume Mapping                                                              |
| Storage           | Volumen                                                                                                |
| Netzwerke         | VLANs                                                                                                  |

## Virtuelle Machine (VM)
Virtuelle Machine sind komplett Virtuelle System, das heißt es wird schon auf dem Hardware level visualisiert.  Darauf kann mann sich genau verhalten wie auf einem Physischen gerät. 

### Warum benutzt man VMs
Virtuelle Maschinen kommen mit vielen Vorteilen. Einer der Größten und meist genannten Vorteile sind, **Platz und Ressourcen Effizienz**. Das bedeutet das man nicht für jedes Programm oder Software eine eigen Physischen Machine hinstellen muss und es in einer Machine zusammenfassen. Die **Ressourcen Effizienz** ist auch genannt, da man hart einen Dienst beschränken kann nur soviel Ressourcen zu nutzen und das laufen von mehren Dienste Parallel auf einer Physischen Machine, die sonst nie parallel Laufen könnten.

Es gibt aber weiter Vorteile die auch oft verwendet werden sind höher Sicherheit, Flexibilität und Optimierung von Software-Test und Entwicklung.

#### Vorteile
| Vorteil                       | Beschreibung                                                                                                                                                 |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Ressourcen Effizienz          | Mann kann mehrere Dienste parallel auf einer Physischen Machine Laufen lassen, die sonst nie auf der selben machine Laufen könnten.                          |
| Platz Effizienz               | Ähnlich wie die Ressourcen Effizienz kann mann viele Physische Machinen auf einen Starke Machine mit VMs vereint werden.                                     |
| Flexibilität                  | Virtuelle Machinen können einfach auf andere Servern verschoben oder Kopiert werden.                                                                         |
| höher Sicherheit              | Mann kann relative einfach Machinen von einander Isolieren, und schnell runtergerissen werden.                                                               |
| Legacy Support                | Es ermöglich auch Software die für alte Hardware Gebaut worden ist mit einer VM laufen zu lassen                                                             |
| Software-Tests & -Entwicklung | Erleichter Entwicklern deren Dienste für Hardware und Betriebssystem zu Entwickeln ohne eine Physischen Computer zu kaufen (Nicht möglich mit MacOS und IOS) |
### Nachteile
