---
title: "Modelos de protocolos de comunicación"
---

Existen diversos modelos que agrupan procedimientos a seguir para un conexión de red adecuada. Estos concentran protocolos de conexión bajo una estructura de capas, entre los más utilizados se encuentra el modelo OSI y el modelo TCP/IP.

## Modelo OSI
### Capa 7. Física
Se encarga de definir la topología de red y de las conexiones de la computadora hacia la red, se refiere tanto al medio físico (cables u ondas) como a la forma en la que se transmite la información
### Capa 6. Enlace de datos
Esta capa se ocupa del direccionamiento físico de la red, el acceso y comunicación con el medio físico, de la detección de errores en la conexión y de la distribución ordenada de tramas.
### Capa 5. Red
Se ocupa de identificar el enrutamiento existente en la red. Las unidades de datos se denominan paquetes, y se pueden clasificar en protocolos enrutablesy protocolos de enrutamiento.
### Capa 4. Transporte
Se encarga de proveer la funcionalidad y procedimientos para transferir las secuencias de datos de un emisor al destino (host) mientras mantener la calidad de servicio.
### Capa 3. Sesión
Controla los diálogos (conexiones) entre las computadoras. Establece, administra y elimina las conexiones entre las aplicaciones y la red.
### Capa 2. Presentación
Establece contexto entre las aplicaciones y la manera en laque se relacionan. Ofrece un mapeado para guiar las aplicaciones.
### Capa 1. Aplicación
Ofrece a las aplicaciones el acceso a los servicios de las demás.

![Modelo OSI](https://lh5.googleusercontent.com/proxy/a0d9qW5p_sZPDRFijfFH_ZDXgvxvcXooJs5BYkFyvwBxVyLm_kMHSsiwqn0foSJZhekQCJJWPwHk74b_H-25mwaf_bWjC2nbyqU6jQfWJOjfCcAzv3hY-vCfuaDUhnd-8SM8Cxvr1SsjbMQqBaVTL5e7gA7znVysZAS3qnPJb1tgMHZ0mSzxziDzlg=w1200-h630-p-k-no-nu)

## Modelo TCP/IP
### Capa 4. Aplicación
Esta capa realiza las funciones de las tres últimas capas del modelo OSI, aplicación, presentación y sesión. Es responsable de realizar conexiones de nodo a nodo y controlar la interfaz de usuario.
### Capa 3. Transporte
Esta capa es análoga a la capa de transporte del modelo OSI. Es responsable de realizar conexiones de punto a punto y evitar los errores en el transporte de los datos.
### Capa 2. Internet
Esta capa es el equivalente a la capa de red en el modelo OSI. Define los protocolos que son responsables para la transmisión de datos lógicos por la red.
### Capa 1. Acceso a red
Esta capa combina la capa física y de enlace de datos del modelo OSI. Busca el hardware que se utiliza, direcciones y protocolos presentes para la transmisión de datos.

![Modelo TCP/IP](https://upload.wikimedia.org/wikipedia/commons/7/73/Suite_de_Protocolos_TCPIP.png)
