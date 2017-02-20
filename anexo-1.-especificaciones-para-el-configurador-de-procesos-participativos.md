# Anexo 1: Especificaciones para el Configurador de Procesos Participativos

El configurador de procesos de participación consiste en una estructura genérica o abstracta de lo que es un proceso de participación en Decidim Barcelona, especificando etapas, configuración temática y funciones que se quieren habilitar para cada proceso específico, así como su integración en la plataforma: página principal, usuarios, fases y componentes (propuestas, debates, documentos colaborativos, visualización de datos, etc). Esta estructura permite adaptar el Decidim Barcelona para configurar y administrar procesos de participación específicos (por ejemplo Teatro Arnau, superilles, pacificación de la Avenida Meridiana, normativa de Participación, etc). 

Los componentes de un proceso pueden ser customizables, donde se decide qué fases y componentes tiene cada proceso, o seleccionando una plantilla prediseñada con los componentes ya preconfigurados en base a un proceso específico. Entre los modelos de plantillas de procesos prediseñados se encontrarán: 

1. PAM

   1. Componentes: Propuestas, Debates, Citas

   2. Fases de propuestas: Propuesta, Respuesta y Actuación 

2. Presupuestos Participativos

   1. Componentes: Propuestas, Citas

   2. Fases de propuestas: Recogida de propuestas, priorización, evaluación técnica y económica por parte de los técnicos municipales y votación final.

3. Legislación colaborativa - Normas de regulación

## Metadatos y campos estructurales de cada proceso

Cada proceso contará con una serie de metadatos que definirán y servirán para comunicar su estructura (los campos con asterisco * son obligatorios):

* **Titulo*:** campo de texto corto.

* **Subtítulo*****:** campo de texto un poco más largo

* **Escala*.** Ciudad/distrito/barrio. Debería permitir también a escalas menores, por ejemplo para los casos del Teatre Arnau o Superilles.

* **Grupo promotor****: **Se indica el gestor/a del proceso de participación a nivel político, puede ser sólo el Ajuntament, o un grupo compuesto por técnicos/políticos del Ajuntament + asociaciones, empresas, ciudadanas u otras entidades.

* **Área****(s) **del Ajuntament

* **Entradilla***: Breve descripción del proceso de participación XXX caracteres.

* **Descripción***: explicación del proceso. Tiene que quedar bien indicada cuantos caracteres de este texto se mostrarán en la ficha y a partir de cuantos caracteres se quedará para ver habiendo clicado en el enlace "más información" de la ficha de procesos.

* **Estructura  participativa** y agentes implicados (Grupo Motor, Comisión de Seguimiento, Grupo de  Trabajo, Entidades que han participado en los diversos talleres y reuniones  del proceso de participación)

* **Target*: **a quién va dirigido (edades, distritos, áreas, etc.), deben de ser campos expresados en la ficha de usuaria para poder segmentar las notificaciones de nuevos procesos de participación.

* **Imagen principal**: Con dimensiones similares a 1015x667. [Si no se introduce ninguna imagen se tirará de un archivo o stock de imágenes genéricas]

* **Categorías y subcategorías**: Opcional, permite navegar y clasificar las propuestas, debates y citas presenciales del proceso de participación. 

* **Etiquetas**: tags.

* **Documentos adjuntos**: aparecerán listados debajo del texto de presentación. Deben de ser obligatoriamente documentos en formatos abiertos (odt, rtf, pdf, etc.), el sistema no debe de permitir subir textos en formato .doc y debe de avisar al usuario de que cambio de formato porque ha intentado subir un texto en un formato no libre ni interoperable. Los campos que tendrán los documentos son: 
 * Titulo
 * Descripción
 * Autor
 * Fecha

De todos los documentos se generará una imagen miniatura que lo acompañe como icono.  

* **URL de video**

## Etapas y fases de un proceso de participación

Un proceso participativo se verá reflejado en la plataforma  Decidim Barcelona en distintas **fases**, cada una con una fecha de inicio y  de fin predefinida al comenzar del mismo. De cara a facilitar la navegación se debería agrupar la cantidad de fases con las que cuenta un proceso en distintas etapas, con el objetivo de que la ciudadanía tenga claro en que momento del proceso se encuentra, al estilo de las Propuestas de Gobierno de Irekia (NOTE:   http://irekia.euskadi.eus/es/debates/1001-anteproyecto-ley-empleo-publico-vasco?stage=contribution ). 

### Etapa 1: Inicio

* 0. Anuncio [opcional]

    * Fecha de comienzo del anuncio de la plataforma

    * Texto de anuncio

    * Funcionalidad de "Seguir proceso". A través de un botón un usuario puede recibir actualizaciones por correo electrónico de lo que ocurra en este proceso: cuando se cambie de fase, se haya producido algún avance, cuando se esté por acercar la fecha de una cita presencial, etc. [se podría pensar con un servicio de notificaciones conectable a google calendar y redes sociales?] 

    * Genérico de avisar que el Ajuntament tiene intención de realizar un Proceso Participativo. 

    * Esta fase no se mostraría dentro del menú de un proceso sino que sería sólo visible para "procesos futuros".

* 1. Información [obligatorio] - Presentación

    * Texto de presentación donde se explicará en qué consiste este proceso así como el trabajo previo realizado para el punto de partida del mismo (informes, reuniones, etc) 

    * Se puede convocar una o más **Citas Presenciales **informativas para presentar el proceso de participación. No son citas presenciales de debate (ver siguiente sección) en el sentido de que no salen propuestas de estas citas, ni tienen porqué ir acompañadas de la documentación de una cita presencial standard. Pero se habilita la cita para convocar a gente de manera automática a través del Decidim Barcelona. En principio usamos el mismo módulo de citas presenciales, con todas sus funciones pero se enlazaría desde el cajetín o landing del proceso de participación. Estudiar la posibilidad de crear una categoría de citas y llamar a esta cita de presentación o cita informativa.

    * Contará con documentación adjunta (ver más arriba).

### Etapa 2: Desarrollo

* 2. Diagnóstico [opcional]

    * Apertura de espacios de discusión por parte del Ajuntament sobre ciertas temáticas relacionadas con el Proceso. En caso de considerarse puede habilitarse la apertura de **Debates** por parte de la ciudadanía. Ejemplo de como se vería un debate:[ https://decidim.barcelona/debates/decidim-barcelona-una-eina-de-participacio-digital-que-va-mes-enlla-del-pla-mu](https://decidim.barcelona/debates/decidim-barcelona-una-eina-de-participacio-digital-que-va-mes-enlla-del-pla-mu) 

    * Opción de dejar la apertura de **Debate** abierta a la ciudadanía (crear nuevos debates--y citas asociadas) o cerrado a lo que decida la administradora del proceso de participación

    * Durante la parte de diagnóstico (si el proceso es complejo) también se puede activar un módulo de encuestas.

    * Opción de tener una **Cita Presencial** de debate. 

* 3. Aportaciones-Decisión [obligatorio]

    * La idea de este módulo es recursiva, se pueden anidar combinando secuencias de dos tipos de funciones o subfases: fases de Aportación (propuesta/producción/colaboración) y fases o funciones de toma de decisión. Así en el caso más simple hay una subfase de aportaciones (la gente realiza propuestas) y otra fase de Decisión (se votan o dan apoyos y el resultado prioriza o selecciona cuales se van a implementar). Pero en casos más complejos pueden darse varios ciclos: p.e un proceso con tres ciclos puede ser del siguiente modo. 1A: Propuestas, 1D: priorización por votos libres, 2A: elaboración más detallada de las propuestas seleccionadas, 2D: priorización por votos limitados (sólo puedes elegir 5), 3A: re-elaboración por técnicos del ajuntament, 3D: validación o votación final. 

    * Tipos de Aportación:

        * **Propuestas**: donde la ciudadanía pueda realizar propuestas para este proceso. Por ejemplo:[ https://decidim.barcelona/proposals/cubriment-de-la-ronda-de-dalt-al-seu-pas-per-la-vall-d-hebron](https://decidim.barcelona/proposals/cubriment-de-la-ronda-de-dalt-al-seu-pas-per-la-vall-d-hebron) - En esta fase sólo se permite la creación y discusión y propuestas, la priorización (votación) de las mismas debe realizarse en una fase siguiente. Existe la posibilidad de habilitar para el proceso específico la geo-localización de propuestas (dentro de una zona predefinida). 

        * **Legislación colaborativa**: donde la ciudadanía puede realizar comentarios un texto realizado por el Ajuntament. Por ejemplo:[ https://decide.madrid.es/ordenanza-de-transparencia](https://decide.madrid.es/ordenanza-de-transparencia) 

    * Tipos de Decisión:

        * Votación/apoyos libres para propuestas: puedes apoyar tantas propuestas como quieras.

        * Votación/apoyos/gastos limitados para propuestas: tiene una serie limitada de tokens (dinero, apoyos, etc.) para repartir entre las propuestas.

        * Consulta (podría ser una modalidad de encuesta en la que simplemente hay que validar el resultado final casi a modo de referéndum).

        * Umbrales: dependiendo del tipo de decisión se ponen umbrales para que sea vinculante, o estudiado, o presupuestado. Los umbrales pueden ser fijos o relacionales (p.e. el 20% de las propuestas con más apoyos) y combinarse entre si (p.ej.: estar en el primer cuartil y tener, al menos, 10 votos).

    * Tanto los momentos de "decisión" como los de "aportación" pueden ser abiertos a la participación o limitados a un grupo de usuarios (técnicos, expertos, o representantes).

    * Al menos la última fase debe ser abierta y participativa. Si no se entiende que no sería un proceso participativo sino  brindar información o asesoramiento técnico, por lo que su sitio sería en otra web del Ajuntament.

    * Por ejemplo para los Presupuestos Participativos, se contaría con diversas fases, siempre tratándose de las mismas propuestas, tomando de ejemplo el proceso del Ayuntamiento de Madrid ([https://decide.madrid.es/participatory_budget/in_two_minutes](https://decide.madrid.es/participatory_budget/in_two_minutes)): 

        * Recogida de propuestas: en el que la ciudadanía crea las propuestas.

        * Apoyos: en el que la ciudadanía hace una primera priorización de todas las propuestas, teniendo 10 votos como máximo a repartir entre todas las propuestas. 

        * Evaluación: por parte del Ayuntamiento, donde se valoran económicamente las propuestas.

        * Votación final: donde la ciudadanía puede asignar un presupuesto máximo entre todas las propuestas.  

### Etapa 3: Conclusión

* 4. Resultados: Presentación de Resultados, Validación y Devolución:

    * Pueden añadirse **Citas Presenciales** para comunicar públicamente los resultados

    * Texto de conclusiones: donde se explique el alcance que ha tenido este proceso y las aportaciones que se han tenido en cuenta que se aplicarán. 

    * Se comunica en la home de decidim y a los usuarios que hayan marcado la opción de "Seguir proceso" 

    * Incluye módulo de visualización de datos genérico: número de citas presenciales, número de participantes, número de propuestas total, número de propuestas por categorías.

* 5. Evaluación:

    * Se abren **Debates **y **Citas Presenciales** para evaluar el proceso ya terminado.

    * Posibilidad de mantener un módulo de evaluación abierto durante todo el proceso, para recibir feedback en tiempo real. [en la literatura se recomiendan evaluaciones sobre la marcha, y participativas. En el caso del decidim se abre la posibilidad de trolling, pero con una moderación apropiada y si el proceso marcha bien, creo que funcionaría]

* 6. Seguimiento:

    * Se crea ficha de seguimiento de los resultados (actuación/proyecto/plan) participativos para que la gente pueda hacer un seguimiento

    * Actualizaciones por parte del Ajuntament con enlace a noticias, fotos, videos, etc con los avances que se realice a lo largo de los años en este proceso.

    * Opción. Ejecución participativa. Posibilidad de convocar a ciudadanas interesadas en colaborar (con diferentes formas de retribución) en la ejecución de la actuación/proyecto/plan participativo. 

* 7. Rendición de cuentas:

    * Se abre una **Cita presencial **y un **Debate **para rendir cuentas en la fecha estimada de conclusión del proyecto (una construcción, una legislatura, o actuación).

Cada una de las fases tiene que tener una pequeña descripción de lo que es esa fase.

Se pueden ver los mockups iniciales para discutir en:[ https://app.moqups.com/andreslucena@gmail.com/8idx5dcplc/view](https://app.moqups.com/andreslucena@gmail.com/8idx5dcplc/view) 
