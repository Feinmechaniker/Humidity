# Humidity-Controler
Humidity-Control bestimmt die Temperatur und die relative Luftfeuchtigkeit im Innen- und Außenbereich. Aus diesen Messdaten wird jede Minute für den Innen- und Außenbereich jeweils die absolute Luftfeuchtigkeit in g/m³ berechnet. In Abhängigkeit einer dynamischen Hystereseschwelle kann über ein Relais ein Lüfter angesteuert werden. Liegt die absolute Feuchte im Innenraum über der absoluten Feuchte im Außenbereich und ist die minimale Außentemperatur noch nicht erreicht, wird der Lüfter eingeschaltet. Die Hysterese wird automatisch dynamisch über die minimale Außentemperatur und die Genauigkeit der Feuchtesensoren berechnet. Auf einem OLED-Display können die aktuellen Temperaturen und die absoluten Feuchten abgelesen werden.

![OLED](https://github.com/Feinmechaniker/Humidity/blob/main/06%20Website/OLED.jpg)

## Dashboard
Ein Dashboard ermöglich Abfrage bzw. Änderung
- des Schaltzustandes des Lüfters
- der minimalen Schalttemperatur
- der Temperaturen im Innen- und Außenbereich
- der relativen und absoluten Luftfeuchtigkeiten im Innen- und Außenbereich

![Dashboard](https://github.com/Feinmechaniker/Humidity/blob/main/06%20Website/dashboard.jpg)

(c) 2022 Joe.G
