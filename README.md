# FRONTEND_WPA_SUPPILCANT
Wifi_Network_Manager: | FRONTEND WPA SUPPLICANT |  PYQT5, PYTHON3  version alpha 1.0

FRONTEND para manejar perfiles de RED WIFI con WPA_SUPPLICANT.

Dados los datos (ESSID, ENCRIPTACION, CLAVE), genera un fichero wpasupplicant.conf para realizar la conexión WIFI.

Guarda el fichero en formato especificado por WPASUPPLICANT.

Ejemplo:
__________________________________________
ctrl_interface=/var/run/wpa_supplicant
network={
   ssid="TELEFONICA_WIFI"
   key_mgmt=WPA-PSK
   psk="CLAVEWIFI"
___________________________________________

Una vez generado el fichero lanza wpa_supplicant para realizar la conexión:        
        wpa_supplicant -c/etc/wpa_supplicant/NOMBREDEESSID.conf -iwlan1 &

Hasta aquí la version 1.0. 

Falta acabar de implementar el WIFIRADAR para ver las WIFIS cercagas y conectar a ellas con click.
Y gestion de perfiles WIFI generados guardados con extension .SAVE.


