---
slug: analisis-primera-compra.md
title: 'Análisis de los dispositivos adquiridos en nuestra primera compra'
sidebar_label: "Análisis de dispositivos"
authors:
  - key: MrNetsky
    title: Autor
  - key: nicopace
    title: Colaborador
tags:
  - dispositivos
  - importacion
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';
import useBaseUrl from '@docusaurus/useBaseUrl';

Este artículo se basa en nuestra experiencia personal con los nodos aquí citados, además fueron evaluados en el contexto del uso de un combatiente del fuego. 

Por ende hay nodos que en este contexto, no son óptimos, pero fuera del mismo, puede que sea un gran dispositivo.
Teniendo esto en cuenta lo que nosotros buscamos es:
- Durabilidad en batería.
- Certificación IP.
- Fácil maniobrabilidad, sobre todo con guantes.
- Independencia del teléfono.

Si te interesa conocer más sobre nuestra primera compra de dispositivo LoRa, podrás ver la [<u>primera</u>](/blog/compras-12-25.md) y [<u>segunda</u>](/blog/compras-12-25-p2.md) parte de nuestro proceso.

## Elecrow

Es una marca interesante que ofrece productos con una variedad de funcionalidades y microprocesadores, tienen cuestiones a mejorar pero creemos que van por buen camino además de que poseen precios accesibles. Sin duda si tiene pensado adquirir tecnología LoRa, esta es una marca que NO puede dejar pasar.

<Tabs>
  <TabItem
    value="m1"
    label={
      <div style={{ display: 'flex', alignItems: 'center', gap: '8px' }}>
        <span>ThinkNode M1</span>
      </div>
    }
    default
  >
  Es un nodo cómodo, con una buena terminación, liviano, con una batería aceptable. A su firmware lo podemos diferenciar según su interfaz (UI):
  - <u>UI Estándar</u>: Muestra al usuario bastante información a su usuario, permitiéndole hacer unas cuantas configuraciones desde el dispositivo, lo que le permite en cierto modo, tener un grado de independencia que la otra interfaz no posee.

  - <u>InkHUD</u>: Es más sencilla, más veloz, pero tiene casi una estricta dependencia del celular o pc. Lo positivo es que te permite rotar la pantalla, mejorando la manipulación del dispositivo, algo que con la otra interfaz es imposible.

  Su parlante posee un volumen bajo, lo cual no es útil, debido a ello decidimos deshabilitarlo. El regulador de intensidad de la luz creemos que es poco útil, con un botón que encienda o apague se hubiera resuelto de una mejor manera. Y la duración de la batería nunca superó las 48hs en escenarios sin tráfico de radio, con Bluetooth y GPS encendidos, en ninguno de estos 6 nodos.

  Creemos que es un buen nodo, pero no creemos que sea el definitivo, debería cumplir con estándares necesarios de los combatientes que hoy no los cumple, pero que quizás en un futuro, con unas mejoras, puede que lo haga.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/ThinkNode-M1.jpg")}
    alt="Elecrow ThinkNode M1"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**ThinkNode M1**</p>
</div>

  </TabItem>

  <TabItem
    value="m5"
    label={
      <div style={{ display: 'flex', alignItems: 'center', gap: '8px' }}>
        <span>ThinkNode M5 Pro</span>
      </div>
    }
  >
  Es un nodo cómodo, con una buena terminación, liviano, con una batería aceptable. A su firmware lo podemos diferenciar según su interfaz (UI):
  - <u>UI Estándar</u>: Muestra al usuario bastante información a su usuario, permitiéndole hacer unas cuantas configuraciones desde el dispositivo, lo que le permite en cierto modo, tener un grado de independencia que la otra interfaz no posee. El gran problema de esta interfaz es la constante actualización de la hora y el porcentaje de batería, que limitan en una porción significativa el tiempo de uso.

  - <u>InkHUD</u>: No la hemos probado ya que su proceso de flasheo brickea el dispositivo, al menos con la versión 2.7.15 del firmware.

  Su parlante posee un volumen bajo, lo cual no es útil, debido a ello decidimos deshabilitarlo. El regulador de intensidad de la luz creemos que es poco útil, con un botón que encienda o apague se hubiera resuelto de una mejor manera.

  Creemos que es un buen nodo, pero no creemos que sea el definitivo, debería cumplir con estándares necesarios de los combatientes que hoy no los cumple, pero que quizas en un futuro, con unas mejoras, puede que lo haga.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/ThinkNode-M1.jpg")}
    alt="Elecrow ThinkNode M5 Pro"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**ThinkNode M5 Pro**</p>
</div>

  </TabItem>

  <TabItem
    value="m6"
    label={
      <div style={{ display: 'flex', alignItems: 'center', gap: '8px' }}>
        <span>ThinkNode M6</span>
      </div>
    }
  >

  Este nodo, pese a que en su página se encontraba sin stock al momento de nuestra compra, si lo había en su versión que venía flasheado con LoRaWAN, mismo que NO posee otra diferencia que el firmware con el que viene flasheado de fábrica. Esta lógica nos llevó a adquirir el producto de todas maneras, porque nosotros sabíamos de dónde conseguir el firmware Meshtastic para este nodo y cómo flashearselo. Pero resultó que el problema no era la falta de stock, sino que lo que no había, era el firmware. Lo cual, desde este espacio creemos que NO es correcto publicitar un dispositivo para el cual no hay un firmware disponible. Por ejemplo: Vos te imaginás que queres comprar la hamburguesa más rica del mundo, que incluye dentro de todos sus ingredientes, un medallón de carne y cuando la vas a comer, te das cuenta que está todo, menos el mencionado medallón. Bueno, eso es lo que nos pasó con este dispositivo.

  Actualmente se encuentra en stock, pero no hay un firmware disponible desde la página de [meshtastic web flasher](https://flasher.meshtastic.org/). Esto lo convierte en un nodo inapropiado, ya que el proceso de buscar un firmware, compilarlo y flasherlo excede las capacidades de un combatiente.

  Trae dos antenas que tienen un nombre para que sepas cuál es cual, pero en el instructivo, no explicita, o al menos no de manera clara dónde ubicar c/u de las antenas arriesgándote a quemar el dispositivo por un encendido con las antenas mal colocadas. Además el sistema de agarre, son plásticos, lo cual se ve endeble y limita las superficies donde puede ubicarse el mismo. 

  La compra de este dispositivo, nos dejó 2 enseñanzas a la hora de adquirir un hardware del ecosistema Meshtastic:
  - Buscar reseñas u opiniones respecto al nodo.
  - Verificar que posean firmware disponible.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/ThinkNode-M6.jpg")}
    alt="Elecrow ThinkNode M6"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**ThinkNode M6**</p>
</div>

  </TabItem>

</Tabs>

## Heltec

El MeshPocket Qi2 es un nodo bonito, se ve profesional, caro, pero por sobre todas las cosas, endeble. Posee la pantalla de papel electrónico más barata del mercado, lo que trae problemas como el ghosting que es muy molesto. Tiene una menor resolución, que junto a un tamaño mayor (mayor que la del ThinkNode M1 o M5 Pro y T-Echo) da la sensación de mayor claridad en la pantalla, no es retroiluminada. Además no posee GPS, pero como hasta el momento, esta funcionalidad en Meshtastic no es de lo más preciso, hoy no creo que sea una pérdida, pero si este panorama cambia y el GPS empieza a aumentar su precisión, si será una gran falta.

De manera similar que los ThinkNode M1 y M5 Pro, también posee dos versiones de un mismo firmware, dependiendo de la interfaz de usuario:

- <u>UI Estándar</u>: A diferencia de los nodos de Elecrow ya mencionados... Pese a no poseer un parlante, tiene opciones de manipular sus funciones. El uso de todo el dispositivo recae en un único botón, pese a que posee 3. Su funcionamiento, a diferencia de InkHUD, es aún peor, porque la cantidad de menúes y funcionalidades que ofrece, pasarte por un click, puede convertir tu experiencia de usuario en algo que pasa de molesto a frustrante en muy poco tiempo.

- <u>InkHUD</u>: Hace un buen aprovechamiento de la función de rotación de pantalla, incluso más que los otros dispositivos del mercado, esto se debe a que la pantalla es mucho más ancha que las demás. El uso completo del dispositivo con un único botón es malo, pero como ni siquiera puede enviar mensajes, su dependencia del teléfono, por lo que el mencionado aprovechamiento de la parte de lectura de mensajes, no sirve para nada. Haciendo que instalar esta interfaz en este dispositivo, no aporta en absolutamente en nada. Posiblemente sea mejor usar un WisMesh Tag, acompañado de una powerbank incluso más grande, por el mismo coste.

Creemos que es un aparato que sabe adornar sus faltas, pero son muchas y significativas, por lo que, al menos para el combate contra el fuego, no es de lo más recomendable.

Ya hablando de la marca, no queremos dejar pasar el mal servicio que nos ofrecieron en 2 oportunidades, siendo este el motivo por el cual se tomó la determinación de NO efectuar compras directamente a la marca y por ello adquirimos sus dispositivos a través de un revendedor (Muzi Works). Si te interesa saber más al respecto, [aquí](/blog/compras-12-25-p2.md) podrás ver toda nuestra experiencia con esta marca. Pese a esto la sensación que nos deja es que se sufrió demasiado por un hardware, que quizás, no estuvo a la altura de nuestro sufrimiento. Además mucho del hardware que han creado NO está listo para ser usado y además en su mayoría tiene un ESP32.

Todos estos sucesos han llevado al desinterés por la marca, no obstante la seguiremos de cerca para ver cuáles son sus avances, pero creemos que están por detrás de marcas como Elecrow o seed studio.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/MeshPocket-Qi2.jpg")}
    alt="Heltec MeshPocket Qi2"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**MeshPocket Qi2**</p>
</div>

## LilyGo

La consistencia en el control de calidad y la competitividad de sus precios frente a otras opciones del mercado han sido puntos debatibles. Para proyectos críticos de infraestructura, la confiabilidad de sus componentes sigue siendo un factor a evaluar cuidadosamente.

<Tabs>
  <TabItem 
    value="deck" 
    label={
      <div style={{ display: 'flex', alignItems: 'center', gap: '8px' }}>
        <span>T-Deck</span>
      </div>
    }
    default
  >
    
Es un aparato que no tiene coherencia de diseño. El teclado barato, junto a una distribución de sus teclas que hacen complejo su uso, el trackball que se ve aún más barato, que no funciona al 100% y una pantalla táctil que es de buen tamaño y que salva la usabilidad del dispositivo (con el display de Meshtastic UI). Además dicha pantalla se ve bien en cualquier escenario, lo cual es un aspecto positivo, independientemente de su interfaz de usuario, las cuales explicitamos a continuación: 

- UI Estándar: La misma que tienen todos los dispositivos que poseen una pantalla. Sólo ofrece dos funcionalidades extra, en comparación con las demás. Leerte un mensaje, función que está lejos de ser aceptable y 'aprovechar' el teclado para escribir un mensaje, sin embargo, no es intuitiva la manera de aprovechar esta funcionalidad. Desaprovecha por completo la pantalla táctil, por lo que debes recaer en el uso del trackball  y el "enter" del teclado ya que el trackball, a veces sirve para seleccionar, pero a veces no y esto no habla de la calidad del trackball, que si es baja, sino a los permisos que se le otorgan en determinados menúes, volviendo aún más pobre su uso.

- Meshtastic UI: Es un buen intento, pero necesita mejoras, como ignorar la funcionalidad del trackball, ya que complica de manera innecesaria la experiencia de usuario, porque el funcionamiento es bueno con la pantalla táctil. El uso del BLE, es lo más flojo de este display, ya que para poder usarlo primero debes de encontrar cómo encenderlo, cuya ubicación se encuentra junto al apagado y reinicio, lo que llevaría a uno a pensar que se han equivocado de lugar para poner esta funcionalidad y la peor es que la respuesta a esto es que no, no se encuentra mal ubicado. Esto es porque usar el BLE inhabilita el uso por completo del dispositivo, algo que también hace el dispositivo cuando lo apagas o reinicias. Debido a esto puedes usar el dispositivo sin BLE o conectarlo al teléfono, pero NO usar el dispositivo. Ante esto, uno pensaría que es una opción usar el puerto serie, algo que todos los nodos permiten y que funciona a grandísima velocidad y si es posible, pero la experiencia mala, la velocidad anteriormente mencionada no existe, ralentiza por demás al celular.

Uno de los  tres dispositivos presenta problemas para cargar, sumado a que no dura mucho la batería. Otro problema que tuvimos fue cuando estaba operando Range Test fallando y teniendo que descartar una experiencia completa debido a estos fallos. Razón que nos llevó a descartarlos por completo.

Para cerrar diría que es un nodo que posee buenas intenciones pero que no concreta nada, no recomendaría este nodo para el combate del fuego ya que es muy endeble y no posee certificación IP alguna, seguido de que su firmware, independientemente de su display, necesita muchas mejoras.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/T-Deck.jpg")}
    alt="LilyGo T-Deck"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**T-Deck**</p>
</div>

  </TabItem>

  <TabItem 
    value="echo" 
    label={
      <div style={{ display: 'flex', alignItems: 'center', gap: '8px' }}>
        <span>T-Echo</span>
      </div>
    }
  >
  :::info
  Este nodo NO fue adquirido mediante el proceso de compras porque ya disponíamos de dos unidades previo a la compra, por ello también los analizamos aquí.
  :::
  Es un nodo pequeño, sencillo de usar, cómodo y posee tres botones, uno para encender/apagar la luz de la pantalla, reiniciar, el cual está demasiado expuesto y uno de acción. Actualmente poseemos 2 dispositivos y a uno de ellos, con un bajo uso, ya se le rompió un botón.
  Al igual que todos los nodos que poseen pantalla de papel electrónico, poseen los mismos display que las demás:

  - <u>UI Estándar</u>: Impide que la posibilidad de encender la luz sea sencilla, ya que toma al sensor táctil que tiene esa función y lo convierte en un botón, pero de escasa precisión, por lo que perdimos una funcionalidad a cambio de casi nada. Pero si se puede encender la luz desde el firmware, para ello, en el menú principal deberás mantener el botón de acción un ratito, se desplegará un menú y dentro de las opciones de este deberás usar la opción de Toggle Backlight, lo cual dejará encendida la luz y para apagarla deberás hacer lo mismo, lo cual, es impráctico. No destaca en comparación con el display InkHUD de los ThinkNode M1 y M5 Pro.

  - <u>InkHUD</u>: Provee una experiencia, similar al MeshPocket Qi2, solo posee un botón, lo cual, como hemos mencionado anteriormente, es pobre. Y de manera similar a éste, tampoco puede enviar mensajes, por lo que el celular se convierte en algo indispensable.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/T-Echo.jpg")}
    alt="LilyGo T-Echo"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**T-Echo**</p>
</div>

  </TabItem>
</Tabs>

## Meshnology

Su nodo, el N37 utiliza de hardware interno un Wio Tracker L1, por lo que no hablaremos del funcionamiento sino del "extra" que aporta este ensamblador en comparación al Wio Tracker L1 Pro. Y los diferencian dos cosas:

- Batería: 3000mAh, posee 1000mAh que el L1 Pro, lo cual está bien, pero puede que sea un exceso.
- Carcaza: No posee aspectos positivos.
  + Impresa en 3D, en un material endeble y que no puede ser expuesto al sol o calor.
  + Posee intersticios donde puede ingresar el polvo o humedad.
  + La cantidad de tornillos no alcanza para sellar bien el dispositivo.
  + En una caída de 75cm se rompió la parte que contiene la antena GPS.
  + El joystick imposibilita el uso del dispositivo.
  + Inestabilidad al estar en posición vertical.

No hay motivos para adquirir este producto, no solo en el contexto del combate del fuego, sino en cualquier contexto, ya que el Wio Tracker L1 Pro es mejor y más barato. Es importante que el ensamblador rediseñe esta carcasa y en un material fiable, ya que no se le pide que tenga una certificación IP, pero que al menos no empeore el funcionamiento del hardware.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/N37.jpg")}
    alt="Meshnology N37"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**N37**</p>
</div>

## RAK

El WisMesh Tag, hasta el momento es el inesperado gran ganador de esta jornada de análisis. Posee un diseño sencillo, pero efectivo, posee dos botones uno de acción grande frontal y uno de reset en la parte posterior del dispositivo, que es muy difícil que lo aprietes por accidente, lo que se agradece.

Posee tres luces que indican el estado actual del dispositivo, lo cual es sencillo pero efectivo, posee una batería pequeña pero que nos ha durado más de dos días, viene con una correa para colgarlo del cuello y certificación IP66. 

La única contra de este dispositivo es su cable de carga/datos, el cual tiene un pin particular, por lo que deberás cuidarlo de que no se rompa o extravíe. Es importante destacar que su funcionamiento es impecable, pero la contra viene del lado de la inexistencia de un reemplazo en el mercado local.

Por el momento puede que sea el estándar para los combatientes del fuego, pero quedan pruebas aún por hacer.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/WisMesh-Tag.jpg")}
    alt="RAK WisMesh Tag"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**WisMesh Tag**</p>
</div>

## seed studio

Es la marca más balanceada. Posee buenos precios, una entrega rapidísima de sus productos y los dispositivos que producen tienen coherencia de diseño, calidad. Aparte es la marca que aparenta estar en un constante innovación. Además es una de las pocas que te vende sus productos en un paquete, ya que como hemos mencionado, esto funciona en malla y mientras más nodos, mayor es la cobertura y su extensión, esto muestra la visión de la marca.

<Tabs>
  <TabItem
    value="l1"
    label={
      <div style={{ display: 'flex', alignItems: 'center', gap: '8px' }}>
        <span>Wio Tracker L1 Pro</span>
      </div>
    }
    default
  >

  Es un nodo pequeño, cómodo, con una buena batería, que le permite superar las 72 hs en escenarios sin tráfico de radio, con Bluetooth y GPS encendidos. La pantalla, pese a ser LCD y consumir más que las de papel electrónico, tienen un botón para apagarlas, lo que baja enormemente el consumo, ya que solo estará encendida al momento de su uso, además es mucho más veloz que las pantallas de papel electrónico. 

La carcasa parece impresa en 3D, pero se ve bien, posee un hueco por donde se puede pasar una correa a un dispositivo pero no posee estabilidad de manera vertical, no se queda parado en una mesa.

  Que tenga un botón en el joystick con una función tan central, no creo que sea lo mejor, quizá invertir los roles con el botón que posee al lado, sea lo más óptimo, ya que este último solo sirve para ir hacia atrás o apagar/encender la pantalla. El botón de reset, pese a estar expuesto, no se aprieta con tanta facilidad, posee un interruptor de encendido/apagado del dispositivo. 

  Los problemas que experimentamos con el dispositivo es que la pantalla deja de funcionar, pero el dispositivo está operativo, que el dispositivo se trabe o que tenga desconexiones esporádicas del pc, pero todo esto se soluciona rápidamente con un reinicio. No obstante no creemos que sean problemas menores, pero analizaremos si fueron cuestiones aisladas o más bien si el hardware tiene problemas. 

  Si no fuera por los problemas mencionados anteriormente, diríamos que son los nodos más adecuados dentro de lo que hay en el mercado con pantalla.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/Wio-Tracker-L1.jpg")}
    alt="SeedStudio WioTracker L1"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**WioTracker L1**</p>
</div>

  </TabItem>

  <TabItem
    value="p1"
    label={
      <div style={{ display: 'flex', alignItems: 'center', gap: '8px' }}>
        <span>SenseCAP Solar Node P1</span>
      </div>
    }
  >

  Tiene un buen armazón de agarre en metal, junto a una abrazadera también de metal, posee certificación IP65, posee un cable que permite montar la antena en el armazón y no directamente en el nodo.

  Posee varias luces que indican el estado del nodo y varios botones, junto a un chip nRF52 y una falta de GPS tiene un bajo consumo de energía. Esto es así porque el nodo que hemos adquirido viene sin GPS y baterías, pero el P1 Pro si trae el GPS y las baterías.

  Lo único negativo hasta el momento es que debe usar 4 baterías 18650, lo cual nosotros ya sabíamos, pero no indican que la misma deba tener un relieve en el cátodo, comúnmente conocido como botón o tetón. Igual, creemos que es un buen nodo, a un bajo precio. 

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/SenseCAP-Solar-Node-P1.jpg")}
    alt="SeedStudio SenseCAP Solar Node P1"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**SenseCAP Solar Node P1**</p>
</div>

  </TabItem>
  
  <TabItem
    value="t1000"
    label={
      <div style={{ display: 'flex', alignItems: 'center', gap: '8px' }}>
        <span>SenseCAP T1000-E</span>
      </div>
    }
  >
  Incluye su cable de carga, lo cual se agradece, pero al ser particular y no el típico USB C, era necesario que te lo proveyeran, algo que NO hacen con el WioTracker L1 Pro, porque usa un USB C. Tampoco te dan la correa pese a que posee el espacio por donde puede pasar una.

  En cuanto al aparato en sí es un poco más pequeño de base, altura y espesor que el WisMesh Tag, parece más endeble, posee una certificación IP menor que el mencionado nodo,una batería más pequeña y su armazón transparente se ve bien estéticamente hablando pero confunde el botón con el parlante y la luz de notificaciones. No posee botón de reinicio, por lo que para actualizarlo, habrá que hacerlo entrar en modo DFU desde la PC. A diferencia del mencionado WisMesh Tag que posee tres luces de notificación, permitiéndole al usuario entender de manera sencilla los estados que atraviesa el nodo, pero el T1000-E sólo posee una, lo que limita este intercambio de información con el usuario.

  En cuanto a funcionamiento anda bien, no es para nada un mal nodo, pero sí claramente inferior al WisMesh Tag, ya que incluso salen lo mismo. Si tenés interés en comprar como un paquete de nodos, posibilidad que esta empresa te brinda, es un nodo útil, pero si sólo necesitas un nodo tipo card posiblemente sea mejor que pienses en un WisMesh Tag.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/SenseCAP-T1000-E.jpg")}
    alt="SeedStudio SenseCAP T1000-E"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**SenseCAP T1000-E**</p>
</div>

  </TabItem>
</Tabs>

## Spec5

El Voyager es un modelo que presenta una idea interesante, aún nos queda por testear si realmente cumple con estas expectativas o no. Pero lo que podemos decir de este nodo es que posee un buen agarre con los 4 imanes que posee, la antena no destaca y la electrónica tiene una buena aislación, pero... ¿A qué costo? Económicamente a uno elevado, a nivel de diseño, fue uno aún más alto, porque no tenes puerto USB a menos que abras el dispositivo, no hay botones a menos que abras el dispositivo, no hay luces a menos que abras el dispositivo y no hay encendido/ apagado a menos que conectes/desconectes la batería y para ello también había que abrir el dispositivo. 

Creo que falta trabajo de diseño y si la idea que este nodo representa te interesa, antes de adquirirlo, sugeriría que busques alternativas para imprimir en 3D dentro de la comunidad y armar un nodo custom basado en esta idea.

Hablando de la marca, pese a que tenemos un sólo dispositivo, es posiblemente la marca que mejor vea y entienda el mercado de la tecnología LoRa, sus precios son elevados y no podríamos hablar de la calidad de sus productos, pero ya sabe lo que pensamos sobre este único dispositivo que tenemos. No posee envíos a Argentina, por lo que si decides adquirir sus productos, necesitarás un importador, un gasto extra que debes tener en cuenta.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img
    src={useBaseUrl("/img/S5-Voyager.jpg")}
    alt="Spec5 Voyager"
    style={{
      maxWidth: '100%',
      height: 'auto',
      display: 'block',
      margin: '0 auto'
    }}
  />
  <p>**Voyager**</p>
</div>

---

El mercado si bien ofrece una cantidad interesante de nodos, bajo nuestra visión actual de lo que un nodo debe poseer, *no hay uno que cumpla con estas expectativas*, pero entendemos que es una tecnología joven, en constante desarrollo y que aún necesita mejoras. No obstante creemos que el WisMesh Tag posiblemente sea el nodo más adecuado en el escenario portable, mientras que el el aspecto de repetidor, el mejor es el SenseCAP Solar Node P1, en su versión base o Pro.

Haciendo un balance de todos los [fabricantes y ensambladores](/blog/fabricantes-ensambladores) creemos que hasta el momento existen dos marcas, seed studio y Elecrow, que están por delante de las demás, seguidos de cerca por RAK, los demás fabricantes no ofrecen grandes cosas, pero en los ensambladores hay movimientos cada vez más interesantes, que seguiremos de cerca.

Con respectos a las diferencias entre procesadores ESP32 y nRF52. Creemos que aún faltan pruebas concluyentes pero a grandes rasgos no hay diferencias significativas por las cuales descartar a uno u otro. La eficiencia de la batería de la batería no es lo suficientemente determinante como para ponerlo por encima de los ESP32 y en contrapartida no ofrece cualidades específicas determinantes que lo pongan por encima de los nRF52.

Creemos que esta tecnología va por buen camino, nosotros intentaremos contribuir también para sus mejoras, independientemente si esta es usada por Meshtastic o MeshCore.
