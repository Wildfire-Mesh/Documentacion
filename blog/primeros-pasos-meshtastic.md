---
slug: primeros-pasos-meshtastic
title: Meshtastic, la tecnología open source para la comunicación a larga distancia (LoRa)
sidebar_label: Primeros pasos en el mundo Meshtastic
authors: 
  - key: MrNetsky
    title: Autor
  - key: nicopace
    title: Autor
  - key: aguslasp
    title: Colaborador
tags:
  - dispositivos
  - meshtastic
---

![Logo Meshtastic](https://i0.wp.com/pileupdx.com/wp-content/uploads/2024/04/meshtastic-banner.jpg?resize=1024%2C200&ssl=1)
## Introducción

En el combate de incendios forestales y en las operaciones de búsqueda y rescate (SAR), la comunicación es un factor determinante para un accionar eficiente. En zonas de alta montaña o quebradas profundas, las redes celulares son inexistentes y las radios VHF/UHF convencionales suelen fallar debido a la geografía del lugar.

Meshtastic surge como una solución de comunicación alternativa. No depende de infraestructura externa sino que permite crear una infraestructura propia.


### ¿Para qué sirve?

A diferencia de otros sistemas, Meshtastic está diseñado para operar en condiciones extremas:

+ Red de seguridad autónoma 🆘: Si el repetidor central falla o el humo bloquea las señales satelitales, los nodos Meshtastic siguen operando entre sí.
+ Geolocalización del personal 📍: Permite al *puesto de comando* visualizar en tiempo real la posición de cada brigadista o vehículo en el terreno, aumentando la conciencia del entorno y reduciendo riesgos como el de quedar atrapado por cambios en la dirección del viento o de extravío del combatiente. Además de saber dónde está qué y quién, es posible saber cómo llegó allí o dónde fue visto por última vez.
+ Logística Silenciosa 📻: Envío de coordenadas y potencialmente estados de suministro (agua, combustible, etc) y alertas de evacuación mediante texto, evitando la saturación de los canales de voz críticos.

### ¿Cómo lo hace?
Usando una señal de radio de baja potencia llamada LoRa, cada nodo puede enviar mensajes "saltando" de uno a otro, generando así lo que se conoce como malla colaborativa y cuyo alcance de la red se extiende con cada nodo. Los nodos Meshtastic son de bajo consumo energético, permitiéndoles durar días con una sola carga, lo que es perfecto para cubir las jornadas de combate del fuego.

Algunos nodos operan de manera similar que un walkie-tolkie de texto, ya que poseen pantalla, botones, parlante (solo cumplen una función de emisión de sonido con el fin de enviar notificaciones al usuario) e incluso algunos tienen hasta teclado. 
Mientras que los que no cuentan con estas características, pueden vincularse con su teléfono a través de la aplicación Meshtastic, logrando así, compartir mensajes y ubicaciones de forma pública o privada sin depender de redes WiFi o celulares.

![Intercomunicación Meshtastic](https://www.ultimavincam.com/fileman/entradas/10/lora-topology-2-c80684f1eafdf2a71fbaf26e494fb26d.webp)

:::info ¿sabías qué?
Meshtastic es de código abierto y está impulsado por la comunidad, lo que significa que los usuarios tienen la libertad de ejecutar, modificar y mejorar el software. Se crea mediante la colaboración global, en la que todos trabajan juntos para mejorarlo.
:::

### ¿Por qué nos interesa?

Porque posee características deseables en un sistema de comunicación de emergencias. La posibilidad de reenviar mensajes permite que los mensajes lleguen más lejos de lo que la infraestructura existente habilita. El bajo consumo permite que los dispositivos sean pequeños, portables, fáciles de desplegar, requiriendo poca infraestructura y baja inversión para su despliegue.

Las comunicaciones digitales habilitan enviar información que antes, usando la voz, era difícil o imposible. Por ejemplo la ubicación de manera regular, e incluso poder recibir mensajes cuando uno no está prestando atención al dispositivo de comunicación y leerlo en otro momento, como lo haces habitualmente con tu teléfono. Todas estas características creemos que son claves para complementar un plan de comunicación en el combate del fuego.

Entendemos que hay algunas barreras que limitan su implementación. Primero, mucha de la documentación existente para estas plataformas de comunicación se encuentra escrita en lenguaje técnico y su mayoría, en Ingles. Segundo, que al no estar pensada específicamente para el combate del fuego, la documentación no está adaptada a las necesidades del combate del fuego. Este proyecto busca trabajar en estos dos ejes. Por lo cual, esperen más contenido como este pronto. 

---

Meshtastic representa mucho más que una simple aplicación de radio; es una innovadora forma de conectividad, que al aprovechar el poder de la tecnología LoRa, ha creado un paradigma donde el alcance se maximiza y el consumo de energía se minimiza, haciendo que las comunicaciones de largo alcance sean posibles incluso en los lugares más complejos.

No busca reemplazar a ninguno de los métodos actuales de comunicación, busca ofrecer una alternativa necesaria para cuando los demás, por diversos motivos, no pueden funcionar o no están disponibles y sumarse a las estrategias de comunicación que ya existen en el combate del fuego.

