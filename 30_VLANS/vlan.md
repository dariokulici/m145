# VLAN

## Überblick

VLAN ist ausgeschrieben Virtual Local Area Network und bewegt sich auf Layer 2 des ISO/OSI Modells. Damit können Netzwerke logisch getrennt werden und Ressourcen des Netzwerks optimiert werden. VLANs ermöglichen eine höhere Sicherheit und verbessertes Management. 

### Vorteile
- mehr Sicherheit durch logische Trennung des Netzwerks (bspw. Buchhaltung sieht nicht was Security Team versendet)
- verbessertes Management, dadurch dass das Netzwerk in mehrere Netzwerke eingegliedert ist. 
- Ressourcen Einsparungen, weil die Broadcast Domäne nicht mehr alle Geräte beinhaltet. 

### Nachteile
- menschliche Fehler bei Konfiguration machen Brainstorming sehr schwierig
- erhöhter Dokumentationsaufwand

<br>

## Situation

Eine Firma hat zwei Switches, die Stock 1 (Switch 1) und 2 (Switch 2) miteinander verbinden. In beiden Stöcken hat es Einzelbüros wo die Geschäftsleitung arbeitet. Es sollen zwei VLANs für einerseits die Geschäftsleitung und die Mitarbeiter erstellt werden. 

| VLAN ID | Zweck            |
| ------- | ---------------- |
| 100     | Geschäftsleitung |
| 200     | Mitarbeiter      |

Jeder Switch hat 12 Ports. Port 12 auf beiden Switches wird als Trunk Port konfiguriert und geht von Switch 1 auf Switch 2. Auf beiden Switches werden die VLANs entsprechend der oberen Tabelle erstellt. Pro Stock gibt es zwei Einzelbüros, die für die Geschäftsleitung sind. 

### Switch 1

| Port | Type   | VLAN     |
| ---- | ------ | -------- |
| 1    | Access | 200      |
| 2    | Access | 200      |
| 3    | Access | 200      |
| 4    | Access | 200      |
| 5    | Access | 200      |
| 6    | Access | 200      |
| 7    | Access | 200      |
| 8    | Access | 200      |
| 9    | Access | 200      |
| 10   | Access | 100      |
| 11   | Access | 100      |
| 12   | Trunk  | 100, 200 |

### Switch 2

| Port | Type   | VLAN     |
| ---- | ------ | -------- |
| 1    | Access | 200      |
| 2    | Access | 200      |
| 3    | Access | 200      |
| 4    | Access | 200      |
| 5    | Access | 200      |
| 6    | Access | 200      |
| 7    | Access | 200      |
| 8    | Access | 200      |
| 9    | Access | 200      |
| 10   | Access | 100      |
| 11   | Access | 100      |
| 12   | Trunk  | 100, 200 |


