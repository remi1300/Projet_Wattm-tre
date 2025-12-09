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

## Connection au WIFI 
#define EAP_IDENTITY "ewan.michellon@etu.univ-amu.fr"
#define EAP_PASSWORD "!"
#define EAP_USERNAME "ewan.michellon@etu.univ-amu.fr"
const char* ssid = "eduroam";
const char* ssid = "eduroam";
## Utilisation du MQTT
## Calibration des capteurs 
## Traitement 
## Affichage 
Les valeurs récuperées avec le programme vont être envoyées sur un Node-red. 
