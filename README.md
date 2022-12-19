# Humidity-Controller
Humidity-Control, basierend auf einem ESP8266, bestimmt die Temperatur und die relative Luftfeuchtigkeit im Innen- und Außenbereich. Aus diesen Messdaten wird jede Minute für den Innen- und Außenbereich jeweils die absolute Luftfeuchtigkeit in g/m³ berechnet. In Abhängigkeit einer dynamischen Hystereseschwelle kann über ein Relais ein Lüfter angesteuert werden. Liegt die absolute Feuchte im Innenraum über der absoluten Feuchte im Außenbereich und ist die minimale Außentemperatur noch nicht erreicht, wird der Lüfter eingeschaltet. Die Hysterese wird automatisch dynamisch über die minimale Außentemperatur und die Genauigkeit der Feuchtesensoren berechnet. 
Das Zusamenspiel der einzelnen Komponenten zeigt die nachfolgende Abbildung.

![Übersicht](https://github.com/Feinmechaniker/Humidity/blob/main/06%20Website/overview.jpg)

Optional können auf einem OLED-Display die aktuellen Temperaturen und die absoluten Feuchten abgelesen werden.

![OLED](https://github.com/Feinmechaniker/Humidity/blob/main/06%20Website/OLED.jpg)

## Dashboard lokal
Ein Dashboard auf einem lokalen Webserver des Controllers ermöglich Abfrage bzw. Änderung
- des Schaltzustandes des Lüfters
- der minimalen Schalttemperatur
- der Temperaturen im Innen- und Außenbereich
- der relativen und absoluten Luftfeuchtigkeiten im Innen- und Außenbereich

![Dashboard](https://github.com/Feinmechaniker/Humidity/blob/main/06%20Website/dashboard.jpg)

## Dashboard Grafana
Bei Bedarf werden sowohl die Messdaten als auch die daraus berechneten Ergebnisse über MQTT an eine Datenbank gesendet. Diese können dann über eine grafische Visualisierung wie z.B. Grafana dargestellt werden. 

![Grafana](https://github.com/Feinmechaniker/Humidity/blob/main/06%20Website/grafana.jpg)

(c) 2022 Joe.G
