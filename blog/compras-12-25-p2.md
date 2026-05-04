---
slug: compras-12-25-p2
title: 'Nos fuimos de compras: Finalizando nuestra primera experiencia adquiriendo dispositivos Meshtastic'
sidebar_label: "Compras 12/2025 - Parte 2"
authors:
  - key: MrNetsky
    title: Autor
  - key: nicopace
    title: Colaborador
  - key: aguslasp
    title: Colaborador
tags:
  - dispositivos
  - importacion
---

import useBaseUrl from '@docusaurus/useBaseUrl';

:::warning Advertencia
Esta es la segunda parte de nuestro proceso de nuestra de compras, [<u>acá</u>](/blog/compras-12-25.md) podrás ver cómo inició.
:::

## Proceso de recepción de los dispositivos

Los dispositivos fueron llegando con el correr de los días, con relativa rapidez. Uno esperaría que se demoren de mes, a mes y medio en empezar a llegar los dispositivos, incluso no era loco pensar que podrían demorar hasta dos meses, o al menos eso pensábamos nosotros, incluso después de ver que las páginas anunciaban tiempos notablemente más cortos que nuestras expectativas al momento de la compra. Pero lo que realmente sucedió fue que se acercó mucho más a los tiempos estimados de compras que a nuestras expectativas, lo cual es espectacular, porque hay un promedio entre 15 a 21 días para la llegada de los dispositivos. Para nosotros es relativamente rápido, aunque hubo compras que estuvieron debajo del promedio, así como hubo otras que se extendieron de ese plazo, pero en promedio está bien.

**Pero a lo que vinimos... ¿Llegaron todos sin problemas?**

La respuesta corta es no.

Ahora bien, podemos rescatar que el paquete que teníamos miedo de que la aduana lo retuviera, no lo retuvo, llegando sano y salvo a nuestras manos. Lo irónico es que la otra compra en Amazon de dos dispositivos N37 de Meshnology que creíamos que iba a llegar sin ningún problema, no llegó. La compra nunca se terminó de efectuar debido a problemas que desconocemos relacionadas con el pago. Lo positivo es que no se debitó el monto de la tarjeta de crédito. Rehicimos esta compra, pero luego de estar interactuando con los dispositivos decidimos darla de baja, debido a la cuestionable calidad de los mismos y en su lugar efectuamos una compra de 3 Wio Tracker L1 Pro, cuyo hardware es el que Meshnology usó para la creación del N37.

¿Por qué esa elección? La usabilidad del dispositivo era mala y queríamos constatar si era un problema de diseño de la carcasa del N37 o bien era un problema de diseño del hardware del Wio Tracker L1.

¿Llegamos a una conclusión? Si. El mayor problema del N37 está en el diseño del botón que lo hace prácticamente inútil a la hora de intentar interactuar con el dispositivo. Problema que no posee el Wio Tracker L1 Pro, pero si creemos que debe haber mejoras en el joystick. Nos explayaremos mejor al respecto cuando hablemos específicamente de los dispositivos que hemos adquirido en otra publicación.

No fue el único problema que tuvimos, con Heltec no hemos tenido una buena primera experiencia. Ustedes se preguntarán por qué y el motivo fue que nuestra compra estuvo en proceso por más de dos semanas, hasta que cancelaron la compra, no hubo avisos de que esto estaba por ocurrir o el motivo, por lo que, quizás con el diario del lunes, tomamos una mala decisión. Rehicimos la misma compra a Heltec, nuevamente desde su página, pero la compra, luego de casi dos semanas fue cancelada. Parecía una broma de mal gusto.

Esta vez sí nos dieron un motivo, el sobreelevado precio del costo de envío debido a las baterías grandes, recordemos que estos dispositivos tenían una batería de 10.000mAh. Y desde este espacio, apreciamos que nos quieran cuidar el bolsillo, pero también nos surgen preguntas... Si esto lo sabían
+ ¿Por qué no nos dieron la posibilidad de decidir si dar o no de baja la compra? Recordemos que ambas cancelaciones se hicieron unilateralmente por parte de Heltec.
+ ¿Por qué no nos lo informan **antes** de la compra? No sólo a nosotros, sino a los clientes en general, ya que es información sumamente importante.
+ Si este fue el motivo de la cancelación de la primera compra ¿Por qué no nos lo informaron? Ya que recordamos que la primera compra fue dada de baja sin motivo.
+ ¿Fue efectivamente el problema el tamaño de las baterías o el número de dispositivos también tuvo que ver?
+ ¿Por qué al momento de efectuar la segunda compra no nos avisan al momento de esta situación?
+ ¿Por qué se demoró significativamente el reintegro del dinero de las compras que la empresa misma canceló? Recordamos que hay una compra a principios de Diciembre y otra a finales del mismo mes. Es más, nos reintegraron primero el monto de la segunda compra, pero para ambos reintegros se esperó mas de 60 días.

Estas preguntas aún siguen sin respuestas. Y debido a la nueva cancelación se tomó la determinación de **NO** adquirir dispositivos de Heltec, al menos para esta 1er compra, debido a la mala experiencia que tuvimos no una, sino dos veces. No obstante, esperamos desde este espacio que tomen nuestras críticas para mejorar la experiencia de usuario, ya que es de nuestro interés obtener productos de esta marca.

Sin embargo, queremos evaluar el funcionamiento de su tecnología y por ello lo haremos a través de ensambladores que incluyan su hardware o bien revendedores de Heltec que sí sean confiables. Como es el caso de Muzi Works, los cuales no hacen envíos a Argentina, por lo cual, Aerobox (un servicio de importación de Argentina) se tuvo que convertir en héroe.

Una consecuencia extra fue la compra de 3 M5 Pro a Elecrow y 3 T-Deck a LilyGo. Esto fue debido al cambio en la postura inicial y se decidió tener en cuenta dispositivos que incluyan un ESP32. El objetivo era evaluar la duración de la batería en comparación con un nRF52 y evaluar las funcionalidades que pueda brindar, así como mejoras en rendimiento.

Por lo que la compra de los M5 Pro se orientó más a la comparativa directa con nodos como el N37, M1, WisMesh Tag, Wio Tracker L1 Pro o T-Echo, no solo en batería, donde muy probablemente pierda. Lo que a nosotros nos interesa en el aspecto de la batería es saber si puede soportar una jornada completa de combate contra el fuego. Además si hay alguna otra diferencia significativa con respecto a alcance o gestión de mensajería, entre otros aspectos a evaluar.

Mientras que la compra del T-Deck se orientó más a la investigación sobre qué características relevantes puede aportar o si es un gasto innecesario, en el ámbito  del combate del fuego.

Pero el proceso de compra NO terminó aquí ya que, se efectúa una nueva compra de 3 P1, esto fue debido a que necesitábamos más nodos fijos y se optó por este nodo nuevamente por motivos que expicitaremos más adelante sobre el ThinkNode M6 y la desconfianza que nos inspira Heltec. Pero luego de esta compra se decide evaluar el SenseCAP T1000-E, debido a que ahora Seed Studio brinda la posibilidad de comprar 'packs' personalizados de nodos, entre los que incluye al mencionado nodo. Por ello se efectúa la compra de 3 unidades porque si es un nodo viable, esta marca se convierte en la mejor posicionada con respecto a las demás porque en un sitio y de una manera muy cómoda puedes adquirir todos los nodos necesarios en las cantidades necesarias, pensando sobretodo en la logística que deban afrontar los combatientes.

Para cerrar este apartado diría que en líneas generales, fue un proceso que llevamos a cabo con éxito, con sensaciones positivas que nos dejaron muchísimos aprendizajes. Obviamente hubo problemas y sinsabores, pero como suele suceder en la vida, no obstante, nos quedamos con lo positivo de esta experiencia.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img 
    src={useBaseUrl('/img/primer-compra-lora.jpg')}
    alt="1er compra de dispositivos" 
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**En la parte de arriba pordŕa ver de izquierda a derecha al Voyager, ThinkNode M6 y SenseCAP Solar Node P1. En sus soportes podrá ver al SenseCAP T1000-E y al WisMesh Tag. En la parte de abajo al N37, ThinkNode M1 (el M5 Pro se ve exactamente igual), T-Deck, MeshPocket Qi2 y Wio Tracker L1 Pro.**</p>
</div>

## Observaciones

### Envío

Es importante resaltar que mientras más rápido una empresa despacha un producto más rápido podrá llegar a destino, quizás es una obviedad mencionarlo, pero no lo es tanto. Empresas como RAK o SeedStudio entienden y respetan esto, es por ello que han sido los productos que más rápido llegan a destino. 

Elecrow es un caso similar a las anteriores, pero sí hubo un envío que se demoró casi un mes en ser despachado, nosotros creemos que hubo un error por parte de ellos en anunciar un producto (ThinkNode M6), que quizás no había en stock a momento de la compra. Pero insisto que son conjeturas, ya que desde la empresa no hubo comunicados al respecto. Pero para la tercera compra nos enviaron un regalo, el verdadero 'así se cuida a un cliente', realmente unos tipazos.

Meshnology y Spec5 han cumplido, podemos resaltar que para ambos envíos, el embalaje no fue el adecuado, sin dudas los más flojos, pero en cuanto a tiempos, cumplieron. Quién si dejó sensaciones positivas fue Aerobox que formó parte del envío del Spec5 Voyager, ya que fue quien lo trajo desde EEUU a nuestra locación. Fue un servicio rápido, en cuanto a costos similar a DHL y FedEx, que te mantiene informado vía mail del movimiento del paquete. en base a nuestra primera experiencia es recomendable y que tendremos en cuenta para posteriores compras.

Está de más aclarar que Heltec no efectuó envíos. LilyGo en un inicio pareció recorrer el mismo camino que Heltec, ya que se demoró mucho en el despacho del producto. Pero, luego de un mes FedEx lo tuvo en sus manos y en poco tiempo lo tuvimos en las nuestras.

Muzi Works terminó siendo quien más rápido despachó nuestro paquete. Aunque no sabemos si llegó en tiempo a los depósitos de Aerobox. Y usted se preguntará ¿Cómo es esto posible? Bueno... Según Muzzi Works y USPS el paquete llegó una semana antes de lo que informa Aerobox. Hecho que nos preocupó, porque mientras de un lado nos decían paquete entregado, del otro nos decían que no había llegado nada. Pero por suerte todo salió bien. Sin embargo fueron los últimos dispositivos en llegar y por mucho. A diferencia de nuestra primera y gratificante experiencia con AeroBox, la segunda fue todo lo opuesto. Demoras en cada uno de los procesos, que esta vez, nada tenían que ver con nosotros. Pese a todo esto, llegó antes de que finalice Febrero. 

Si creemos que a diferencia de la entrega anterior de Aerobox, donde sus demoras fueron nuestra responsabilidad, en este caso si se han demorado más. ¿Esto es malo? No, sigue siendo un buen servicio y relativamente rápido, pero es algo que no queríamos dejar de comentar.

Quería también hablar de los couriers. FedEx el primer paquete que nos entregó, no nos comunicó nada hasta que estuvo en puerta, nos dieron una cuenta a la que hacer la transferencia, lo cual es curioso cuanto menos, ya que uno espera un servicio más 'profesional'. Pero ya para la segunda entrega si nos avisaron cuando estaban aduana, pagamos los impuestos y posteriormente nos entregaron el paquete. Es un servicio costoso, pero llega en el tiempo estipulado. Creemos que es un buen servicio pero lo que sí nos llama la atención es que no nos trasladaron 3 ThinkNode M1 porque contenían baterías, hecho que nos obligó a cambiar de courier, pero si trajeron los T-Deck que poseían baterías más grandes. Por lo que no sabemos si traen o no baterías desde el exterior, la única diferencia relevante entre las compras que trajo FedEx fue el país, una de China y otro de EEUU, respectivamente.

DHL es y por escándalo lo mejor, no solo la velocidad sino la claridad del proceder, te avisaban cuando tenían tu pedido, cuando estaba en aduana, cuánto deberías pagar, realmente un muy buen servicio. En cuanto a precios, no sabríamos ubicarlos ya que los hubo muy bajos y muy altos, pero es un servicio por el que vale la pena pagar. Pero, no todo lo que brilla es oro y este también es un gran pero, hay problemas con los montos facturados. Resaltamos el buen servicio de atención al cliente vía teléfono y mail, no así vía wpp, pero lo que realmente nos parece importante destacar es la predisposición y la rapidez a la hora de solucionarte, además de que luego de mostrarles el error, nos reintegraron todo. Por lo que vuelvo a repetir, muy buen servicio.

### Primer encendido 

Los primeros nodos que se encendieron, fueron los N37. Aquí cometimos nuestro primer error, a 5 minutos de haber encendido el dispositivo. Intentamos flashear el firmware vía bluetooth, algo que no se puede hacer desde la app de Android, por lo menos a la fecha de publicación de este artículo (y no es que no se pueda en la actualidad, nosotros no quisimos ahondar en este proceso por ahora), pero que en su momento nosotros sabíamos, lo que derivó en que el dispositivo se 'rompa'. Sin embargo, lo arreglamos a la brevedad.

Para ello debimos desarmarlo, desconectar la batería y conectarlo vía USB al PC, es importantísimo que al momento de conectarlo, tenga la antena LoRa conectada, porque de lo contrario podemos dañar el dispositivo de manera permanente. Al tenerlo conectado, lo hacemos entrar en modo DFU, para ello oprimimos dos veces el botón de reset. Luego desde la página de web, flasheamos el firmware y resucitó.

El proceso de actualización del firmware a la versión beta 2.7.15 es algo que aplicó a todos los dispositivos.

Posteriormente se flashearon los firmware de los WisMesh Tag y SenseCAP Solar Node P1. Ambos con sensaciones muy positivas. El primero por su durabilidad pese a su pequeña batería y simpleza de uso.

El segundo por su armado sencillo y la calidad de sus materiales, pero sí hay una cuestión que desde la página no se informó o al menos nosotros no lo vimos y es la forma de la batería. ¿Por qué es relevante? Porque si bien nosotros sabíamos que usaban 4 baterías 18650, no sabíamos que necesariamente debían ser con relieve en el cátodo (comúnmente conocido como botón o tetón). Entonces nosotros teníamos 4 baterías de esa forma, pero necesitábamos el doble (porque tenemos dos nodos). Lo que sí es relevante es que con dos baterías el rendimiento es muy bueno.

:::info ¿Sabías que...? 
Nos hemos propuesto reciclar baterías de litio 18650 de dispositivos rotos o en desuso con el fin de poder reutilizarlas. En nuestro caso particular son las que usamos dentro de los SenseCAP P1. Aunque también tenemos pensado agrupar las que sobren en un powerbank casero. 
:::

De los M1 llamó poderosamente la atención el alto consumo de energía, impactando en una durabilidad del dispositivo que no supera las 48hs. Aún no descubrimos la configuración de uso con la que pueda, si es que puede, superar tal estimado tiempo ya que utilizamos tanto el GPS, como el Bluetooth encendidos.

El ThinkNode M6 no tenía firmware disponible al momento de la compra, recién en Abril del corriente año, estuvo disponible en la página de [flasher web meshtastic](https://flasher.meshtastic.org/). Entonces... ¿Dónde lo conseguimos? En el siguiente repositorio de GitHub, un héroe se puso a la tarea de crearlo, además allí te enseña cómo compilarlo y flashearlo. [Aquí les dejamos el repo en cuestión.](https://github.com/meshtastic/firmware)

Con respecto al Wio Tracker L1 Pro, pudimos constatar las diferencias en el manejo del joystick con el N37.

El Spec5 Voyager en funcionamiento anda muy bien. En cuanto a interacción con el mismo, es claramente el menos logrado. Es gastar 219 U$D por un nodo que no tiene acceso al puerto USB, a botones o aunque sea una luz para saber si está o no en funcionamiento. Y si no hay botones... ¿Cómo se enciende? Deberás desarmarlo y conectar la batería. Y si quisieras saber si está operativo, deberás buscarlo desde alguna app o nodo, ya sea para conectarte a él o ver que el mismo se encuentre operativo. Un dispositivo que, pese a sus interesantísimas características, está poco logrado. Aún más teniendo en cuenta su elevado precio. Para flashear el firmware deberás buscar el disponible para el WisBlock.

También en esta etapa se decidió que se necesitaba un nodo para el dron, con la posibilidad de hacer de puente para comunicaciones en donde sea más rápido desplegarse vía aérea. Pero luego de la dudable calidad del producto de Spec5, se decidió no adquirir el Spec5 Copilot, se buscaron opciones de la comunidad como carcasas impresas en 3D junto a hardware adaptado. 

Finalmente se fue por lo más sencillo, imprimir un soporte 3D para el WisMesh Tag que se agarre con un precinto a la parte baja del dron. El resultado, aunque sencillo, fue muy bueno. El primer prototipo nos falló en dimensiones, por lo que tuvimos que reeimprimirlo, pero con las medidas correctas, pero el primer prototipo no se perdió ya que con la llegada del T1000-E, pudimos usarlo de soporte para éste.

Obviamente no se podía despegar o aterrizar en el suelo, pero desde el funcionamiento superó ampliamente nuestras expectativas.

<div style={{
  display: 'flex',
  gap: '20px',
  justifyContent: 'center',
  alignItems: 'flex-start'
}}>
  <div style={{ flex: 1, textAlign: 'center' }}>
    <img
      src={useBaseUrl('/img/wmtag-soporte.jpeg')}
      alt="WisMesh Tag"
      style={{ height: '300px', width: 'auto', objectFit: 'contain' }}
    />
    <p>**WisMesh Tag con soporte**</p>
  </div>
  
  <div style={{ flex: 1, textAlign: 'center' }}>
    <img
      src={useBaseUrl('/img/dron-repetidor-meshtastic-1.jpeg')}
      alt="Dron repetidor"
      style={{ height: '300px', width: 'auto', objectFit: 'contain' }}
    />
    <p>**Anclaje a dron**</p>
  </div>
</div>

¿Es esta la solución de los nodos para drones? La respuesta corta es no. Pero si creemos que aportó sensaciones positivas y por un bajísimo coste económico y de tiempo, se pudieron realizar unas primeras pruebas de manera óptima. 

De los nodos cuyo procesador es un ESP32. Los primeros en llegar fueron los M5 Pro y su proceso de actualización fue preocupante. Porque cuando lo actualizamos se 'rompió', pero esta vez, parecía peor que el anterior dispositivo mencionado. Tanto que el primer día no pudimos solucionar el problema. Hecho que nos condujo a comunicarnos, vía mail con Elecrow contándoles nuestra situación. Ellos se comunicaron con nosotros en menos de 24hs, nos sugirieron que NO usemos la opción de 'InkHUD', e intentemos nuevamente. Nosotros el día anterior, habíamos probado esto sin éxito, pero lo intentamos una vez más y funcionó. ¿Por qué funcionó ahora y no antes? Lo ignoramos por completo, creemos que se debió a un problema ajeno al proceso en sí, ya que la página cambió de interfaz de un día a otro, vuelvo a recalcar que ignoramos el motivo, esto es una suposición nuestra. Lo verdaderamente importante es que nuestro nodo volvió a la vida, mismo que a primeras luces no parece tener diferencias significativas con el M1.

El otro ESP32 es el T-Deck Plus. Muy esperado por nuestra parte, cuyas expectativas se encontraban divididas, por lo que podía ofrecer, entre las limitaciones que posee. Creemos que el balance es más negativo que positivo, al menos en este primer encendido, porque posee dos interfaces gráficas que no aprovechan del todo el hardware disponible. Obviamente faltan pruebas y se verá qué función desempeña finalmente y cómo puede hacerlo, pero aún creemos que puede llegar a ser útil.

Los MeshPocket Qi2 dejan sensaciones encontradas. Creo que puede andar bien como una powerbank, pero da la sensación que no termina de cumplir como nodo Meshtastic porque se ve sofisticado, pero se a su vez es endeble y la pantalla es muy barata. Tiene un efecto absurdo de ghosting, aunque el tamaño la vuelve más cómoda que las de los M1 o T-Echo. La rotación, junto a la distribución de los botones, mejora la experiencia y es algo que los otros nodos anteriormente nombrados, pese a tener la misma función, no aprovechan.

Por últimolos SenseCAP T1000-E y la verdad es que es un buen nodo, pero claramente inferior al WisMesh Tag. Si piensan adquirir el paquete de nodos de SeedStudio va a andar bien, pero si queres particularmente un nodo tipo tarjeta, es más recomendable el WisMesh Tag.

---

El proceso de compra que inició en los primeros días de Diciembre se extendió hasta finales de Marzo con las cancelaciones y las compras posteriores. Fue un proceso que se extendió más de lo previsto, pero los dispositivos, llegaron aceptablemente rápido. 

Se adquirieron 39 unidades de todos los fabricantes de hardware. Nodos que pueden cumplir diferentes funciones y abarcando los dos procesadores del mercado como lo son el ESP32 y el nRF52.

Creemos que es un buen punto de partida para empezar a testear escenarios posibles y coordinar con nuestro equipo, así como con combatientes y gente aficionada que quiera formar parte de las primeras pruebas de campo en esta zona. Estamos felices y expectantes de los resultados que arrojarán estas pruebas así como ansiosos de poder ayudar a nuestra comunidad.

