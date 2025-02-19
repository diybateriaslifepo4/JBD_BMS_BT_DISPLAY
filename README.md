# PANTALLA BMS JBD BLUETOOTH
UNA SOLUCIÓN FÁCIL Y BARATA PARA EL PROBLEMA DE SEGURIDAD DE LOS BMS JBD

Me he decidido a crear esta solcuión debido al importante problema de seguridad que hay con todas las baterías LiFePO4 que montan el bms de marca JBD con acceso bluetoth
Este problema lo explico en el video de youtube https://www.youtube.com/watch?v=i-yVY5qM5bE

La solución se basa en un display que se conecta por bluetooth con nuestra batería, bloqueando así el acceso a terceros malintencionados.
Está basado en ESPHome y mezcla código de creación propia (la parte del display), con código tomado del proyecto de SISSY (https://github.com/syssi/esphome-jbd-bms) para comunicar el ESP32 con ESPHome
https://github.com/syssi/esphome-jbd-bms

PARA QUE FUNCIONE CON TU BATERÍA TIENES QUE PONER LA MAC CORRESPONDIENTE EN EL YAML
Generar el firmware BIN con ESPHOME y flashear directamente o desde ESPHOME WEB
Al funcionar con ESPHome también se puede integrar de forma nativa en Home Assistant, solamente descomentando la línea Api: 
También se puede tener una interfaz web accesible por red local si descomentamos las líneas del web_server:

El código es totalmente libre y puede ser usado como referencia para adaptarlo a tus necesidades, solo te pido mostrar las fuentes de referencia.

![image](https://github.com/user-attachments/assets/8c752d76-68f1-40ea-9e28-1a3763701e57)

References
https://github.com/syssi/esphome-jbd-bms
https://esphome.io/components/touchscreen/axs15231.html
https://esphome.io/components/display/qspi_dbi.html
https://esphome.io/components/display/
https://esphome.io/components/lvgl/
www.bateriaslifepo4.com
