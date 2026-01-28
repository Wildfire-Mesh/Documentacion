---
slug: formatos-digitales-de-comunicacion
title: Explorando los ecosistemas de comunicación de bajo ancho de banda y larga distancia
sidebar_label: Formatos de comunicación digital Off-Grid
authors: 
  - key: MrNetsky
    title: Autor
  - key: nicopace
    title: Colaborador
tags: [dispositivos]
---
 
Nuestra dependencia de las infraestructuras de comunicación centralizadas (desde las torres celulares hasta la fibra óptica) ha crecido exponencialmente. Esto ha traído una comodidad sin precedentes, pero también ha creado dependencias. Desastres naturales, fallos de infraestructura o la simple necesidad de operar en áreas remotas revelan que nuestra conectividad no es tan robusta como imaginamos. Esta fragilidad es la que afrontan los combatientes del fuego y nos ha impulsado en la búsqueda de una alternativa y así hemos arribado a la conectividad descentralizada.

Pero... ¿A qué nos referimos con una 'conectividad descentralizada'?

Se refiere a una red donde la información y el control no pasan a través de una única entidad o punto central (como un servidor principal, una torre celular o una autoridad de gobierno), sino que se distribuyen entre múltiples participantes, conocidos como *nodos*. Este enfoque puede aplicarse a través de tecnologías como *redes de malla.*

¿Y qué es una red mesh o red de malla?

Es un sistema de comunicación en donde los nodos trabajan juntos para crear una única red inalámbrica extendida, eliminando zonas sin cobertura. A diferencia de los routers tradicionales, que emiten una señal desde un solo punto, los sistemas mesh distribuyen la señal desde varios nodos interconectados. Esto permite una cobertura más amplia y estable.

Desde este espacio nos hemos propuesto explorar este ecosistema descentralizado y dentro del mismo, diferenciaremos dos grupos.

#### LoRa: Alcance extremo y resiliencia

El secreto detrás de las soluciones de larga distancia y bajo consumo energético como *Meshtastic* y *Meshcore* es la modulación LoRa (Long Range). Esta modulación es excepcionalmente robusta y le permite al receptor detectar la señal en condiciones muy adversas, otorgando un alcance extremo y una alta adaptabilidad ante las interferencias. Como contrapartida, LoRa se limita a un limitado ancho de banda, haciéndola ideal para la transmisión de pequeños paquetes de datos (texto, telemetría o coordenadas GPS). 

Lo positivo de estas tecnologías es su bajo coste de implementación, ya que los nodos son económicos y con el conocimiento necesario, puedes armar uno propio, bajando aún más los costes. El firmware al ser software libre, es de público uso y modificación, además operan en bandas ISM, lo cual no requiere de una licencia de Radioaficionado para poder operarlas.

Dentro de este grupo, el firmware [**Meshtastic**](https://meshtastic.org/) se ha establecido como la opción de código abierto por excelencia. Opera una Malla Nómada, donde cualquier nodo puede extender la cobertura de la red repitiendo los mensajes que escucha, y utiliza un protocolo de enrutamiento específico para que los mensajes encuentren el destino de forma automática. Esto lo logra enviando el mensaje a todos los dispositivos disponibles, saltando entre ellos, con el fin de encontrar el destinatario, pero esta capacidad de salto está a limitada a un máximo de 8.

Por otro lado [**Meshcore**](https://meshcore.co.uk/) utiliza la misma modulación pero implementa una Malla Fija, donde solo algunos nodos designados, actúan como repetidores y el enrutamiento similar al anterior, envía el mensaje a todos los dispositivos disponibles, con el fin de encontrar la ruta más corta de llegada a un nodo, una vez logrado esto, guarda la ruta, haciendo que la comunicación sea más rápida y que un mensaje pueda saltar hasta 64 veces, mucho más que en Meshtastic.

#### RF Digital Licenciada: Agilidad y arquitectura propietaria

Las plataformas como *goTenna* y *Beartooth* optan por una modulación distinta a las tecnologías del bloque anterior. Poseen una mayor velocidad de datos relativa y una gestión de red que puede estar mejor optimizada para tareas específicas. Además estas tecnologías poseen un mejor soporte que las anteriormente mencionadas.

Ambas soluciones crean una red de malla, un concepto fundamental que describe una red formada de manera espontánea por dispositivos que se comunican directamente sin depender de una infraestructura central.

[**goTenna**](https://gotenna.com/) Mesh utiliza su propio protocolo propietario Aspen Grove para crear esta red mesh. Su diseño está optimizado para la mensajería de texto y GPS, ofreciendo una experiencia plug-and-play con un firmware cerrado que opera en bandas VHF (142-175 MHz) y UHF (445-480 MHz). Sumado a una potencia significativamente superior a las demás, logra un alcance superior, además de la calidad militar de sus componente, hacen que sorteen mejor la interferencia por ruido u obstáculos. Pero es y con diferencia, la tecnología más costosa de las aquí presentadas.

[**Beartooth**](https://beartooth.com/), por su parte, se enfocó en paquetes de datos más grandes, como la Voz PTT (Push-to-Talk), aprovechando la mayor velocidad de datos. Se encuentra operada en bandas ISM, lo que le permite ser utilizado sin licencia. En cuanto al alcance está por detras de las demás tecnologías también permite trabajar con la ubicación GPS.

---

La exploración de los formatos de comunicación digital fuera de la red revela un panorama donde no existe una solución única, cada una tiene caractísticas particularmente únicas y positivas, así como también sus contras. Cada uno de estos sistemas puede complementar los medios de comunicación habitualmente usados, con el fin de satisfacer necesidades de comunicación específicas en contextos vulnerables.

Desde este espacio queremos resaltar que el futuro de la conectividad descentralizada no reside en la victoria de una tecnología sobre otra. Sin embargo, nosotros **NO** hemos definido una tecnología con la cual llevar adelante este proyecto, pero por el momento intentaremos utilizar la tecnología Meshtastic, aunque estamos abiertos al uso de una tecnología complementaria o a un cambio de tecnología en un futuro, de ser necesario. 

Creemos que Meshtastic nos permite solucionar los mencionados problemas de comunicación a un costo asequible, además de brindar un panorama estable de partida con el cual empezar a trabajar. Somos conscientes que es una tecnología en desarrollo, que nos queda mucho por aprender y practicar, pero estamos dispuestos a ello para ayudar tanto a los combatientes y rescatistas, como al proyecto Meshtastic, así como su comunidad hispanoparlante.
