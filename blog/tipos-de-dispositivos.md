---
slug: tipos-de-dispositivos
title: 'Más alla del tamaño: La guía definitiva para elegir un dispositivo basado en su función'
sidebar_label: Tipos de dispositivos
authors: 
  - key: MrNetsky
    title: Autor
  - key: nicopace
    title: Colaborador 
  - key: aguslasp
    title: Colaborador
tags: [dispositivos]
---
 
En un mundo cada vez más dependiente de la infraestructura centralizada, la capacidad de comunicarse fuera de la red (u off-grid) se ha convertido en una necesidad vital. El proyecto Meshtastic, basado en la robusta tecnología de radio LoRa, ofrece precisamente esta solución: una red de malla descentralizada, sin necesidad de Wi-Fi o cobertura celular.

La clave para desplegar y optimizar tu propia red radica en elegir el dispositivo correcto para cada función. La comunidad Meshtastic ha generado una impresionante diversidad de hardware, lo que puede resultar abrumador a la hora de decidir.

Esta guía ha sido diseñada para simplificar esa elección. Analizaremos los nodos Meshtastic separándolos en dos grandes pilares según su propósito y entorno operativo:

:::tip Para tener en cuenta...
En este artículo se hablará sobre chips nRF52840 y ESP32, que se utilizan para el funcionamiento de los dispositivos Meshtastic, en este artículo NO se ahondará sobre las diferencias técnicas, lo que SÍ debe saber es que el primero consume menos energía que el segundo. 
:::


## Portables

Si la meta principal de Meshtastic es la comunicación descentralizada, los nodos portátiles son las herramientas que ponen esa capacidad directamente en manos del usuario, el excursionista o el explorador. A diferencia de los nodos que pueden utilizarse como estaciones o bases estáticas, estos dispositivos están diseñados para operar con baterías de manera eficiente y acompañarte en el campo.

Esta categoría es la más diversa y se define por un constante equilibrio entre la portabilidad y la funcionalidad. Aquí, la elección se reduce a dos preguntas clave: ¿necesitas interacción inmediata o máxima autonomía?. En base a ello, te presentamos las siguientes opciones:

### Con pantalla

Son dispositivos diseñados para funcionar como pequeños comunicadores autónomos, similares a un walkie-talkie de texto, lo que los hace ideales para un usuario que quiere inmediatez y visibilidad del estado de la red sin depender siempre de un móvil. Busca un equilibrio entre la retroalimentación visual y la autonomía de la batería. Su propósito principal no es escribir mensajes, sino mostrar información clave de forma inmediata.

Pueden incluir una pantalla OLED, LCD o E-Paper (las más eficientes en consumo de energía), buzzer y sensores. La mayoría se controlan mediante botones, algunos incluyen la posibilidad de encender o apagar el GPS, permitiendo extender la duración de la batería, ya que el uso del GPS resulta ser el mayor consumo del dispositivo.

La resolución y el tamaño limitan la cantidad de información que se puede mostrar a la vez. El usuario debe seguir utilizando el móvil para la mayoría de las interacciones, escritura y configuración avanzada.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img 
    src="https://meshnology.com/cdn/shop/files/meshnology-n37-black-1pcs.png?v=1763800746&width=800" 
    alt="Dispositivo portable con pantalla" 
    style={{ 
      maxWidth: '100%', 
      height: 'auto', 
      display: 'block', /* Elimina espacio extra debajo de la imagen */
      margin: '0 auto' /* Centra la imagen si es más pequeña que el 100% */
    }}
  />
  <p>**Meshnology N37 (basado en un WioTracker L1)**</p>
</div>

### Sin pantalla

Perfectos para aquellos que solo necesitan un nodo que funcione como rastreador GPS o repetidor personal, sin llamar la atención u ocupar mucho espacio..

La ausencia de pantalla le permite un mayor espacio para antenas y baterías, que junto a un chip nRF52840, obtiene una eficiencia energética similar al que viene con pantalla, independientemente del tipo de ésta.

La gran mayoría no poseen una certificación IP (a excepción de RM-1 Ruggedized MANET Radio, de Constellation Response, pero su precio es muy alto en comparación al resto de la categoría e incluso comparado con todos los tipos de dispositivos Meshtastic).

Si hay problemas de conexión Bluetooth o el firmware falla, puede ser difícil de diagnosticar y actualizar sin conectar un cable USB. La interacción es menos intuitiva que en un dispositivo con pantalla. Esto es un problema que no solo pertenece a este tipo de dispositivo, sino a todo aquel que no posea una pantalla, ya que la pantalla resulta versátil especialmente para lograr la conexión bluetooth entre este y el teléfono.

<div style={{ display: 'flex', gap: '20px', justifyContent: 'center' }}>
  <div style={{ flex: 1, textAlign: 'center' }}>
    <img 
      src="https://atlavox.com/cdn/shop/files/M1915Swivel.png?v=1752610387&width=823" 
      alt="Dispositivo portable sin pantalla" 
      style={{ 
        maxWidth: '100%', 
        height: 'auto', 
        maxHeight: '300px', /* Limita la altura para que ambas queden bien */
        objectFit: 'contain' /* Asegura que la imagen se vea completa */
      }}
    />
    <p>**Atlavox M1**</p>
  </div>

  <div style={{ flex: 1, textAlign: 'center' }}>
    <img 
      src="https://store.rakwireless.com/cdn/shop/files/wismesh-mini-pocket-11_d7d736c7-860b-4a50-b297-6b3dacd0c42e_900x.progressive.png?v=1745821658" 
      alt="Dispositivo portable sin pantalla" 
      style={{ 
        maxWidth: '100%', 
        height: 'auto', 
        maxHeight: '300px', /* Aplica la misma limitación de altura */
        objectFit: 'contain' 
      }}
    />
    <p>**WisMesh pocket mini**</p>
  </div>
</div>

### Tipo tarjeta

Ultra-delgados y livianos, a menudo pensados para caber cómodamente en una billetera, bolsillo de ropa o integrarse en objetos pequeños. Ideales para tracking. Permiten una duración de batería aceptable a pesar de tener una capacidad muy limitada. Son perfectos para usuarios no técnicos que solo necesitan un nodo que funcione y reporte su posición.

Poseen una ficha de carga distinta (como puede verse en la imágen inferior), no el convencional USB tipo C, lo que nos obliga a extremar los cuidados sobre el cargador ya que, hasta el momento, en base a nuestra investigación no hemos encontrado sustitutos alternativos en el mercado argentino y cuando lleguen al mercado habrá que testear la compatibilidad y la funcionalidad, es decir, por el momento es necesario usar el original. En caso de tener dos o más dispositivos se reutiliza el de otro dispositivo, pero si no, deberás indagar sobre la disponibilidad en el mercado extranjero para importar uno, ya que este tipo de nodo no posee otro tipo puerto de carga.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img 
    src="https://media-cdn.seeedstudio.com/media/catalog/product/cache/bb49d3ec4ee05b6f018e93f896b8a25d/_/_/___1_.jpg" 
    alt="Dispositivo portable tipo card" 
    style={{ 
      maxWidth: '100%', 
      height: 'auto', 
      display: 'block', 
      margin: '0 auto' 
    }}
  />
  <p>**SenseCAP card tracker T-1000**</p>
</div>

### Powerbank

Ideal para usar como nodo de reserva en una mochila, nodo de viaje o como un repetidor temporal de "larga vida".  Lo que este autor se pregunta es si vale la pena este tipo de dispositivos, ya que por el precio puedes conseguir powerbanks más grandes y de mayor calidad para abastecer tu dispositivo Meshtastic principal.  En el caso de que necesites un nodo de reserva, podés utilizar otro de los mencionados anteriormente.

Los hay con y sin pantalla, con la potencia de radio similar a los dispositivos tipo tarjeta. Poseen una batería de gran capacidad y en el caso particular del dispositivo que se muestra en pantalla, posee carga inalámbrica. Cabe aclarar que según nuestras investigaciones hasta la fecha, no existen dispositivos que puedan aprovechar esta funcionalidad, pero si hay celulares que pueden. También recomendamos ejemplares que posean un chip nRF52840, ya que los ESP32 disminuyen el potencial del nodo porque demandan un mayor consumo de energía.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img 
    src="https://heltec.org/wp-content/uploads/2025/03/a-6-1536x1536.jpg" 
    alt="Dispositivo portable tipo powerbank" 
    style={{ 
      maxWidth: '100%', 
      height: 'auto', 
      display: 'block', 
      margin: '0 auto' 
    }}
  />
  <p>**Meshpocket Qi2**</p>
</div>

### Smartwach

Combinan la portabilidad extrema con una interacción directa limitada. Al estar sujeto en la muñeca del usuario, minimizan la posibilidad de que el dispositivo se extravíe. Esto es relevante, porque donde esté el dispositivo casi con seguridad también se encontrará el combatiente. Esto gana importancia en caso de que el combatiente se encuentre incapacitado para comunicarse.

Es una iniciativa interesante, ya que, además de su posición, potencialmente puede enviar datos de vital importancia relacionado con la salud en tiempo real del combatiente del fuego como lo puede ser la oxigenación en sangre o presión. Permitiendo a quienes coordinan el operativo saber en todo momento no sólo dónde se encuentran sus combatientes, sino también su estado de salud. Aunque en este momento esta es una funcionalidad NO existente.

Actualmente, tienen una escasa variedad en lo que a cantidad, modelos y marcas se refiere. Los modelos existentes poseen un chip ESP32, que es más demandante en cuanto a energía y sumado a una pequeña batería lo hace poco autónomo. Desde este espacio estamos atentos y a la expectativa de cómo avanza la tecnología de estos dispositivos.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img 
    src="https://lilygo.cc/cdn/shop/files/LILYGO-T-Watch-S3_1.jpg?v=1685513964&width=823" 
    alt="Dispositivo portable tipo smartwatch" 
    style={{ 
      maxWidth: '100%', 
      height: 'auto', 
      display: 'block', 
      margin: '0 auto' 
    }}
  />
  <p>**LilyGo T-Watch S3**</p>
</div>

### Tipo celular

Estos dispositivos están diseñados para ser las unidades principales de comunicación personal en una red Meshtastic. Tienen una pantalla grande con teclado físico o una pantalla táctil y la capacidad de llevar una antena externa de alta eficiencia. Permite una operación totalmente independiente del móvil, un gran plus en entornos donde el móvil puede fallar o estar apagado.

Al igual que los dispositivos tipo smartwach, poseen un ESP32, que, sumado a todas las funcionalidades que aportan, limitan mucho la autonomía de la batería del aparato. Debido a esto, puede que dependa de un powerbank para poder usarse en una jornada completa de combate contra el fuego, pero puede ser una unidad interesante en posiciones donde tenga acceso a energía de donde recargarse.

<div style={{ display: 'flex', gap: '20px', justifyContent: 'center' }}>
  <div style={{ flex: 1, textAlign: 'center' }}>
    <img 
      src="https://lilygo.cc/cdn/shop/files/T-DECK-PLUS_6.jpg?v=1748422600&width=823" 
      alt="Dispositivo portable tipo celular N°1" 
      style={{ 
        maxWidth: '100%', 
        height: 'auto', 
        maxHeight: '300px', /* Limita la altura para que ambas queden bien */
        objectFit: 'contain' /* Asegura que la imagen se vea completa */
      }}
    />
    <p>**LilyGo T-deck Plus**</p>
  </div>

  <div style={{ flex: 1, textAlign: 'center' }}>
    <img 
      src="https://specfive.com/cdn/shop/files/2_8809a9c0-7ad4-433b-99e5-2838c0eaf02a.png?v=1738930723&width=810" 
      alt="Dispositivo portable tipo celular N°2" 
      style={{ 
        maxWidth: '100%', 
        height: 'auto', 
        maxHeight: '300px', /* Aplica la misma limitación de altura */
        objectFit: 'contain' 
      }}
    />
    <p>**Spec5 Spectre**</p>
  </div>
</div>

:::danger ACLARACIÓN:
El T-deck Plus es una unidad autónoma que solo ejecuta meshtastic. El Spec5 Spectre es un nodo meshtastic conectado a un telefono android mini.
:::

## Fijos

Si los dispositivos portátiles son los comunicadores en primera línea, los nodos fijos son la infraestructura que da sentido a la red Meshtastic. Esta categoría incluye los nodos de alta potencia montados en estaciones de trabajo y los dispositivos para vehículos, cuya misión es garantizar la máxima cobertura y estabilidad a largo plazo.

### Estaciones de trabajo

Están diseñados para usar antenas externas de alta ganancia para maximizar el alcance y la recepción. Se montan típicamente en altura para obtener la mejor línea de visión.

Pueden configurarse como Gateways para enlazar la red LoRa con Internet (a través de Wi-Fi/Ethernet) usando protocolos como MQTT. Esto permite a los usuarios enviar mensajes a través de Meshtastic a otros nodos en cualquier parte del mundo.

Incluyen, en su mayoría, paneles solares y disponibilidad 24/7. Al estar conectados permanentemente, no tienen tiempo de inactividad, además la mayoría de los modelos incluyen baterías que le dan un poco más de autonomía en caso de un corte en el suministro energético.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img 
    src="https://store.rakwireless.com/cdn/shop/files/meshtastic-wismesh-repeater-mounted_865x@2x.progressive.png?v=1751439728" 
    alt="Dispositivo fijo" 
    style={{ 
      maxWidth: '100%', 
      height: 'auto', 
      display: 'block', 
      margin: '0 auto' 
    }}
  />
  <p>**WisMesh Repeater**</p>
</div>

### Para vehículos

Es una forma dinámica y eficiente de mapear y extender el alcance de la red sobre grandes distancias, como una carretera. Viene dotado de un panel y una batería, además de la posibilidad de conectarlo directamente al vehículo para alimentación alternativa.

Ideal para logística, seguimiento de flotas o simplemente para compartir la ubicación durante un viaje en grupo. Quedará para un artículo del futuro hablar sobre si la interferencia electromagnética del auto afecta a la señal del nodo.

<div style={{ textAlign: 'center', marginBottom: '40px' }}>
  <img 
    src="https://specfive.com/cdn/shop/files/5_2d20a3eb-3499-47bd-b3d9-f158698a2f97.jpg?v=1753353253&width=810" 
    alt="Dispositivo fijo para vehículos" 
    style={{ 
      maxWidth: '100%', 
      height: 'auto', 
      display: 'block', 
      margin: '0 auto' 
    }}
  />
  <p>**Spec5 Voyager**</p>
</div>

---

El proyecto Meshtastic no es solo un conjunto de dispositivos; es una plataforma de resiliencia y comunicación descentralizada habilitada por la tecnología LoRa. Elegir el nodo adecuado, tal como hemos visto, se reduce a alinear la capacidad del hardware con la misión o el entorno operativo específico.

Para el usuario en movimiento (excursionista, combatiente, explorador), la decisión se centra en el equilibrio entre inmediatez y autonomía:

        + Los dispositivos con pantalla y los de tipo celular ofrecen una interfaz de comunicación directa, vital cuando no se puede depender de un smartphone, a costa de una menor eficiencia energética (especialmente con chips ESP32).

        + Los nodos sin pantalla y de tipo tarjeta priorizan la máxima autonomía y la portabilidad discreta, siendo ideales como trackers personales o repetidores de bolsillo de larga duración, sobre todo cuando usan el chip nRF52 de bajo consumo.

Por otro lado, la estabilidad y el alcance definen la categoría de nodos Fijos:

        + Las Estaciones de trabajo y los Repetidores para vehículos son la columna vertebral de la red, garantizando la máxima cobertura y ofreciendo funcionalidades avanzadas como la conectividad Gateway para enlazar la red local LoRa con el Internet global, esencial para operaciones de gran escala o logísticas.

En definitiva, la verdadera potencia de Meshtastic reside en la capacidad de combinar inteligentemente estos distintos tipos de nodos. Una red de malla optimizada usará repetidores fijos de alta potencia en puntos estratégicos (Estaciones de trabajo) para crear un área de cobertura robusta, mientras que el personal en el terreno llevará dispositivos portátiles (sin pantalla para rastreo y con pantalla para comunicación) adaptados a las demandas de su jornada.

Al comprender las fortalezas y debilidades —desde la durabilidad hasta la autonomía del chip (nRF52 vs. ESP32)—, el usuario puede diseñar una red de malla verdaderamente a medida, garantizando la comunicación off-grid en cualquier escenario, desde la aventura solitaria hasta un complejo operativo de respuesta ante emergencias.





