# Modem GSM #
## 1. Leds ##
Distribución de los leds de izquierda a derecha:
+ Parte frontal:
 1. Operación
 2. Estado
 3. Red Celular / Saldo
 4. Señal Celular
 5. Puerto USB
+ Parte posterior:
 6. Pulsador de encendido/apagado
 7. Conector de alimentación
 8. Conector de antena celular

## 2. Instalación y configuración
Antes de instalar el modem, posiciónelo en un lugar donde exista buena recepción celular. Luego siga los siguientes pasos:
- Conectar la fuente de alimentación.
- Conectar un extremo del cable USB al modem.
- Conectar el otro extremo a la PC.
- Presionar el pulsador por un segundo o hasta que el led de Operación esté encendido.
El modem iniciará el proceso de instalación y el sistema operativo reconocerá el nuevo dispositivo. 

### 2.1 Instalación del driver
En la PC, cuando el sistema operativo solicite buscar un driver, utilice el driver proporcionado: `“Universal GSM Modem driver”`.

En caso contrario abra el Administrador de Dispositivos, para hacer esto debe de haber iniciado sesión como Administrador.

Comando para abrir el Administrador de Dispositivos: `mmc devmgmt.msc`
- Seleccione el nuevo dispositivo detectado.
- Click derecho, Actualizar software de controlador.
- Buscar software de controlador en el equipo.
- Click en Examinar…
- Seleccione la carpeta: “Universal GSM Modem driver”, Aceptar.
- Click en Siguiente.
- Iniciará el proceso de instalación del dispositivo.
Al finalizar la instalación correctamente el led de Operación permanecerá encendido contantemente.
Ingrese nuevamente al Administrador de Dispositivos y en la sección Puertos (COM y LPT) identifique el nuevo dispositivo instalado con el nombre `“USB Serial Port”`, anote el nombre del puerto asignado.

### 2.2 Configuración del Modem
Después de la instalación del driver en la PC, el modem empezara a configurarse.

El led de Estado se encenderá cuando el modem termine de iniciarse.

El led de Red Celular se encenderá cuando el modem logre comunicarse con alguna antena celular cercana. En caso contrario parpadeara junto con el led de Estado.

El led de Señal Celular parpadeara alternadamente con el led de Red Celular indicando que el Modem esta consultado en “Saldo” de la tarjeta SIM del modem. Si no se cuenta con saldo en la tarjeta SIM, solo un led quedara encendido.

Si la configuración del termina correctamente los cuatro leds permanecerán encendidos.

En algunos casos el led Señal Celular parpadeara de acuerdo a la intensidad de la señal que recibe la antena del modem de la siguiente manera:
- Intensidad excelente: led prendido.
- Intensidad buena: parpadeo rápido.
- Intensidad baja: parpadeo lento.
- Intensidad nula o muy baja: led apagado.