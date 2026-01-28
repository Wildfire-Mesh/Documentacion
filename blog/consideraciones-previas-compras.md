---
slug: consideraciones-previas-compras
title: ¿Qué debes saber antes de comprar tu primer dispositivo Meshtastic?
sidebar_label: Consideraciones técnicas previas a la compra de dispositivos
authors: 
  - key: MrNetsky
    title: Autor
  - key: nicopace
    title: Colaborador
tags: [dispositivos]
---
 
En los últimos años Meshtastic y proyectos similares han ido ganando popularidad, al punto que hoy ya empieza a parecer una tecnología que puede que deje de ser solo para hobbistas. Sin embargo, la amplia variedad de dispositivos disponibles en el mercado, que van desde simples placas de desarrollo hasta productos finales robustos, puede ser abrumadora. Antes de invertir en un nodo, es crucial entender cómo las especificaciones técnicas del hardware ya que afectarán tu experiencia de uso, sea en entornos urbanos densos o en vastas áreas rurales. Esperamos que esta guía te ayude a navegar por las especificaciones más importantes, para que puedas elegir el dispositivo que  se adapte a tu uso.

En esta guía nos centraremos exclusivamente en dispositivos listos para usar, dejando de lado la posibilidad de construir tu nodo por tus propios medios (DIY), ya que esto requiere de conocimientos técnicos más avanzados.

### Frecuencia y Región

Este es un punto muy importante, ya que comprar la frecuencia incorrecta hace que el dispositivo sea inutilizable en tu área. Por ello es necesario conocer la verificación regulatoria ya que los dispositivos LoRa operan en bandas de frecuencia ISM (industrial, ciencia, y medicina) que son diferentes en cada continente. Debes asegurarte de que el dispositivo que compres está configurado para la banda de tu región. En nuestro caso, en Argentina la adecuada es 915Mhz. Además la antena debe estar ajustada específicamente para la frecuencia elegida (ej. una antena de 868 MHz funcionará muy mal a 915 MHz).

### Microcontrolador (MCU) y Conectividad

El chip principal determina el rendimiento, las capacidades y el consumo de energía del dispositivo. En este aspecto, encontramos 2 alternativas:

+ *ESP32* (de Espressif Systems):
ESP32 (de Espressif Systems): Es el más común y versátil. Suele ser más económico, tiene mucha memoria e incluye Wi-Fi. Pero conlleva un mayor consumo de energía, lo que reduce la duración de la batería. Actualmente es el más utilizado en dispositivos tipo celular, smartwatch.

+ *nRF52* (de Nordic Semiconductor):
No incluyen Wi-Fi, son más costosos y menos potente. Aún con ello su consumo de energía ultra bajo, lo hacen los más recomendables en nodos portátiles o tipo powerbank.

Ambos incluyen conexión Bluetooth, necesaria para concetar el dispositivo con el teléfono.

Hay otras opciones, pero no encontramos dispositivos terminados con ellas, por lo que quedaron excluidas de esta lista.

:::tip NOTA:
¿Quieres saber cuales son o qué características conllevan los tipos de dispositivos aquí mencionados? <u> [***Aquí tenemos un artículo donde hablamos de ello***](/blog/tipos-de-dispositivos) </u>
:::

### GPS

Es un apartado importante e innecesario a la vez y esto se debe al tipo de dispositivo que lo tenga. Me explico, si hablamos de dispositivos móviles, es una utilidad necesaria, e incluso hay dispositivos que pueden encender y apagar la posición según desee o si la necesidad de ahorrar batería apremia. Pero en nuestro caso particular, donde dirigimos el uso de estos dispositivos a los bomberos, se vuelve vital su uso.

En contrapartida, en un nodo fijo, es mejor no tenerlo pues aumenta el precio del mismo y el consumo energético, pero si ya lo incluye, es mejor no hacer uso, porque demanda un consumo de energía y no aporta en absolutamente nada.

Entonces usted en este momento se preguntará el por qué esta diferencia. Y esto se debe a que un nodo fijo se ubicará en un lugar específico, usted sabrá donde se encuentra, incluso puede mapearlo, sumado a que generalmente tienen un suministro constante de energía y baterías para cubrir los momentos en los que no, por lo que está conectado 24/7 y si desea saber si el nodo está activo sólo deberá comunicarse con el mismo.

Además es importante saber con qué velocidad puede hacer GPS Lock, ya que mientras mayor sea ésta, mejor será. Otra apartado es el económico. ya que el incluir o no GPS, puede aumentar o disminuir el costo. Tenerlo en cuenta es vital si se tiene un presupuesto ajustado y no necesita en todos o en ningún dispositivo esta funcionalidad.

### Pantalla y tipo

Son útiles para interactuar con el dispositivo y existen 3 tipos:
+ *LCD*: 
        * Menos eficiencia energética.
        * Pobre visibiliad en el exterior.
        * Más económica.
+ *OLED*: 
        * Eficiencia energética media.
        * Posee una mejor visibilidad que la LCD, pero inferior a la E-Ink. Pero si posee el mejor contraste de las 3.
        + Costo itermedio
+ *E-Paper*: 
        * Mayor eficiencia energética.
        * Ostenta la mejor vibilidad en el exterior. Suelen incluir un interruptor o reglador de luz. 
        * Tiempo de respuesta significativamente mayor en comparación con las otras.
        * Más costosa.

Su consumo de energía disminuye la durabilidad de la batería. Por lo que para nodos portátiles será mejor usar un nRF52, en busca de una autonomía que permita ser usado durante una jornada completa de combate contra el fuego, sin la necesidad de depender de un powerbank o un nodo de repuesto. Las más usadas son las OLED y la de papel electrónico.

Debido a la ausencia actual de pantallas en dispositivos fijos, este autor se pregunta, ¿serán de utilidad?. Y si lo fueran ¿cuán útiles serían?, ¿Qué tamaño deberían tener? ¿De qué tipo debería ser? ¿Esta decisión dependerá de un MCU específico?

### Batería(mAh)

Una capacidad mayor de miliamperios-hora es mejor. Sin embargo, el rendimiento final de la batería dependerá del MCU, si utiliza una pantalla cuyo consumo dependerá según sea el tipo y a qué información está enviando, ya que enviar la posición constantemente consume energía. Esto también aplica para cuando envía datos de los sensores. 

No interesa en si el tamaño de la batería, sino que la misma pueda nos permita completar las tareas, sin la necesidad de depender de un powerbank para poder completarlas. 

### Armazón

Algunos de los aspectos que nos interesan son los siguientes: 

* <u>Protección Ambiental:</u>
  * Certificación IP67/IP68: Es lo más importante. Significa que es totalmente estanca al polvo y puede sumergirse en agua. Esta certificación puede aplicar a todo el dispositivo o a sólo una parte, como el puerto USB por ejemplo.

  * Resistencia UV: Si vas a dejar el nodo en un techo o una montaña, el plástico común se rompe con el sol. Lo ideal es ABS, ASA o Policarbonato.

* <u>Material no conductor:</u> Evita carcasas de fibra de carbono o metales si la antena va interna, ya que interfieren con la señal.

* <u>Usabilidad y Montaje:</u> 
  * Puntos de anclaje: Ranuras para pasar precintos (zip-ties), correas o imanes potentes para pegarlo a superficies metálicas.

  * Interacción: Que su/s puertos o botón/es estén disponibles para el uso, sin la necesidad de tener que abrir el case para poder interactuar con ellos directamente desde la placa.

### Antenas 

En Meshtastic, las antenas se diferencian por tres factores clave:

* <u>Conectores (SMA vs. RP-SMA):</u> Es el error más común al comprar repuestos. El conector SMA (estándar en la mayoría de estos equipos) tiene un pin central en el cable. El RP-SMA (común en routers Wi-Fi) tiene el hueco. Si no coinciden, no habrá contacto físico y podrías dañar el transmisor de tu nodo.

* <u>Ganancia (dBi):</u> Imagina que la señal es una linterna.

  * Baja ganancia (2-3 dBi): La señal sale como una esfera en todas direcciones. Es ideal para bomberos en terrenos montañosos o con muchos desniveles, donde la señal debe "subir y bajar" cerros.

  * Alta ganancia (8-12 dBi): La señal se aplasta y se estira como un disco plano para llegar muy lejos. Es perfecta para nodos fijos en techos o torres que necesitan conectar con otros puntos distantes en el horizonte.

* <u>Tipo de construcción:</u>

  * Rubber Duck (Varilla): Son las pequeñas y flexibles que vienen de fábrica, ideales para llevar en la mochila o el cinturón.

  * Fibra de Vidrio (Omnidireccionales): Tubos rígidos y largos diseñados para exterior. Son la mejor opción para infraestructura fija por su durabilidad y rendimiento.

  * Direccionales (Yagi): Solo envían y reciben señal en una dirección específica. Son útiles únicamente para "puentes" fijos entre dos puntos conocidos que están muy alejados.

---

La incursión en el ecosistema Meshtastic exige pasar de la mera curiosidad tecnológica a una compra estratégica informada. Como hemos analizado, la elección del dispositivo es un ejercicio de equilibrio de compromisos que debe estar rigurosamente alineado con el entorno operativo y los objetivos de la misión.

En última instancia, el dispositivo ideal es aquel que sacrifica la funcionalidad innecesaria para potenciar lo esencial. Para la comunicación de primera línea (móvil), la autonomía y el GPS confiable son innegociables, favoreciendo los chips nRF52 y las pantallas E-Paper. Para la infraestructura (fija), el enfoque está en la estabilidad 24/7, la potencia de transmisión y la carga solar robusta para asegurar la continuidad de la red.
