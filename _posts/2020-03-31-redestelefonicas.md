---
title: "Redes telefónicas y voIP"
---

VoIP o la voz sobre el protocolo de internet hace referencia a una tecnología que agrupa recursos que hacen posible que las ondas producidas y encapsuladas en señales de la voz, viaje a través de Internet mediante el protocolo de paquetes IP; es decir, la señal producida por la voz es enviada de manera digital en paquetes de datos con valores discretos de 1s y 0s, en lugar de ser enviada de forma analógica con valores continuos a través de circuitos que utiliza la telefonía tradicional, es decir, las redes telefónicas conmutadas.

## Elementos de la voIP

### Cliente

El cliente es quién establece las llamadas de voz con su infraestructura de entrada (micrófono del usuario), que después de codifica, empaqueta y se envía, para luego decodificarse y reproducirse en la salida de otro usuario (altavoces o auriculares).

### Servidores

Los servidores manejan las operaciones de conexión entre usuarios y hosts en tiempo real. Algunas de sus operaciones son la contabilidad, recolección, administración, monitoreo, control y enrutamiento del registro de usuarios.

### Gateways o puertas de enlace

Las puertas de enlace brindan una conexión entre todos los usuarios con el fin de proveer interfaces con las telefonía tradicional, que funcionará como la plataforma para los clientes.

#### Arquitectura de red
Consiste en tres elementos fundamentales:

- Terminales: Dispositivo parecido a un teléfono que permite transmitir y recibir datos utilizando una red IP. Utiliza una conexión de red de datos, en lugar de una conexión de red telefónica.
![Terminal IP](https://f0.pngfuel.com/png/290/658/yealink-ip-phone-sip-t-voip-phone-terminal-ip-session-initiation-protocol-telephone-voip-png-clip-art.png)
- Gatekeepers: Organizan la voIP y sustituyen las centrales telefónicas. Todas las comunicaciones pasan por este software.
- Gateways: Brindan una conexión entre todos los usuarios con el fin de proveer interfaces con las telefonía tradicional, que funcionará como la plataforma para los clientes.

### Parámetros de la VoIP

El principal problema y desventaja de la VoIP y en general de las aplicaciones que utilizan los paquetes IP es garantizar la mejor calidad de servicio (QoS o quality of service) en el internet debido a las limitaciones de ancho de banda que causa problemas como los siguientes.

#### Códecs

Los códecs tienen la función de codificar el audio (para esta aplicación, la voz) para que pueda ser transmitida por los paquetes IP. Los códecs garantizan una correcta codificación y comprensión de media para que luego no existan problemas de decodificación y descompresión antes de generar la media en el dispositivo receptor.

Los códecs afectan el ancho de banda puesto que requieren el mismo para la codificación y decodificación de los datos. Según el códec utilizado en la transmisión, se utilizará un valor de ancho de banda u otro establecido, sin embargo, también se debe tener en cuenta el tamaño de los datos y el tráfico de otras capas en la red.

| Códec | Ancho de banda de codificación |
|:-----:|:------------------------------:|
|  GSM  |             13kbps             |
|  iLBC |             15kbps             |
| G.711 |           56 a 64kbps          |
| G.722 |         48, 56 a 64kbps        |
| G.723 |          5.3 a 6.4kbps         |
| G.726 |       16, 24, 32 a 40kbps      |
| G.728 |             16kbps             |
| G.729 |           8 a 13kbps           |
| Speex |         2.15 a 44.2kbps        |

#### Retardo o latencia

Debido al retardo por el tráfico de red o por el procesamiento se pueden producir pérdidas de tramas durante el recorrido por la red IP donde ciertos tramos de la señal pueden perderse, que en el caso de llamadas, no es práctico hacer su retransmisión debido a que puede ocasionar retardos adicionales o confusión en la salida del receptor por silabas que suenan de la nada durante la transmisión. Sin embargo, existen sistemas de interpolación para estas situaciones, donde basándose en muestras de voz previas el decodificador puede completar las tramas perdidas (técnica PLC).

#### Calidad del servicio

La calidad de servicio de un sistema se mide por diversos parámetros de velocidad y exactitud durante la transmisión de datos.

 - Entrega. Los datos deben de ser recibidos por el dispositivo adecuado.
 - Exactitud. Los datos que se alteran en la transmisión deben ser los correctos sean de una señal analógica a digital o viceversa, de lo contrario son incorrectos.
 - Puntualidad. Los datos entregados tarde suelen perder relevancia, la entrega puntual significa entregar los datos a medida que se producen, en el mismo orden en que se producen y sin retraso significativos. Este tipo de entregas se llama transmisión en tiempo real.
 - Jitter (retardo variable). Se refiere a la variación en el tiempo de llegada de los paquetes de datos. En el retraso inesperado en la entrega de paquetes de audio o video, por ejemplo asumamos que los paquetes de video llegan cada 30s. Si algunos llegan en 30s y otros con 40s, el resultado es una mala calidad del video.

##### Métodos básicos de calidad de servicio

 - Mejor esfuerzo. Envía paquetes como los recibe, no aplica ninguna tarea de procesamiento en ellos y por lo tanto no existe garantía de calidad.
 - Servicios integrados. Tiene como función definir un camino para los datos que tienen prioridad, sin embargo, no es un método escalable por la cantidad de recursos que se necesitan para reservar ancho de banda para cada dato, pero asegura un trato preferente con ciertos datos prioritarios tendrán mayor prioridad en tráfico con menor probabilidad de causar errores por congestión.
 - Servicios diferenciados. Cada dispositivo tiene la responsabilidad de manejar paquetes de manera individual, y configurar sus propias políticas de QoS. Con ello se puede brindar mayor servicio.
