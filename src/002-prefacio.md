# Prefacio

Si has elegido este libro, es probable que hayas sentido profundamente el dolor de gestionar datos sin tener control sobre su ingestión y generación. Aunque en un momento dado nuestro sector se centró en implementaciones locales bien pensadas con modelos de datos robustos, el auge de la computación en la nube y la explosión de productos de datos dentro de las organizaciones, a través de la IA, han incentivado la rapidez de comercialización a costa de convertir la capa de datos en un caos. Muchos equipos de datos que se encuentran en esta situación se ven obligados a actuar de forma reactiva, solucionando repetidamente los siguientes problemas relacionados con los datos dentro de la empresa.

En esencia, creemos que este reto en nuestro sector se deriva de la dificultad de gestionar el cambio entre equipos de productores y consumidores de datos que históricamente han estado aislados. Concretamente, existe una desconexión entre el código de las aplicaciones upstream, que define cómo se capturan los datos dentro de un sistema de software, y los productos de datos downstream que aprovechan estos datos. Defendemos que los contratos de datos sirven como mecanismo para alinear a los productores y consumidores de datos mediante la automatización y la definición de expectativas como código.

## ¿Qué son los contratos de datos?

Los contratos de datos son un patrón de arquitectura que permite un acuerdo entre los productores y los consumidores de datos que se establece, actualiza y aplica a través de una API. Forman parte de un movimiento más amplio denominado «shift left», en el que se utiliza la automatización para permitir a los desarrolladores de software ascendentes tener en cuenta la aplicación necesaria pertinente a su dominio; este enfoque se validó por primera vez en DevOps y DevSecOps.

Los contratos de datos constan de cuatro componentes clave:

- Activos de datos que necesitan protección mediante la gestión de cambios

- Un archivo de especificaciones contractuales que codifica las expectativas de los activos de datos como código controlado por versiones

- Detección mediante la capacidad de extraer, analizar y tomar medidas sobre los cambios en los metadatos relacionados con los activos de datos bajo contrato

- Prevención mediante la automatización de la aplicación de contratos de datos dentro del flujo de trabajo de los desarrolladores, normalmente durante los procesos de CI/CD

Sostenemos que la industria de los datos está viviendo su momento de «shift left» y que los contratos de datos son fundamentales para este cambio.

## Cómo utilizar este libro

Uno de los principales motivos que nos llevó a escribir este libro fue la temprana reacción negativa de que el concepto de los contratos de datos era demasiado teórico. Este punto de vista es comprensible, ya que muchas implementaciones no eran públicas en ese momento, pero sabíamos que los contratos de datos estaban ganando adeptos. Hemos entrevistado a cientos de empresas y hemos ayudado a numerosos equipos a adoptar sus propios contratos de datos.

Por lo tanto, nuestro objetivo con este libro es que sirva como guía práctica para 1) enmarcar los problemas de nuestra industria que crean la necesidad de contratos de datos, 2) implementar contratos de datos (incluso mediante el uso de un repositorio público de GitHub con un entorno sandbox) y 3) generar aceptación entre los líderes ejecutivos y ampliar la adopción en toda la organización.

Hemos organizado los capítulos en tres partes diferenciadas, para que puedas volver a consultar este libro a lo largo de tu proceso de implementación de contratos de datos.

### Parte I: Introducción a la arquitectura de contratos de datos

Los capítulos 1 a 4 proporcionan el contexto histórico y de mercado que explica por qué los retos de la gestión de datos siguen persistiendo en la actualidad, al tiempo que ofrecen una comprensión básica de la calidad de los datos, la infraestructura de datos y el flujo de trabajo de los contratos de datos para el cumplimiento de las expectativas. A continuación se ofrece un desglose:

- Capítulo 1: Por qué la industria necesita ahora contratos de datos

- Capítulo 2: La calidad de los datos no se refiere a datos impecables

- Capítulo 3: Los retos de escalar la infraestructura de datos

- Capítulo 4: Introducción a los contratos de datos

### Parte II: Implementación de la arquitectura de contratos de datos

Los capítulos 5 a 8 detallan los componentes técnicos de la arquitectura de contratos de datos y proporcionan una guía para implementar contratos de datos a través de un repositorio GitHub adjunto. Además, destacamos múltiples casos prácticos reales de contratos de datos en producción, que van desde startups hasta grandes empresas. Esta parte incluye lo siguiente:

- Capítulo 5: Los componentes de los contratos de datos: activos de datos y definición de contratos

- Capítulo 6: Los componentes de los contratos de datos: detección y prevención

- Capítulo 7: Implementación de contratos de datos

- Capítulo 8: Casos prácticos reales de contratos de datos en producción

### Parte III: Obtención del apoyo de los directivos para la arquitectura de contratos de datos

Los capítulos 9 a 12 subrayan cómo los contratos de datos resuelven los problemas sociotécnicos que se derivan de la dificultad de gestionar el cambio dentro de las organizaciones. Resolver estos problemas requiere tener una enorme influencia para alinear a varios equipos que históricamente han estado aislados entre sí. Estos capítulos son el resultado de las lecciones que hemos aprendido al ayudar a las organizaciones a adoptar los contratos de datos, aumentar su adopción y medir su impacto. Los capítulos de esta parte son los siguientes:

- Capítulo 9: Cambio hacia la izquierda: el cambio cultural necesario para los contratos de datos

- Capítulo 10: Gestión del cambio: el quid de la cuestión en cuanto a personas, procesos y tecnología

- Capítulo 11: Cómo obtener tus primeros éxitos con los contratos de datos

- Capítulo 12: Medición del impacto de los contratos de datos

## Convenciones utilizadas en este libro

En este libro se utilizan las siguientes convenciones tipográficas:

_Cursiva_

Indica nuevos términos, URL, direcciones de correo electrónico, nombres de archivos y extensiones de archivos.

`Constant width`

Se utiliza para listados de programas, así como dentro de párrafos para hacer referencia a elementos de programas, como nombres de variables o funciones, bases de datos, tipos de datos, variables de entorno, instrucciones y palabras clave.

`<Constant width in angled brackets>`
Muestra el texto que debe sustituirse por valores proporcionados por el usuario o por valores determinados por el contexto.

> **NOTA**

> Este elemento indica una nota general.

> **ADVERTENCIA**

> Este elemento indica una advertencia o precaución.

## Uso de ejemplos de código

El material complementario (ejemplos de código, ejercicios, etc.) se puede descargar en https://github.com/data-contract-book. Esto incluye un entorno sandbox, que puedes ejecutar localmente o dentro del navegador, que te guía a través de la implementación de contratos de datos y el flujo de trabajo de violación de contratos de datos.

Si tienes alguna pregunta técnica o algún problema al utilizar los ejemplos de código, envía un correo electrónico a support@oreilly.com.

Además, el libro cuenta con un sitio web complementario que ofrece artículos adicionales de los autores, así como vídeos correspondientes para guiarte en la lectura de los capítulos.

Este libro está aquí para ayudarte a realizar tu trabajo. En general, si se ofrece código de ejemplo con este libro, puedes utilizarlo en tus programas y documentación. No es necesario que te pongas en contacto con nosotros para solicitar permiso, a menos que reproduzcas una parte significativa del código. Por ejemplo, escribir un programa que utilice varios fragmentos de código de este libro no requiere permiso. La venta o distribución de ejemplos de libros de O'Reilly sí requiere permiso. Responder a una pregunta citando este libro y el código de ejemplo no requiere permiso. Incorporar una cantidad significativa de código de ejemplo de este libro en la documentación de tu producto sí requiere permiso.

Agradecemos la atribución, pero por lo general no la exigimos. La atribución suele incluir el título, el autor, el editor y el ISBN. Por ejemplo:«Data Contracts, de Chad Sanderson, Mark Freeman y B.E. Schmidt (O'Reilly). Copyright 2026 Manifest Data Labs, Inc. y Benjamin Schmidt, 978-1-098-15763-0».

Si consideras que tu uso de los ejemplos de código no entra dentro del uso legítimo o del permiso otorgado anteriormente, no dudes en ponerte en contacto con nosotros en permissions@oreilly.com.

## Aprendizaje en línea de O'Reilly

> **Nota**

> Durante más de 40 años, O'Reilly Media ha proporcionado formación, conocimientos y perspectivas sobre tecnología y negocios para ayudar a las empresas a alcanzar el éxito.

Nuestra exclusiva red de expertos e innovadores comparte sus conocimientos y experiencia a través de libros, artículos y nuestra plataforma de aprendizaje en línea. La plataforma de aprendizaje en línea de O'Reilly te ofrece acceso bajo demanda a cursos de formación en directo, itinerarios de aprendizaje en profundidad, entornos de programación interactivos y una amplia colección de textos y vídeos de O'Reilly y más de 200 editoriales. Para obtener más información, visita https://oreilly.com.

## Cómo ponerse en contacto con nosotros

Envía tus comentarios y preguntas sobre este libro a la editorial:

O'Reilly Media, Inc.

141 Stony Circle, Suite 195

Santa Rosa, CA 95401

800-889-8969 (en Estados Unidos o Canadá)

707-827-7019 (internacional o local)

707-829-0104 (fax)

support@oreilly.com

https://oreilly.com/about/contact.html

Tenemos una página web para este libro, donde enumeramos las erratas y cualquier información adicional. Puedes acceder a esta página en https://oreil.ly/DataContracts.

Para obtener noticias e información sobre nuestros libros y cursos, visita https://oreilly.com.

Encuéntranos en LinkedIn: https://linkedin.com/company/oreilly-media.

Síguenos en YouTube: https://youtube.com/oreillymedia.

## Agradecimientos

Aunque nuestros nombres aparecen en la portada, este libro no habría sido posible sin el apoyo de nuestros colegas y nuestra comunidad. Queremos dar las gracias a nuestros colegas de Gable que nos han acompañado durante todo el proceso de profundización en la comprensión de los contratos de datos y la implementación de los mismos: Aaron Phillips, Adrian Kreuziger, Adrian Kuepker, Alex DeMeo, Andrew Oliver, Chayanne Aranda, Daniel Dicker, Daniil Tiganov, Demetrios Brinkmann, Geoffrey Wukelic, Hana Um, James Frost, Jasmine Simpelo, Jazmia Henry, Jon Shaiman, Karan Banwasi, Kidanekal Hailu, Leonie Jean Parojinog, Maks Sydorenko, Max Zunti, Mike Perrone, Mindaugas Rukas, Nazar Repak, Rachel Rosefigura, Ran Liu, Ravi Vooda, Rebecca Swords, Russell Rivera, Sara La Torre, Suzanne Wen, Tom Erwin, Tommy Guy y Yuhang An. También queremos dar las gracias a los inversores de Gable, que fueron de los primeros en creer y respaldar la idea de los contratos de datos: Apoorva Pandhi (Zetta Venture Partners), Scott Sage (Crane Venture Partners), Nick Giometti (B Capital) y nuestros otros inversores ángeles y posteriores.

Además, queremos dar las gracias a nuestros increíbles editores de O'Reilly Media, con quienes trabajamos directamente durante todo el proceso de redacción del libro: Aaron Black, Melissa Potter (y Evie, la gata) y Katherine Tozer. Agradecemos a nuestros amigos de Omniscient Digital, que también apoyaron nuestros esfuerzos en la redacción del libro: Alex Birkett y Megan Otto.

Por último, queremos dar las gracias a los miembros de la comunidad Shift Left Data, que nos han proporcionado comentarios sobre el libro y muchas ideas sobre los contratos de datos: Aishvarya Verma, Ali Khalid, Amanda Manley, Ashraf Mohammad, Ben Heron, Bill Coulam, Christian van Eeden, Cristóbal Carvajal Benavides, Eddy Zulkifly, Eric Callahan, Eric Dressler, Erik Dahlberg, Gene Vestel, Ignatius Soputro, Joel Anderson, Jon Yeo, Jonathan Bergenblom, Jose Santos, Kiran S., Lars Nielsen, Luka Stepinac, Mahesh Kumar, Matt Nylin, Michael Day, Mohamed Mansour, Nachiket Mehta, Narayanan V., Nidhi Vichare, Oliver Rudolph, Pawel Stradowski, Perry Philipp, Prashant Verma, Rafael Socorro, Raghu Mundru, Rubén Arévalo, Rukmani All, Saqib Ali, Satya Vandrangi, Sharon Sokoloff, Tanya Mackinnon, Thanh Khong, Tony McCray, Wei Hao, Yesh Kaushik y Zakariah Siyaji.

_Chad Sanderson_

Este libro ha sido todo un viaje. No habría sido posible sin el apoyo de personas increíbles, tanto a nivel profesional como personal. Mis cofundadores, Adrian, James y Daniel, por trabajar sin descanso cuando los contratos de datos no eran más que una idea. Todo el equipo de Gable por hacer realidad los contratos de datos. Nuestros inversores, Apoorva, Scott, Nick y tantos otros, por creer en el poder de los contratos de datos cuando nadie más veía la visión.

A nivel personal, me gustaría dedicar este libro a mi maravillosa esposa, Laila, que ha sido un ángel perfecto durante todo este proceso, así como a mis hermanas, Cat, Izzy y Taylor, a mi maravillosa madre y a mi padre, que fue quien me animó a empezar a escribir. Os quiero a todos.

_Mark Freeman_

Creo firmemente que se necesita un pueblo para alcanzar los distintos hitos de la vida. Por eso, me gustaría dar las gracias a mi maravillosa esposa por su apoyo, paciencia y ánimo incansables durante la redacción de este libro (así como a nuestro querido perro, Albus). También me gustaría dar las gracias a mi madre, mi padre, Justin, Charene y otros familiares y amigos que me han brindado un apoyo similar.

Además, me gustaría dar las gracias a todos mis mentores que han invertido su tiempo en apoyar mi carrera en el campo de los datos. La lista incluye, aunque no es exhaustiva, al Centro de Investigación Preventiva de Stanford (Dr. Michael Baiocchi, Dra. Janine Bruce, mis asesores de Investigación en Salud Comunitaria y Prevención, mis colegas de investigación de WELL for Life), Lisa Tealer, Dr. Joe Orsini, Omead Arami, Dra. Stefanie Tignor, Joe Reis y Vin Vashishta.

Por último, quiero expresar mi más sincero agradecimiento a mis coautores, Chad y Ben, ya que ha sido un verdadero trabajo en equipo y he aprendido mucho de ustedes dos.

_B. E. Schmidt_

Gracias a mis dos coautores por invitarme amablemente a participar en esta excelente aventura, y a la inteligente y amable gente de Omniscient Digital por la oportunidad de trabajar con Chad y Mark en primer lugar.

Gracias, en general, a los buenos editores y buenos amigos, y al intercambio vital que permiten con los escritores en sus vidas.

Y, por último, gracias y todo mi amor a mi paciente esposa, a nuestros dos hijos y a la mayoría de nuestros tres perros.

(No hagas caso a los que te critican, Gus. Eres un buen chico).
