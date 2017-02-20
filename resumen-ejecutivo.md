# Resumen Ejecutivo

* Este documento detalla el futuro desarrollo de la **plataforma digital de participación de l´Ajuntament de Barcelona**, decidim.barcelona (disponible en URL [https://decidim.barcelona](https://decidim.barcelona)). 

## Marco

* En un contexto de creciente mediación tecnológica de la vida social y política, la **transición digital** de las estructuras gubernamentales se ha convertido en una oportunidad de **democratización**, pero también de **negocio**. Decidim.barcelona aspira a encarnar un modelo de **infraestructura democrática para la democracia**, una infraestructura digital de **código abierto, de producción y gestión público-común**. Este modelo **se opone al modelo privativo-corporativo** de plataforma digital, que hace de la extracción de datos, la provisión de servicios comerciales y la orientación de la conducta social un negocio masivo. Decidim.barcelona parte del software **Consul** (desarrollado por el Ayuntamiento de Madrid para su plataforma disponible en [https://decide.madrid.es](https://decide.madrid.es)), software libre, abierto y transparente.

## Plan de desarrollo 

* Los principales **objetivos de la plataforma** son articular, estandarizar, visualizar y comunicar todos los procesos de participación del Ajuntament de Barcelona y de la ciudad ofreciendo un servicio de infraestructura digital para la democracia directa y participativa a todas las escalas territoriales y asociativas de Barcelona. Estos objetivos llevarán consigo un incremento en la calidad de la plataforma, haciéndola cada vez más inclusiva, accesible, segura y respetuosa con la privacidad de las personas usuarias. También se busca facilitar el desarrollo de procesos y la auto-organización por parte de la ciudadanía, y ofrecer herramientas para la colaboración social. 

* Entre los aspectos clave del desarrollo de decidim.barcelona como proyecto sociotécnico se encuentran: la gobernanza, inicialmente llevada a cabo por la *Direcció de Recerca, Desenvolupament i Innovació* y que estará a cargo de la comunidad decidim a medio-largo plazo; el diseño tecnopolítico, que ha de atender tanto a las funcionalidades técnicas tanto como a los requisitos políticos y democráticos; la contratación y gestión del desarrollo del software, así como la administración de procesos participativos concretos; la investigación y evaluación de la actividad y dinámicas en la plataforma para mejorar la calidad democrática; la formación y capacitación crítica en el uso de la misma; por último, la coordinación del desarrollo de la plataforma con otros ayuntamientos e instituciones.

* El **flujo de desarrollo** está marcado por el tipo de programación **(desarrollo extremo)**, en el que el software se va adaptando a los cambios a la vez que se prueba en procesos de participación real, lo que implica satisfacer rápidamente funcionalidades o mejoras. El flujo se basa en lo propuesto inicialmente por el proyecto de software libre *git flow*[^1], diferenciando las siguientes ramas: **master**: es la versión estable, la que tomarán otras entidades que vayan a usar el software; **develop**: es la versión en desarrollo sobre la que se integran las demás ramas; **release**: acumula los desarrollos y las features para la siguiente versión estable, publicándose a través de releases de GitHub; **hotfixes**: sólo para corregir fallos rápidamente; **feature-X**: donde X son diferentes funcionalidades que pueden o constituir un hito o milestone concreto del master.

* La **arquitectura** es un aspecto clave del desarrollo del decidim a largo plazo. A fin de garantizar la **sostenibilidad, usabilidad y escalabilidad** se ha optado por un **desarrollo modular** sobre la aplicación web *Ruby on Rails*. El desarrollo estará basado en **Engines**, **componentes diferenciados para las distintas funcionalidades** (Propuestas, Debates, Legislación colaborativa, Citas presenciales, etc) y contará con mejoras en la documentación, tanto para su instalación como para su reutilización y adaptación por parte de otras entidades.  

* A fin de definir la **ontología** o conjunto de elementos del decidim se elabora un **glosario**, que define expresiones como  "proceso participativo", “espacios de participación, “componentes”, etc.

* En el documento se presentan las **funcionalidades descritas distribuidas en tres periodos: corto (2016), medio (2017) y largo plazo (2018)**. Asimismo se apuntan las **revisiones periódicas** a las que se someterá la plataforma, a fin de garantizar unos altos estándares de **apertura, privacidad, robustez y seguridad **en el código.

* Se calendarizan las **versiones** planeadas por el momento (0.5, en Octubre de 2016; 1, en Enero de 2017; y 1.5, en Marzo de 2017), así como los roles y gestión de usuarias en cada una. 

* También se define el **flujo de gestión de incidencias** mediante el uso de diferentes herramientas (como mailing y *Redmine*) y se definen los diferentes roles en el mismo. 

* El plan también detalla el carácter interdisciplinar, la organización y la estructura interna del **grupo de desarrollo**. El equipo está formado inicialmente por personas de  ámbitos diversos: **Ajuntament de Barcelona, universidades, profesionales especializados en programación**. A su vez el plan presenta el software usado para la coordinación y gestión de proyectos.

* Más tarde se presenta el **MetaDecidim**, un espacio en el decidim.barcelona y un proceso participativo para (re)diseñar las funcionalidades de la plataforma, priorizar las líneas de desarrollo, decidir proyectos de mejora y deliberar sobre los usos y posibilidades futuras de la herramienta. Metadecidim servirá también para crear una comunidad y un ecosistema de producción que ponga sobre la mesa el papel de gran calado democrático que representa la plataforma para la ciudadanía.

* **Más allá del decidim.barcelona**, se apuntan las posibilidades de una red de producción popular y gobernanza comunitaria  para las Superillas. 

* En el apéndice se define uno de los elementos innovadores del decidim.barcelona, la estructura del **configurador de procesos participativos**. 

* El plan se cierra proponiendo decidim.barcelona como infraestructura democrática para la democracia, base para la **democracia del futuro, hoy.**

[^1]: Ver "A successful Git branching model" por Vincent Driessen publicado el 5 de enero de 2010 http://nvie.com/posts/a-successful-git-branching-model/