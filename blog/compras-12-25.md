---
slug: compras-12-25
title: 'Nos fuimos de compras: Nuestra primera experiencia adquiriendo dispositivos Meshtastic'
sidebar_label: Compras 12/2025 - Parte 1
authors:
  - key: MrNetsky
    title: Autor
  - key: nicopace
    title: Colaborador
tags: [dispositivos]
---

En el camino hacia la implementación de redes de comunicación descentralizadas para combatientes del fuego, la teoría y la planificación deben dar paso a la acción concreta. Después de un riguroso análisis de las funciones y especificaciones técnicas ideales para nuestros nodos Meshtastic, llegó el momento decisivo: el proceso de adquisición. Esta etapa, aparentemente sencilla, se transformó en una verdadera aventura logística y económica.

Este artículo detalla nuestra primera experiencia de compra de dispositivos Meshtastic a nivel internacional, una inmersión forzosa en la dinámica del e-commerce global. Nuestro objetivo no solo era obtener el hardware necesario para iniciar talleres de formación y pruebas de campo, sino también evaluar los desafíos logísticos que enfrentará cualquier implementador en Argentina. A continuación, desglosamos cuáles fueron los dispositivos elegidos, el intrincado proceso de compra, los variados métodos de envío, los precios finales y los tiempos, tanto estimados como reales, de entrega. Esta guía está diseñada para convertir nuestra curva de aprendizaje en un camino más llano para futuros proyectos.

## ¿Cuáles son y por qué elegimos estos dispositivos?

Nuestro objetivo fue intentar abarcar la mayor cantidad de dispositivos que, a nuestro juicio, los combatientes pueden sacarle partido para poder llevar a cabo talleres de formación y prubas de campo. La elección sobre qué dispositivos se iban a adquirir no fue sencilla, pues hicimos un equilibrio entre la [*función*](/blog/tipos-de-dispositivos) que pueden desempeñar y sus [*especificaciones técnicas*](/blog/consideraciones-previas-compras), sin dejar afuera a ningún fabricante (tenga en cuenta que fabricante y ensamblador NO son lo mismo y [*aquí*](/blog/fabricantes-ensambladores) puede ver la diferencia). 

Si bien existe una gran cantidad de dispositivos en el mercado, luego de un análisis riguroso, los dispositivos y las cantidades que decidimos adquirir, son las siguientes:

<div style={{ marginLeft: 'auto', marginRight: 'auto', width: 'fit-content' }}>

  | Modelo | Marca | Tipo | Cantidad |
  | :---: | :---: | :---: | :---: |
  | N37 | Meshnology | Portable c/pantalla | 6 |
  | MeshPocket Qi2 | Heltec | Powerbank | 6 |
  | SenseCAP P1-Pro | SeedStudio | Fijo | 2 |
  | Voyager | Spec5 | Fijo p/Vehículo | 1 |
  | ThinkNode M1 | Elecrow | Portable c/pantalla | 6|
  | ThinkNode M6 | Elecrow | Fijo | 2 |
  | WisMesh Tag | RAK | Tarjeta | 6 |

</div>

## Proceso de elección

:::warning ADVERTENCIA:
Nuestra elección de dispositivos y cantidades están dirigidas a los combatientes del fuego, a las situaciones que deben afrontar y a nuestras creencias sobre las necesidades que deben estar cubiertas.
<!-- Este proceso de elección seguramente cambiará una vez realizada las pruebas de campo con los bomberos. Y en una eventual compra futura, aquí se adjuntará su respectivo blog. -->
:::

Si hablamos de los dispositivos **portables**, adquirimos 6 de c/u (N37 y M1) y 6 MeshPocket. Aunque estos últimos son powerbanks (de 10.000mAh en el modelo elegido), también pueden desempeñarse como los dos anteriores. Es de nuestro intrés saber cómo trabajan estos dispositivos en entornos donde los dispositivos son homogéneos, para luego evaluarlos en escenarios mixtos, y contrastar los resultados obtenidos, ya que este último posiblemente se aproxime más a la realidad.

La elección de los portables tuvo varios aspectos en cuenta. Desde un inicio se decidió NO contar con los procesadores ESP32, debido a su alto consumo de energía. La disponibilidad fue otra arista a evaluar, ya que modelos como el Nano G2 Ultra no se encuentran en stock. El precio también fue un factor, por lo que modelos como el WisMesh Pocket V2 quedaron fuera, pues en comparación a los elegidos, no ofrecía, bajo nuestro criterio, algo que justificara pagar la diferencia. El T-Echo de LilyGo no se tuvo en cuenta, ya que, contamos con 2 unidades y decidimos probar nuevas opciones, (no obstante,en un futuro próximo se publicará una reseña de este modelo y de todos los que se adquieran). Por ello elegimos al **ThinkNode M1** y al **N37** (basado en un WioTracker L1 de SeedStudio).

Dentro del universo de dispositivos portables que no poseen una pantalla, elegimos a los tipo tarjeta. Estos dispositivos son un buen punto de partida para personas que no estén interesadas tanto en recibir mensajes, sino en transmitir su ubicación y ser repetidores, pensado más para personas que tienen menos exposición a la tecnología. Evaluaremos si este aparato cumple con esta función, cómo lo hará y si cumple con las expectativas, o por el contrario, necesitamos un aparato más robusto. Con esto en mente, elegimos al *WisMesh Tag* ya que hacía un gps lock en menor tiempo que su similar de seedstudio, mientras que el M3 de Elecrow no fue tomado en cuenta por su falta de stock.

Para los dispositivos fijos, el **P1** y el **M6** fueron los elegidos. En cuanto a las prestaciones había mucha paridad, por lo que el aspecto económico, en este caso, fue más determinante que en las elecciones anteriores. Pero también se eligió el P1 sobre su versión Pro por varios aspectos: uno fue el envío, debido a que no incluye baterías es más fácil de gestionar su entrega con un courier, ya que hay empresas (como FedEx) que no hacen envíos cuyos productos poseen baterías. Consume menos energía, al no tener GPS integrado y por último, pero no menos importante, debido a que no posee baterías ni GPS, en comparación a sus similares del mercado, su precio es el más bajo.

En el caso de del Spec5 Voyager, su compra fue un hecho aún más experimental, sumado a su precio, se decidió solamente adquirir una única unidad. Principalmente creemos que es importante saber dónde se encuentran todos los vehículos que participan del combate contra el fuego, pero también pueden contribuir a expandir la red ubicándose en puntos estratégicos. Esta función podrá desempeñarse por un largo tiempo debido al panel solar que incluye.

Se decidió inicialmente conformar un kit de 4 nodos portátiles, 2 tipo tarjeta y 1 nodo fijo. Creemos que es suficiente para una brigada pequeña, al menos en un inicio. No obstante, está sujeto a modificaciones, ya que aún no se realizaron pruebas de campo junto a los combatientes.

Otros factores que influyeron en la decisión fueron la necesidad de testear al menos un dispositivo de cada una de las empresas manufactureras (que si te genera curiosidad saber cuales son [*aquí*](/blog/fabricantes-ensambladores) puedes verlas). También fue de nuestro interés usar distintos lugares de compra (sitio web propietario de la empresa, o sitios externos de reventa, como AliExpress o Amazon) con el fin de conseguir dispositivos en stock, comparar precios, costos(de envío, impuestos o algún otro costo extra), tiempos estimados de llegada, así como tiempos reales y cotejar los diferentes couriers disponibles (FedEx, DHL, UPS, etc.).

## Proceso de compra

Se definieron en primer lugar, los sitios de compra. Posteriormente algunos tuvieron que variar por su falta de stock o por errores nuestros al intentar armar la ingeniería de envío, dándonos cuenta al momento de la compra que el sitio web NO hace envíos a Argentina. Errores de los cuales nos hemos reído y aprendido.

También se definieron las cantidades de cada producto por envío. Esto fue limitado a 3 debido a la modalidad de pequeños envíos, la ley de importación que usamos/usaron los couriers para entrar nuestros paquetes a Argentina. La misma, permite importar productos para uso personal, sin fines comerciales, con un tope de hasta USD 3.000 por vuelo y 50 kg por paquete a un máximo de 3 unidades iguales de la misma especie por envío.

Razón por la cual, en Heltec, por ejemplo, hicimos dos compras de 3 unidades. En Amazon encontramos una buena oferta de los N37: dos unidades a 99 U$D. Sin embargo, no sabíamos si era posible comprar 2 packs (4 unidades en total), por cómo lo tomaría la aduana, por lo que probaremos y también estaremos comunicando nuestros resultados (a cruzar los dedos para que no lo retenga la aduana :crossed_fingers:).

Con respecto a los envíos, páginas como RAK y Heltec no nos dieron tiempos estimados de entrega, suponemos que, mientras está siendo procesado, no habrá una fecha, y seguramente nos la comunicarán una vez que hayan despachado nuestro paquete. Spec5 es una de las páginas que NO hace envíos a Argentina, de hecho, es muy limitado el número de países a los que sí envía. ¿Cómo resolvimos esto? Comprando en la tienda oficial, pero con la dirección de los depósitos de **AeroBox** en Estados Unidos. La finalidad es que ellos lo traigan hasta Argentina. Posteriormente, nosotros lo retiraremos en sus depósitos de nuestro país o pagaremos el envío al interior; aún no lo definimos. Lo que si queríamos comentar que el envío más económico de Spec5 dentro de USA demora aproximadamente **12 días**, lo cual es llamativo para tratarse de un envío dentro del mismo país, ya que hemos pagado envíos, con diferencias menores a 6U$D que en ese tiempo, supuestamente, lo trae hasta nuestra casa en ese mismo tiempo.

Creemos que **Amazon** nos ha brindado la experiencia más gratificante de compra, con buen precio y facilidad de envío. El gran problema aquí es que no tienen variedad en los dispositivos Meshtastic. Pierde mucho en este aspecto con **Rockland**, que si posee variedad en aparatos de RAK, Heltec o LilyGo, pero pierde mucho en el envío, ya que no los hace a Argentina y comprar allí para que luego Aerbox lo importe, no tenía sentido desde lo económico y logístico. **Tiendamía** es un servicio similar a AeroBox, pero con un funcionamiento diferente. Ellos te efectúan la compra desde Amazon, eBay ó AliExpress y te lo importan. El problema es que no funcionó bien con los enlaces de compras de AliExpress y, al no manejar stock y variedad de las tiendas alojadas en EEUU (Amazon o eBay, ya que en Rockland hasta el momento no se puede) no pudimos efectuar compras por esta vía, aunque sigue siendo una posibilidad para una futura adquisición.

**AliExpress** tiene diferentes formas de envío, stock en la mayoría de productos, marcas con su tienda oficial ahí (como SeedStudio o Elecrow), precios competentes pero... Y este es un **GRAN PERO**, no puedes hacer compras sucesivas con la misma tarjeta, al menos en nuestra experiencia. Esto es debido al método que poseen de antifraude, lo cual es positivo, pero no hay información previa de lo que puede ocurrir y dicho suceso hemos visto, han sufrido otras personas que han usado el sitio. Razón por la cual, solo compramos 3 WisMesh Tag y no pudimos hacer la compra de los otros 3 con un envío diferente. Intentamos cambiar de día y de perfil, pero aún así no pudimos. 

Esto contribuyó a que **SeedStudio**, fuera un auténtico dolor de cabeza, ya que desde su página oficial no tiene casi stock de nada, muchos de sus productos estan en back order, otros sin stock y algunos con stock o bajo orden pero solo en USA o EU Entonces ustedes se preguntarán, ¿cuál es el problema?, si a esta altura del partido ya habían hecho compras en Estados Unidos y no existían motivos para no importar desde la Unión Europea. Bueno, la cuestión es que el warehuse que hace envíos a todo el mundo es China, los otros dos solo venden donde residen. De todas formas, conseguimos productos en stock en AliExpress, aquí el problema, era que no podíamos usar la tarjeta. A esta altura, las esperanzas se desvanecen, pero hubo un guiño del destino, luego de aproximadamente 3 semanas, conseguimos al **P1** en stock, nostros ni lentos ni perezosos efectuamos nuestra compra, completando así toda la lista.

---

Este proceso de adquisición de hardware Meshtastic, más allá de llenar nuestro inventario, ha proporcionado una lección práctica e invaluable sobre la planificación logística internacional y las barreras de importación. Hemos confirmado que la implementación de redes de comunicación descentralizada en regiones con regulaciones aduaneras estrictas no depende únicamente de la tecnología, sino también de la ingeniería comercial y logística.

Nuestra experiencia ha revelado varios puntos críticos para cualquier proyecto similar:

1. <u>Flexibilidad de suministro:</u> La dependencia de un único fabricante o plataforma (como la restricción de tarjetas de AliExpress o la falta de stock en sitios oficiales) es un riesgo operativo significativo. Fue esencial recurrir a múltiples canales (Amazon, couriers especializados como AeroBox, y tiendas oficiales) para asegurar la lista completa de dispositivos.

2. <u>Baterías:</u> La restricción de envío de baterías por parte de couriers internacionales obliga a una planificación modular. Elegir dispositivos sin batería (como el P1) o utilizar servicios de importación indirecta (como con Spec5) añade complejidad, pero garantiza la llegada del hardware.

3. <u>Costo total de adquisición:</u> El precio inicial del dispositivo es solo una parte. Los costos de envío internacional y los impuestos aduaneros, sumados a la necesidad de usar servicios de re-shipping (AeroBox) para fabricantes que no envían a Argentina, redefinen el verdadero costo del proyecto.

4. <u>Tiempos reales de entrega:</u> La amplia dispersión en los tiempos de tránsito (desde envíos veloces de Amazon hasta las demoras en warehouses o la falta de fechas estimadas) subraya la necesidad de calendarios de implementación holgados y tolerantes al riesgo.

En conclusión, es una aventura, la cual, aún no ha finalizado y nos estaremos viendo de nuevo en la segunda parte de esta experiencia, donde podrá ver los tiempos reales de entrega, los precios finales de c/u de los dispositivos y demás observaciones pertinentes. ¡Hasta luego!
