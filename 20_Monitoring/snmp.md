# SNMP

Das Simple Network Management Protocol dient zur Überwachung von Geräten. 

### Kontrollfragen

- Welche Hauptkomponenten umfasst SNMP?​

Der Netzwerk Manager, der Agent und die MIB Datenbank. 
   
- Auf welchen Ports arbeitet SNMP standardmäßig?​

161, 162 und bei Verschlüsselung 10161, 10162. 
   
- Was ist eine MIB (Management Information Base) in SNMP?​

Sie enthält die Möglichen Einträge und ist für jedes Gerät anders. Sie wird nicht mit dem Agent mitgeliefert. 
   
- Welche SNMP-Versionen gibt es und welche Sicherheitsunterschiede bestehen zwischen ihnen?​

Version 1 ist am unsichersten und hat wenig Funktionalität. Version 2c ist sicherer und hat ein wenig mehr Funktionen. Version 3 ist sicher, da sie heutige Sicherheitsstandard einhält, ist aber komplex um einzurichten. 

- Welche grundlegenden SNMP-Operationen gibt es und wofür werden sie verwendet?​

Get, um Daten zu holen, Set um Werte zu definieren und Trap um Benachrichtigungen zu senden bei plötzlichen Events. 
   
- Was ist der Unterschied zwischen SNMP-Traps und Polling?​

Beim Polling werden konstant Daten vom Manager abgefragt während Traps von einem Host bei Events ausgelöst werden. 
   
- Wie wird die Authentifizierung und Verschlüsselung in SNMPv3 verbessert?​

SNMP 1 und 2 haben keine Verschlüsselung daher ist bei SNMP 3 schon mal gut, dass es überhaupt verschlüsselt wird. 
   
- Welche Rolle spielt der SNMP-Agent und wo wird er eingesetzt?​

Er wird auf den Hosts installiert und ist zuständig dafür um Daten des Geräts zu senden. 

- Was ist eine OID (Object Identifier) und wofür wird sie verwendet?​

Ein Object Identifier die Identifikation der Werte, die ausgelesen werden können. Er muss bei einer Operation angegeben werden, damit klar ist welche Daten ausgelesen werden sollen. 

- Wie kann man den Zugriff auf SNMP-Daten sicherer gestalten?​

SNMP 3 nutzen und Best Practices anwenden beim Setup. 