# Netzwerk-Dokumentation interpretieren

### Ressourcen

- [Netzwerk-Dokumentation](https://gitlab.com/ch-tbz-it/Stud/m145/-/blob/main/10_Netzwerkdokumentation/02_Interpretieren/media/Netzwerkdoku1.pdf)

#### Fragen / Beantwortung

- Wie lautet die Netzwerkadresse vom Standort Samedan?

Wenn mit der Netzwerkadresse die IP des LANs vom Standort Samedan gemeint ist dann ist es die `192.168.3.0/24`. Die Public IP könnte auch gemeint sein, allerdings ist diese nicht in der Dokumentation ersichtlich. 

- Auf welcher IP-Adresse befindet sich der AccessPoint in Bellinzona?

Der Access Point in Bellinzona hat die IP `192.168.4.30`. 

- In welchem VLAN befinden sich die Arbeitsplatz-PCs?

Die Arbeitsplatz PC's befinden sich in VLAN 2. 

- Über welche IP-Adresse erreicht man den Manageable-Switch am Standort Chur?

Der Switch ist über die IP `192.168.2.253`. 

- Welche IP-Adressen LAN-seitig und tunnelseitig ist der VPN-Gateway am Standort Bellinzona konfiguriert?

Der VPN Gateway am Standort Bellinzona hat den Gateway `172.200.4.1`.

- Wie lautet der am Standort Samedan an den Arbeitsplatz-PCs eingetragene Standardgateway?

Der Standardgateway bei den Workstations am Standort Samedan ist `192.168.3.1`. 

- Ein Aussendienstmitarbeiter benötigt Zugriff auf das Firmennetzwerk. Wie muss er seine VPN-SW IP-mässig konfigurieren?

Der Gateway muss auf `ingcaprez.ch` zeigen und es wird, je nach dem ob die IP Zuweisung des VPNs dynamisch passiert (in der Doku steht dies nicht), eine IP der Netze 172.200.3.1/24, 72.200.4.1/24 und 72.200.5.1/24 zugewiesen sodass der Mitarbeiter Zugriff auf das Firmennetzwerk hat. 

- Wer hat im Büro CAD Wasserbau die VoIP-Telefone installiert?

`abisang` hat die Telefone im Büro CAD Wasserbau installiert. 

- Wann wurde im Bistro der AccesPoint installiert?

Der AP im Bistro wurde am 23.7.2014 installiert. 

- Der IT-Mitarbeiter Rene Sauter (rsauter) verlässt die Firma. Welche Arbeiten bzw. Verantwortlichkeiten sind davon betroffen? Wenn würden sie als zukünftigen Ansprechpartner bei Problemen vorschlagen?

Rene hat in fast allen Büros des Hauptsitzes Arbeiten vollbracht. Ich würde vorschlagen, dass `abisang` die Verantwortlichkeit von Rene übernehmen könnte, da sie in den gleichen Büros Arbeiten hatte. 

- Wieviele RJ45-Steckdosen stehen ihnen im Bauleiterbüro zur Verfügung und wieviele davon sind zurzeit noch nicht belegt?

Total sind es 8 Dosen und davon 2, die zur Verfügung stehen. 

- Im Büro CAD Tiefbau muss ein weiteres VoIP-Telefon zur Verfügung stehen. Wie soll diese Verbindung gepatched werden? Verlangt wird die Patchpanelbelegung und der Switch-Port.

Der Port E2/2 kann verwendet werden, dass heisst auf dem Switch muss noch ein weiter Port verwendet werden. Der Switch ist nicht dokumentiert also kann ich keine genau Angabe machen. 

- Im Bistro soll eine Projektpräsentation stattfinden. Dafür muss ein Ethernetkabelverbindung bereitgestellt werden.

Im Bistro sind noch 3 Ports verfügbar. E9/1 könnte dafür verwendet werden. 

- Im Büro CAD Wasserbau soll temporär ein weiterer Arbeitsplatz eingereichtet werden. Wie werden sie diese Aufgabe lösen?

Da im Wasserbau Büro alle Ports von Telefonen und Computern belegt sind würde ich einen Mini Switch nutzen um ein weiteres Telefon und Computer anschliessen zu können. 

- Wieviele Switchs stehen ihnen am Standort Chur zur Verfügung?

Zwei Switches und somit 48 Ports stehen in Chur zur Verfügung. 

- Frau Sommer arbeitet an der CAD-Workstation und meldet ihnen, dass sie keine Verbindung ins Internet mehr hat. Was werden sie überprüfen?

Ich würde überprüfen welche CAD-Workstation es betrifft, danach Prüfen ob das Kabel richtig eingesteckt ist beim Computer und letztlich die Funktionalität des Switches kontrollieren. 

- Wie lautet die SSID des Churer-AccessPoint?

Dies steht nicht in der Dokumentation, daher würde ich `rsauter` fragen gehen. 