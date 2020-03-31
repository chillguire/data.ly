---
title: "Operaciones y técnicas de manejo de ondas y señales"
---

Las redes de comunicaciones tienden a ser más complejas conforme el número de usuarios utilizándolas aumenta, por lo tanto, si no está bien diseñada con posibles problemas pensados de antemano, esta red colapsará. Es por esto, que existen reglas esenciales que se deben cumplir para la creación de un sistema de comunicación, como que el sistema al entregar la información debe transmitirla sin cambios en su integridad, debe garantizar que los datos llegarán únicamente donde se tiene previsto con el fin de no tener problemas de privacidad y la información debe llegar en el menor tiempo posible previsto con el menor retraso. 
Esto se logra con técnicas que permiten modificar ondas electromagnéticas para transmitir información modificando ciertos parámetros de la misma, o haciendo que varias señales de la onda se transmitan por un mismo medio, entre otros artificios capaces de modificar ondas con un fin en específico. Las principales técnicas son las siguientes:

## Modulación
Se refiere al conjunto de técnicas utilizadas para almacenar información dentro de una onda. Se logra variando de manera extrema alguna característica de la onda, sea la anchura, la frecuencia o adelantando/retrasando la fase una cantidad extrema de grados (de 180º en adelante). Esto hace que sea mucho más rápido la de-modulación de la onda por parte del receptor.
### PAM - Modulación por amplitud de pulsos
Es una técnica de modulación en señales analógicas donde la fase y la frecuencia no varia mientras que la amplitud de la onda sí, mediante la elección de la separación en ciertos puntos de la onda.

![PAM](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e2/PAM_neutral.svg/1200px-PAM_neutral.svg.png)

### PCM - Modulación por pulsos codificados
Es un proceso por el cual se convierte una señal analógica en una digital mediante el muestreo o interpolación de los datos de la onda analógica, en números reales basados en el sistema decimal, que se aproximan y se transforman en secuencias de números binarios que puede entender el procesador.

![PCM](https://cdn.eeweb.com/articles/quizzes/PCM-1425894655.jpg)

## Multiplexación
Es el conjunto de técnicas enfocados en combinar señales para enviar varias comunicaciones a la vez. En general, consisten en dividir la onda en canales que corresponden a distintas propiedades de las ondas que han sido previamente moduladas con información dentro de sí.
### TDM - Multiplexación por división de tiempo
Es una técnica cuyo objetivo es transmitir y recibir señales en una transmisión con interruptores sincronizados en cada punta del canal de transmisión, conformado por un canal de entrada y otro de salida, que alternan entre abierto y cerrado por un intervalo de tiempo; el sistema contiene varias ranuras paralelas en ambos canales, donde se abre uno a uno y almacenan los bits de datos mientras el interruptor está abierto en su ranura correspondiente. Es ampliamente utilizado en las comunicaciones telefónicas hoy en día.

## Conmutación
Son las técnicas utilizadas para establecer un camino en el cual transcurra la información de un emisor a un receptor. Funcionan de tal manera que existe un dispositivo o nodo intermedio que almacena la información mientras termina con la cola de información que debe enviar a distintos receptores y finalmente, calcula la ruta más óptima para la transmisión de la información y lo envía.
