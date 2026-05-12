---
slug: experiencia-con-la-chilca
title: 'Prueba de campo Meshtastic con la brigada La Chilca: Alcance, bosques y desafíos de hardware'
sidebar_label: Experiencia con La Chilca
authors:
  - key: MrNetsky
    title: Autor
  - key: aguslasp
    title: Colaborador
  - key: nicopace
    title: Colaborador
tags: 
  - dispositivos
  - importacion
---

import useBaseUrl from '@docusaurus/useBaseUrl';

En el diseño de redes de comunicación para emergencias, la teoría y la práctica suelen chocar de frente cuando salimos al terreno. Sabemos que las señales de los dispositivos Meshtastic (tecnología LoRa) pueden viajar cientos de kilómetros si hay línea de vista directa. ¿Pero qué pasa cuando le sumamos la realidad de nuestro entorno?

Junto a Sofi y Caro de la brigada forestal [La Chilca](https://www.instagram.com/brigadalachilca/), salimos a responder esta pregunta en [José de la Quintana](https://maps.app.goo.gl/tkhwQghCG9jQNv5d6) (Departamento Santa María, Provincia de Córdoba, Argentina).

El objetivo inicial era claro, determinar cuánto afecta la copa de los árboles a la señal de los dispositivos Meshtastic. Entender cómo los obstáculos regulares entorpecen la comunicación es vital para diseñar redes robustas. Además, veníamos de algunas pruebas de alcance fallidas y necesitábamos un escenario real para demostrar el verdadero potencial de esta tecnología.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/caminata-conjunta-la-chilca.jpg")}
    alt="Caminata con La Chilca"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**Ascendiendo al punto elevado donde ubicaremos nuestro nodo fijo, junto a Sofi y Caro**</p>
</div>

## El Despliegue: Nodos, Sierras y Motos

Para esta prueba de alcance, preparamos cinco dispositivos con hardware totalmente distinto, todos configurados con la misma versión del firmware Meshtastic (2.7.15) y el preset de radio LongFast:

- SenseCAP Solar Node P1 (Seeed Studio) - Nodo fijo.  
- Wio Tracker L1 (Seeed Studio) - Nodo móvil.  
- ThinkNode M1 (Elecrow) - Nodo móvil.  
- T-Deck (LilyGo) - Nodo móvil.  
- WisMesh Tag (RAK Wireless) - Llevado como repetidor para el dron, pero no se llegó a usar.  
- MeshPocket Qi2 (Heltec) - Sólo se usó como powerbank para poder mantener encendido el T-Deck.

Además, cada grupo fue equipado con una radio VHF y celulares para poder conectarse a un nodo vía Bluetooth. ¿La estrategia? Nos dividimos en dos equipos. Un equipo ascendió unos 20 minutos por una pendiente empinada hasta la parte más alta de la cuchilla para instalar el nodo solar (SenseCAP Solar Node P1) a pleno sol.

El otro equipo (Pablo) inició un recorrido en moto llevando los nodos móviles (T-Deck, Wio Tracker L1 y ThinkNode M1) para mapear la cobertura en la zona baja.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/cobertura-p1.png")}
    alt="Área teórica de cobertura"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**Aquí podrá observar el área que estimada de cobertura según Meshtastic Site Planner**</p>
</div>

## El misterio de los árboles y los resultados de cobertura

El recorrido en moto implicó más de dos horas de tiempo neto de prueba, cubriendo un trayecto extenso que culminó en [Los Molinos](https://www.google.com/maps/place/Los+Molinos,+C%C3%B3rdoba/@-31.8550044,-64.3793484,17z/data=!4m10!1m2!2m1!1sLos+molinos!3m6!1s0x95d2aa4d413d375b:0x78606aab0556bdbd!8m2!3d-31.854921!4d-64.3789851!15sCgtMb3MgbW9saW5vc5IBCGxvY2FsaXR54AEA!16s%2Fg%2F120kn2sr?entry=ttu&g_ep=EgoyMDI2MDUxMC4wIKXMDSoASAFQAw%3D%3D).

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/cobertura-experiencia.png")}
    alt="Área de cobertura de la experiencia"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**Aquí podrá observar el área que estimamos habrá cobertura en base a los resultados de nuestra experiencia**</p>
</div>

El resultado de RF fue un éxito rotundo y nos dio una respuesta clara sobre la vegetación. La experiencia demostró que la copa de los árboles en el contexto de José de la Quintana (árboles de espinas, con follaje medio, no extremadamente densos) no afectó significativamente la señal. Los mensajes llegaron perfectos a través del monte.

Además, descubrimos un dato operativo excelente, la posición de la antena de los nodos móviles no influyó en la comunicación. Durante gran parte de la experiencia, la antena no estuvo en una posición vertical perfecta, y sin embargo, la transmisión de datos se dio de muy buena manera.

Lo que verdaderamente dictó las reglas del juego fue la topografía: la línea de vista es muy importante. El único momento en que la señal se bloqueó por completo fue yendo hacia Los Molinos, justo cuando dimos la vuelta a un monte y perdimos la línea de vista directa con la cuchilla. Apenas hay un desnivel de tierra o piedra que interrumpe la visual, se acaba la comunicación. Es absolutamente esencial la elección de puntos estratégicos y altos para instalar los nodos repetidores.

## La realidad del hardware: No todo lo que brilla es oro

Si bien la red demostró su potencial, el hardware nos dio varias lecciones importantes:

- *Inestabilidad en el Nodo Solar (P1)*: El nodo debió ser reiniciado 3 o 4 veces a lo largo de toda la experiencia. No tenemos la certeza de si estos fallos se debieron a mantener un teléfono conectado por Bluetooth o a otra causa técnica. Lo que sí sabemos es que, en una experiencia anterior donde lo usamos puramente como repetidor (sin conexión Bluetooth), el P1 funcionó de manera impecable. Es un comportamiento que estamos investigando a fondo.
- *El fracaso del T-Deck*: A los 500 metros de iniciado el recorrido, perdió la señal por completo y quedó "sordo". Debido a esto se decidió encender la función de Range Test y curiosamente los mensajes si llegaban con frecuencia al nodo fijo, pero el T-Deck sólo recibía mensajes si el Wio Tracker L1 actuaba como repetidor, a pesar de estar a la misma distancia del nodo principal. La conclusión es clara, **el T-Deck queda fuera de nuestras pruebas operativas por ahora.**
- *Dudas sobre Seeed Studio*: Aunque el Wio Tracker L1 funcionó muy bien esta vez, los fallos recurrentes del P1 en esta prueba, sumados a cuelgues de otros L1 en el pasado, nos llevan a prestar atención a su confiabilidad. Por ello estamos investigando si es un problema de la marca o si es propio de los nodos cuyo procesador sea un nRF52.

---

El ejercicio cumplió su cometido, vimos el alcance real cruzando la vegetación local, comprobamos la robustez de la señal independientemente de la posición de la antena, y confirmamos que la topografía es el verdadero límite. También detectamos los eslabones débiles de nuestro equipamiento. Los próximos pasos son evaluar a fondo la inestabilidad de los nodos solares, descartar hardware problemático y seguir trabajando junto a las brigadas para que esta tecnología sea, muy pronto, una herramienta indispensable en su mochila.

Queda mucho aún por aprender y experimentar, pero este ejercicio nos dió buenas sensaciones devolviendonos parte de la esperanza que con los experimentos fallidos con anterioridad habíamos perdido.
