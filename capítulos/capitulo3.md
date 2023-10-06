# Capítulo 3

## ¿Qué?

Tercer capítulo del TFG, en el cual se abordan las disciplinas de análisis y diseño, que tienen como objetivos:

|Análisis|Diseño|
|-|-|
|Refinar aún más los requisitos de la captura de requisitos para lograr una comprensión más precisa de los mismos, una descripción que sea más fácil de mantener y que nos ayudan a estructurar el sistema|Desarrollar modelos enfocados sobre los requisitos no funcionales y el dominio de la solución y preparar para la implementación y pruebas del sistema|

## ¿Por qué?

Habiendo definido los límites del sistema, nos toca enfocarnos en dar una especificación más precisa de los requisitos obtenidos en el capítulo anterior, para describir usando el lenguaje de los desarrolladores, introducir más formalismo y poder tomar decisiones sobre el funcionamiento interno del sistema; de modo que se pueda abordar el desarrollo enfocados *ahora sí* en los requisitos no funcionales y en el dominio de la solución.

## ¿Para qué?

Se trata de crear una abstracción sin fisuras de la implementación del sistema, de tal modo que la aplicación sea un refinamiento *sencillo* del diseño mediante la cumplimentación de la *carne* (código), pero sin cambiar *el esqueleto* (el diseño).

Se busca adquirir un conocimiento en profundidad de los temas sobre los requisitos no funcionales y limitaciones relacionadas con los lenguajes de programación, la reutilización de componentes, sistema operativo, tecnologías de distribución y concurrencia, tecnologías de bases de datos, tecnologías de interfaz de usuario, las tecnologías de gestión de transacciones, etc.

## ¿Cómo?

### Disciplina de análisis y diseño

|Análisis|Diseño|
-|-
Analizar la arquitectura | Diseñar la arquitectura
Analizar casos de uso | Diseñar casos de uso
Analizar clases | Diseñar clases
Analizar paquetes | Diseñar paquetes

Partiendo de los requisitos expresados como Casos de Uso, podemos obtener las clases de diseño obvias:

|Clases Modelo|Clases Vista|Clase Controlador (1xCdU)|
|-|-|-|
Estudiando la descripción de los Casos de Uso y el Modelo de Dominio existente|Una clase de vista por cada actor humano siendo ésta clase representante de la ventana principal en el interfaz de usuario en el que actor interactua<br><br>Una clase de vista primitiva por cada clase de modelo encontrada anteriormente<br><br>Una clase de vista central por cada actor que sea un sistema externo representando el interfaz de comunicaciones|Una clase controladora responsable de manejar el control y coordinación de la realización del Caso de Uso y entonces refinar esta clase de control acorde a los requisitos del Caso de Uso

- Identificadas las clases trazar sus nombres, responsabilidades y relaciones en un Diagrama de Clases
- Identificar sus relaciones: asociaciones, agregaciones o generalizaciones.

## A tener en cuenta

### Diapos de IdSw

- [IdSw: análisis y diseño](https://drive.google.com/drive/folders/1gZU_teZiNH4l7W3ltxuQ0bS3hQPTaCNQ?usp=share_link), incluyendo estrategias de clasificación, relaciones entre clases, cohesión, acoplamiento, etc...

### Eres el jefe de proyecto de la aplicación

|||
|-|-|
¿Por qué parte comenzarías, continuarías y terminarias la producción de código?|Casos de Uso Priorizados y especificados,
¿Qué medidas aplicarías para obtener la calidad del software adecuada para facilitar la depuración de errores, la mantenibilidad corrective, perfective o adaptativa?|Análisis de la Arquitectura<br>Análisis de Casos de Uso<br>Análisis de Clases, revisión<br>Análisis de Paquetes, revisión<br>
¿Cómo repartirías las tareas de producción entre las personas del equipo de desarrollo?|Estimando cada actividad, entre 2 y 20 horas, y repartiendo cohesivamente entre el equipo de desarrollo

…​ con trazabilidad de todo!