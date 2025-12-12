# Projet Wattmètre 
![image](https://aircarto.fr/images/ModuleAir_InstaWhite.jpg) <br>
<br>
Ce projet réalisé par des étudiants à pour objectif de réaliser un Wattmètre à partir d'un ampèrmetre et un d'un voltmètre. 
L'association de ces deux capteurs de courant et tension altenative permet d'otenir une valeur de puissance. 

## Materiel utilisé 
* ESP32
* Pince ampèremétrique : AC Current Sensor V1.0 (DFRRobot) 
* Voltmètre : Grove AC Voltage Sensor
* Conditionneur

## Les librairies 

* <Arduino.h>
* "PubSubClient.h"
* "WiFi.h"
* "esp_wpa2.h"

## Configuration du WIFI et MQTT 

```
#define EAP_IDENTITY ""
#define EAP_PASSWORD ""
#define EAP_USERNAME ""
const char* ssid = "";
const char* ssid = "eduroam";
const char *mqtt_broker = "";
const int mqtt_port = 1883;
```
```
const char *topic_I_eff = "courrantefficace";
const char *topic_U_eff = "tensionefficace";
const char *topic_Phase = "dephasage";          
const char *topic_P_app = "puissanceapparente";
const char *topic_P_act = "puissanceactive";
WiFiClient espClient;
PubSubClient client(espClient);
```

## Calibration des capteurs 

```
const int Pin_Voltage = 34;
const int Pin_Current = 35;

const float FACTOR_CURRENT = -0.0161;
const float FACTOR_VOLTAGE = 0.13;

const float PHASE_ERROR_OFFSET = 9.0;

const int N = 100; // Echantillons
int Uraw[N];
int Iraw[N];
 ```





## Traitement 
## Affichage 
Les valeurs récuperées avec le programme vont être envoyées sur un Node-red. 
