# PANTALLA BMS JBD BLUETOOTH
UNA SOLUCIÓN FÁCIL Y BARATA PARA EL PROBLEMA DE SEGURIDAD DE LOS BMS JBD<br/>
<br/>
Me he decidido a crear esta solución debido al importante problema de seguridad que hay con todas las baterías LiFePO4 que montan el bms de marca JBD con acceso bluetoth<br/>
Este problema lo explico en el video de youtube https://www.youtube.com/watch?v=i-yVY5qM5bE<br/>
<br/>
La solución se basa en un display que se conecta por bluetooth con nuestra batería, bloqueando así el acceso a terceros malintencionados.<br/>
Está basado en ESPHome y mezcla código de creación propia (la parte del display), con código tomado del proyecto de SISSY para comunicar el ESP32 con ESPHome por BT<br/>
<br/>
PARA QUE FUNCIONE CON TU BATERÍA TIENES QUE PONER LA MAC CORRESPONDIENTE EN EL YAML<br/>
Generar el firmware BIN con ESPHOME y flashear directamente o desde ESPHOME WEB<br/>
Al funcionar con ESPHome también se puede integrar de forma nativa en Home Assistant, solamente descomentando la línea Api: <br/>
También se puede tener una interfaz web accesible por red local si descomentamos las líneas del web_server:<br/>
<br/>
El código es totalmente libre y puede ser usado como referencia para adaptarlo a tus necesidades, solo te pido mostrar las fuentes de referencia.<br/>
<br/>
## **Requerimientos**
Pantalla JC4832W535
https://s.click.aliexpress.com/e/_oo1Pjho<br/>

![image](https://github.com/user-attachments/assets/8c752d76-68f1-40ea-9e28-1a3763701e57)
<br/>
## **Referencias**
https://github.com/syssi/esphome-jbd-bms<br/>
https://esphome.io/components/touchscreen/axs15231.html<br/>
https://esphome.io/components/display/qspi_dbi.html<br/>
https://esphome.io/components/display/<br/>
https://esphome.io/components/lvgl/<br/>
www.bateriaslifepo4.com<br/>
