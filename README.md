# README

**Descripción breve**

Proyecto Arduino que mueve un servo con un sensor de ultrasonidos (HC-SR04) para escanear un sector. Mientras escanea, un LED verde está encendido. Si el sensor detecta un objeto a menos de 20 cm, el servo que porta el sensor se detiene y se activa otro servo que hace un barrido preciso sobre el objeto; mientras dura ese barrido se enciende un LED rojo y suena un zumbador. Al terminar el barrido el sistema vuelve a escanear.

**Conexiones**

LED rojo → Pin 1 (a través de resistencia 220Ω)

LED verde → Pin 2 (a través de resistencia 220Ω)

HC-SR04 TRIG → Pin 3

HC-SR04 ECHO → Pin 4

Servo sensor (giro) → Pin 5

Servo barrido → Pin 6

Buzzer → Pin 7 (opcional si quieres otro pin puedes cambiarlo en el código)

GNDs todos comunes (Arduino, servos, sensor, buzzer)

VCC del sensor y servos → 5V (si usas fuente externa para servos, conecta GNDs)
