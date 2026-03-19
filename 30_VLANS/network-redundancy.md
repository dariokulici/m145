# Network Redundancy

### Ressourcen

- [Theorie Network Redundancy](https://gitlab.com/ch-tbz-it/Stud/m145/-/blob/2d199c212962d6e78a25bb7cd4089841c95aae8a/31_Layer2_Redundanzen/README.md)

### Kontrollfragen

1. Welches grundlegende Problem verhindert das Spanning Tree Protocol (STP) in einem Layer-2-Netzwerk?
STP verhindert grundsätzlich Endlosschlaufen, die entstehen würden wenn man Switches, z.B in einem Dreieck, zusammensteckt. 

2. Aus welchen zwei Werten setzt sich die Bridge ID zusammen, die für die Wahl der Root Bridge entscheidend ist?
Die Bridge ID besteht aus der gesetzten Bridge ID und die Mac-Adresse des Switches. 

3. Warum dauert die Konvergenz bei klassischem 802.1D STP standardmäßig bis zu 30-50 Sekunden?
STP (802.1D) ist das klassische STP und die Konvergenz dauert ca. 30-50 Sekunden, weil starre Timer lange brauchen, um herauszufinden ob ein Loop entsteht. 

4. Wofür wird der Befehl `spanning-tree portfast` genutzt und an welchen Ports sollte man ihn konfigurieren?

5. Warum reicht STP für die Netzwerkausfallsicherheit nicht aus, sodass wir Protokolle wie HSRP oder VRRP benötigen?
6. Was ist der Unterschied zwischen der physischen IP eines Routers und der virtuellen IP (VIP) bei HSRP?
7. Nenne zwei technische Unterschiede zwischen VRRP und HSRP (z.B. Multicast-Adresse, Terminologie).
8. Welchen Zweck erfüllt der Befehl `standby 10 preempt`?
9. Was ist der konzeptionelle Unterschied zwischen "Router-on-a-Stick" und der Nutzung von SVIs (Switched Virtual Interfaces)?
10. Welcher Befehl ist auf einem Router-Subinterface zwingend notwendig, damit es die VLAN-Tags eines bestimmten VLANs versteht?

