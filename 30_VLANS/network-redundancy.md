# Network Redundancy

### Ressourcen

- [Theorie Network Redundancy](https://gitlab.com/ch-tbz-it/Stud/m145/-/blob/2d199c212962d6e78a25bb7cd4089841c95aae8a/31_Layer2_Redundanzen/README.md)

### Kontrollfragen

1. Welches grundlegende Problem verhindert das Spanning Tree Protocol (STP) in einem Layer-2-Netzwerk?
STP verhindert grundsätzlich Endlosschlaufen, die entstehen würden wenn man Switches, z.B in einem Dreieck, zusammensteckt. 

2. Aus welchen zwei Werten setzt sich die Bridge ID zusammen, die für die Wahl der Root Bridge entscheidend ist?
Die Bridge ID besteht aus der gesetzten Bridge ID und die Mac-Adresse des Switches. 

3. Warum dauert die Konvergenz bei klassischem 802.1D STP standardmäßig bis zu 30-50 Sekunden?
STP (802.1D) ist das klassische STP und die Konvergenz dauert ca. 30-50 Sekunden, weil starre Timer definiert sind, um den STP Tree zu berechnen. Beim neu berechnen des STP Baumes wird der Switch auf Listening gestellt, was genau 15 Sekunden dauert und danach auf Learning, welches auch 15 Sekunden dauert. Zusätzlich kommt das max Age dazu, welches 20 Sekunden dauern kann wenn, z.B ein anderer Switch einen kurzen Delay hat. 

4. Wofür wird der Befehl `spanning-tree portfast` genutzt und an welchen Ports sollte man ihn konfigurieren?
Der portfast Befehl kann auf Ports angewendet werden, die dann sofort in den Forwarding-Zustand wechseln, ohne die Listening/Learning Phase durchzumachen. Ports, an denen Clients angesteckt sind können niemals Loops verursachen, das heisst diese Ports sollten direkt in den Forwarding-Zustand wechseln. 
5. Warum reicht STP für die Netzwerkausfallsicherheit nicht aus, sodass wir Protokolle wie HSRP oder VRRP benötigen?
STP ermöglicht Layer 2 Ausfallsicherheit. Sobald der Router (Single Point of Failure) ausfällt, ist das Netzwerk lahm. HSRP und VRRP sind FHRP (First Hop Redundancy Protocols), um Router vor Ausfällen zu sichern. 
6. Was ist der Unterschied zwischen der physischen IP eines Routers und der virtuellen IP (VIP) bei HSRP?
Die physische IP eines Routers kann es nur einmal geben während virtuelle IPs auf mehreren Routern existieren können. 
7. Nenne zwei technische Unterschiede zwischen VRRP und HSRP (z.B. Multicast-Adresse, Terminologie).
Preemption ist bei HRRP standardmässig ausgeschaltet und die Multicast Adressen sind 224.0.0.2 (HSRP) und 224.0.0.18 (VRRPv2/3). 
8. Welchen Zweck erfüllt der Befehl `standby 10 preempt`?
Der Befehl aktiviert Preemption ohne Priorität. Das heisst ein anderer Router sollte active sein und dieser würde bei Ausfall des anderen übernehmen. 

9. Was ist der konzeptionelle Unterschied zwischen "Router-on-a-Stick" und der Nutzung von SVIs (Switched Virtual Interfaces)?
Bei Router on a Stick wird Inter VLAN Routing auf dem Router gemacht während bei SVIs dies auf einem Layer 3 Switch passiert. 
10. Welcher Befehl ist auf einem Router-Subinterface zwingend notwendig, damit es die VLAN-Tags eines bestimmten VLANs versteht?
`encapsulation dot1Q VLAN_ID` muss ausgeführt werden, damit der Router weiss welches VLAN Tag er beim senden und empfangen hinzufügen und entfernen muss. 

