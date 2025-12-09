# Projet Wattmètre 
![Logo de mon domaine](https://mondomaine.fr/logo.png) <br>
<br>
Ce projet réalisé par des étudiants à pour objectif de réaliser un Wattmètre à partir d'un ampèrmetre et un d'un voltmètre. 
L'association de ces deux capteurs de courant et tension altenative permet d'otenir une valeur de puissance. 


## Materiel utilisé 
* ESP32
* Pince ampèremétrique : AC Current Sensor V1.0 (DFRRobot) 
* Voltmètre : Grove AC Voltage Sensor
* Conditionneur

## Les librairies 

Concernant les capteurs :
* "MCMVoltSense.h"

Concernant l'ESP32 : 
* <Arduino.h>
* "PubSubClient.h"
* "PubSubClient.h"
* "WiFi.h"
* "esp_wpa2.h"

## Affichage 
Les valeurs récuperées avec le programme vont être envoyées sur un Node-red. 
