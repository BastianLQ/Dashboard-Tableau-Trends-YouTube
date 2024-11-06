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
Después de hablar con los administradores de la base de datos, se reunieron los requisitos técnicos:

- __Objetivo de negocios:__ analizar el historial de tendencias de videos en YouTube
- __Con qué frecuencia se usará el dashboard:__ al menos una vez al día
- __Usuario objetivo del dashboard:__ gerentes de planificación de videos publicitarios
- __Contenido de los datos del dashboard:__
  - Tendencias pasadas de videos, ordenadas por día y categoría
  - Tendencias de videos, ordenadas por país
  - Una tabla de correspondencia entre categorías y países
- __Parámetros para agrupar los datos:__
  - Fecha y hora de tendencia
  - Categoría de video
  - País
- __Los datos:__
  - Historial de tendencias — valores absolutos ordenados por día (dos gráficos: números absolutos y proporción de porcentaje)
  - Eventos, ordenados por país — valores relativos (% de eventos)
  - La correspondencia entre las categorías y los países — valores absolutos (una tabla)
- __Importancia:__ todaos los gráficos son igualmente importantes
- __Fuentes de datos para el dashboard:__ los ingenieros crearon una tabla de agregación llamada `trending_by_time`. Esta es la estructura:
  - `record_id`: la clave primaria
  - `region`: país/región geográfica
  - `trending_date`: fecha y hora
  - `category_title`: categoría del video
  - `videos_count`: número de videos en la sección de tendencias
- La tabla está en la base de datos `youtube`, que se creó especialmente para necesidades de análisis.
- __Intervalo de actualización de los datos:__ una vez cada 24 horas, a la media noche UTC
- __Gráficos, controles de dashboard y su orden:__
<image src="https://github.com/BastianLQ/Dashboard-trends-YouTube/blob/main/plan.png" alt="Estructura de dashboard">

## Ejecuta el proyecto [aquí](https://portfoliodabastianlopez.on.drv.tw/Portafolio/An%C3%A1lisis%20Instacart.html)
Para ver el diccionario de datos, el desarrollo completo en código, todos los gráficos y las conclusiones, haga click en el enlace de arriba.
