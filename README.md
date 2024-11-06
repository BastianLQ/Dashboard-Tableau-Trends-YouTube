# Dashboard-trends-YouTube
__Creación de dashboard interactivo en Tablau__

<image src="https://github.com/BastianLQ/Dashboard-trends-YouTube/blob/main/dashboard.jpg" alt="Dashboard">

_Fragmentos del notebook, para ver proyecto completo hacer click [aquí](https://portfoliodabastianlopez.on.drv.tw/Portafolio/An%C3%A1lisis%20Instacart.html)_

## Descripción del Proyecto
Se trabaja como analista de vídeos publicitarios para la agencia de publicidad Sterling & Draper. Se dedica mucho tiempo a analizar tendencias de vídeos en YouTube para determinar qué contenido merece atención para la mercadotecnia.

Cada video tiene una categoría específica (entretenimiento, música, noticias y política, etc.), una región y una fecha en que se hace tendencia.

Un video puede estar en la sección de tendencias durante varios días seguidos.

Cada semana, se solicita la siguiente información:

- ¿Qué categorías estaban en las tendencias de la semana pasada?
- ¿Cómo se distribuyeron en diversas regiones?
- ¿Qué categorías fueron particularmente populares en los Estados Unidos?
  
Debido a esta situación es que se debe crear un dashboard para automatizar el proceso de obtener respuestas a estas preguntas.

## Proceso del Proyecto
- __Descripción de los datos:__ Los datos fueron extraídos de [cinco datasets](https://drive.google.com/drive/folders/11ludpzThvf-xB6LfZW_xzCBK1Z91M_KA?usp=sharing) proporcionados por Instacart _(los datasets están en Drive porque superan el peso máximo permitido de GitHub)_, en esta fase, también, se les da una revisión superficial y se corrigen problemas de importación si es que llegasen a surgir.
- __Preprocesamiento de los datos:__ Se realizaron varias operaciones de limpieza, incluyendo manejo de valores nulos, normalización y formateo de datos.
- __Análisis Exploratorio de Datos (EDA):__ Esta fase se centró en analizar la integridad de los datos y rescatar insights valiosos. Utilizando pandas se exploraron los datos para obtener una comprensión inicial, intermedia y avanzada, y con matplotlib, se generaron visualizaciones para ilustrar los hallazgos clave del análisis.
- __Resultados:__ Se identificaron patrones y tendencias en los datos, como los productos más vendidos y reordenados, y el comportamiento general de los clientes en términos de cantidad de artículos por pedido.

## Ejecuta el proyecto [aquí](https://portfoliodabastianlopez.on.drv.tw/Portafolio/An%C3%A1lisis%20Instacart.html)
Para ver el diccionario de datos, el desarrollo completo en código, todos los gráficos y las conclusiones, haga click en el enlace de arriba.
