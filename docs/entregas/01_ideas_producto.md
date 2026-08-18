# Entrega 1 - Propuesta inicial de ideas de producto

## Idea 1 - FilmFit

### Problema que resuelve

Actualmente existen grandes catálogos de películas y series repartidos entre distintas plataformas de streaming. Aunque estas plataformas incorporan sistemas de recomendación, muchas veces las sugerencias se basan principalmente en el historial de consumo o en contenidos similares a los ya vistos, sin tener suficientemente en cuenta qué le apetece ver al usuario en ese momento.

El problema no es únicamente encontrar una película bien valorada, sino decidir qué ver entre miles de opciones teniendo en cuenta factores como los gustos personales, el género deseado, el estado de ánimo, el tiempo disponible, si se quiere una película o una serie, y las plataformas a las que el usuario tiene acceso.

FilmFit plantearía un sistema de recomendación personalizado que combine el historial de valoraciones del usuario con su intención actual. Por ejemplo, permitiría realizar peticiones como: “quiero una película de terror psicológico, de menos de dos horas y que esté incluida en alguna de mis plataformas”.

No se plantea como un simple ejercicio técnico de clasificación de películas, sino como un sistema de apoyo a una decisión cotidiana en la que existe una gran cantidad de información y demasiadas alternativas.

### Motivación para realizar el proyecto

La idea resulta interesante porque permite trabajar uno de los problemas clásicos de Data Science, los sistemas recomendadores, pero incorporando componentes adicionales de personalización y contexto.

El proyecto permitiría aplicar contenidos del máster relacionados con análisis de datos, sistemas de recomendación, machine learning, procesamiento de lenguaje natural, embeddings e IA generativa. Una posible evolución sería utilizar lenguaje natural para interpretar lo que busca el usuario y explicar posteriormente por qué se recomienda cada contenido.

También existe una gran cantidad de datos públicos de valoraciones y metadatos de películas, lo que hace que la idea parezca viable desde el punto de vista de los datos. Además, sería posible evaluar objetivamente distintos modelos comprobando si son capaces de recomendar contenidos que sabemos que han gustado a usuarios similares.

La principal duda de esta propuesta es que un recomendador de películas puede parecer inicialmente una idea poco original. Por ello, el interés estaría en desarrollar una solución contextual, explicable y personalizada, y no limitarse a recomendar películas similares a las ya vistas.

### A quién impacta

El usuario principal sería una persona que consume habitualmente películas o series en plataformas de streaming y que tiene dificultades para decidir qué ver entre un catálogo muy amplio.

También podría resultar útil para grupos de amigos, parejas o familias, ya que una posible ampliación sería generar recomendaciones que intentasen satisfacer simultáneamente los gustos de varias personas.

### Por qué tiene valor

FilmFit podría reducir el tiempo que una persona dedica a buscar contenido y mejorar la calidad de las recomendaciones recibidas.

Su principal valor estaría en combinar tres elementos que normalmente se tratan por separado:

- preferencias históricas del usuario;
- intención o contexto actual;
- restricciones reales, como duración, género o plataformas disponibles.

Además de mejorar la experiencia del usuario, el proyecto permitiría generar conocimiento sobre perfiles de gusto, patrones de consumo y factores que influyen en que un contenido conecte con una determinada audiencia.

---

## Idea 2 - RaceStrategy

### Problema que resuelve

En actividades de resistencia como running o ciclismo, una parte importante del rendimiento depende de cómo se distribuye el esfuerzo a lo largo de una ruta. Mantener un ritmo demasiado alto al comienzo puede provocar una pérdida importante de rendimiento posteriormente, mientras que una estrategia demasiado conservadora puede impedir aprovechar correctamente la capacidad del deportista.

La dificultad aumenta cuando el recorrido contiene subidas, bajadas, cambios de pendiente o condiciones meteorológicas diferentes. En rutas largas e irregulares resulta difícil saber si el ritmo que se lleva en un momento concreto es realmente el adecuado para alcanzar un objetivo final.

RaceStrategy plantearía un sistema capaz de analizar una ruta antes de realizarla y, a partir de un tiempo objetivo, estimar qué ritmo, tiempo acumulado o nivel de esfuerzo debería llevar el deportista en cada tramo. Por ejemplo, para una ruta que se quiera completar en 1 hora y 40 minutos, el sistema podría indicar en qué tiempo debería alcanzarse cada punto relevante del recorrido y en qué zonas conviene reservar fuerzas o aumentar el esfuerzo.

Para generar esta estrategia se podrían utilizar variables como distancia, desnivel, pendiente, velocidad o ritmo, frecuencia cardíaca, condiciones meteorológicas y el histórico de actividades del propio deportista.

La idea no consiste únicamente en predecir un tiempo final, sino en apoyar una decisión concreta: cómo gestionar el esfuerzo durante cada parte de una ruta para intentar alcanzar un objetivo determinado.

### Motivación para realizar el proyecto

Esta idea tiene una motivación especialmente personal. Desde hace años mi padre realiza en bicicleta el recorrido entre Los Garres y nuestra casa de la playa en Lo Pagán, una ruta de aproximadamente 44 km. Cuando era pequeño alguna vez intenté hacerla con él, aunque por la distancia y el esfuerzo me resultaba demasiado exigente.

Desde hace cuatro veranos, varios amigos y yo hemos convertido esa ruta en un pequeño reto personal: intentar superar el mejor tiempo de mi padre. Su referencia durante mucho tiempo fue de unas 2 horas. El verano pasado conseguimos bajar ese registro hasta 1 hora y 50 minutos, pero posteriormente mi padre volvió a realizar la ruta en 1 hora y 45 minutos. Desde entonces el objetivo ha dejado de ser simplemente completar el recorrido y se ha convertido en intentar optimizar cada vez más el tiempo.

El problema es que normalmente realizamos la ruta solo una vez cada verano. Al tratarse de un recorrido largo y bastante irregular en cuanto a pendientes y tramos, no tenemos suficientes intentos como para aprender por prueba y error cuál es la mejor estrategia. A medida que los tiempos bajan, cada mejora resulta además más difícil de conseguir.

Por eso resultaría especialmente útil disponer de una herramienta que, para un objetivo concreto —por ejemplo completar la ruta en 1 hora y 40 minutos—, indicase qué tiempo acumulado deberíamos llevar en cada tramo y dónde convendría apretar, mantener el esfuerzo o reservar fuerzas. Esto permitiría afrontar la ruta con una estrategia previa en lugar de gestionar el esfuerzo únicamente por sensaciones.

Más allá de la motivación personal, el proyecto resulta técnicamente interesante por su combinación de datos deportivos, series temporales, información geoespacial, meteorología, personalización y optimización. Permitiría aplicar contenidos del máster relacionados con análisis de datos, machine learning, tratamiento de datos GPS y posiblemente optimización. En una fase avanzada podría estudiarse incluso un funcionamiento en tiempo real, en el que el sistema recibiese la posición y el rendimiento actual del deportista y recalculase la estrategia durante la actividad.

Además, el propio recorrido permitiría realizar una validación práctica del sistema comparando la estrategia propuesta con los tiempos obtenidos en intentos reales.

La principal dificultad sigue siendo la calidad y heterogeneidad de los datos. Las actividades deportivas pueden contener errores de GPS, dispositivos diferentes y variables que no siempre están disponibles, como frecuencia cardíaca o potencia. También será necesario estudiar cómo validar de forma objetiva que una estrategia propuesta es realmente mejor que otra.

### A quién impacta

El proyecto estaría dirigido principalmente a corredores y ciclistas aficionados que quieran preparar mejor una ruta, entrenamiento o prueba.

También podría resultar útil para deportistas que ya registran sus actividades con aplicaciones o dispositivos deportivos y disponen de un histórico suficiente como para personalizar las recomendaciones.

### Por qué tiene valor

RaceStrategy podría ayudar al deportista a tomar mejores decisiones antes y durante una actividad, evitando una mala distribución del esfuerzo y adaptando la estrategia a las características reales del recorrido.

El valor principal estaría en pasar de recomendaciones generales a estrategias personalizadas basadas en datos históricos del propio usuario.

Además, permitiría visualizar y comprender mejor cómo afectan al rendimiento factores como la pendiente, la distancia acumulada, la fatiga o las condiciones meteorológicas.

---

## Idea 3 - BeachMatch

### Problema que resuelve

Elegir una playa no depende únicamente de su cercanía o popularidad. La playa más adecuada puede variar según la actividad que se quiera realizar, las condiciones del mar, el viento, la temperatura, la calidad del agua, los servicios disponibles o las necesidades concretas del usuario.

Por ejemplo, una playa que puede ser adecuada para surf puede no ser la mejor opción para pasar el día en familia, nadar en aguas tranquilas o jugar al vóley playa. Además, las condiciones pueden cambiar notablemente según el día y la franja horaria.

Actualmente, esta información suele encontrarse repartida entre distintas fuentes y el usuario tiene que consultarla por separado y realizar la comparación por su cuenta.

BeachMatch plantearía un sistema de apoyo a la decisión que analizase las características de las playas junto con las condiciones ambientales y las preferencias del usuario para identificar qué playas y momentos pueden resultar más adecuados para una determinada actividad.

No se pretende sustituir avisos oficiales de seguridad ni afirmar que una playa es completamente segura, sino facilitar la comparación de alternativas a partir de datos objetivos y contextualizados.

### Motivación para realizar el proyecto

La idea permite trabajar con información geográfica, meteorológica y ambiental, además de plantear un problema de recomendación y apoyo a la decisión diferente de los sistemas recomendadores tradicionales.

Podría integrar variables como oleaje, viento, temperatura, calidad del agua, servicios, accesibilidad, distancia y características de la playa. Esto permitiría aplicar contenidos del máster relacionados con integración y limpieza de datos, análisis exploratorio, visualización geoespacial, machine learning y sistemas de recomendación.

También parece razonable pensar que existen datos públicos suficientes para desarrollar una primera versión, ya que distintas administraciones y servicios meteorológicos publican información sobre playas, calidad del agua y condiciones marítimas.

La principal dificultad sería integrar correctamente fuentes con distinta granularidad espacial y temporal. Por ejemplo, una medición marítima obtenida en una boya cercana no representa necesariamente de forma exacta lo que ocurre en la orilla de una playa concreta. Por ello, sería necesario comunicar claramente el nivel de incertidumbre de las recomendaciones.

### A quién impacta

Los principales usuarios serían personas que quieren elegir una playa en función de una actividad concreta, especialmente:

- familias que buscan determinadas características y servicios;
- nadadores;
- surfistas;
- personas interesadas en vóley playa u otras actividades deportivas;
- turistas que desconocen las diferencias entre las playas de una zona.

### Por qué tiene valor

BeachMatch reduciría el tiempo necesario para consultar y comparar información procedente de distintas fuentes y permitiría tomar decisiones más informadas sobre dónde y cuándo realizar una actividad.

Su valor estaría en transformar datos ambientales, geográficos y de servicios en información comprensible y personalizada para el usuario.

Además, podría ayudar a descubrir alternativas menos conocidas que encajen mejor con las necesidades de una persona que las playas más populares o cercanas.

---

## Valoración inicial de las tres ideas

Las tres propuestas parecen viables dentro de un proyecto de Data Science e IA, aunque presentan niveles de riesgo diferentes.

**FilmFit** es actualmente la idea más segura desde el punto de vista técnico y de los datos. Existen grandes conjuntos de valoraciones y está bastante claro cómo construir y evaluar progresivamente diferentes modelos de recomendación. Su principal reto sería aportar suficiente diferenciación respecto a otros recomendadores existentes.

**RaceStrategy** parece la idea con mayor potencial de originalidad y experimentación. El resultado final podría ser especialmente interesante si fuese posible generar y validar estrategias personalizadas sobre rutas reales. Sin embargo, también es la propuesta que presenta más incertidumbre debido a la calidad de los datos deportivos y a la dificultad de validar objetivamente una estrategia óptima.

**BeachMatch** se sitúa en un punto intermedio. Tiene un problema concreto, permite integrar diferentes fuentes de datos y ofrece posibilidades interesantes de análisis geoespacial y recomendación. Su principal dificultad sería representar correctamente la incertidumbre asociada a las condiciones ambientales y a la diferente precisión de las fuentes disponibles.

En las siguientes entregas será necesario estudiar con más detalle la disponibilidad y calidad de los datos antes de decidir cuál de las tres propuestas resulta más adecuada para desarrollar durante el resto del curso.
