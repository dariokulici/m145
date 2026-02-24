# Monitoring

Die grundlegenden Komponenten der Netzwerküberwachung sind:

- IP Adressen und Subnetze
- Switching und Routing
- DNS
- DHCP

Netzwerküberwachung deckt drei von fünf Ziele des Netzwerkmanagements ab: **Leistungsüberwachung, Fehlerüberwachung und Kontoüberwachung**. 

<br>

### Überwachungstechniken und Protokolle

Folgende Punkte sind zwingend nötig, um Netzwerke, Server oder Systeme erfolgreich zu überwachen. 

- Daten und Informationen von Elementen im Netzwerk. Die Daten beinhalten Informationen über die Funktionsweise, den aktuellen Status, der Leistung und Gesundheit des Elements. Beispielsweise wird ein Mailserver betrieben. Somit muss geprüft werden, ob die Mailserver Applikation läuft und die API Endpoints erreichbar (healthy) sind. 
- Die Applikation oder Überwachungssoftware muss Daten in einem benutzerfreundlichen Format sammeln, sie verarbeiten und darstellen können. Zudem sollen Benutzer über bevorstehende Probleme auf Grundlage der Schwellenwerte informiert werden. Beispielsweise wird ein Administrator per Mail benachrichtigt, dass der Mailserver 80% Festplattenkapazität überstiegen hat und kann somit Massnahmen einleiten. 
-  Ein Protokoll oder Methode, um die Informationen vom überwachten Element zur Überwachungssoftware zu übertragen. 

<br>

### Ping
Mit Ping (ICMP) kann der Status eines Geräts geprüft werden ob der Host aktiv ist oder nicht. 

### SNMP
Das Simple Network Management Protocol ist zum Austausch von Informationen zwischen Hosts in einem Netzwerk da. Folgende Komponenten sind vorhanden:

- Verwaltetes Gerät (Das Gerät welches verwaltet werden soll)
- Agent (Ein Programm, welches auf dem überwachten Gerät installiert ist, die Daten an den Überwachungsserver sendet)
- Netzwerkverwaltungssystem (Der Monitoring Server, welcher die Daten von den Hosts erhält)

### Syslog
Syslog ist ein Protokoll, welches Ereignisbenachrichtigungen übers Netzwerk zu senden. Viele Geräte, z.B Druckern, Router oder Firewall, unterstützen Syslog. 

### Skripte
Wenn bestimmte Funktionen nicht von einem NMS angeboten werden, können Skripte verwendet werden, um das neue Feature zu schaffen. Bash, Perl oder Python Skripte sind gängige Programmiersprachen um solche Skripte zu erstellen. 

### FCAPS
FCAPS sind 5 verschiedene Kategorien des Netzwerkmanagements