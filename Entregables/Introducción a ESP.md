# INTRODUCCIÓN A ESP32

## 1.- ¿Qué es ESP32?
Es un microcontrolador de un coste bajo que cuenta con la posibilidad de conectarse a Internet y Bluetooth, esto, principalmente, debido a que está diseñado para IoT (Internet of Things o Internet de las cosas en español). Para la realización de nuestro proyecto, el ESP32 nos permite recibir los resultados obtenidos de la medición de pH y turbidez mediante conexión a la red, evitando así cableados que podrían resultar tediosos y dificultar la portabilidad que se tiene pensada.
Con la finalidad de aprender más sobre el uso de este microcontrolador, se propuso lo siguiente:

## 2.- Actividad propuesta:
Ploteo de la lectura de un potenciómetro como divisor de tensión en un puerto analógico del ESP32 o ESP8266

## 3.- Herramientas utilizadas:
- ESP-WROOM-32
- Potenciómetro
- Laptop
- Cable USB-B
- Protoboard
- Kit A y B

## 4.- Procedimiento:
1. Primero, se conectó la laptop al ESP32 haciendo uso del cable USB-B, esto con el propósito de poder vincular ambos dispositivos y ver los resultados al momento de correr el código.
<p align="center">
  <img src="https://github.com/aquinoestoyxd/FD-Grupo2/blob/main/Imágenes/esp32(1).jpg?raw=true" alt="Imagen 1"
</p>
 
2. Luego, se identificaron los puertos a utilizar para la conexión a GND, 3.3V y un pin que se usaría para la parte del código, todo ello en base al mapa del modelo:
<p align="center">
  <img src="https://github.com/aquinoestoyxd/FD-Grupo2/blob/main/Imágenes/esp32(2).png?raw=true" alt="Imagen 1"
</p>
<p align="center">
  <img src="https://github.com/aquinoestoyxd/FD-Grupo2/blob/main/Imágenes/esp32(3).jpg?raw=true" alt="Imagen 1"
</p>

3. Para finalizar con las conexiones del ESP32, se conectaron los cables de GND, 3.3V y el pin34 a un protoboard con el potenciómetro. La idea es que, al girar este elemento, en la laptop se refleje un cambio en la lectura.
<p align="center">
  <img src="https://github.com/aquinoestoyxd/FD-Grupo2/blob/main/Imágenes/esp32(4).jpg?raw=true" alt="Imagen 1"
</p>


4. Finalmente, se ejecutó el código en Arduino IDE, y en el Serial Monitor se vieron reflejados los cambios de lectura de acuerdo al movimiento del potenciómetro.
<p align="center">
  <img src="https://github.com/aquinoestoyxd/FD-Grupo2/blob/main/Imágenes/esp32(5).png?raw=true" alt="Imagen 1"
</p>

**Link de Funcionamiento**

https://drive.google.com/drive/folders/1i0GfJTXejX1uP06ug9ueC-nii7gR1SB6?usp=share_link
 
## 5.- Código utilizado:
<p align="center">
  <img src="https://github.com/aquinoestoyxd/FD-Grupo2/blob/main/Imágenes/esp32(6).png?raw=true" alt="Imagen 1"
</p>

## 6.- Errores y soluciones:
- Al inicio hubo problemas al momento de realizar las conexiones, esto porque el modelo otorgado en el laboratorio era distinto al presentado en clase, por tanto, la ubicación de los pines también era distinta. Anteriormente se mostró el mapa del esp32 utilizado, abajo se adjunta el mapa del modelo enseñado en la clase.
<p align="center">
  <img src="https://github.com/aquinoestoyxd/FD-Grupo2/blob/main/Imágenes/esp32(7).png?raw=true" alt="Imagen 1"
</p>

- Pese a la correcta instalación de librerías, hubo problemas al momento de ejecutar el código. Esto porque, al menos para el modelo empleado, se tenía que mantener pulsado el botón Boot situado en la parte trasera del esp32, esto hasta que aparezca Conecting en la consola, el botón EN, por su parte, debía pulsarse por 1 segundo.
