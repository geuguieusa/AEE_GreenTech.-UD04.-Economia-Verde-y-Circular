
## Auditoría del código original
El código inicial tenía desarrollos insostenibles, tenía una sobrecarga injustificada en el lado del cliente y mediante la importación de frameworks pesaba mucho más.

## Refactorización y ecodiseño aplicado
Para alinear el MVP con los principios de sostenibilidad, se han aplicado las siguientes medidas en el ecodiseño:
* **Transición a tecnologías nativas:** He eliminado las librerías externas, bootstrap se ha sustituido por CSS Flexbox nativo, jQuery por Vanilla JS y FontAwesome por un único icono en formato SVG embebido.
* **Optimización multimedia:** la imagen de fondo se ha reestructurado usando una etiqueta '<img>' con los atributos 'loading="lazy"' y 'decoding="async"', reduciendo además su resolución mediante parámetros de servidor (de 3000px a 1200px).
* **Eficiencia y tipogografía:** solo se solicitan los pesos estrictamente necesarios (400 y 700) de la fuente Montserrat.

## 3. Impacto medioambiental y prevención de la obsolescencia
Las decisiones arquitectónicas que he tomado tienen un impacto directo en la reducción de residuos y consumo energético:
* **Reducción del carbono embebido:** al requerir una fracción menor del ancho de banda original, se minimiza la energía consumida por los centros de datos y la infraestructura de red durante la transmisión de la página.
* **Freno a la obsolescencia programada:** Un DOM más limpio y sin dependencias JavaScript que procesar exige menos ciclos de CPU y RAM, entoces esto evita el sobrecalentamiento y la degradación térmica de las baterías en teléfonos móviles más modestos, prolongando la vida útil del hardware y previniendo la generación prematura de basura electrónica (e-waste).
