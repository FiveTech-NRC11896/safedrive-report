![Logo UPC](assets/images/Upc/Banner-UPC.png)

**Nombre de la Universidad:** Universidad Peruana de Ciencias Aplicadas  
**Facultad:** Ingeniería  
**Carrera:** Ingeniería de Software / Sistemas de Información  
**Ciclo:** 2026-10

**Código del curso:** 1ASI0729  
**Nombre del curso:** Desarrollo de Aplicaciones Open Source  
**NRC:** 11896  
**Nombre del profesor:** Efraín Ricardo Bautista Ubillús

**"Informe de Trabajo Final"**
**Nombre del startup:** FiveTech  
**Nombre del producto:** SafeRoute

**Relación de integrantes:**
* U202315968 - Costa Morales, Christofer William
* U201717085 - Revilla Quispe, Renzo Zamir
* U20241D922 - Quispe Serrano, Julio Frank
* U202424059 - De la Cruz De los Santos, Mathias Marcelo
* U202316852 - Ortega Quintana, José Zacarias


**Abril, 2026**

---

## Registro de Versiones del Informe

| Avance | Fecha      | Autor                                                                                                                                                         | Descripción de Modificación                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| :----- | :--------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AV1    | --/04/2026 | De La Cruz De Los Santos, Mathias Marcelo; Ortega Quintana, Jose Zacarias; Quispe Serrano, Julio Frank; Costa Morales, Christofer William; Revilla Quispe, Renzo Zamir | Se desarrolló el Sprint Review correspondiente a la Semana 4, incluyendo la elaboración del Final Project Documentation Report, la presentación del Final Project Keynote y el reporte individual de desempeño de los integrantes. A nivel de implementación, se desarrolló y desplegó la primera versión del Landing Page. El informe incorpora la carátula, registro de versiones, insights de colaboración, student outcome, y los capítulos I al V, abarcando desde la introducción, levantamiento y especificación de requerimientos, diseño del producto, hasta la implementación, validación y despliegue. Además, se documenta la gestión de configuración del software, el entorno de desarrollo, control de código fuente, convenciones de estilo y configuración de despliegue. Finalmente, se incluye la evidencia completa del Sprint 1: planificación, backlog, desarrollo, ejecución, documentación de servicios, despliegue y análisis de la colaboración del equipo, junto con conclusiones, bibliografía y anexos. |

---

## Project Report Collaboration Insights

El equipo ha utilizado un flujo de trabajo en github: [https://github.com/FiveTech-NRC11896/SafeRoute-report](https://github.com/FiveTech-NRC11896/SafeRoute-report)

---

## Contenido

1. [Student Outcome](#student-outcome)
2. [Capítulo I: Introducción](#capítulo-i-introducción)
3. [Capítulo II: Requirements Elicitation & Analysis](#capítulo-ii-requirements-elicitation--analysis)
4. [Capítulo III: Requirements Specification](#capítulo-iii-requirements-specification)
5. [Capítulo IV: Product Design](#capítulo-iv-product-design)
6. [Capítulo V: Product Implementation, Validation & Deployment](#capítulo-v-product-implementation-validation--deployment)
7. [Conclusiones](#conclusiones)
8. [Bibliografía](#bibliografía)

---

## Student Outcome

**ABET - EAC - Student Outcome 3:** Capacidad de comunicarse efectivamente con un rango de audiencias.

---

## Capítulo I: Introducción

### 1.1. Startup Profile

#### 1.1.1. Descripción de la Startup

FiveTech es una startup de tecnología conformada por estudiantes de Ingeniería de Software de la Universidad Peruana de Ciencias Aplicadas (UPC), orientada al desarrollo de soluciones digitales que resuelven problemas reales en sectores con baja penetración tecnológica. Nació con la convicción de que la seguridad de los niños durante su traslado escolar no debería depender de llamadas telefónicas, mensajes de WhatsApp o registros manuales en papel.
Nuestra propuesta de valor se materializa en SafeRoute, una plataforma web de movilidad institucional inteligente diseñada para digitalizar y optimizar la gestión del transporte escolar. SafeRoute permite a cualquier organización de transporte escolar ya sea un grupo de padres que se organizaron para compartir una movilidad, un conductor independiente o una pequeña empresa del rubro que busquen centralizar la administración de sus rutas, conductores, alumnos y la comunicación en un solo lugar.

#### 1.1.2. Perfiles de integrantes del equipo

|                  Foto                   | Apellidos y Nombres         |    Código     | Carrera                | Resumen                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| :-------------------------------------: | :-------------------------- | :-----------: | :--------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                 ![foto]                 | [Apellido 1], [Nombre 1]    | [U20XXXXXXXX] | Ingeniería de Software | [Descripción de conocimientos técnicos y habilidades que aporta al equipo]                                                                                                                                                                                                                                                                                                                                                                             |
|              ![Renzo Revilla](./assets/images/renzo.png)              | Revilla Quispe, Renzo Zamir   | U201717085 | Ingeniería de Software | Soy Renzo Revilla, estudiante de Ingenieria de Software en la Universidad Peruana de Ciencias Aplicadas, con experiencia en desarrollo web y movil. Me destaco por mis habilidades en comunicacion efectiva y trabajo en equipo, lo que facilita la coordinación y el cumplimiento de objetivos dentro del grupo. Disfruto de la natacion y del aprendizaje continuo. Mi aporte al equipo se centra en el desarrollo tecnico y en la gestion del proyecto, contribuyendo a mantener un trabajo organizado y eficiente.  |
| ![foto](assets/images/FrankFT.png) | Quispe Serrano, Julio Frank | [U20241D922]  | Ingeniería de Software | Mi nombre es Julio Frank Quispe Serrano, tengo 20 años,actualmente estoy cursando el 5to ciclo de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Soy un apasionado por la programación, el gym y explorador de música en distintos géneros. Mi aporte en este grupo será el de brindar soluciones prácticas y eficientes ante situaciones de adversidad que estanquen la fluidez de la elaboración del trabajo. |
|              ![foto](assets/images/MathiasFt.jpg)               | De la Cruz De los Santos, Mathias Marcelo    | [U202424059] | Ingeniería de Software | Soy estudiante de la carrera de Ingeniería de Software y actualmente me encuentro cursando el 5to ciclo de la carrera en la Universidad Peruana de Ciencias Aplicadas. Me considero un fanático de la programación, del futbol y los videojuegos. Considero que puedo aportar al equipo y al proyecto mis conocimientos técnicos, además de considerarme una persona disciplinada, responsable y que valora el trabajo en equipo.                                                                                                                                                                                                                                                                                                                                                     |
|              ![foto]               | [Apellido 5], [Nombre 5]    | [U20XXXXXXXX] | Ingeniería de Software | [Descripción de conocimientos técnicos y habilidades que aporta al equipo]                                                                                                                                                                                                                                                                                                                                                                             |

### 1.2. Solution Profile

#### 1.2.1 Antecedentes y problemática

Who (¿Quiénes son los afectados?)
Los afectados son dos grupos claramente identificables. En primer lugar, los padres de familia con hijos en nivel inicial, kínder y primaria que utilizan servicios de transporte escolar privado, quienes no cuentan con información en tiempo real sobre el estado del traslado de sus hijos. En segundo lugar, los conductores de transporte escolar independientes o pertenecientes a pequeñas empresas que gestionan múltiples alumnos y rutas sin herramientas digitales de apoyo.

What (¿Cuál es el problema?)
El transporte escolar privado en el Perú opera en su gran mayoría de forma tradicional y sin soporte tecnológico. La comunicación entre padres y conductores depende de canales no estructurados como llamadas telefónicas y grupos de WhatsApp, lo que genera desorganización, pérdida de información y una sensación constante de incertidumbre en los padres respecto a la seguridad de sus hijos. Por su parte, los conductores y administradores del servicio carecen de herramientas para registrar asistencia, gestionar rutas, reportar incidencias y llevar un historial ordenado de cada trayecto.

Where (¿Dónde ocurre?)
El problema se presenta principalmente en zonas urbanas de Lima Metropolitana, donde la demanda de transporte escolar privado es alta y la oferta opera de manera fragmentada e incluso a veces informal. Sin embargo, la problemática es extensible a cualquier ciudad del Perú con alta densidad de centros educativos privados y colegios que no cuentan con flota propia.

When (¿Cuándo ocurre?)
El problema se manifiesta de forma recurrente durante los horarios de entrada y salida escolar, típicamente entre las 6:00 a.m. y 8:30 a.m., y entre las 12:30 p.m. y 5:00 p.m. Es en estos momentos cuando la falta de información en tiempo real genera mayor ansiedad en los padres y mayor presión operativa en los conductores.

Why (¿Por qué es un problema?)
La ausencia de digitalización en este sector genera consecuencias concretas, por ejemplo los padres no saben si su hijo abordó la movilidad, si llegó al colegio o si ocurrió algún incidente en el camino. Los conductores cometen errores en las paradas, olvidan recoger alumnos o no tienen cómo comunicar retrasos de forma ordenada. Los administradores del servicio pierden tiempo valioso coordinando manualmente lo que podría automatizarse, y no cuentan con registros históricos que les permitan mejorar la operación.

How (¿Cómo se manifiesta?)
Se manifiesta en llamadas y mensajes constantes de padres al conductor durante el trayecto, listas de alumnos escritas en papel o en hojas de cálculo no compartidas, ausencia de registros de incidencias, imposibilidad de verificar el cumplimiento de las paradas, y falta de trazabilidad sobre qué alumnos abordaron o no en cada viaje.

How much (¿Cuál es la magnitud?)
Si bien no existen datos precisos y actualizados que cuantifiquen de forma específica el mercado del transporte escolar privado en el Perú, los indicadores educativos y de transporte disponibles permiten dimensionar la magnitud del problema.
Según el Censo Educativo 2022-2023 del Ministerio de Educación (MINEDU, 2023), en Lima Metropolitana existen aproximadamente 1.9 millones de estudiantes distribuidos en cerca de 7,602 instituciones educativas, de las cuales el 74% son de gestión privada. Esta alta concentración de colegios privados implica que muchas familias dependen de servicios externos de transporte escolar, dado que pocas instituciones cuentan con flotas propias.
Este panorama se ve agravado por una reducción en la oferta formal del servicio. Según la Autoridad de Transporte Urbano para Lima y Callao (ATU, 2024), la cantidad de movilidades escolares autorizadas disminuyó en un 25% en solo un año, lo que sugiere un incremento en la informalidad del sector y, con ello, una mayor ausencia de herramientas de control y monitoreo sobre el servicio que reciben los menores.
Respecto a la seguridad, la Superintendencia de Transporte Terrestre de Personas, Carga y Mercancías (SUTRAN, 2024) ejecutó campañas de sensibilización que alcanzaron a más de 47,000 escolares, evidenciando que la seguridad en el transporte escolar continúa siendo una preocupación activa para las autoridades. Sin embargo, no se dispone públicamente de cifras desagregadas de incidentes específicos en este sector entre 2022 y 2025.

**Figura 1** Distribución de estudiantes de Educación Inicial y Primaria en instituciones privadas y zonas urbanas en el Perú
![CensoEstudiantil](/assets/images/CensoEstudiantil.png)
_Nota._ Adaptado de Resultados del Censo Educativo 2022 (p. 12), por Ministerio de Educación, 2023.

#### 1.2.2 Lean UX Process

##### 1.2.2.1. Lean UX Problem Statements

El transporte escolar privado en el Perú opera mayoritariamente de forma informal, coordinándose mediante llamadas telefónicas, mensajes de WhatsApp y registros manuales en hojas privadas. En este contexto, tanto los padres de familia como los transportistas escolares enfrentan dificultades que comprometen la seguridad y eficiencia del servicio.
Hemos observado un factor crítico que afecta a este ecosistema, los padres de familia no cuentan con visibilidad sobre el trayecto de sus hijos, mientras que los transportistas carecen de herramientas digitales para gestionar rutas, alumnos e incidencias de forma estructurada. Estas dos necesidades son interdependientes, mientras que por un lado los padres necesitan visibilidad, y por el otro los transportistas no tienen los medios para proporcionársela.
¿Cómo podemos desarrollar una plataforma que permita a los transportistas escolares gestionar su operación de forma digital, mientras ofrece simultáneamente a los padres de familia la visibilidad y tranquilidad que necesitan sobre el traslado de sus hijos?

##### 1.2.2.2. Lean UX Assumptions

**Business Assumptions**

- Creemos que existe demanda suficiente para digitalizar el transporte escolar privado en Lima Metropolitana, dado que opera mayoritariamente de forma tradicional y sin soporte tecnológico.
- Creemos que los padres de familia adoptarán la plataforma si el proceso de incorporación es simple y la información que reciben sobre el trayecto de sus hijos es clara y confiable.
- Creemos que los transportistas adoptarán la plataforma si la interfaz operativa durante el trayecto es simple, rápida y no distrae la conducción.
- Creemos que el modelo de suscripción por planes escalonados Básico, Intermedio y Completo permite capturar tanto a grupos pequeños de padres organizados como a empresas de transporte escolar con flotas más grandes.
- Creemos que SafeRoute transmite ahorro de tiempo, reduccion de errores y confianza al transporte de los escolares frente a los padres de familia, lo que justifica el costo de la suscripción.
- Sabremos que estamos equivocados si los administradores abandonan la plataforma en los primeros 60 días por considerar que la curva de aprendizaje es demasiado alta o que el valor percibido no justifica el costo.

**User Assumptions**

- ¿Quién es el usuario?
  Los padres de familia con hijos en nivel inicial, kínder y primaria que utilizan un servicio de transporte escolar ya contratado, y los transportistas escolares como por ejemplo los conductores independientes o responsables de pequeñas empresas que operan ese servicio. Dentro de la plataforma, cualquiera de estos segmentos puede asumir además el rol de Administrador.
- ¿Dónde encaja nuestro producto en su vida?
  Para el transportista, en su jornada laboral operativa diaria. Para el padre, en los momentos de entrada y salida escolar de sus hijos.
- ¿Qué problemas resuelve?
  Elimina la gestión manual y la comunicación no estructurada del transporte escolar, proporcionando al transportista herramientas operativas digitales y al padre visibilidad del trayecto de sus hijos.
- ¿Cuándo y cómo es usado?
  El transportista lo usa durante cada trayecto para gestionar abordajes, paradas e incidencias. El padre lo consulta en los horarios de traslado escolar para monitorear el estado del viaje de sus hijos.
- ¿Qué características son importantes?
  Registro de abordaje por alumno, visualización de ruta y paradas, reporte de incidencias, historial de trayectos y gestión centralizada de usuarios y rutas.
- ¿Cómo debe verse y comportarse?
  Interfaz limpia, responsiva, rápida y accesible (a11y), disponible en español e inglés (i18n), e intuitiva para usuarios con distintos niveles de familiaridad tecnológica.

##### 1.2.2.3. Lean UX Hypothesis Statements

- Hipótesis 1: "Creemos que lograremos que los padres de familia reduzcan su incertidumbre durante el traslado escolar si ofrecemos a los padres registrados en SafeRoute una vista del estado del trayecto con marcación de abordaje por alumno y visualización de paradas.
  Sabremos que esto es verdad cuando veamos que al menos el 70% de los padres activos consulten el estado del trayecto al menos una vez por día durante las primeras 4 semanas de uso."

- Hipótesis 2: "Creemos que lograremos que los transportistas gestionen el trayecto con menos errores y menor carga operativa si ofrecemos a los conductores registrados en SafeRoute una interfaz operativa simple para marcar abordajes, seguir paradas y reportar incidencias durante el viaje.
  Sabremos que esto es verdad cuando veamos que el 80% de los trayectos registrados incluyan el check-list de abordaje completado durante las primeras 4 semanas de operación."

- Hipótesis 3: "Creemos que lograremos que los administradores centralicen la gestión de su servicio en SafeRoute si ofrecemos a los administradores del plan Básico un panel único para registrar usuarios, conductores, hijos, asignaciones y rutas. Sabremos que esto es verdad cuando veamos que al menos el 75% de los administradores registren la totalidad de sus usuarios y rutas dentro de los primeros 15 días tras el onboarding."

- Hipótesis 4: "Creemos que lograremos que los administradores escalen su plan de suscripción si demostramos a los administradores de los planes inferiores que las funcionalidades de los plan superiores reducen significativamente el tiempo de coordinación del servicio. Sabremos que esto es verdad cuando veamos que al menos el 20% de los administradores de los planes Básico o Intermedio actualicen al algun plan superior dentro de los primeros 3 meses de uso."

##### 1.2.2.4. Lean UX Canvas

| Sección                                                                                  | Contenido                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| :--------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1. Business Problem                                                                      | El transporte escolar privado en el Perú opera de forma tradicional y sin soporte tecnológico. Los padres no tienen visibilidad sobre el trayecto de sus hijos y los transportistas gestionan su operación con llamadas, WhatsApp y hojas privadas, lo que genera errores, ineficiencia y una experiencia de servicio poco confiable.                                                                                                                                                                                                           |
| 2. Business Outcomes                                                                     | Lograr que el 75% de administradores completen el registro de su operación en los primeros 15 días. Retener al 80% de suscriptores activos durante los primeros 3 meses. Alcanzar una tasa de upgrade del plan Básico al Intermedio del 20% en los primeros 3 meses de uso.                                                                                                                                                                                                                                                                     |
| 3. Users                                                                                 | Los segmentos que interactúan con SafeRoute son los padres de familia con hijos en nivel inicial, kínder y primaria que utilizan un servicio de transporte escolar ya contratado, y los transportistas escolares conductores independientes o responsables de pequeñas empresas que operan ese servicio. Cualquiera de estos puede asumir además el rol de Administrador dentro de la plataforma.                                                                                                                                               |
| 4. User Outcomes & Benefits                                                              | Los padres buscan reducir su incertidumbre sobre el trayecto de sus hijos, pudiendo monitorear el estado del viaje sin necesidad de interrumpir al conductor. Los transportistas buscan gestionar rutas, alumnos e incidencias de forma digital, reduciendo errores operativos y proyectando mayor profesionalismo frente a las familias. Quienes asumen el rol de administrador buscan centralizar toda la operación del servicio en un solo panel, eliminando la coordinación manual y el uso de herramientas desconectadas.                  |
| 5. Solution Ideas                                                                        | Ofrecemos un panel de administración de usuarios, conductores, hijos y rutas. Tambien, Check-list de abordaje digital por conductor. Vista de paradas y estado del trayecto para padres. Registro de incidencias por ruta. Historial de trayectos por comunidad de ruta. Seguimiento GPS en tiempo real (plan Completo). Apertura a integración IoT futura.                                                                                                                                                                                     |
| 6. Hypotheses                                                                            | - Si ofrecemos a los padres una vista de estado del trayecto, al menos el 70% la consultará diariamente en las primeras 4 semanas.<br> - Si ofrecemos al conductor una interfaz operativa simple, el 80% de los trayectos tendrán el check-list completado en las primeras 4 semanas.<br> - Si ofrecemos al administrador un panel único de gestión, el 75% completará su registro en los primeros 15 días.<br> - Si demostramos el valor del plan Intermedio, el 20% de administradores del plan Básico harán upgrade en los primeros 3 meses. |
| 7. What's the most important thing we need to learn first?                               | ¿El administrador del servicio percibe suficiente valor en SafeRoute como para abandonar los métodos informales actuales y pagar una suscripción mensual?                                                                                                                                                                                                                                                                                                                                                                                       |
| 8. What's the least amount of work we need to do to learn the next most important thing? | Realizar entrevistas con 3 a 5 administradores de servicios de transporte escolar (padres representantes o transportistas independientes) para validar su disposición al cambio y las funcionalidades que consideran imprescindibles antes de desarrollar el MVP.                                                                                                                                                                                                                                                                               |

### 1.3. Segmentos objetivo

SafeRoute está dirigido a dos segmentos que forman parte del ecosistema del transporte escolar privado en Lima Metropolitana.

- **Segmento 1: Padres de Familia**
  El primer segmento está conformado por padres de familia o apoderados con hijos en nivel inicial, kínder y primaria que utilizan un servicio de transporte escolar privado ya contratado. Se trata de personas que han delegado el traslado de sus hijos a un tercero y que, durante el trayecto, no cuentan con información estructurada sobre el estado del viaje. Este segmento no está delimitado por un nivel socioeconómico específico, sino por la condición de tener hijos en edad escolar que usan transporte privado y de contar con acceso a internet desde un dispositivo con navegador web. Su principal motivación al usar SafeRoute es, precisamente, reducir la incertidumbre que genera no saber si sus hijos abordaron con seguridad, en qué parte del recorrido se encuentran o si ocurrió alguna novedad durante el viaje. Para dimensionar este segmento, según el Censo Educativo 2022-2023, en Lima Metropolitana existen aproximadamente 1.9 millones de estudiantes distribuidos en cerca de 7,602 instituciones educativas, de las cuales el 74% son de gestión privada (Ministerio de Educación, 2023). Esta alta proporción de colegios privados implica que una parte significativa de las familias limeñas depende de servicios externos de transporte escolar, dado que pocas instituciones cuentan con flotas propias.

- **Segmento 1: Transportistas Escolares**
  El segundo segmento está conformado por las personas o entidades que operan el servicio de transporte escolar privado. Dentro de este segmento conviven tres perfiles distintos. El primero corresponde a personas independientes que ofrecen el servicio de forma autónoma. El segundo agrupa a conductores que han sido asignados para operar una movilidad organizada por un conjunto de familias. El tercero engloba a los responsables de pequeñas empresas de transporte escolar que cuentan con una flota de vehículos y conductores a su cargo. A pesar de sus diferencias, todos comparten un factor común, pues operan sin herramientas digitales especializadas, apoyándose en métodos manuales e informales para gestionar una actividad que involucra directamente la seguridad de menores. La relevancia de este segmento se ve reflejada en que la cantidad de movilidades escolares autorizadas en Lima disminuyó en un 25% en solo un año, lo que evidencia un incremento en la informalidad del sector y, con ello, una mayor ausencia de mecanismos de control y monitoreo sobre el servicio que reciben los menores (Autoridad de Transporte Urbano para Lima y Callao, 2024). Adicionalmente, la Superintendencia de Transporte Terrestre de Personas, Carga y Mercancías ejecutó en 2024 campañas de sensibilización que alcanzaron a más de 47,000 escolares, lo que confirma que la seguridad en este sector continúa siendo una preocupación activa para las autoridades (SUTRAN, 2024). Por ello, la principal motivación de este segmento al usar SafeRoute es digitalizar y profesionalizar su operación, reducir los errores en la gestión de rutas y alumnos, y ofrecer a las familias que atienden una experiencia de servicio más confiable y transparente.

---

## Capítulo II: Requirements Elicitation & Analysis

### 2.1. Competidores

### Identificación de Competidores

En esta sección se describen los principales competidores (directos e indirectos) con modelos de negocio basados en productos digitales similares o servicios complementarios de monitoreo.

#### Life360
**Descripción:** Es una aplicación de rastreo familiar líder a nivel global que permite compartir la ubicación en tiempo real entre miembros de un grupo, así como recibir alertas de llegada y salida de lugares definidos. Está orientada a mejorar la seguridad y comunicación entre familias mediante funciones de geolocalización avanzada.

* **Enfoque:** Seguridad familiar general.
* **URL:** [https://www.life360.com/](https://www.life360.com/)

#### Find My Kids
**Descripción:** Es una aplicación de monitoreo parental diseñada para que los padres conozcan la ubicación en tiempo real de sus hijos mediante GPS. Permite revisar el historial de movimientos, escuchar el entorno en caso de emergencia y recibir alertas. Se destaca por su integración con relojes inteligentes (smartwatches) para niños.

* **Enfoque:** Monitoreo infantil y seguridad parental.
* **URL:** [https://findmykids.org/](https://findmykids.org/)

#### OnTrack School
**Descripción:** Es un sistema digital integral enfocado específicamente en la gestión y monitoreo del transporte escolar. Permite el seguimiento de vehículos en tiempo real, envío de notificaciones automáticas a los padres y control administrativo de rutas y conductores. Está orientado principalmente a instituciones educativas y flotas de transporte escolar.

* **Enfoque:** Gestión logística y transporte escolar corporativo.
* **URL:** [https://ontrack.global/school/](https://ontrack.global/school/)

---

### 2.1.1 Análisis Competitivo - Landscape

**¿Por qué llevar a cabo este análisis?**
El objetivo es contrastar SafeRoute con soluciones líderes de geolocalización familiar y gestión escolar, identificando oportunidades para posicionarnos como la herramienta preferida de los transportistas independientes en Lima que buscan profesionalizar su servicio.

| Categoría | Detalle | **SafeRoute** | **Life360** | **Find My Kids** | **OnTrack School** |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Perfil** | **Overview** | Gestión y monitoreo especializado en transporte escolar. | App de seguridad familiar y rastreo GPS general. | App de monitoreo infantil enfocada en smartwatches. | Plataforma integral de logística para transporte escolar. |
| **Perfil** | **Ventaja competitiva** | Roles específicos (Conductor/Padre) y flujo de abordaje manual. | Círculos familiares privados y detección de choques. | Escucha ambiental y compatibilidad con relojes GPS. | Optimización de rutas avanzada para flotas de colegios. |
| **Marketing** | **Mercado objetivo** | Padres y conductores independientes en Lima. | Familias con adolescentes y adultos mayores. | Padres con niños pequeños (5-12 años). | Colegios privados y empresas de transporte masivo. |
| **Marketing** | **Estrategias** | Seguridad digital y profesionalización del sector. | Marketing masivo de "Tranquilidad familiar". | Enfoque en seguridad infantil y prevención de extravíos. | Ventas corporativas (B2B) y eventos educativos. |
| **Producto** | **Productos & Servicios** | App, Dashboard Web, Alertas IoT y API para devs. | App móvil, asistencia en carretera y alertas de velocidad. | App móvil, rastreadores físicos y notificaciones SOS. | Software de logística, portal para padres y conductores. |
| **Producto** | **Precios & Costos** | Suscripción mensual ($9.99 - $49.99). | Freemium (Suscripciones Gold/Platinum desde $14.99). | Suscripción mensual o pago único de por vida. | Cotización personalizada por número de rutas/colegios. |
| **Producto** | **Canales de distribución**| Web (Landing Page) y tiendas de apps. | App Store, Play Store y web global. | App Store, Play Store y fabricantes de smartwatches. | Web corporativa y equipo de ventas directas. |
| **SWOT** | **Fortalezas** | Sistema especializado con control de abordaje y registro de incidencias para estructurar el servicio informal. | Alta precisión en rastreo en tiempo real . | Especialización en el segmento de niños pequeños. | Robustez técnica y algoritmos de optimización. |
| **SWOT** | **Debilidades** | Marca nueva en un mercado con desconfianza. | No está diseñada para el flujo de transporte escolar. | Funcionalidades limitadas si el niño no tiene reloj. | Costo elevado y difícil implementación para independientes. |
| **SWOT** | **Oportunidades** | Nicho desatendido de transportistas independientes en Perú que buscan organización y confianza. | Creciente preocupación por la seguridad familiar | Crecimiento del mercado de wearables infantiles. | Digitalización de colegios en mercados emergentes. |
| **SWOT** | **Amenazas** | Informalidad que prefiere usar solo WhatsApp. | Mejoras en los sistemas nativos de Google/Apple. | Regulaciones estrictas de privacidad infantil (COPPA). | Nuevas startups locales con precios de introducción bajos. |

---

### 2.1.2 Estrategias y tácticas frente a competidores

En base al análisis competitivo y SWOT realizado, SafeRoute plantea las siguientes estrategias y tácticas para diferenciarse aprovechando las debilidades de la competencia y el contexto local:

#### Enfoque en especialización del problema
- SafeRoute se posicionará como una solución especializada en transporte escolar, integrando funcionalidades específicas como control de abordaje, gestión de rutas y registro de incidencias.
- Esto permitirá cubrir necesidades logísticas que las soluciones genéricas de GPS ignoran.

#### Estrategia de digitalización del sector no estructurado
- Enfoque en transportistas independientes que actualmente dependen de WhatsApp y procesos manuales.
- Oferta de una plataforma simple e intuitiva para una transición digital sin fricciones técnicas.

#### Diferenciación por simplicidad y accesibilidad
- Priorización de facilidad de uso y costos accesibles frente a soluciones corporativas complejas como OnTrack School.
- Experiencia de usuario optimizada para minimizar la carga operativa del conductor durante el trayecto.

#### Estrategia de confianza y seguridad para padres
- Reducción de la incertidumbre mediante notificaciones automáticas de abordaje y alertas en tiempo real.
- Reemplazo de la comunicación informal por una estructura de datos confiable y profesional.

#### Estrategia de crecimiento progresivo (escalabilidad)
- Modelo de planes escalables (Básico, Intermedio, Completo) que acompaña el crecimiento de la flota del cliente.
- Facilita la adopción inicial con un ticket de entrada bajo.

#### Estrategia de posicionamiento local
- Adaptación a las dinámicas operativas y geográficas de Lima Metropolitana antes de escalar a otras ciudades del Perú.

#### Estrategia de preparación tecnológica futura
- Arquitectura preparada para la integración de sensores y cámaras IoT en etapas posteriores, garantizando competitividad a largo plazo.


### 2.2. Entrevistas

#### 2.2.1. Diseño de entrevistas

##### Guion de Entrevistas - Proyecto SafeRoute

###### **Segmento Objetivo 1: Conductor**

**Fase 1: Contexto del Usuario**
1. ¿Cuál es tu nombre?
2. ¿Cuál es tu edad?
3. ¿Podrías contarme un poco sobre tu entorno familiar? Por ejemplo, si vives con una familia o tienes hijos.
4. ¿En qué distrito o zona sueles trabajar?
5. ¿Podrías contarme un poco sobre tu trabajo como conductor de transporte escolar?
6. ¿Trabajas de manera independiente o en coordinación con otro grupo de personas o empresa?
7. En tu día a día, ¿qué herramientas o medios utilizas para organizar tu trabajo?

**Fase 2: Exploración del Problema**

8. Cuéntame cómo realizas normalmente el proceso de recoger y dejar a los alumnos.
9. Durante el recorrido, ¿cómo llevas el control de los alumnos?
10. ¿Qué suele pasar cuando ocurre algún cambio o imprevisto en la ruta?
11. ¿Cómo te comunicas con los padres durante el servicio?
12. ¿Qué partes de tu trabajo sientes que requieren más atención o te generan mayor carga?
13. ¿Qué tan organizado sientes que es tu proceso actual de trabajo?

**Fase 3: Exploración de Oportunidades**
> **Contexto:** Nuestro proyecto es una aplicación web que ayude a organizar y dar mayor visibilidad al servicio de transporte escolar, centralizando la información y comunicación.

14. Si pudieras mejorar algún aspecto de tu trabajo diario, ¿cuál sería y por qué?
15. ¿Qué tipo de información te ayudaría a sentir mayor control durante el recorrido?
16. ¿Qué preocupaciones tendrías al usar algún tipo de sistema durante el trayecto?
17. ¿Cómo te gustaría que fuera la comunicación con los padres para que no interfiera con tu conducción?
18. ¿Qué tendría que tener una herramienta así para que realmente la uses?
19. ¿Qué tan dispuesto estarías a usar una herramienta que te ayude a organizar y monitorear tu trabajo? ¿Por qué?

---

###### **Segmento Objetivo 2: Padre de Familia**

**Fase 1: Contexto del Usuario**
1. Para comenzar, ¿podrías indicarme tu nombre?
2. ¿Cuál es tu edad?
3. ¿En qué distrito o zona resides?
4. ¿Podrías contarme un poco sobre tu entorno familiar?
5. ¿Qué edades tienen tus hijos que utilizan transporte escolar?
6. ¿Qué rol cumple el transporte escolar dentro de tu día a día?
7. ¿Qué tan cómodo(a) te sientes utilizando tecnología en tu vida diaria?

**Fase 2: Exploración del Problema**

8. Cuéntame cómo haces actualmente para saber que tu hijo llegó bien a su destino.
9. ¿Qué es lo que más te preocupa cuando tu hijo está en el transporte escolar?
10. ¿Cómo te comunicas normalmente con el conductor o responsable del transporte?
11. ¿Recuerdas alguna situación en la que hayas sentido preocupación o falta de información? ¿Qué ocurrió?
12. ¿Qué tipo de información sientes que hoy no tienes y te gustaría tener?
13. ¿Qué aspectos del servicio de transporte actual te generan más desconfianza o incomodidad?

**Fase 3: Exploración de Oportunidades**
> **Contexto:** Nuestro proyecto es una aplicación web que ayude a organizar y dar mayor visibilidad al servicio de transporte escolar, centralizando la información y comunicación.

14. Si pudieras mejorar alguna parte del servicio de transporte escolar, ¿cuál sería y por qué?
15. ¿Qué opinas de una herramienta que te permita tener mayor visibilidad del transporte escolar de tu hijo?
16. ¿En qué aspectos crees que una solución así podría ayudarte en tu día a día?
17. ¿Qué preocupaciones tendrías al usar una herramienta digital para monitorear este servicio?
18. Para finalizar, ¿qué consideras indispensable para sentirte tranquilo(a) con el transporte de tu hijo?


#### 2.2.2. Registro de entrevistas

#### 2.2.3. Análisis de entrevistas

### 2.3. Needfinding

#### 2.3.1. User Personas

En esta sección se presentan los arquetipos de usuario diseñados para representar los segmentos objetivo de SafeRoute: el conductor de transporte escolar independiente y el padre de familia. 

La elaboración de estas fichas es el resultado de una síntesis detallada entre el análisis de la competencia y el proceso de Needfinding. Se han identificado características críticas como la alta dependencia de herramientas informales (WhatsApp/Llamadas), la ansiedad generada por la incertidumbre del tráfico en Lima y la necesidad de profesionalizar un sector mayoritariamente no estructurado.

###### **Segmento Objetivo 1: Conductor **
![UserPersona1](./assets/images/UserPerson1.png)

---
###### **Segmento Objetivo 2: Padre de Familia**
![UserPersona2](./assets/images/UserPersona2.png)

#### 2.3.2. User Task Matrix

En esta sección se presenta la matriz de tareas de usuario , la cual consolida las actividades fundamentales que tanto el conductor (Carlos Ramírez) como el padre de familia (Rosita Nery) ejecutan para asegurar un traslado escolar exitoso. 

Es importante destacar que estas tareas representan necesidades y procesos intrínsecos del servicio que existen independientemente de la existencia de una solución de software; el objetivo de SafeRoute es optimizar y digitalizar estas interacciones para reducir la carga operativa y la incertidumbre.

#### Cuadro: User Task Matrix

| Tarea (User Task) | Conductor - Frecuencia | Conductor - Importancia | Padre - Frecuencia | Padre - Importancia |
|:---|:---:|:---:|:---:|:---:|
| Verificar lista de asistencia de alumnos | Alta | Alta | N/A | N/A |
| Identificar alumnos en el punto de recojo | Alta | Alta | N/A | N/A |
| Confirmar el abordaje seguro del alumno | Alta | Crítica | Alta | Crítica |
| Gestionar comunicación entre conductores y padres | Alta | Alta | Alta | Alta |
| Notificar retrasos o imprevistos en la ruta | Media | Alta | Alta | Crítica |
| Monitorear el progreso del trayecto | Media | Media | Alta | Alta |
| Confirmar llegada al destino final | Alta | Crítica | Alta | Crítica |
| Registrar la entrega del alumno al responsable | Alta | Crítica | Alta | Crítica |
| Coordinar cambios de último momento en el servicio | Baja | Media | Baja | Alta |
| Reportar incidencias de seguridad o salud | Baja | Crítica | Baja | Crítica |
| Consultar el estado actual del servicio | Media | Media | Alta | Alta |
| Revisar historial de trayectos realizados | Baja | Media | Media | Media |
| Organizar y optimizar rutas y paradas | Alta | Alta | N/A | N/A |

---

#### Análisis y Explicación de la Matriz

Tras el análisis de la matriz, se desprenden las siguientes conclusiones clave sobre el comportamiento y necesidades de los segmentos:

* **Coincidencias en Tareas Críticas:** Existe una convergencia total en las tareas de "Confirmar abordaje", "Confirmar llegada" y "Registrar entrega". Para ambos segmentos, estas acciones representan la columna vertebral de la confianza en el servicio, manteniendo una importancia **Crítica** debido a que involucran la seguridad directa del menor.
* **Diferencias de Rol:** La carga operativa de planificación y ejecución (verificación de listas y organización de rutas) recae exclusivamente en el conductor. Por el contrario, el padre de familia se enfoca en tareas de supervisión pasiva como "Monitorear el progreso", que tiene una frecuencia alta debido a la ansiedad constante que genera el tráfico de la ciudad.
* **Gestión de Incidencias:** Se observa que tareas como "Reportar incidencias" tienen una frecuencia baja, pero su importancia es crítica. Esto valida la necesidad de que SafeRoute ofrezca canales de comunicación prioritarios que garanticen que, ante un imprevisto, la información fluya sin errores.
* **Fricción en la Comunicación:** La tarea de "Notificar retrasos" es de frecuencia media para el conductor pero de importancia crítica para el padre, lo que resalta el mayor punto de fricción actual: la necesidad de información en tiempo real para reducir el estrés parental.

#### 2.3.3. User Journey Mapping
En esta sección se presentan los User Journey Maps en versión As-Is correspondientes a los dos segmentos objetivo definidos previamente: conductor escolar y padre de familia. El propósito es comprender la experiencia actual del servicio de transporte escolar, identificando emociones, fricciones operativas, puntos críticos de comunicación y oportunidades de mejora antes de la implementación de SafeRoute.
A continuación, se presentan los diagramas detallados para cada User Persona, vinculando sus objetivos y puntos de dolor con las etapas del proceso actual.

User Journey Map: Carlos Ramírez (Conductor-Segmento Objetivo 1)
![UserJourneyMap1](./assets/images/UserJourneyMap-Carlos.png)
----
User Journey Map: Rosita Nery (Padre de Familia-Segmento Objetivo 2)
![UserJourneyMap2](./assets/images/UserJourneyMap-Rosita.png)

#### 2.3.4. Empathy Mapping
En esta sección se presenta el análisis de empatía realizado para nuestros segmentos objetivo buscando responder las preguntas ¿Con quién estamos empatizando? ¿Qué necesita hacer? ¿Qué está
diciendo? ¿Qué está viendo? ¿Qué está haciendo? ¿Qué está escuchando? ¿Cómo sesiente y qué piensa? E identificando sus Pains y Gains.

Segmento Objetivo 1: Conductor 
![EmpathyMapping1](./assets/images/EmpathyMapping-Carlos.png)

---
Segmento Objetivo 2: Padre de familia 
![EmpathyMapping2](./assets/images/EmpathyMapping-Rosita.png)

### 2.4. Big Picture Event Storming
En esta sección, se presenta el desarrollo y los resultados de la sesión de Big Picture Event Storming realizada por el equipo para el proyecto SafeRoute. Este proceso consistió en una sesión colaborativa de modelado dirigida al dominio, donde el equipo se enfocó en comprender el ecosistema del negocio de movilidad escolar de manera integral.

A través de esta dinámica, se logró plasmar los eventos significativos y sus interrelaciones, construyendo una primera aproximación visual de alto nivel que explora el landscape completo del negocio.

![BigPictureEventStorming](./assets/images/BigPictureEventStorming.jpg)
* **URL:** [[https://miro.com/](https://miro.com/app/board/uXjVGg_8JKU=/?share_link_id=308871936592)]

### 2.5. Ubiquitous Language
En esta sección se presenta el glosario de términos de negocio utilizados dentro del dominio de SafeRoute. 
| Term (English) | Término equivalente | Definición |
|:---|:---|:---|
| Student | Estudiante / Alumno | Menor de edad que utiliza el servicio de movilidad escolar para trasladarse entre su hogar y el centro educativo. |
| Parent | Padre / Apoderado | Persona responsable del estudiante que supervisa su traslado y recibe notificaciones del servicio. |
| Driver | Conductor | Persona encargada de operar el vehículo escolar y ejecutar la ruta asignada. |
| Vehicle | Vehículo | Unidad de transporte utilizada para movilizar estudiantes. |
| School Route | Ruta Escolar | Recorrido planificado con paradas definidas para recoger y entregar alumnos. |
| Daily Trip | Viaje Diario | Operación completa de traslado realizada en una jornada específica. |
| Return Trip | Ruta de Retorno | Trayecto de regreso desde el colegio hacia los domicilios. |
| Incident | Incidencia | Evento no planificado que afecta la operación normal del servicio. |
| Critical Incident | Incidencia Crítica | Situación grave que compromete seguridad, salud o continuidad del servicio. |
| Check-in | Confirmación de Entrada | Validación de que el estudiante ingresó correctamente al vehículo o al colegio. |
| Check-out | Confirmación de Salida | Validación de entrega del estudiante al responsable autorizado. |
| Notification | Notificación | Mensaje enviado al padre o conductor con información relevante del servicio. |
| Service Plan | Plan de Servicio | Modalidad comercial contratada por el cliente para acceder a SafeRoute. |
| Subscription | Suscripción | Vigencia activa del servicio contratado por el transportista o administrador. |
| Fleet | Flota | Conjunto de vehículos administrados por una misma operación. |
| Guardian | Tutor / Responsable | Persona autorizada para recibir al estudiante al final del trayecto. |
| No-show Student | Alumno Ausente | Estudiante programado que no aborda la unidad en el punto establecido. |

---

## Capítulo III: Requirements Specification

### 3.1. User Stories
Las siguientes User Stories representan los requisitos detallados del sistema SafeRoute, cubriendo la operación completa, la Landing Page y la API técnica.

| Epic / ID | Título | Descripción | Escenarios de Aceptación (Gherkin: 2 Positivos / 1 Negativo) | Relacionado con |
|:---|:---|:---|:---|:---|
| **E1** | **Gestión Administrativa** | Control de planes, usuarios y flota | | |
| US1 | Contratar Plan | Como administrador, quiero elegir un plan, para escalar mi operación. | **S1:** Given el admin elige "Plan Pro", When confirma pago, Then los límites de rutas se actualizan. <br> **S2:** Given un plan activo, When elige "Upgrade", Then se prorratea el pago. <br> **S3:** Given tarjeta sin fondos, When intenta contratar, Then se muestra "Error de transacción". | E1 |
| US2 | Registro de Conductores | Como administrador, quiero crear cuentas de conductores, para asignar responsabilidades. | **S1:** Given datos válidos, When guarda, Then perfil se crea. <br> **S2:** Given licencia subida, When sistema valida, Then estado cambia a "Verificado". <br> **S3:** Given DNI duplicado, When intenta guardar, Then muestra "Usuario ya existe". | E1 |
| US3 | Registro de Padres | Como administrador, quiero registrar a los padres, para habilitar el monitoreo. | **S1:** Given correo válido, When registra, Then envía invitación. <br> **S2:** Given vínculo con alumno, When confirma, Then habilita vista de mapa. <br> **S3:** Given correo inválido, When intenta enviar, Then muestra "Formato no soportado". | E1 |
| US4 | Alta de Alumnos | Como administrador, quiero registrar alumnos, para incluirlos en los recorridos. | **S1:** Given datos del menor, When guarda, Then aparece en lista de espera. <br> **S2:** Given foto subida, When guarda, Then se muestra en carné digital. <br> **S3:** Given campos vacíos, When intenta guardar, Then resalta campos obligatorios. | E1 |
| US5 | Creación de Rutas | Como administrador, quiero trazar rutas y paradas, para optimizar el tiempo. | **S1:** Given puntos A y B, When traza en mapa, Then calcula tiempo estimado. <br> **S2:** Given paradas nuevas, When agrega a ruta, Then recalcula orden óptimo. <br> **S3:** Given puntos inaccesibles, When intenta trazar, Then muestra "Ruta no transitable". | E1 |
| US6 | Asignación de Roles | Como administrador, quiero asignar conductores a rutas, para organizar la operación. | **S1:** Given conductor libre, When asigna a ruta X, Then conductor recibe alerta. <br> **S2:** Given cambio de unidad, When reasigna, Then se actualiza en tiempo real. <br> **S3:** Given conductor ya ocupado, When intenta asignar, Then muestra "No disponible". | E1 |
| US7 | Analítica de Flota | Como administrador, quiero ver reportes de rendimiento, para evaluar eficiencia. | **S1:** Given Plan Completo, When abre dashboard, Then muestra consumo de combustible. <br> **S2:** Given periodo mensual, When filtra, Then genera PDF de rendimiento. <br> **S3:** Given Plan Básico, When intenta abrir analítica, Then pide "Upgrade". | E1 |
| US8 | Gestión de Notificaciones | Como administrador, quiero enviar avisos globales, para informar eventos del colegio. | **S1:** Given evento imprevisto, When escribe mensaje global, Then todos los padres reciben push. <br> **S2:** Given aviso programado, When elige fecha, Then se envía automáticamente. <br> **S3:** Given mensaje vacío, When intenta enviar, Then el botón se bloquea. | E1 |
| US9 | Auditoría de Logs | Como administrador, quiero ver logs de sistema, para rastrear errores técnicos. | **S1:** Given fallo reportado, When busca en logs, Then identifica hora y usuario. <br> **S2:** Given exportar datos, When elige formato CSV, Then descarga el historial. <br> **S3:** Given usuario sin permisos, When intenta acceder, Then muestra "Acceso Denegado". | E1 |
| **E2** | **Operación del Conductor** | Herramientas para la ejecución del servicio | | |
| US10 | Inicio de Trayecto | Como conductor, quiero activar la ruta, para notificar a los padres. | **S1:** Given ruta lista, When pulsa "Iniciar", Then cambia estado a "En camino". <br> **S2:** Given GPS activo, When inicia, Then comienza transmisión de coordenadas. <br> **S3:** Given sin conexión, When intenta iniciar, Then muestra "Modo Offline: reconectando". | E2 |
| US11 | Marcación de Abordaje | Como conductor, quiero registrar el abordaje, para confirmar asistencia. | **S1:** Given parada alcanzada, When marca check, Then notifica al padre. <br> **S2:** Given código QR, When escanea al alumno, Then registra abordaje automático. <br> **S3:** Given alumno equivocado, When intenta marcar, Then alerta "Alumno no pertenece a esta parada". | E2 |
| US12 | Reporte de Incidencias | Como conductor, quiero informar problemas, para que el admin tome medidas. | **S1:** Given tráfico denso, When reporta retraso, Then actualiza ETA de todos los padres. <br> **S2:** Given falla mecánica, When selecciona tipo, Then avisa a central de auxilio. <br> **S3:** Given falta de GPS, When intenta reportar, Then pide ingreso manual de ubicación. | E2 |
| US13 | Botón de Pánico | Como conductor, quiero usar el SOS, para emergencias críticas. | **S1:** Given peligro, When presiona 3 seg, Then envía alerta con ubicación GPS. <br> **S2:** Given alerta activa, When admin responde, Then abre canal de audio. <br> **S3:** Given presión accidental, When cancela en 2 seg, Then no envía la alerta. | E2 |
| US14 | Finalización de Ruta | Como conductor, quiero cerrar la sesión, para concluir el turno. | **S1:** Given fin de recorrido, When pulsa "Cerrar", Then detiene GPS. <br> **S2:** Given alumnos pendientes, When intenta cerrar, Then advierte "Hay alumnos a bordo". <br> **S3:** Given error de servidor, When cierra, Then guarda datos localmente. | E2 |
| US15 | Bitácora de Viajes | Como conductor, quiero ver mi historial, para revisar recorridos pasados. | **S1:** Given menú historial, When selecciona día, Then muestra mapa del recorrido. <br> **S2:** Given resumen semanal, When consulta, Then indica horas totales manejadas. <br> **S3:** Given sin historial previo, When abre pestaña, Then muestra "Sin viajes registrados". | E2 |
| US16 | Navegación Integrada | Como conductor, quiero usar mapas externos, para ver la mejor ruta. | **S1:** Given viaje iniciado, When pulsa "Navegar", Then abre app externa. <br> **S2:** Given cambio de tráfico, When mapas sugiere desvío, Then el sistema actualiza el ETA. <br> **S3:** Given app de mapas no instalada, When intenta abrir, Then sugiere descarga. | E2 |
| US17 | Check de Seguridad | Como conductor, quiero una lista de chequeo, para revisar el bus antes de salir. | **S1:** Given inicio de día, When marca luces y frenos, Then habilita el inicio de ruta. <br> **S2:** Given falla detectada, When reporta en check, Then bloquea unidad por seguridad. <br> **S3:** Given check incompleto, When intenta iniciar viaje, Then recuerda "Revisión obligatoria". | E2 |
| **E3** | **Monitoreo y Seguridad (Padres)** | Visibilidad y tranquilidad para la familia | | |
| US18 | Rastreo en Tiempo Real | Como padre, quiero ver el bus en el mapa, para calcular la hora de llegada. | **S1:** Given viaje activo, When abre mapa, Then ve el icono moverse. <br> **S2:** Given parada propia, When toca icono, Then muestra distancia en KM. <br> **S3:** Given viaje finalizado, When abre mapa, Then muestra "Servicio concluido". | E3 |
| US19 | Alerta de Proximidad | Como padre, quiero recibir un aviso previo, para bajar a la parada a tiempo. | **S1:** Given bus a 500m, When entra a geovalla, Then recibe notificación push. <br> **S2:** Given bus a 2min, When tiempo se cumple, Then vibra el teléfono. <br> **S3:** Given notificaciones desactivadas, When bus llega, Then solo registra el evento en log. | E3 |
| US20 | Confirmación de Llegada | Como padre, quiero saber si mi hijo llegó al colegio, para estar tranquilo. | **S1:** Given bus en colegio, When conductor cierra viaje, Then recibe notificación de éxito. <br> **S2:** Given viaje de retorno, When llega a casa, Then recibe "Hijo entregado". <br> **S3:** Given retraso mayor a 20min, When tiempo pasa, Then recibe alerta de demora. | E3 |
| US21 | Acceso a Cámara | Como padre, quiero ver el interior del bus, para verificar la seguridad. | **S1:** Given Plan Intermedio, When solicita video, Then carga cámara en vivo. <br> **S2:** Given modo nocturno, When poca luz, Then activa visión infrarroja. <br> **S3:** Given fallo de internet, When carga video, Then muestra "Señal débil". | E3 |
| US22 | Historial de Asistencia | Como padre, quiero ver los días que mi hijo abordó, para control mensual. | **S1:** Given pestaña asistencia, When elige mes, Then muestra calendario con checks. <br> **S2:** Given falta justificada, When marca día, Then el sistema cambia icono a "Justificado". <br> **S3:** Given mes futuro, When intenta ver, Then la opción aparece bloqueada. | E3 |
| US23 | Perfil del Estudiante | Como padre, quiero gestionar datos médicos, para informar alergias al conductor. | **S1:** Given editar perfil, When escribe "Alergia a maní", Then el conductor ve alerta en su panel. <br> **S2:** Given foto actualizada, When sube imagen, Then se actualiza en el panel del bus. <br> **S3:** Given campo vacío, When intenta guardar, Then mantiene datos anteriores. | E3 |
| US24 | Chat con Soporte | Como padre, quiero un chat interno, para reportar ausencias. | **S1:** Given ausencia programada, When escribe al chat, Then el admin recibe el aviso. <br> **S2:** Given respuesta de soporte, When llega mensaje, Then se muestra notificación. <br> **S3:** Given mensaje fuera de hora, When envía, Then recibe respuesta automática. | E3 |
| **E4** | **Landing Page (Visitantes)** | Captación de clientes e Internacionalización (i18n) | | |
| US25 | Visualización de Hero | Como visitante, quiero ver la propuesta de valor, para entender SafeRoute. | **S1:** Given carga de URL, When ve sección principal, Then lee "Seguridad en cada ruta". <br> **S2:** Given botón CTA, When hace clic, Then lo lleva a Registro. <br> **S3:** Given fallo de carga, When URL es errónea, Then muestra página 404 personalizada. | E4 |
| US26 | Navegación de Funciones | Como visitante, quiero ver las funcionalidades, para conocer el alcance técnico. | **S1:** Given sección funciones, When hace scroll, Then ve iconos de monitoreo. <br> **S2:** Given tarjetas de info, When pasa el mouse, Then se expande la descripción. <br> **S3:** Given pantalla pequeña, When usa móvil, Then las funciones se apilan verticalmente. | E4 |
| US27 | Detalle de Roles | Como visitante, quiero conocer las vistas por perfil, para ver los beneficios. | **S1:** Given sección roles, When elige "Padre", Then muestra capturas de la App de padres. <br> **S2:** Given rol "Conductor", When elige, Then muestra gestión de rutas. <br> **S3:** Given opción no seleccionada, When ve la sección, Then muestra el rol "Admin" por defecto. | E4 |
| US28 | Consulta de Precios | Como visitante, quiero ver los costos, para evaluar mi presupuesto. | **S1:** Given tabla de precios, When elige "Anual", Then aplica 20% de descuento. <br> **S2:** Given moneda local, When cambia región, Then muestra precios en Soles (PEN). <br> **S3:** Given plan no disponible, When intenta ver, Then aparece etiqueta "Próximamente". | E4 |
| US29 | Sección "¿Cómo funciona?" | Como visitante, quiero ver los pasos iniciales, para saber cómo empezar. | **S1:** Given infografía, When sigue los pasos 1-5, Then entiende el flujo de contrato. <br> **S2:** Given video demo, When pulsa play, Then visualiza el funcionamiento real. <br> **S3:** Given navegador antiguo, When carga video, Then muestra imagen estática. | E4 |
| US30 | Implementación i18n | Como visitante, quiero cambiar el idioma (ES/EN), para navegar cómodamente. | **S1:** Given selector de idioma, When marca "English", Then todo el texto cambia a inglés. <br> **S2:** Given navegador en inglés, When carga sitio, Then se muestra en inglés por defecto. <br> **S3:** Given idioma no soportado, When detecta región, Then carga español por defecto. | E4 |
| US31 | Testimonios Reales | Como visitante, quiero leer reseñas, para confiar en la marca. | **S1:** Given sección testimonios, When desliza, Then ve fotos y opiniones de colegios. <br> **S2:** Given estrellas de calificación, When ve promedio, Then nota 4.8/5 de satisfacción. <br> **S3:** Given sin internet, When carga sección, Then muestra testimonios cacheados. | E4 |
| US32 | Formulario de Contacto | Como visitante, quiero enviar dudas, para recibir una cotización. | **S1:** Given formulario completo, When envía, Then recibe mensaje "Enviado con éxito". <br> **S2:** Given campos obligatorios, When intenta enviar vacío, Then marca errores en rojo. <br> **S3:** Given bot detectado, When envía spam, Then el Captcha bloquea el envío. | E4 |
| US33 | Suscripción al Newsletter | Como visitante, quiero dejar mi correo, para recibir tips de seguridad. | **S1:** Given campo de email, When ingresa dato, Then recibe correo de bienvenida. <br> **S2:** Given checkbox de privacidad, When marca "Acepto", Then habilita botón Suscribir. <br> **S3:** Given correo duplicado, When intenta registrar, Then dice "Ya estás suscrito". | E4 |
| US34 | Visualización de Partners | Como visitante, quiero ver marcas aliadas, para validar la seriedad del servicio. | **S1:** Given sección aliados, When carga logos, Then se ven marcas de seguros y seguridad. <br> **S2:** Given enlace en logo, When hace clic, Then abre web del partner. <br> **S3:** Given logo roto, When no carga imagen, Then muestra el nombre en texto. | E4 |
| US35 | Preguntas Frecuentes (FAQ) | Como visitante, quiero ver dudas comunes, para evitar llamadas de soporte. | **S1:** Given lista de FAQs, When toca una pregunta, Then se despliega la respuesta. <br> **S2:** Given buscador de FAQs, When escribe "precio", Then filtra preguntas relacionadas. <br> **S3:** Given duda no resuelta, When baja al final, Then ve botón de contacto directo. | E4 |
| US36 | Responsive Design i18n | Como visitante, quiero que el texto se ajuste en móvil, para evitar cortes por traducción. | **S1:** Given idioma Alemán (texto largo), When ve en móvil, Then el contenedor se expande. <br> **S2:** Given modo horizontal, When gira teléfono, Then el menú se ajusta al idioma. <br> **S3:** Given fuente muy grande, When el texto desborda, Then aplica elipsis automáticamente. | E4 |
| US37 | Blog de Seguridad | Como visitante, quiero leer artículos, para aprender sobre movilidad escolar. | **S1:** Given lista de posts, When elige uno, Then abre lectura completa. <br> **S2:** Given botones sociales, When comparte post, Then abre ventana de RRSS. <br> **S3:** Given post sin imagen, When carga, Then usa una imagen corporativa por defecto. | E4 |
| US38 | Demo Interactiva | Como visitante, quiero probar un simulador de mapa, para ver la experiencia real. | **S1:** Given mapa demo, When pulsa "Play", Then ve un bus moviéndose ficticiamente. <br> **S2:** Given alertas demo, When bus llega a punto, Then suena un aviso de prueba. <br> **S3:** Given navegador sin JS, When intenta ver demo, Then pide activar JavaScript. | E4 |
| US39 | SEO & Meta Tags i18n | Como visitante, quiero encontrar la web en buscadores, según mi idioma local. | **S1:** Given búsqueda en Google (ES), When escribe "Transporte Seguro", Then aparece SafeRoute. <br> **S2:** Given búsqueda en Google (EN), When escribe "Safe School Bus", Then aparece SafeRoute. <br> **S3:** Given link compartido, When pega URL, Then muestra preview con título traducido. | E4 |
| US40 | Verificación de SSL | Como visitante, quiero ver el candado de seguridad, para confiar mis datos. | **S1:** Given acceso a la web, When ve la barra de direcciones, Then aparece el prefijo HTTPS. <br> **S2:** Given envío de datos, When procesa formulario, Then viajan cifrados. <br> **S3:** Given certificado vencido, When entra, Then el navegador muestra aviso de "Sitio no seguro". | E4 |
| US41 | Chatbot de Ventas | Como visitante, quiero interactuar con un bot, para resolver dudas rápidas. | **S1:** Given duda sobre planes, When pregunta al bot, Then recibe respuesta del catálogo. <br> **S2:** Given intención de compra, When solicita asesor, Then el bot deriva a un humano. <br> **S3:** Given texto incoherente, When escribe, Then el bot ofrece opciones de menú fijas. | E4 |
| US42 | Política de Cookies i18n | Como visitante, quiero aceptar cookies, para cumplir con normativas legales. | **S1:** Given primera visita, When aparece el banner, Then puede elegir "Aceptar todas". <br> **S2:** Given idioma inglés, When ve el banner, Then los términos están en inglés. <br> **S3:** Given rechazo de cookies, When navega, Then solo carga las técnicas esenciales. | E4 |
| US43 | Soporte Multimoneda | Como visitante, quiero ver precios en mi moneda, para facilitar la comparación. | **S1:** Given geolocalización Perú, When ve precios, Then muestra en Soles (PEN). <br> **S2:** Given cambio manual a USA, When selecciona, Then muestra precios en Dólares (USD). <br> **S3:** Given moneda desconocida, When carga sitio, Then muestra precios en USD por defecto. | E4 |
| **E5** | **SafeRoute RESTful API** | Integraciones para desarrolladores | | |
| US44 | API: Obtener Alumnos | Como developer, quiero listar alumnos por ruta, para integraciones externas. | **S1:** Given GET `/students`, When token Admin, Then retorna JSON lista. <br> **S2:** Given filtro por ID, When consulta, Then retorna datos de 1 alumno. <br> **S3:** Given token expirado, When consulta, Then retorna 401 Unauthorized. | E5 |
| US45 | API: Registro GPS | Como developer, quiero enviar coordenadas, para actualizar la posición del bus. | **S1:** Given alta frecuencia, When envía 10 req/seg, Then el sistema procesa sin delay. <br> **S2:** Given coordenadas inválidas, When envía null, Then retorna 400 Bad Request. | E5 |


### 3.2. Impact Mapping
Segmento Objetivo 1: Carlos Ramirez, conductor
![ImpactMapping1](./assets/images/ImpactMap1.png)

---
Segmento Objetivo 2: Rosita Nery, padre de familia
![ImpactMapping2](./assets/images/ImpactMap2.png)
### 3.3. Product Backlog
# Product Backlog - SafeRoute

| Orden | User Story ID | Título | Descripción | Story Points |
|------:|---------------|--------|-------------|-------------|
| 1 | US25 | Visualización de Hero | Como visitante, deseo ver la propuesta de valor de SafeRoute para entender rápidamente el servicio. | 2 |
| 2 | US28 | Consulta de Precios | Como visitante, deseo ver los planes y precios para evaluar mi presupuesto. | 3 |
| 3 | US32 | Formulario de Contacto | Como visitante, deseo enviar mis datos para solicitar información o una demo comercial. | 3 |
| 4 | US29 | Sección ¿Cómo funciona? | Como visitante, deseo entender el proceso del servicio antes de contratar. | 2 |
| 5 | US31 | Testimonios Reales | Como visitante, deseo leer reseñas para confiar en la marca. | 2 |
| 6 | US30 | Implementación i18n | Como visitante, deseo cambiar idioma ES/EN para navegar cómodamente. | 5 |
| 7 | US1 | Contratar Plan | Como administrador, deseo elegir un plan para digitalizar y escalar mi operación. | 5 |
| 8 | US2 | Registro de Conductores | Como administrador, deseo crear cuentas de conductores para asignar responsabilidades. | 3 |
| 9 | US4 | Alta de Alumnos | Como administrador, deseo registrar alumnos para incluirlos en rutas. | 5 |
| 10 | US3 | Registro de Padres | Como administrador, deseo registrar padres para habilitar monitoreo. | 3 |
| 11 | US5 | Creación de Rutas | Como administrador, deseo crear rutas y paradas para optimizar tiempos. | 8 |
| 12 | US6 | Asignación de Roles | Como administrador, deseo asignar conductores a rutas para organizar operaciones. | 3 |
| 13 | US10 | Inicio de Trayecto | Como conductor, deseo iniciar la ruta para notificar que estoy en camino. | 3 |
| 14 | US11 | Marcación de Abordaje | Como conductor, deseo registrar el abordaje para confirmar asistencia. | 5 |
| 15 | US18| Rastreo en Tiempo Real | Como padre, deseo ver la movilidad en el mapa para calcular hora de llegada. | 8 |
| 16 | US19 | Alerta de Proximidad | Como padre, deseo recibir aviso cuando el vehículo esté cerca. | 5 |
| 17 | US20 | Confirmación de Llegada | Como padre, deseo saber si mi hijo llegó al colegio para estar tranquilo. | 3 |
| 18 | US14 | Finalización de Ruta | Como conductor, deseo cerrar la ruta para concluir el servicio. | 2 |
| 19 | US12 | Reporte de Incidencias | Como conductor, deseo informar retrasos o problemas durante la ruta. | 5 |
| 20 | US16 | Navegación Integrada | Como conductor, deseo abrir mapas externos para usar la mejor ruta disponible. | 3 |
| 21 | US7 | Analítica de Flota | Como administrador, deseo revisar métricas de rendimiento operativo. | 8 |
| 22 | US22 | Historial de Asistencia | Como padre, deseo revisar asistencia mensual de mi hijo. | 5 |
| 23 | US15 | Bitácora de Viajes | Como conductor, deseo consultar historial de viajes realizados. | 3 |
| 24 | US23 | Perfil del Estudiante | Como padre, deseo registrar alergias o datos médicos relevantes. | 5 |
| 25 | US24 | Chat con Soporte | Como padre, deseo reportar ausencias o dudas desde la app. | 5 |
| 26 | US13 | Botón de Pánico | Como conductor, deseo activar SOS en emergencias críticas. | 8 |


---

## Capítulo IV: Product Design

## 4.1. Style Guidelines

### 4.1.1. General Style Guidelines

El diseño de SafeRoute se fundamenta en decisiones visuales estratégicas destinadas a proyectar seguridad, fiabilidad y modernidad. El objetivo principal es construir una experiencia de usuario que genere confianza inmediata, tanto en los padres de familia que buscan tranquilidad como en los transportistas que necesitan eficiencia.

#### Colores
La selección cromática de SafeRoute no es meramente estética; responde a una psicología del color aplicada a la seguridad y el entorno escolar, garantizando accesibilidad y jerarquía visual. Cada tono desempeña una función específica en la interfaz:

![Foto de paleta de colores](assets/images/ChapterIV/paleta-colores.png)

- Azul Noche Profundo - #1A1A2E: Este color transmite autoridad, seriedad máxima y seguridad corporativa. En SafeRoute, se utiliza estratégicamente en el texto principal del logotipo y como fondo en secciones críticas de cierre, como el CTA final y el footer, para anclar la percepción de una plataforma robusta y confiable.

- Azul Marino - #1D3F6E y #16305a:Esta gama de azules medios y oscuros refuerza la percepción de una herramienta tecnológica, profesional y estable. Se emplean principalmente en títulos secundarios y elementos estructurales clave, estableciendo la jerarquía visual y la formalidad que el servicio requiere.

- Naranja Ámbar - #FFB74D: Este color funciona como el punto focal de acento y acción principal en SafeRoute, aportando vitalidad, energía y una conexión visual amigable con el entorno escolar. Se reserva exclusivamente para incentivar la acción en los botones de llamado a la acción principales y elementos destacados.

- Verde Éxito - #22C55E: Este color se asocia directamente con estados positivos, confirmación y seguridad. Se emplea de forma sutil en indicadores de estado (como el check en el mockup del teléfono) para validar acciones exitosas y reforzar la tranquilidad del usuario.

- Gris Neutro - #6B7280: Se ha seleccionado para el texto de cuerpo y párrafos largos. Ofrece una legibilidad excelente sobre fondos claros, reduciendo la fatiga visual y aportando un acabado limpio y moderno.

- Gris Claro y Neutral - #F8F9FB y #F4F7FA: Estos tonos muy claros se utilizan como fondos alternos para delimitar secciones (como el Hero, Planes o ¿Cómo funciona?). Su función es estructurar la página, proporcionando descansos visuales y una sensación de limpieza tecnológica y amplitud.

#### Tipografía

Se seleccionó la tipografía “Plus Jakarta Sans” como fuente principal para los títulos de la plataforma de SafeRoute por su estilo geométrico moderno y su capacidad para captar la atención del usuario con un toque tecnológico pero amigable. Se utiliza en pesos altos para asegurar que los encabezados sean visualmente impactantes, sólidos y de fácil lectura.

![Foto de ejemplo Jakarta Sans](assets/images/ChapterIV/ejemplo-jakarta.png)

Asimismo, optamos por la tipografía “DM Sans” como fuente secundaria para los textos de cuerpo y navegación por su diseño extremadamente legible, limpio y neutro. Su apariencia estética y claridad garantizan una experiencia de uso accesible y agradable, reduciendo la fatiga visual del usuario al leer información detallada sobre funciones o planes.

![Foto de ejemplo DM Sans](assets/images/ChapterIV/ejemplo-dm.png)

En cuanto al tamaño, se utiliza jerárquicamente en toda la página para resaltar títulos principales, botones de acción y texto de soporte. Los tamaños más grandes en los encabezados guían al usuario rápidamente por los puntos clave del mensaje, mientras que los más pequeños en los párrafos aseguran la comprensión y la eficiencia en la lectura de detalles secundarios.

#### Branding

El branding de SafeRoute está diseñado para reflejar simplicidad, confianza y profesionalismo. El logo y los íconos adoptan un enfoque minimalista, con líneas claras y formas simples que comunican el propósito de seguridad de la plataforma. El diseño incluye un símbolo que combina un escudo y un marcador de posición, representado de tal manera que simboliza protección y monitoreo con una apariencia limpia que es fácilmente reconocible, tanto en entornos web como móviles.

<img src="assets/images/ChapterIV/logo.jpeg" alt="Foto de logo" width="400px" />

#### Espaciado

El diseño de SafeRoute utiliza una estrategia de espacios en blanco diseñada para transmitir orden y claridad, factores críticos en una herramienta de seguridad escolar. En lugar de saturar la vista, aprovechamos márgenes amplios en los laterales de cada sección para que el usuario pueda diferenciar rápidamente entre los beneficios para padres, conductores y colegios. El contenido se mantiene estructurado mediante el uso de Flexbox y CSS Grid, lo que evita que la información se disperse y mantiene una jerarquía visual equilibrada que facilita la lectura de las características del servicio. Además, los rellenos (padding) en elementos como las tarjetas de planes y funciones garantizan una distribución adecuada del contenido.

#### Dimensiones para el tono de comunicación y lenguaje aplicado

En SafeRoute, definimos cuidadosamente el tono de nuestra comunicación para alinearlo con la misión de la plataforma: garantizar la seguridad y la tranquilidad en el transporte escolar para padres, conductores e instituciones educativas. Nuestro tono de voz busca proyectar confianza y control, combinando una comunicación clara, directa y altamente profesional.

Optamos por un tono formal pero empático, que permita a los padres de familia sentirse seguros al interactuar con funciones críticas como el monitoreo en vivo o las notificaciones de abordaje. Queremos que cada interacción refleje eficiencia para fomentar la puntualidad y el orden, pero también serenidad, asegurando que los usuarios sientan que el bienestar de los estudiantes es nuestra prioridad absoluta. Este equilibrio nos permite inspirar autoridad en la gestión logística, al tiempo que proyectamos cercanía y compromiso con la comunidad escolar.

Además, se han considerado los siguientes aspectos clave en el diseño de SafeRoute:

- Consistencia: La coherencia visual y textual es fundamental para brindar una experiencia confiable. Todos los elementos, desde los mensajes de estado hasta las etiquetas de los botones, mantienen una línea comunicativa uniforme. Esto facilita que los usuarios se familiaricen rápido con el sistema, algo vital en una operación diaria que requiere precisión.
- Navegación: La estructura ha sido pensada para ser lógica y sin fricciones. Los usuarios pueden acceder rápidamente a la información relevante según su rol, ya sea para verificar una ruta o reportar una incidencia. Los menús son minimalistas para evitar confusiones y optimizar el tiempo de respuesta en entornos dinámicos.
- Accesibilidad: La plataforma está optimizada para ser inclusiva y funcional en diversos contextos. Mediante el uso de etiquetas claras y un diseño responsivo, aseguramos que la información sea legible tanto para un administrador en una oficina como para un padre que revisa el celular en movimiento, garantizando una experiencia de uso fluida para todos.

#### Elementos de diseño

Además de los lineamientos generales sobre colores, tipografía y branding, en el diseño visual de SafeRoute se han aplicado de manera consciente diversos elementos fundamentales del diseño gráfico que enriquecen la experiencia del usuario y refuerzan la identidad de seguridad de la plataforma.

Uno de los elementos clave es la **línea**, utilizada sutilmente para separar secciones y delimitar las tarjetas de planes y roles, lo que organiza visualmente la interfaz y guía la lectura sin saturar al usuario. El **color** cumple un rol fundamental no solo en la identidad, sino en la comunicación funcional; la paleta incluye el azul noche para la autoridad, el naranja ámbar para la acción y el verde para confirmaciones, seleccionados por su capacidad para transmitir estados de seguridad y éxito.

En cuanto al **tamaño**, se utiliza jerárquicamente para resaltar títulos, botones y texto de soporte. Los tamaños más grandes en los encabezados captan la atención en puntos clave como el Hero, mientras que los más pequeños se emplean para detalles secundarios en las tarjetas de características, mejorando la comprensión y la eficiencia. Por su parte, la **textura** es limpia y moderna, gracias al uso de fondos suaves y superficies blancas que aportan una sensación de amplitud tecnológica sin distraer de las funciones de monitoreo.

El **espacio** es uno de los elementos más destacados del diseño de SafeRoute. Se han implementado márgenes amplios y rellenos generosos entre secciones, lo que permite una interfaz despejada y cómoda para padres y conductores. A nivel de **brillo** (value), se aplican contrastes claros que diferencian los botones de acción del fondo, guiando al usuario de forma intuitiva hacia la conversión.

Respecto a las **formas**, se ha optado por geometrías amigables con bordes redondeados en botones y tarjetas. Estos acabados suavizados no solo mejoran la estética profesional, sino que también transmiten una imagen de accesibilidad y cercanía, alineándose con una herramienta diseñada para el cuidado y protección escolar.

#### Principios de diseño

En cuanto a los principios de diseño, el **contraste** se emplea para asegurar que los elementos críticos, como los llamados a la acción (CTA) de "Ver planes" o las etiquetas de "Sistema en vivo", sean claramente visibles y resalten sobre los fondos neutros. Este principio es fundamental para la accesibilidad visual, permitiendo que tanto padres como conductores identifiquen los puntos de interacción más importantes de la plataforma de manera inmediata.

La **repetición** de colores como el azul noche y el naranja ámbar, junto con una iconografía coherente de escudos y mapas, refuerza la familiaridad y la consistencia del sistema visual. Al utilizar componentes visuales recurrentes en toda la landing, los usuarios comprenden rápidamente la función de cada sección, lo que reduce la curva de aprendizaje al interactuar con las herramientas de monitoreo.

La **alineación** contribuye a la profesionalidad y solidez del diseño: la estructura de la página, los listados de roles y las tarjetas de precios mantienen una disposición coherente lograda mediante el uso de Flexbox y CSS Grid. Esta organización clara y alineada facilita una navegación intuitiva, transmitiendo el orden necesario para una plataforma de gestión logística.

Por último, el principio de **proximidad** agrupa de manera lógica los elementos relacionados, como los iconos de las funciones con sus respectivas descripciones o los beneficios específicos para cada rol. Al mantener los elementos vinculados cerca entre sí, se mejora significativamente la lectura y la comprensión de cada bloque de información, permitiendo que el usuario asocie rápidamente las soluciones de SafeRoute con sus necesidades específicas.

Estos elementos y principios no se aplican de forma aislada, sino como parte integral de un sistema visual que busca ser funcional, estético y coherente con la misión de SafeRoute: digitalizar y dar seguridad al transporte escolar a través de una experiencia clara, confiable y eficiente.

### 4.1.2. Web Style Guidelines

El diseño web de SafeRoute está optimizado para proporcionar una experiencia de usuario fluida y profesional, centrada en la legibilidad y la facilidad de navegación. Se emplean estructuras de contenedores flexibles que permiten que el contenido se organice de manera clara, utilizando amplios espacios en blanco para evitar la saturación visual y garantizar la accesibilidad de la información crítica sobre seguridad. Los elementos visuales, como tarjetas de planes y secciones de roles, mantienen proporciones equilibradas para guiar la vista del usuario de forma jerárquica.

En cuanto a la interactividad, la plataforma utiliza una lógica de componentes claramente identificables. Los botones de acción (CTAs) emplean colores contrastantes y estados visuales (como hover y active) que ofrecen una retroalimentación inmediata, reforzando la confianza del usuario al interactuar con el sistema. La navegación se apoya en transiciones suaves y menús persistentes que aseguran que las herramientas principales, como el sistema de internacionalización (i18n), estén siempre al alcance del usuario, facilitando un flujo de trabajo intuitivo y eficiente dentro de la landing page.

![Mockup Landing Page](assets/images/ChapterIV/Landing/Mock-ups/mockup_landingPage.png)
![Mockup Planes](assets/images/ChapterIV/Landing/Mock-ups//mockup_planes.png)
![Mockup footer](assets/images/ChapterIV/Landing/Mock-ups//mockup_footer.png)

_Nota_: Elaboración propia.

## 4.2. Information Architecture

### 4.2.1. Organization Systems

En el sistema SafeRoute, se emplea la organización jerárquica (visual hierarchy) para destacar información crítica, como el mapa de monitoreo en tiempo real, las alertas de emergencia y las notificaciones de abordaje de los alumnos en los dashboards principales. Esta jerarquía visual permite que tanto padres como conductores identifiquen de forma inmediata los datos más relevantes según el contexto operativo, relegando datos secundarios del perfil a niveles inferiores.

Asimismo, se aplica una organización secuencial (step-by-step) en procesos que requieren una guía estructurada. En la landing page, este sistema se evidencia en la sección "¿Cómo funciona?", donde se orienta al visitante a través de 5 pasos para la adopción del servicio. En la Web Application, este esquema se utilizará para el flujo de registro de paradas y asistencia que el conductor debe seguir durante su ruta, asegurando una progresión lógica que minimice errores de registro.

Respecto a los esquemas de categorización, no se utilizan organizaciones alfabéticas o matriciales complejas. En su lugar, se emplea una organización cronológica para la visualización de datos históricos, permitiendo que los padres de familia revisen los registros pasados de asistencias y llegadas de sus hijos de manera ordenada por fecha y hora. Además, el contenido se clasifica según audiencia, segmentando las interfaces y funcionalidades de acuerdo con los dos User Personas identificados: Conductores, enfocados en la gestión de ruta y paradas, y Padres de Familia, orientados al monitoreo y recepción de avisos de seguridad.

### 4.2.2. Labeling Systems

El sistema de etiquetado de SafeRoute ha sido desarrollado bajo un criterio de funcionalidad operativa, buscando que cada término actúe como una señal clara que reduzca el esfuerzo cognitivo de los usuarios. Se han seleccionado etiquetas descriptivas que permiten una navegación intuitiva tanto en el proceso de descubrimiento (Landing Page) como en el uso crítico de la aplicación (Web Application).

**Landing Page**

  - **Funciones**: Agrupa las capacidades técnicas y herramientas de gestión de la plataforma.
  - **Roles**: Define los accesos y beneficios específicos para los dos perfiles del sistema.
  - **Planes**: Estructura la oferta comercial basándose en la escala de la flota de transporte.
  - **¿Cómo funciona?**: Etiqueta de apoyo que resuelve dudas sobre la implementación del servicio.
  - **Comenzar**: Botón de acción principal diseñado para motivar la conversión inmediata.

**Aplicación Web – Conductores**

  - **Mis Rutas**: Vista principal donde se gestionan los trayectos diarios asignados.
  - **Lista de Alumnos**: Relación detallada de estudiantes por paradas, optimizando el tiempo de recogida.
  - **Estado de Abordaje**: Sistema de etiquetas rápidas ("Abordado", "Ausente", "En espera") que permite al conductor registrar la asistencia con un solo toque.
  - **Iniciar Ruta**: Etiqueta de alta visibilidad que dispara el envío de alertas GPS a los padres.
  - **Botón de Incidencia**: Acceso directo para reportar eventos imprevistos (tráfico, accidentes) de forma estandarizada.

**Aplicación Web – Padres de Familia**

  - **Monitoreo**: Sección central que integra el mapa en tiempo real y la ubicación de la unidad.
  - **Historial de Viajes**: Registro cronológico de las horas de recogida y entrega de sus hijos.
  - **Alertas**: Centro de notificaciones sobre la proximidad del bus o confirmaciones de llegada.
  - **Datos del Bus**: Información transparente sobre el vehículo y el conductor asignado para generar confianza.

### 4.2.3. SEO Tags and Meta Tags

1. **Landing Page**

**Charset**

  `<meta charset="UTF-8" />`

Esta línea establece la codificación universal de caracteres. Su función es garantizar que el navegador interprete correctamente los textos del sistema i18n, asegurando que tildes, la letra "ñ" y símbolos especiales se visualicen sin errores en español e inglés, evitando una mala experiencia de lectura.

**Viewport (Responsive)**

  `<meta name="viewport" content="width=device-width, initial-scale=1.0"/>`

Controla el escalado de la página en diferentes dispositivos. Su función es hacer que la landing sea responsiva, ajustando el ancho del contenido al tamaño de la pantalla. Esto es vital para que los padres de familia visualicen la información de manera legible desde sus smartphones.

**Title (SEO)**
  
  `<title>SafeRoute — Transporte Escolar Seguro</title>`

Define el título que aparece en la pestaña del navegador y en los resultados de búsqueda. Su función es proporcionar una identificación inmediata de la marca y su propósito principal, siendo un factor crítico para el posicionamiento orgánico.

**Meta Description (SEO)**

  `<meta name="description" content="Plataforma integral para el monitoreo en tiempo real, control de asistencia y comunicación segura entre conductores y padres de familia.">`

Provee un resumen conciso del contenido del sitio. Su función es aparecer como el fragmento de texto (snippet) en Google, atrayendo a los usuarios al explicar claramente cómo SafeRoute resuelve la inseguridad en el transporte escolar.

**Meta Keywords (SEO)**

  `<meta name="keywords" content="transporte escolar, monitoreo GPS, seguridad, SafeRoute, logística escolar, app bilingüe">`

Especifica palabras clave relevantes para la temática de la página. Su función es ayudar a los algoritmos de indexación a clasificar el sitio dentro del nicho de tecnología de transporte y seguridad educativa.

**Meta Author**

  `<meta name="author" content="FiveTech Team">`
Identifica formalmente a los creadores de la plataforma. Su función es atribuir la autoría del proyecto al equipo de FiveTech, vinculando el desarrollo técnico con el startup responsable.

**Meta Copyright**

  `<meta name="copyright" content="FiveTech 2026">`

Esta línea establece legalmente la propiedad intelectual de la página. Su función es indicar la titularidad de los derechos de autor y el año de vigencia, protegiendo el contenido y diseño del sitio.

**Meta Robots**

  `<meta name="robots" content="index, follow">`

Instruye a los motores de búsqueda sobre cómo tratar el sitio. Su función es permitir que los "robots" incluyan la página en sus índices y sigan los enlaces internos, lo cual es fundamental para el crecimiento del tráfico hacia la plataforma.

**Meta Language**

  `<html lang="en">`

Declara el idioma principal de la estructura del sitio. Su función es informar a los navegadores y buscadores que el texto base está en ingles, mejorando la segmentación del público objetivo internacionalmente.

### 4.2.4. Searching Systems

En esta sección se describen los mecanismos de asistencia y recuperación de información diseñados para SafeRoute. El objetivo primordial es evitar la desorientación del usuario ante el flujo constante de datos logísticos, garantizando que la información sobre rutas y alumnos sea accesible de manera inmediata.

**Vista del Conductor / Dueño de Unidad**

**1. Medios de ayuda para la búsqueda de datos**

  - Barra de búsqueda operativa: Ubicada en los módulos de "Rutas" y "Lista de Alumnos" para acceso rápido.
  - Autocompletado inteligente: Sugiere nombres de alumnos o puntos de parada conforme el conductor escribe, facilitando la operación en dispositivos móviles.
  - Mensajes contextuales: En caso de no hallar un registro, el sistema ofrece opciones como "¿Desea registrar un nuevo alumno en esta parada?".
  - Búsqueda por proximidad: Sugerencia automática de la siguiente parada basada en la ubicación GPS actual.

**2. Filtros y opciones**

  - Por Nombre del Alumno: Localización directa de la ficha de contacto y datos de emergencia.
  - Por Estado de Asistencia: Filtrado rápido de alumnos "Abordados", "Pendientes" o "Ausentes".
  - Por Punto de Parada: Visualización de todos los estudiantes vinculados a un hito específico de la ruta.
  - Por Turno: Filtrado entre rutas de "Recojo" (mañana) y "Retorno" (tarde).

**3. Visualización de resultados**

  - Tarjetas de Alumno (Cards): Incluyen foto, nombre, grado y una etiqueta de estado de alta visibilidad.
  - Indicadores de Color:
      - Amarillo: Alumno en espera.
      - Verde: Alumno ya abordó la unidad.
      - Rojo: Alumno reportado como ausente.
  - Acciones rápidas: Botones directos para "Marcar Asistencia", "Llamar a Apoderado" o "Reportar Incidencia".

**Vista del Padre de Familia**

**1. Medios de ayuda para la búsqueda de datos**

  - Buscador de historial: Permite localizar eventos específicos dentro de la bitácora de viajes del alumno.
  - Sugerencias por fecha: Calendario interactivo para seleccionar días específicos de consulta.
  - Acceso directo a Unidad: Buscador para identificar los datos del bus asignado mediante la placa o nombre del conductor.

**2. Filtros y opciones**

  - Por Fecha: Consulta de registros de asistencia de días o meses anteriores.
  - Por Tipo de Evento: Filtrado entre "Notificaciones de Proximidad", "Confirmación de Abordaje" y "Llegada al Destino".
  - Por Estado del Viaje: Filtrado entre rutas "Completadas", "En curso" o "Canceladas".

**3. Visualización de resultados**

  - Timeline de Eventos: Lista cronológica detallada con la hora exacta de cada suceso.
  - Mapa de Resultados: Al buscar un historial, se muestra el trazado que siguió la unidad en esa fecha específica.
  - Colores de Estado:

      - Check Verde: Evento completado con éxito.
      - Reloj Naranja: Retraso reportado en el punto de entrega.
      - Círculo Rojo: Registro de inasistencia justificada.


### 4.2.5. Navigation Systems

La navegación en SafeRoute ha sido diseñada para ser intuitiva y guiada mediante componentes de interfaz que permiten a los usuarios gestionar la seguridad del transporte de forma fluida y sin fricciones. En la landing page, se utiliza un sistema de desplazamiento vertical (smooth scroll) que permite explorar de forma narrativa los beneficios, los roles de usuario y los planes de suscripción, guiando al visitante estratégicamente hacia los llamados a la acción (CTAs) para el contacto. Esta navegación se apoya en una barra superior persistente (Sticky Nav) que incluye un selector de idioma (i18n), permitiendo cambiar el contexto lingüístico en cualquier punto del recorrido.

Dentro de la aplicación web, la navegación principal se organiza mediante una barra lateral fija (Sidebar) que otorga acceso inmediato a las secciones críticas: Monitoreo en Tiempo Real, Lista de Alumnos, Historial de Rutas, Alertas de Seguridad y Configuración de Perfil. Este diseño permite que, por ejemplo, un conductor pueda alternar entre su hoja de ruta y el reporte de incidencias con un solo toque, manteniendo siempre la visibilidad del estado del viaje.

La experiencia de navegación también se adapta dinámicamente según el tipo de usuario. Los Padres de Familia acceden a una vista simplificada centrada en el mapa y las notificaciones de sus hijos, mientras que los Conductores disponen de controles operativos más robustos. El uso de pestañas (tabs) y botones de acción rápida dentro de cada módulo asegura que el usuario pueda ejecutar tareas específicas, como marcar la asistencia o llamar a un apoderado, sin perder el contexto de la ruta activa, garantizando un flujo de trabajo coherente con la naturaleza crítica del servicio.

## 4.3. Landing Page UI Design

### 4.3.1. Landing Page Wireframe

A continuación, se presentan los wireframes de las principales secciones de la landing page. Cada imagen ilustra el diseño propuesto para las diferentes funcionalidades, flujos de navegación y elementos de interacción de la plataforma.

**Principios Aplicados**

- **Jerarquía visual clara:** Los contenidos se ordenan priorizando la información de confianza en el Hero Section (Seguridad y Gestión). Se guía al usuario progresivamente a través de las estadísticas de impacto, los beneficios específicos para padres y conductores, la tabla comparativa de planes y, finalmente, el tutorial operativo.

- **Consistencia visual:** Se mantuvieron patrones uniformes utilizando la tipografía Plus Jakarta Sans para títulos impactantes y DM Sans para la legibilidad del cuerpo. Se aplicó la paleta institucional (azul marino para seguridad y ámbar para alertas) de manera coherente en todos los componentes.

- **Contraste y accesibilidad:** Se garantizó un contraste elevado entre el texto y los fondos para facilitar la lectura en condiciones de luz exterior (común para conductores y padres en ruta). Los botones de acción cuentan con estados visuales claros para confirmar la interacción del usuario.

- **Optimización para dispositivos móviles:** Los wireframes y el diseño final contemplan una navegación móvil dedicada. Se implementó un menú lateral (sidebar) activado por un botón hamburguesa para ahorrar espacio, se ajustaron las cuadrículas (grids) a una sola columna para evitar el desplazamiento horizontal y se optimizaron las áreas de contacto en botones para una interacción táctil precisa.

- **Diseño inclusivo:** La estructura es totalmente compatible con el sistema i18n, permitiendo que el diseño se adapte dinámicamente al largo de las palabras en español e inglés. Además, se aseguró que la navegación sea lógica y accesible mediante teclado y lectores de pantalla, facilitando el uso para cualquier tipo de usuario.

##### Versión Desktop Web Browser:

En esta primera sección se presenta la pantalla Home de la landing page, donde se observa el encabezado principal con la propuesta de valor y el acceso al sistema de internacionalización (i18n). Se aprecia un botón call-to-action principal diseñado para captar el interés de los padres de familia y conductores independientes.

<img src="assets/images/ChapterIV/Landing/Wireframes/wireframe-LP1.png" alt="Home SafeRoute" width="900px">

A continuación, se muestra la Sección de Características, donde se detallan los pilares y eficiencia que sustentan la plataforma SafeRoute, utilizando iconos y textos breves para una lectura rápida.

<img src="assets/images/ChapterIV/Landing/Wireframes/wireframe-LP2.png" alt="Características SafeRoute" width="900px">

Se presenta la sección de Funcionalidades, la cual profundiza en las capacidades tecnológicas del sistema, como el monitoreo en tiempo real y las notificaciones automáticas.

<img src="assets/images/ChapterIV/Landing/Wireframes/wireframe-LP3.png" alt="Funcionalidades" width="900px">

El siguiente frame corresponde a los Roles del Sistema, donde se segmentan los beneficios específicos para cada usuario objetivo: los padres de familia, enfocados en la tranquilidad y el seguimiento, y los conductores, enfocados en la gestión operativa de la ruta.

<img src="assets/images/ChapterIV/Landing/Wireframes/wireframe-LP4.png" alt="Roles SafeRoute" width="900px">

Se presenta la sección de Planes, donde se muestra la estructura de precios y niveles de servicio, diseñada de forma escaneable para facilitar la toma de decisiones.

<img src="assets/images/ChapterIV/Landing/Wireframes/wireframe-LP5.png" alt="Planes SafeRoute" width="900px">

A continuación, se detalla el flujo de uso del sistema en la sección "¿Cómo funciona?". Este tutorial visual guía al nuevo usuario a través de los pasos necesarios para implementar la plataforma con éxito.

<img src="assets/images/ChapterIV/Landing/Wireframes/wireframe-LP6.png" alt="Tutorial SafeRoute" width="900px">

Finalmente, se presenta la sección de Footer, la cual incluye el cierre de la página con los créditos correspondientes al equipo de desarrollo de FiveTech.

<img src="assets/images/ChapterIV/Landing/Wireframes/wireframe-LP7.png" alt="Footer SafeRoute" width="900px">

#### Versión Mobile Web Browser

A continuación, se presenta la adaptación responsiva de SafeRoute para dispositivos móviles. En estas vistas se observa la reorganización de los elementos en una estructura vertical y el uso de componentes optimizados para la interacción táctil.

Pantalla Home y Menú Lateral (Sidebar):
Se muestra la adaptación del Hero Section y el funcionamiento del menú hamburguesa, el cual despliega una barra lateral para facilitar la navegación en pantallas pequeñas sin obstruir el contenido.

<img src="assets/images/ChapterIV/Landing/Wireframes/wireframe-mobile-1.png" alt="Home Mobile" width="700px">

Secciones de Características y Funcionalidades en Móvil:
Los pilares de seguridad y las capacidades tecnológicas del sistema se reorganizan en una sola columna. Esto permite que los iconos y textos descriptivos mantengan un tamaño adecuado para la lectura táctil, evitando que el usuario deba realizar zoom para comprender las funciones de monitoreo y alertas.

<img src="assets/images/ChapterIV/Landing/Wireframes/wireframe-mobile-2.png" alt="Características y Funcionalidades Mobile" width="800px">

Sección de Roles del Sistema en Móvil:
Se adapta la segmentación de beneficios para padres y conductores mediante un flujo vertical. Cada rol se presenta de forma independiente para asegurar que el impacto visual de los beneficios específicos no se pierda en pantallas de dimensiones reducidas.
 
<img src="assets/images/ChapterIV/Landing/Wireframes/wireframe-mobile-3.png" alt="Roles Mobile" width="700px">

Planes, Tutorial y Footer Móvil:
La tabla de precios se transforma en tarjetas individuales desplazables de arriba hacia abajo, seguida del flujo paso a paso del tutorial. El cierre de página se optimiza para mostrar los créditos de FiveTech de manera compacta al final del recorrido del usuario.

<img src="assets/images/ChapterIV/Landing/Wireframes/wireframe-mobile-4.png" alt="Planes y Footer Mobile" width="1000px">

### 4.3.2. Landing Page Mock-up

A continuación, se presentan los mock-ups de las principales secciones de la landing page. Cada imagen ilustra el diseño propuesto para las diferentes funcionalidades, flujos de navegación y elementos de interacción de la plataforma.

En esta primera sección se presenta la pantalla Home de la landing page, donde se observa el encabezado principal con la propuesta de valor y el acceso al sistema de internacionalización (i18n). Se aprecia un botón call-to-action principal diseñado para captar el interés de los padres de familia y conductores independientes.

<img src="assets/images/ChapterIV/Landing/Mock-ups/mockup-LP1.png" alt="Home SafeRoute" width="900px">

A continuación, se muestra la Sección de Características, donde se detallan los pilares y eficiencia que sustentan la plataforma SafeRoute, utilizando iconos y textos breves para una lectura rápida.

<img src="assets/images/ChapterIV/Landing/Mock-ups/mockup-LP2.png" alt="Características SafeRoute" width="900px">

Se presenta la sección de Funcionalidades, la cual profundiza en las capacidades tecnológicas del sistema, como el monitoreo en tiempo real y las notificaciones automáticas.

<img src="assets/images/ChapterIV/Landing/Mock-ups/mockup-LP3.png" alt="Funcionalidades" width="900px">

El siguiente frame corresponde a los Roles del Sistema, donde se segmentan los beneficios específicos para cada usuario objetivo: los padres de familia, enfocados en la tranquilidad y el seguimiento, y los conductores, enfocados en la gestión operativa de la ruta.

<img src="assets/images/ChapterIV/Landing/Mock-ups/mockup-LP4.png" alt="Roles SafeRoute" width="900px">

Se presenta la sección de Planes, donde se muestra la estructura de precios y niveles de servicio, diseñada de forma escaneable para facilitar la toma de decisiones comerciales.

<img src="assets/images/ChapterIV/Landing/Mock-ups/mockup-LP5.png" alt="Planes SafeRoute" width="900px">

A continuación, se detalla el flujo de uso del sistema en la sección "¿Cómo funciona?". Este tutorial visual guía al nuevo usuario a través de los pasos necesarios para implementar la plataforma con éxito.

<img src="assets/images/ChapterIV/Landing/Mock-ups/mockup-LP6.png" alt="Tutorial SafeRoute" width="900px">

Finalmente, se presenta la sección de Footer, la cual incluye el cierre de la página con los créditos correspondientes al equipo de desarrollo de FiveTech.

<img src="assets/images/ChapterIV/Landing/Mock-ups/mockup-LP7.png" alt="Footer SafeRoute" width="900px">

#### Versión Mobile Web Browser

A continuación, se presentan los mock-ups de la versión móvil de la aplicación. Cada imagen muestra la adaptación responsiva de las principales funcionalidades y secciones diseñadas para ofrecer una experiencia de usuario optimizada en dispositivos móviles.

Pantalla Home y Menú Lateral (Sidebar):
Se muestra la adaptación del Hero Section y el funcionamiento del menú hamburguesa, el cual despliega una barra lateral para facilitar la navegación en pantallas pequeñas sin obstruir el contenido.

<img src="assets/images/ChapterIV/Landing/Mock-ups/mockup-mobile-1.png" alt="Home Mobile" width="700px">

Secciones de Características y Funcionalidades en Móvil:
Los pilares de seguridad y las capacidades tecnológicas del sistema se reorganizan en una sola columna. Esto permite que los iconos y textos descriptivos mantengan un tamaño adecuado para la lectura táctil, evitando que el usuario deba realizar zoom para comprender las funciones de monitoreo y alertas.

<img src="assets/images/ChapterIV/Landing/Mock-ups/mockup-mobile-2.png" alt="Características y Funcionalidades Mobile" width="800px">

Sección de Roles del Sistema en Móvil:
Se adapta la segmentación de beneficios para padres y conductores mediante un flujo vertical. Cada rol se presenta de forma independiente para asegurar que el impacto visual de los beneficios específicos no se pierda en pantallas de dimensiones reducidas.
 
<img src="assets/images/ChapterIV/Landing/Mock-ups/mockup-mobile-3.png" alt="Roles Mobile" width="700px">

Planes, Tutorial y Footer Móvil:
La tabla de precios se transforma en tarjetas individuales desplazables de arriba hacia abajo, seguida del flujo paso a paso del tutorial. El cierre de página se optimiza para mostrar los botones de contacto y los créditos de FiveTech de manera compacta y accesible al final del recorrido del usuario.

<img src="assets/images/ChapterIV/Landing/Mock-ups/mockup-mobile-4.png" alt="Planes y Footer Mobile" width="1000px">

## 4.4. Web Applications UX/UI Design

### 4.4.1. Web Applications Wireframes

Los siguientes wireframes representan la arquitectura visual de la aplicación web de SafeRoute, diseñada para centralizar la gestión de seguridad y logística del transporte escolar.

#### Principios aplicados

- Jerarquía funcional clara: El flujo de navegación prioriza las acciones críticas para la seguridad, como el acceso al mapa de rastreo en vivo y la gestión de alertas de pánico.

- Consistencia y patrones de diseño: Se mantiene la uniformidad visual en componentes de formularios y tablas de datos, asegurando una curva de aprendizaje mínima para todos los usuarios.

- Accesibilidad en interfaces: Se implementaron contrastes elevados y fuentes legibles (Plus Jakarta Sans), facilitando el uso en dispositivos móviles y de escritorio.

- Diseño adaptativo: El diseño es responsivo, permitiendo que la plataforma sea funcional tanto en estaciones de monitoreo (Desktop) como en tablets de conductores.

#### Versión Desktop Wireframes - Acceso y Configuración (Universal)

##### Autenticación y Acceso

Registro de Cuenta
Pantalla unificada de registro donde el usuario selecciona su rol (Padre, Conductor o Administrador) y completa sus datos básicos. Es el punto de partida para que cualquier actor del sistema pueda interactuar con la plataforma.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/universalregister.png" width="900px" alt="register">

Inicio de Sesión (Login) Interfaz de acceso donde los usuarios ingresan sus credenciales. El sistema valida el rol del usuario y lo redirige automáticamente a su panel de control correspondiente.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/universallogin.png" width="900px" alt="login">

Cambio de Contraseña Formulario de seguridad que permite restablecer el acceso mediante la verificación de identidad tras un código, garantizando que solo el propietario de la cuenta pueda modificar sus credenciales.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/password-change1.png" width="900px" alt="password-change">
<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/password-change2.png" width="900px" alt="password-change">
<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/password-change3.png" width="900px" alt="password-change">

#### Versión Desktop Wireframes - Administradores 

##### Configuración y Gestión Administrativa

Panel de Inicio y Navegación (US20)

Dashboard central que organiza todos los módulos del sistema a través de un sidebar lateral, facilitando el salto entre la gestión de rutas, alumnos y reportes.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/home-dashboard.png" width="900px" alt="home-dashboard">

Asignación de Roles (US6)

Módulo exclusivo para el administrador donde se definen los permisos específicos de cada usuario registrado, garantizando la integridad de los datos.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/role-assignment.png" width="900px" alt="role-assignment">

##### Gestión Comercial y Planes

Contratación de Planes (US1)

Vista comercial que permite al dueño de la unidad o institución seleccionar y contratar el nivel de servicio adecuado según la cantidad de buses y alumnos.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/hire-plan.png" width="900px" alt="hire-plan">
<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/hire-plan2.png" width="900px" alt="hire-plan">

Consulta de Precios y Tarifas (US22)

Sección informativa donde se detallan los costos operativos y las tarifas vigentes para la gestión del transporte escolar.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/pricing-query.png" width="900px" alt="pricing-query">

##### Gestión de Logística y Alumnos
Alta y Gestión de Alumnos (US4, US24)

Interfaz conectada a la API que permite visualizar la lista completa de estudiantes, agregar nuevos registros o actualizar la información de los existentes.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/student-management.png" width="900px" alt="student-management">
<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/student-management2.png" width="900px" alt="student-management">

Registro de Conductores (US2)

Formulario dedicado a la creación del perfil del conductor, donde se almacenan sus datos personales, licencias y contacto de emergencia.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/driver-registration1.png" width="900px" alt="driver-registration">
<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/driver-registration2.png" width="900px" alt="driver-registration">

Registro de Padres (US3)

Formulario dedicado a la creación del perfil del padre de familia, donde se almacenan sus datos personales y estudiante del cual es apoderado.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/parent-registration.png" width="900px" alt="driver-registration">

Creación y Edición de Rutas (US5)

Herramienta de diseño logístico donde el administrador traza los recorridos, define paradas clave y asigna los tiempos estimados de viaje.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/route-creation.png" width="900px" alt="route-creation">

#### Versión Desktop Wireframes - Conductores

##### Operación de Viaje

Inicio de Trayecto (US8)

Pantalla de activación donde el conductor confirma que está listo para empezar el recorrido. Al hacer clic en "Iniciar Viaje", se dispara el rastreo GPS para los padres.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/start-trip1.png" width="900px" alt="start-trip">
<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/start-trip2.png" width="900px" alt="start-trip">

Marcación de Abordaje (US9)

Lista interactiva de alumnos por parada. El conductor marca con un solo toque quién ha subido al bus, actualizando el estado de asistencia en tiempo real.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/boarding-check.png" width="900px" alt="boarding-check">

Finalización de Ruta (US12)

Vista de cierre donde el conductor reporta el término del trayecto, asegurando que todos los alumnos hayan descendido en sus destinos correspondientes.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/route-end.png" width="900px" alt="route-end">

Bitácora de Viajes Histórica (US13)

Resumen diario de los trayectos realizados, permitiendo al conductor revisar las horas de inicio, fin e incidencias ocurridas durante sus turnos.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/trip-log.png" width="900px" alt="trip-log">

##### Seguridad y Alertas

Reporte de Incidencias en Ruta (US10)

Módulo para notificar eventos imprevistos como tráfico pesado, accidentes o fallas mecánicas, enviando una alerta automática a la central y a los padres.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/incident-report.png" width="900px" alt="incident-report">

Botón de Pánico (US11)

Funcionalidad de emergencia de un solo clic que envía una señal de auxilio inmediata a los administradores con la ubicación exacta del vehículo.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/panic-button.png" width="900px" alt="panic-button">

#### Versión Desktop Wireframes - Padres de Familia

##### Monitoreo y Supervisión

Rastreo en Tiempo Real (US14)

Vista de mapa interactivo que permite al padre seguir el movimiento del bus y ver el tiempo estimado para que llegue a su parada.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/real-time-tracking.png" width="900px" alt="real-time-tracking">

Acceso a Cámara Interna (US17)

Funcionalidad que permite visualizar el interior de la unidad mediante streaming de video, proporcionando una capa adicional de tranquilidad sobre la seguridad del niño.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/camera-access.png" width="900px" alt="camera-access">

Alerta de Proximidad (US15)

Interfaz de notificación que avisa visualmente cuando el bus entra en un radio cercano al hogar (ej. 500 metros), indicando que es momento de salir a la parada.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/proximity-alert.png" width="900px" alt="proximity-alert">

Confirmación de Llegada (US16)

Aviso automático que recibe el padre cuando la unidad llega satisfactoriamente al colegio o al punto de destino final.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/arrival-confirmation.png" width="900px" alt="arrival-confirmation">

Historial de Asistencia (US18)

Calendario detallado donde el padre puede revisar los días asistidos, las horas de abordaje y cualquier incidencia registrada en viajes pasados.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Desktop/attendance-history.png" width="900px" alt="attendance-history">

#### Versión Mobile Wireframes - Acceso y Configuración (Universal)

##### Autenticación y Acceso

Registro de Cuenta
Pantalla unificada de registro donde el usuario selecciona su rol (Padre, Conductor o Administrador) y completa sus datos básicos. Es el punto de partida para que cualquier actor del sistema pueda interactuar con la plataforma.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/universalregister.png" width="400px" alt="register">

Inicio de Sesión (Login) Interfaz de acceso donde los usuarios ingresan sus credenciales. El sistema valida el rol del usuario y lo redirige automáticamente a su panel de control correspondiente.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/universallogin.png" width="400px" alt="login">

Cambio de Contraseña Formulario de seguridad que permite restablecer el acceso mediante la verificación de identidad tras un código, garantizando que solo el propietario de la cuenta pueda modificar sus credenciales.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/password-change.png" width="900px" alt="password-change">

#### Versión Mobile Wireframes - Administradores 

##### Configuración y Gestión Administrativa

Panel de Inicio y Navegación (US20)

Dashboard central que organiza todos los módulos del sistema a través de un sidebar lateral, facilitando el salto entre la gestión de rutas, alumnos y reportes.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/home-dashboard.png" width="600px" alt="home-dashboard"> 

Asignación de Roles (US6)

Módulo exclusivo para el administrador donde se definen los permisos específicos de cada usuario registrado, garantizando la integridad de los datos.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/role-assignment.png" width="400px" alt="role-assignment">

##### Gestión Comercial y Planes

Contratación de Planes (US1)

Vista comercial que permite al dueño de la unidad o institución seleccionar y contratar el nivel de servicio adecuado según la cantidad de buses y alumnos.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/hire-plan.png" width="900px" alt="hire-plan">

Consulta de Precios y Tarifas (US22)

Sección informativa donde se detallan los costos operativos y las tarifas vigentes para la gestión del transporte escolar.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/pricing-query.png" width="900px" alt="pricing-query">

##### Gestión de Logística y Alumnos
Alta y Gestión de Alumnos (US4, US24)

Interfaz conectada a la API que permite visualizar la lista completa de estudiantes, agregar nuevos registros o actualizar la información de los existentes.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/student-managament.png" width="900px" alt="student-management">

Registro de Conductores (US2)

Formulario dedicado a la creación del perfil del conductor, donde se almacenan sus datos personales, licencias y contacto de emergencia.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/driver-registration.png" width="900px" alt="driver-registration">

Registro de Padres (US3)

Formulario dedicado a la creación del perfil del padre de familia, donde se almacenan sus datos personales y estudiante del cual es apoderado.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/parent-registration.png" width="400px" alt="driver-registration">

Creación y Edición de Rutas (US5)

Herramienta de diseño logístico donde el administrador traza los recorridos, define paradas clave y asigna los tiempos estimados de viaje.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/route-creation.png" width="400px" alt="route-creation">

#### Versión Mobile Wireframes - Conductores

##### Operación de Viaje

Inicio de Trayecto (US8)

Pantalla de activación donde el conductor confirma que está listo para empezar el recorrido. Al hacer clic en "Iniciar Viaje", se dispara el rastreo GPS para los padres.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/trip-start.png" width="900px" alt="start-trip">

Marcación de Abordaje (US9)

Lista interactiva de alumnos por parada. El conductor marca con un solo toque quién ha subido al bus, actualizando el estado de asistencia en tiempo real.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/boarding-check.png" width="400px" alt="boarding-check">

Finalización de Ruta (US12)

Vista de cierre donde el conductor reporta el término del trayecto, asegurando que todos los alumnos hayan descendido en sus destinos correspondientes.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/route-end.png" width="400px" alt="route-end">

Bitácora de Viajes Histórica (US13)

Resumen diario de los trayectos realizados, permitiendo al conductor revisar las horas de inicio, fin e incidencias ocurridas durante sus turnos.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/trip-log.png" width="400px" alt="trip-log">

##### Seguridad y Alertas

Reporte de Incidencias en Ruta (US10)

Módulo para notificar eventos imprevistos como tráfico pesado, accidentes o fallas mecánicas, enviando una alerta automática a la central y a los padres.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/incident-report.png" width="400px" alt="incident-report">

Botón de Pánico (US11)

Funcionalidad de emergencia de un solo clic que envía una señal de auxilio inmediata a los administradores con la ubicación exacta del vehículo.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/panic-button.png" width="400px" alt="panic-button">

#### Versión Mobile Wireframes - Padres de Familia

##### Monitoreo y Supervisión

Rastreo en Tiempo Real (US14)

Vista de mapa interactivo que permite al padre seguir el movimiento del bus y ver el tiempo estimado para que llegue a su parada.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/real-time-tracking.png" width="400px" alt="real-time-tracking">

Acceso a Cámara Interna (US17)

Funcionalidad que permite visualizar el interior de la unidad mediante streaming de video, proporcionando una capa adicional de tranquilidad sobre la seguridad del niño.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/camera-access.png" width="400px" alt="camera-access">

Alerta de Proximidad (US15)

Interfaz de notificación que avisa visualmente cuando el bus entra en un radio cercano al hogar (ej. 500 metros), indicando que es momento de salir a la parada.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/proximity-alert.png" width="400px" alt="proximity-alert">

Confirmación de Llegada (US16)

Aviso automático que recibe el padre cuando la unidad llega satisfactoriamente al colegio o al punto de destino final.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/arrival-confirmation.png" width="400px" alt="arrival-confirmation">

Historial de Asistencia (US18)

Calendario detallado donde el padre puede revisar los días asistidos, las horas de abordaje y cualquier incidencia registrada en viajes pasados.

<img src="assets/images/ChapterIV/WebApp/Wireframes/Mobile/attendance-history.png" width="400px" alt="attendance-history">

### 4.4.2. Web Applications Wireflow Diagrams



### 4.4.2. Web Applications Mock-ups

#### Versión Desktop Mockups - Acceso y Configuración (Universal)

##### Autenticación y Acceso

Registro de Cuenta
Pantalla unificada de registro donde el usuario selecciona su rol (Padre, Conductor o Administrador) y completa sus datos básicos. Es el punto de partida para que cualquier actor del sistema pueda interactuar con la plataforma.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/universalregister.png" width="900px" alt="register">

Inicio de Sesión (Login) Interfaz de acceso donde los usuarios ingresan sus credenciales. El sistema valida el rol del usuario y lo redirige automáticamente a su panel de control correspondiente.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/universallogin.png" width="900px" alt="login">

Cambio de Contraseña Formulario de seguridad que permite restablecer el acceso mediante la verificación de identidad tras un código, garantizando que solo el propietario de la cuenta pueda modificar sus credenciales.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/password-change1.png" width="900px" alt="password-change">
<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/password-change2.png" width="900px" alt="password-change">
<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/password-change3.png" width="900px" alt="password-change">

#### Versión Desktop Mockups - Administradores 

##### Configuración y Gestión Administrativa

Panel de Inicio y Navegación (US20)

Dashboard central que organiza todos los módulos del sistema a través de un sidebar lateral, facilitando el salto entre la gestión de rutas, alumnos y reportes.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/home-dashboard.png" width="900px" alt="home-dashboard">

Asignación de Roles (US6)

Módulo exclusivo para el administrador donde se definen los permisos específicos de cada usuario registrado, garantizando la integridad de los datos.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/role-assignment.png" width="900px" alt="role-assignment">

##### Gestión Comercial y Planes

Contratación de Planes (US1)

Vista comercial que permite al dueño de la unidad o institución seleccionar y contratar el nivel de servicio adecuado según la cantidad de buses y alumnos.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/hire-plan.png" width="900px" alt="hire-plan">
<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/hire-plan2.png" width="900px" alt="hire-plan">

Consulta de Precios y Tarifas (US22)

Sección informativa donde se detallan los costos operativos y las tarifas vigentes para la gestión del transporte escolar.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/pricing-query.png" width="900px" alt="pricing-query">

##### Gestión de Logística y Alumnos
Alta y Gestión de Alumnos (US4, US24)

Interfaz conectada a la API que permite visualizar la lista completa de estudiantes, agregar nuevos registros o actualizar la información de los existentes.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/student-management.png" width="900px" alt="student-management">
<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/student-management2.png" width="900px" alt="student-management">

Registro de Conductores (US2)

Formulario dedicado a la creación del perfil del conductor, donde se almacenan sus datos personales, licencias y contacto de emergencia.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/driver-registration1.png" width="900px" alt="driver-registration">
<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/driver-registration2.png" width="900px" alt="driver-registration">

Registro de Padres (US3)

Formulario dedicado a la creación del perfil del padre de familia, donde se almacenan sus datos personales y estudiante del cual es apoderado.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/parent-registration.png" width="900px" alt="driver-registration">

Creación y Edición de Rutas (US5)

Herramienta de diseño logístico donde el administrador traza los recorridos, define paradas clave y asigna los tiempos estimados de viaje.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/route-creation.png" width="900px" alt="route-creation">

#### Versión Desktop Mockups - Conductores

##### Operación de Viaje

Inicio de Trayecto (US8)

Pantalla de activación donde el conductor confirma que está listo para empezar el recorrido. Al hacer clic en "Iniciar Viaje", se dispara el rastreo GPS para los padres.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/start.png" width="900px" alt="start-trip">
<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/start-trip.png" width="900px" alt="start-trip">

Marcación de Abordaje (US9)

Lista interactiva de alumnos por parada. El conductor marca con un solo toque quién ha subido al bus, actualizando el estado de asistencia en tiempo real.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/boarding-check.png" width="900px" alt="boarding-check">

Finalización de Ruta (US12)

Vista de cierre donde el conductor reporta el término del trayecto, asegurando que todos los alumnos hayan descendido en sus destinos correspondientes.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/route-end.png" width="900px" alt="route-end">

Bitácora de Viajes Histórica (US13)

Resumen diario de los trayectos realizados, permitiendo al conductor revisar las horas de inicio, fin e incidencias ocurridas durante sus turnos.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/trip-log.png" width="900px" alt="trip-log">

##### Seguridad y Alertas

Reporte de Incidencias en Ruta (US10)

Módulo para notificar eventos imprevistos como tráfico pesado, accidentes o fallas mecánicas, enviando una alerta automática a la central y a los padres.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/incident-report.png" width="900px" alt="incident-report">

Botón de Pánico (US11)

Funcionalidad de emergencia de un solo clic que envía una señal de auxilio inmediata a los administradores con la ubicación exacta del vehículo.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/panic-button.png" width="900px" alt="panic-button">

#### Versión Desktop Wireframes - Padres de Familia

##### Monitoreo y Supervisión

Rastreo en Tiempo Real (US14)

Vista de mapa interactivo que permite al padre seguir el movimiento del bus y ver el tiempo estimado para que llegue a su parada.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/real-time-tracking.png" width="900px" alt="real-time-tracking">

Acceso a Cámara Interna (US17)

Funcionalidad que permite visualizar el interior de la unidad mediante streaming de video, proporcionando una capa adicional de tranquilidad sobre la seguridad del niño.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/camera-access.png" width="900px" alt="camera-access">

Alerta de Proximidad (US15)

Interfaz de notificación que avisa visualmente cuando el bus entra en un radio cercano al hogar (ej. 500 metros), indicando que es momento de salir a la parada.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/proximity-alert.png" width="900px" alt="proximity-alert">

Confirmación de Llegada (US16)

Aviso automático que recibe el padre cuando la unidad llega satisfactoriamente al colegio o al punto de destino final.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/arrival-confirmation.png" width="900px" alt="arrival-confirmation">

Historial de Asistencia (US18)

Calendario detallado donde el padre puede revisar los días asistidos, las horas de abordaje y cualquier incidencia registrada en viajes pasados.

<img src="assets/images/ChapterIV/WebApp/Mockups/Desktop/attendance-history.png" width="900px" alt="attendance-history">



#### Versión Mobile Mockups - Acceso y Configuración (Universal)

##### Autenticación y Acceso

Registro de Cuenta
Pantalla unificada de registro donde el usuario selecciona su rol (Padre, Conductor o Administrador) y completa sus datos básicos. Es el punto de partida para que cualquier actor del sistema pueda interactuar con la plataforma.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/universalregister.png" width="400px" alt="register">

Inicio de Sesión (Login) Interfaz de acceso donde los usuarios ingresan sus credenciales. El sistema valida el rol del usuario y lo redirige automáticamente a su panel de control correspondiente.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/universallogin.png" width="400px" alt="login">

Cambio de Contraseña Formulario de seguridad que permite restablecer el acceso mediante la verificación de identidad tras un código, garantizando que solo el propietario de la cuenta pueda modificar sus credenciales.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/password-change.png" width="900px" alt="password-change">

#### Versión Mobile Mockups - Administradores 

##### Configuración y Gestión Administrativa

Panel de Inicio y Navegación (US20)

Dashboard central que organiza todos los módulos del sistema a través de un sidebar lateral, facilitando el salto entre la gestión de rutas, alumnos y reportes.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/home-dashboard.png" width="900px" alt="home-dashboard"> 

Asignación de Roles (US6)

Módulo exclusivo para el administrador donde se definen los permisos específicos de cada usuario registrado, garantizando la integridad de los datos.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/role-assignment.png" width="400px" alt="role-assignment">

##### Gestión Comercial y Planes

Contratación de Planes (US1)

Vista comercial que permite al dueño de la unidad o institución seleccionar y contratar el nivel de servicio adecuado según la cantidad de buses y alumnos.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/hire-plan.png" width="900px" alt="hire-plan">

Consulta de Precios y Tarifas (US22)

Sección informativa donde se detallan los costos operativos y las tarifas vigentes para la gestión del transporte escolar.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/pricing-query.png" width="900px" alt="pricing-query">

##### Gestión de Logística y Alumnos
Alta y Gestión de Alumnos (US4, US24)

Interfaz conectada a la API que permite visualizar la lista completa de estudiantes, agregar nuevos registros o actualizar la información de los existentes.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/student-managament.png" width="900px" alt="student-management">

Registro de Conductores (US2)

Formulario dedicado a la creación del perfil del conductor, donde se almacenan sus datos personales, licencias y contacto de emergencia.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/driver-registration.png" width="900px" alt="driver-registration">

Registro de Padres (US3)

Formulario dedicado a la creación del perfil del padre de familia, donde se almacenan sus datos personales y estudiante del cual es apoderado.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/parent-registration.png" width="400px" alt="driver-registration">

Creación y Edición de Rutas (US5)

Herramienta de diseño logístico donde el administrador traza los recorridos, define paradas clave y asigna los tiempos estimados de viaje.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/route-creation.png" width="400px" alt="route-creation">

#### Versión Mobile Mockups - Conductores

##### Operación de Viaje

Inicio de Trayecto (US8)

Pantalla de activación donde el conductor confirma que está listo para empezar el recorrido. Al hacer clic en "Iniciar Viaje", se dispara el rastreo GPS para los padres.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/start-trip.png" width="800px" alt="start-trip">

Marcación de Abordaje (US9)

Lista interactiva de alumnos por parada. El conductor marca con un solo toque quién ha subido al bus, actualizando el estado de asistencia en tiempo real.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/boarding-check.png" width="400px" alt="boarding-check">

Finalización de Ruta (US12)

Vista de cierre donde el conductor reporta el término del trayecto, asegurando que todos los alumnos hayan descendido en sus destinos correspondientes.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/route-end.png" width="400px" alt="route-end">

Bitácora de Viajes Histórica (US13)

Resumen diario de los trayectos realizados, permitiendo al conductor revisar las horas de inicio, fin e incidencias ocurridas durante sus turnos.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/trip-log.png" width="400px" alt="trip-log">

##### Seguridad y Alertas

Reporte de Incidencias en Ruta (US10)

Módulo para notificar eventos imprevistos como tráfico pesado, accidentes o fallas mecánicas, enviando una alerta automática a la central y a los padres.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/incident-report.png" width="400px" alt="incident-report">

Botón de Pánico (US11)

Funcionalidad de emergencia de un solo clic que envía una señal de auxilio inmediata a los administradores con la ubicación exacta del vehículo.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/panic-button.png" width="400px" alt="panic-button">

#### Versión Mobile Mockups - Padres de Familia

##### Monitoreo y Supervisión

Rastreo en Tiempo Real (US14)

Vista de mapa interactivo que permite al padre seguir el movimiento del bus y ver el tiempo estimado para que llegue a su parada.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/real-time-tracking.png" width="400px" alt="real-time-tracking">

Acceso a Cámara Interna (US17)

Funcionalidad que permite visualizar el interior de la unidad mediante streaming de video, proporcionando una capa adicional de tranquilidad sobre la seguridad del niño.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/camera-access.png" width="400px" alt="camera-access">

Alerta de Proximidad (US15)

Interfaz de notificación que avisa visualmente cuando el bus entra en un radio cercano al hogar (ej. 500 metros), indicando que es momento de salir a la parada.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/proximity-alert.png" width="400px" alt="proximity-alert">

Confirmación de Llegada (US16)

Aviso automático que recibe el padre cuando la unidad llega satisfactoriamente al colegio o al punto de destino final.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/arrival-confirmation.png" width="400px" alt="arrival-confirmation">

Historial de Asistencia (US18)

Calendario detallado donde el padre puede revisar los días asistidos, las horas de abordaje y cualquier incidencia registrada en viajes pasados.

<img src="assets/images/ChapterIV/WebApp/Mockups/Mobile/attendance-history.png" width="400px" alt="attendance-history">

### 4.4.3. Web Applications User Flow Diagrams

### User Flows Desktop

#### Desktop User Flow 1:

Relacionado con User Goal 1:
Como suscriptor, quiero poder acceder a mi cuenta de la aplicación.

El usuario ingresa a la pantalla de inicio de sesión e introduce sus credenciales (correo y contraseña). Si los datos son correctos, el sistema valida la información y redirige al usuario a la sección principal "Inicio" junto con el menú lateral habilitado. En caso de no contar con una cuenta, el usuario puede dirigirse a la sección de registro, completar el formulario con sus datos personales y guardar el nuevo usuario para luego iniciar sesión.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Desktop/.png" width="400px" alt="attendance-history">

#### Desktop User Flow 2:

Relacionado con User Goal 2:
Como suscriptor, quiero poder cambiar mi contraseña para mantener mi cuenta asegurada.

Desde la pantalla de inicio de sesión, el usuario selecciona la opción "Cambio de Contraseña". El sistema muestra un formulario donde el usuario ingresa su correo registrado y la nueva contraseña. Al confirmar, el sistema actualiza las credenciales y permite al usuario ingresar nuevamente con la nueva contraseña. Esto garantiza el acceso continuo incluso si se olvidó la contraseña anterior.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Desktop/.png" width="400px" alt="attendance-history">

#### Desktop User Flow 3:

Relacionado con User Goal 3: 
Como administrador, quiero ingresar nuevos conductores y crear sus nuevas rutas.

Tras iniciar sesión, el administrador accede al módulo de "Registro de Conductor" e ingresa los datos del personal operativo. Luego navega a la sección "Creación de Rutas", donde traza los puntos de parada, asigna tiempos estimados y vincula la ruta al conductor registrado. El sistema confirma el guardado y refleja los cambios en el panel de gestión.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Desktop/.png" width="400px" alt="attendance-history">

#### Desktop User Flow 4:

Relacionado con User Goal 4: 
Como administrador, quiero organizar los roles y rutas de manera centralizada.

Desde el panel principal, el administrador accede a "Asignación de Roles" para configurar los permisos de cada miembro del equipo, habilitando accesos de edición o solo lectura según corresponda. Posteriormente, puede revisar y reasignar rutas desde la vista centralizada, asegurando que cada conductor tenga su ruta correctamente vinculada.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Desktop/.png" width="400px" alt="attendance-history">

#### Desktop User Flow 5:

Relacionado con User Goal 5: 
Como administrador, quiero mejorar las características de la aplicación con un nuevo plan.

El administrador navega a la sección de "Contratación del Plan" y visualiza las opciones de suscripción disponibles según el tamaño de su flota. Al seleccionar un plan, es redirigido a la pasarela de pagos donde ingresa su información financiera y confirma la contratación. Una vez procesado el pago, el sistema actualiza los beneficios disponibles y el administrador puede consultar el balance de costos en "Consulta de Precios".

<img src="assets/images/ChapterIV/WebApp/UserFlow/Desktop/.png" width="400px" alt="attendance-history">

#### Desktop User Flow 6:

Relacionado con User Goal 6: 
Como conductor, quiero tener un control claro de los alumnos durante la ruta.

El conductor inicia sesión y desde su panel principal selecciona la ruta asignada. Presiona "Iniciar Trayecto" para activar la transmisión GPS. El sistema carga automáticamente la lista de alumnos correspondiente a esa ruta. En cada parada, el conductor localiza al estudiante y registra su abordaje pulsando "Marcación de Abordaje". Al llegar al destino, presiona "Finalización de Ruta" para cerrar el trayecto.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Desktop/.png" width="400px" alt="attendance-history">

#### Desktop User Flow 7:

Relacionado con User Goal 7: 
Como conductor, quiero brindar un servicio más profesional y confiable.

El conductor accede a su "Bitácora de Viajes" para revisar el historial completo de sus trayectos anteriores, incluyendo horarios, estudiantes transportados e incidencias registradas. Esta información le permite identificar patrones, mejorar su puntualidad y contar con un registro formal de su desempeño ante el administrador.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Desktop/.png" width="400px" alt="attendance-history">

#### Desktop User Flow 8:

Relacionado con User Goal 8: 
Como conductor, quiero comunicar alguna incidencia u avance de la ruta durante el viaje.

Durante una ruta activa, el conductor detecta un imprevisto y accede al módulo de seguridad del Dashboard. Selecciona una categoría predefinida dentro de "Reporte de Incidencias" (retraso, desvío, obstáculo, etc.) y envía la notificación. El sistema propaga el aviso al administrador y a los padres afectados en tiempo real.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Desktop/.png" width="400px" alt="attendance-history">

#### Desktop User Flow 9:
Relacionado con User Goal 9: Como conductor, quiero una manera inmediata de informar una emergencia.

Ante una situación de peligro inminente durante la ruta, el conductor mantiene presionado el "Botón de Pánico" por 2 segundos. El sistema dispara de forma automática una alerta roja hacia los servicios de emergencia, el administrador y los padres de familia de todos los alumnos a bordo. Tras la resolución del incidente, el conductor puede revisar el evento registrado en su Bitácora de Viajes.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Desktop/.png" width="400px" alt="attendance-history">

#### Desktop User Flow 10:

Relacionado con User Goal 10: 
Como padre de familia, quiero estar informado de la ubicación y situación en tiempo real del vehículo.

El padre inicia sesión y accede al seguimiento del bus asignado a su hijo. El sistema renderiza el mapa con la ubicación en tiempo real del vehículo. El usuario puede activar el switch de "Acceso a la Cámara" para visualizar la transmisión de video en vivo del interior de la unidad. Al acercarse al radio de 500 metros del destino, el sistema emite automáticamente una "Alerta de Proximidad".

<img src="assets/images/ChapterIV/WebApp/UserFlow/Desktop/.png" width="400px" alt="attendance-history">

#### Desktop User Flow 11:
Relacionado con User Goal 11: Como padre de familia, quiero recibir notificaciones sin tener que preguntar.

El padre recibe notificaciones automáticas del sistema en distintos momentos del trayecto: cuando el bus inicia la ruta, cuando se aproxima a su parada y ante cualquier incidencia reportada por el conductor. Estas alertas llegan sin necesidad de que el padre esté activamente consultando la aplicación, manteniéndolo informado de forma pasiva y continua.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Desktop/.png" width="400px" alt="attendance-history">

#### Desktop User Flow 12:

Relacionado con User Goal 12: 
Como padre de familia, quiero saber si mi hijo abordó el transporte y quedó registrado.

Una vez que el conductor marca el abordaje del estudiante, el padre recibe en pantalla una "Confirmación de Llegada" con la hora exacta del registro. El sistema almacena este evento en el "Historial de Asistencia", donde el padre puede seleccionar un rango de fechas para auditar los horarios de recogida y entrega, generando un reporte visual de la puntualidad del servicio.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Desktop/.png" width="400px" alt="attendance-history">

### User Flows Mobile

#### Mobile User Flow 1:

Relacionado con User Goal 1: 
Como suscriptor, quiero poder acceder a mi cuenta de la aplicación.

El usuario ingresa a la pantalla de inicio de sesión e introduce sus credenciales (correo y contraseña). Si los datos son correctos, el sistema valida la información y redirige al usuario a la sección principal "Inicio" junto con el menú lateral habilitado. En caso de no contar con una cuenta, el usuario puede dirigirse a la sección de registro, completar el formulario con sus datos personales y guardar el nuevo usuario para luego iniciar sesión.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Mobile/.png" width="400px" alt="attendance-history">

#### Mobile User Flow 2:

Relacionado con User Goal 2:
Como suscriptor, quiero poder cambiar mi contraseña para mantener mi cuenta asegurada.

Desde la pantalla de inicio de sesión, el usuario selecciona la opción "Cambio de Contraseña". El sistema muestra un formulario donde el usuario ingresa su correo registrado y la nueva contraseña. Al confirmar, el sistema actualiza las credenciales y permite al usuario ingresar nuevamente con la nueva contraseña. Esto garantiza el acceso continuo incluso si se olvidó la contraseña anterior.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Mobile/.png" width="400px" alt="attendance-history">

#### Mobile User Flow 3:

Relacionado con User Goal 3: 
Como administrador, quiero ingresar nuevos conductores y crear sus nuevas rutas.

Tras iniciar sesión, el administrador accede al módulo de "Registro de Conductor" e ingresa los datos del personal operativo. Luego navega a la sección "Creación de Rutas", donde traza los puntos de parada, asigna tiempos estimados y vincula la ruta al conductor registrado. El sistema confirma el guardado y refleja los cambios en el panel de gestión.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Mobile/.png" width="400px" alt="attendance-history">

#### Mobile User Flow 4:

Relacionado con User Goal 4: 
Como administrador, quiero organizar los roles y rutas de manera centralizada.

Desde el panel principal, el administrador accede a "Asignación de Roles" para configurar los permisos de cada miembro del equipo, habilitando accesos de edición o solo lectura según corresponda. Posteriormente, puede revisar y reasignar rutas desde la vista centralizada, asegurando que cada conductor tenga su ruta correctamente vinculada.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Mobile/.png" width="400px" alt="attendance-history">

#### Mobile User Flow 5:

Relacionado con User Goal 5: 
Como administrador, quiero mejorar las características de la aplicación con un nuevo plan.

El administrador navega a la sección de "Contratación del Plan" y visualiza las opciones de suscripción disponibles según el tamaño de su flota. Al seleccionar un plan, es redirigido a la pasarela de pagos donde ingresa su información financiera y confirma la contratación. Una vez procesado el pago, el sistema actualiza los beneficios disponibles y el administrador puede consultar el balance de costos en "Consulta de Precios".

<img src="assets/images/ChapterIV/WebApp/UserFlow/Mobile/.png" width="400px" alt="attendance-history">

#### Mobile User Flow 6:

Relacionado con User Goal 6: 
Como conductor, quiero tener un control claro de los alumnos durante la ruta.

El conductor inicia sesión y desde su panel principal selecciona la ruta asignada. Presiona "Iniciar Trayecto" para activar la transmisión GPS. El sistema carga automáticamente la lista de alumnos correspondiente a esa ruta. En cada parada, el conductor localiza al estudiante y registra su abordaje pulsando "Marcación de Abordaje". Al llegar al destino, presiona "Finalización de Ruta" para cerrar el trayecto.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Mobile/.png" width="400px" alt="attendance-history">

#### Mobile User Flow 7:

Relacionado con User Goal 7: 
Como conductor, quiero brindar un servicio más profesional y confiable.

El conductor accede a su "Bitácora de Viajes" para revisar el historial completo de sus trayectos anteriores, incluyendo horarios, estudiantes transportados e incidencias registradas. Esta información le permite identificar patrones, mejorar su puntualidad y contar con un registro formal de su desempeño ante el administrador.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Mobile/.png" width="400px" alt="attendance-history">

#### Mobile User Flow 8:

Relacionado con User Goal 8: 
Como conductor, quiero comunicar alguna incidencia u avance de la ruta durante el viaje.

Durante una ruta activa, el conductor detecta un imprevisto y accede al módulo de seguridad del Dashboard. Selecciona una categoría predefinida dentro de "Reporte de Incidencias" (retraso, desvío, obstáculo, etc.) y envía la notificación. El sistema propaga el aviso al administrador y a los padres afectados en tiempo real.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Mobile/.png" width="400px" alt="attendance-history">

#### Mobile User Flow 9:

Relacionado con User Goal 9: 
Como conductor, quiero una manera inmediata de informar una emergencia.

Ante una situación de peligro inminente durante la ruta, el conductor mantiene presionado el "Botón de Pánico" por 2 segundos. El sistema dispara de forma automática una alerta roja hacia los servicios de emergencia, el administrador y los padres de familia de todos los alumnos a bordo. Tras la resolución del incidente, el conductor puede revisar el evento registrado en su Bitácora de Viajes.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Mobile/.png" width="400px" alt="attendance-history">

#### Mobile User Flow 10:

Relacionado con User Goal 10: 
Como padre de familia, quiero estar informado de la ubicación y situación en tiempo real del vehículo.

El padre inicia sesión y accede al seguimiento del bus asignado a su hijo. El sistema renderiza el mapa con la ubicación en tiempo real del vehículo. El usuario puede activar el switch de "Acceso a la Cámara" para visualizar la transmisión de video en vivo del interior de la unidad. Al acercarse al radio de 500 metros del destino, el sistema emite automáticamente una "Alerta de Proximidad".

<img src="assets/images/ChapterIV/WebApp/UserFlow/Mobile/.png" width="400px" alt="attendance-history">

#### Mobile User Flow 11:
Relacionado con User Goal 11: 
Como padre de familia, quiero recibir notificaciones sin tener que preguntar.

El padre recibe notificaciones automáticas del sistema en distintos momentos del trayecto: cuando el bus inicia la ruta, cuando se aproxima a su parada y ante cualquier incidencia reportada por el conductor. Estas alertas llegan sin necesidad de que el padre esté activamente consultando la aplicación, manteniéndolo informado de forma pasiva y continua.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Mobile/.png" width="400px" alt="attendance-history">

#### Mobile User Flow 12:

Relacionado con User Goal 12: 
Como padre de familia, quiero saber si mi hijo abordó el transporte y quedó registrado.

Una vez que el conductor marca el abordaje del estudiante, el padre recibe en pantalla una "Confirmación de Llegada" con la hora exacta del registro. El sistema almacena este evento en el "Historial de Asistencia", donde el padre puede seleccionar un rango de fechas para auditar los horarios de recogida y entrega, generando un reporte visual de la puntualidad del servicio.

<img src="assets/images/ChapterIV/WebApp/UserFlow/Mobile/.png" width="400px" alt="attendance-history">

## 4.5. Web Applications Prototyping

## 4.6. Domain-Driven Software Architecture

Plantilla de colores:
![Plantilla](assets/images/ChapterIV/EventStorming/ColorPosit.png)

1. Unstructured Exploration
   ![BigPicture](assets/images/ChapterIV/EventStorming/BigPicture.png)

En esta fase inicial, identificamos los eventos de dominio fundamentales para la movilidad escolar. El objetivo es capturar los hitos de negocio que permiten la interacción segura entre padres, conductores y administradores sin priorizar aún la cronología. Los eventos se organizan en seis ejes principales:

- Identidad y Gestión de Accesos (IAM): Maneja la seguridad y autenticación de la plataforma. Incluye eventos como el inicio de sesión (Login), autenticación de usuarios (Authenticate User), emisión de tokens JWT para sesiones seguras y el registro de administradores.

- Gestión de Suscripciones y Planes: Controla el acceso comercial a las funcionalidades de la plataforma. Abarca la selección de planes, el procesamiento de pagos a través de pasarelas externas y la activación de funciones de gestión de rutas según el plan elegido (básico, intermedio o completo).

- Gestión de Stakeholders y Activos: Administra los perfiles de los actores involucrados y sus relaciones. Incluye el registro de conductores, padres y estudiantes, así como la creación de grupos y la vinculación de hijos a sus respectivos padres para el seguimiento personalizado.

- Planificación de Flota y Rutas: Define la logística previa al viaje. Comprende la creación de geocercas para las rutas (RouteGeofenceCreated), la selección de puntos de parada (Pick Waypoints), la asignación de estudiantes a vehículos y la definición de horarios de salida.

- Ejecución y Monitoreo de Viajes: Es el núcleo operativo en tiempo real. Captura el inicio del trayecto por el conductor (TripStarted), el registro del estado de abordaje de cada estudiante (StudentStatus) y la consulta activa de la información de la ruta durante el recorrido.

2. Timelines
   ![TimeLines](assets/images/ChapterIV/EventStorming/Timelines.png)

En este paso, los eventos se organizan en secuencias cronológicas para comprender el flujo natural de los procesos de negocio. Las líneas de tiempo clave incluyen:

- Flujo de Incorporación y Suscripción: Registro de administrador → Creación de organización → Selección de plan de suscripción → Procesamiento de pago → Activación de cuotas de servicios.

- Gestión de Stakeholders y Activos: Registro de conductores y padres → Vinculación de estudiante a padre → Creación de grupos de transporte → Registro de vehículos → Asignación de conductor a vehículo.

- Planificación de Rutas Institucionales: Definición de geocerca de la ruta → Selección de puntos de parada (waypoints) → Asignación de estudiantes a la ruta → Establecimiento de horarios de salida → Finalización de la activación de ruta.

- Ejecución de Viajes y Monitoreo: Inicio de viaje por el conductor → Consulta de información de ruta → Registro de abordaje del estudiante → Notificación automática al padre → Seguimiento de progreso en tiempo real.

- Gestión de Comunicaciones e Incidentes: Detección de anomalía → Generación de alerta de pánico de alta prioridad → Despacho de alerta a administradores/padres → Difusión de mensajes de estado (broadcast) → Visualización en línea de tiempo.

- Cierre de Operación: Llegada al destino final → Confirmación de descenso total de estudiantes → Finalización de viaje → Archivamiento de datos de ejecución → Liberación de recursos de flota.

Estas líneas de tiempo revelan las dependencias temporales y la naturaleza secuencial de las operaciones dentro del sistema, asegurando que el flujo de información viaje correctamente desde la base de datos hasta las notificaciones en el dispositivo del padre.

3. Pain Points
   ![PainPoints](assets/images/ChapterIV/EventStorming/PainPoints.png)

En esta etapa, se identifican las situaiciones en las que se generan los puntos de fricción, cuellos de botella y ciertos problemas que surgen durante los procesos operativos y administrativos. Los pain points detectados incluyen:

- Sincronización de Notificaciones: Retrasos en la entrega de alertas push al padre cuando el estudiante aborda el vehículo, generando incertidumbre innecesaria.

- Gestión de Errores en Abordaje: Fallos manuales del conductor al registrar el estado del estudiante (StudentStatus), lo que puede resultar en registros de asistencia incorrectos.

- Validaciones de Seguridad: Bloqueos o fallos en la generación de alertas de pánico de alta prioridad durante emergencias debido a pérdida de conectividad o errores del sistema.

- Asignación de Recursos: Errores en la vinculación manual de conductores a vehículos o rutas, impidiendo el inicio correcto del viaje en la plataforma.

- Fricción en el Pago y Suscripción: Interrupciones en el procesamiento de pagos que inhabilitan las cuotas de rutas y bloquean la operación diaria de la institución.

- Precisión de Geolocalización: Problemas de precisión en el GPS que confunden la ubicacion de checkpoints.

Identificar estos puntos críticos permite al equipo de SafeRoute priorizar el desarrollo de mecanismos de redundancia y mejorar la experiencia de usuario, asegurando que la comunicación entre el transporte y el hogar sea infalible.

4. Pivotal Points
   ![PivotalPoints](assets/images/ChapterIV/EventStorming/PivotalPoints.png)

Los puntos pivotales son eventos determinantes que marcan transiciones críticas en el ciclo de vida del servicio. Estos incluyen:

Activación de Suscripción: Este hito marca la transición de un estado de configuración restringida a uno operativo, habilitando las cuotas de rutas y conductores necesarias para funcionar.

Finalización de Definición de Ruta: Es el punto donde la planificación técnica termina y la ruta queda lista para ser asignada a un vehículo y un conductor.

Inicio de Viaje: Este evento activa el monitoreo en tiempo real y permite que los padres comiencen a visualizar el progreso del transporte en sus aplicaciones.

Registro de Abordaje (Student Boarded): Es el evento pivotal de comunicación; confirma la seguridad del estudiante y dispara automáticamente la notificación push hacia el tutor legal.

Generación de Alerta de Pánico: Cambia el estado del viaje de "Normal" a "Emergencia", activando protocolos de respuesta inmediata y priorizando la comunicación de red de seguridad.

Completación de Viaje: Marca el fin de la responsabilidad operativa del conductor sobre los estudiantes y archiva el registro para liberar los recursos de la flota.

Estos puntos son determinantes para la continuidad y el éxito de la movilidad escolar, ya que aseguran que cada fase del proceso se cumpla antes de pasar a la siguiente.

5. Commands
   ![Commands](assets/images/ChapterIV/EventStorming/Commands.png)

Los comandos representan las acciones o intenciones de los usuarios que desencadenan eventos en el sistema. Los principales comandos identificados son:

- Gestión de Identidad y Acceso (IAM): Registrar administrador, iniciar sesión, autenticar usuario, asignar rol, revocar privilegios.

- Gestión de Suscripciones y Planes: Seleccionar plan, iniciar proceso de pago, activar funciones de gestión, actualizar cuotas de conductores, cancelar servicio.

- Gestión de Stakeholders y Activos: Registrar conductor, registrar padre, vincular estudiante a pariente, registrar vehículo, crear grupo de transporte, asignar miembros al grupo.

- Gestión de Flota y Rutas: Definir geocerca, seleccionar puntos de parada (waypoints), asignar estudiantes a ruta, asignar vehículo a ruta, establecer horario de salida, finalizar activación de ruta.

- Ejecución de Viajes y Monitoreo: Iniciar viaje, consultar información de ruta, registrar estado de abordaje del estudiante, reportar incidente (botón de pánico), finalizar viaje.

- Comunicación y Notificaciones: Preparar notificación push, despachar alerta a padres, publicar mensaje de difusión (broadcast), mostrar mensaje en línea de tiempo.

6. Policies
   ![Policies](assets/images/ChapterIV/EventStorming/Polices.png)

Las políticas automatizan la lógica de negocio y aseguran la coherencia del sistema ante eventos críticos. Las políticas clave incluyen:

- Cuando el pago es exitoso → Activar suscripción y habilitar cuotas de rutas/conductores automáticamente.

- Cuando el conductor inicia un viaje → Notificar a todos los padres vinculados a esa ruta sobre el inicio del monitoreo en tiempo real.

- Cuando se registra el abordaje del estudiante → Despachar notificación push inmediata al dispositivo del padre correspondiente.

- Cuando se reporta un incidente (pánico) → Generar alerta de alta prioridad y transmitirla instantáneamente a los administradores y padres del grupo.

- Cuando se publica un mensaje de difusión → Mostrar el mensaje en la línea de tiempo de todos los miembros del grupo seleccionado.

- Cuando se confirma el descenso total de estudiantes → Marcar el viaje como completado y archivar los datos de ejecución.

- Cuando falla el registro de un stakeholder → Enviar una notificación de error con los detalles de validación al administrador.

7. Read Models
   ![ReadModels](assets/images/ChapterIV/EventStorming/ReadModels.png)

Los principales modelos de lectura identificados para garantizar la visibilidad del sistema son:

- Dashboard del Conductor: Vista detallada de la ruta asignada, lista de estudiantes por recoger, puntos de parada (waypoints) y estado de abordaje en tiempo real.

- Panel de Monitoreo para Padres: Visualización en tiempo real de la ubicación del vehículo, estado de seguridad del estudiante y línea de tiempo de eventos del viaje.

- Vista de Gestión de Grupos: Listado de estudiantes agrupados por ruta, vinculación con sus respectivos padres y estado de asistencia mensual.

- Estado de la Flota: Registro de vehículos activos, conductores asignados a cada unidad y disponibilidad de recursos para nuevas rutas.

- Historial de Incidentes: Registro cronológico de alertas de pánico, mensajes de difusión enviados y resoluciones de eventos de seguridad.

- Panel de Suscripción y Cuotas: Información sobre el plan activo, estado de los pagos y uso de las cuotas de rutas y conductores contratados.

- Directorio de Stakeholders: Lista completa de perfiles de usuarios (padres, conductores y administradores) con sus respectivos roles y privilegios de acceso.

8. External Systems
   ![ExternalSystems](assets/images/ChapterIV/EventStorming/ExternalSystems.png)

Las integraciones identificadas para la solución incluyen:

- Leaflet (Proveedor de Mapas): Se encarga de la visualización interactiva de las rutas, el trazado de geocercas (geofencing) y la gestión de coordenadas geográficas para el monitoreo en tiempo real.

- Resend (Servicio de Email): Utilizado para el envío de notificaciones transaccionales y correos electrónicos automáticos, como mensajes de bienvenida, confirmaciones de registro y alertas administrativas.

- PayPal (Pasarela de Pago): Servicio encargado de procesar de forma segura las transacciones financieras para la activación, renovación y actualización de los planes de suscripción institucional.

- MySQL (Gestión de Base de Datos): Actúa como el sistema externo de persistencia relacional encargado de almacenar y organizar toda la estructura de usuarios, rutas, vehículos y registros operativos.

9. Aggregates
   ![Aggregates](assets/images/ChapterIV/EventStorming/Aggregates.png)

Basado en los dominios operativos identificados, los agregados son:

User (Raíz): Gestiona la identidad del usuario, incluyendo credenciales de autenticación, roles asignados (Administrador, Padre, Conductor) y privilegios de acceso al panel de control.

Organization (Raíz): Controla la configuración de la institución, la gestión de miembros y la vinculación de la cuenta con los parámetros base del sistema institucional.

Subscription (Raíz): Administra el ciclo de vida del plan de servicios, integrando el procesamiento de pagos a través de PayPal para habilitar o restringir las cuotas de rutas y conductores disponibles.

Stakeholder (Raíz): Encapsula la información de padres y conductores, gestionando la vinculación crítica entre el tutor (padre) y el estudiante para asegurar el flujo de notificaciones.

Vehicle (Raíz): Maneja el registro de las unidades de transporte, sus especificaciones técnicas y los cambios de estado (activo/inactivo) dentro de la flota.

Route (Raíz): Coordina la definición logística del recorrido, incluyendo la creación de geocercas, la selección de paraderos (waypoints) y la asignación previa de estudiantes a la ruta.

Trip (Raíz): Controla la ejecución operativa en tiempo real, registrando el inicio del trayecto, los cambios en el estado de abordaje de los estudiantes y el log de incidentes generados durante el viaje.

10. Bounded Contexts
    ![BoundedContexts](assets/images/ChapterIV/EventStorming/BoundedContexts.png)

Los contextos delimitados organizan los agregados en dominios de negocio independientes, permitiendo que cada uno evolucione de manera autónoma para facilitar la escalabilidad del sistema:

- Identity & Access Management: Este contexto gestiona la seguridad perimetral, incluyendo la autenticación de usuarios, la creación de organizaciones, y la asignación de roles y privilegios para administradores, padres y conductores. Agregados: User, Organization.

- Subscription & Plan Management: Administra el ciclo de vida comercial del servicio. Se encarga de la selección de planes, el procesamiento de pagos mediante la integración con PayPal y la activación de las cuotas operativas de rutas y conductores contratados. Agregados: Subscription.

- Stakeholder & Asset Management: Maneja los perfiles de los actores críticos y los recursos físicos de la institución. Incluye el registro de conductores y padres, la vinculación esencial entre padres e hijos (estudiantes), y la gestión de la flota de vehículos. Agregados: Stakeholder, Vehicle.

- Route Planning & Execution: Coordina la logística integral, desde la planificación técnica hasta la operación en tiempo real. Cubre la definición de geocercas, la selección de paraderos, el monitoreo del abordaje de estudiantes y la gestión de incidentes durante el trayecto. Agregados: Route, Trip.

- Notifications & Communication: Actúa como el eje de interacción inmediata entre el transporte y el hogar. Orquesta el envío de notificaciones push (como el estado de abordaje del estudiante), alertas de pánico y mensajes de difusión general para mantener informados a los padres y administradores.

#### 4.6.2. Software Architecture Context Diagram

El diagrama de contexto presenta a SafeRoute como el sistema central, rodeado por sus tres tipos de usuarios y los sistemas externos con los que interactúa. El Administrador gestiona la plataforma configurando rutas, registrando actores y administrando suscripciones. El Conductor accede para ejecutar viajes, registrar el abordaje de estudiantes y emitir alertas de pánico. El Padre/Tutor monitorea en tiempo real el estado de la ruta de su hijo y recibe notificaciones. SafeRoute se integra con PayPal para el procesamiento de pagos, Leaflet + OpenRouteService para la visualización de mapas y cálculo de rutas escolares, y Resend como proveedor de correo transaccional para el despacho de alertas y notificaciones.

![ContextDiagram](/assets/images/ChapterIV/C4/SystemContext-dark.png)

#### 4.6.3. Software Architecture Container Diagrams

Aquí se detallan las unidades de despliegue principales del sistema. El diagrama muestra cómo SafeRoute se divide en una Landing Page estática (HTML5, CSS3, JavaScript), una aplicación web interactiva en el cliente desarrollada en Angular con Angular Material, una API backend modularizada construida con Spring Boot y Java, un Shared Kernel como librería Java de tipos compartidos entre contextos, y un repositorio persistente central en MySQL.

![ContainerDiagram](/assets/images/ChapterIV/C4/ContainerDiagram-dark.png)

### 4.6.4. Software Architecture Components Diagrams

**BackEnd**

- Web Services:
![WebServices](/assets/images/ChapterIV/C4/WebServiceComponents-dark.png)
Este diagrama ofrece la visión macro del backend. Demuestra cómo el monolito de Spring Boot está organizado lógicamente en seis Bounded Contexts independientes y un Shared Kernel (núcleo compartido de Value Objects), asegurando una separación clara de responsabilidades a nivel de dominio.


- Identity & Access Management:
  Desglosa el módulo de identidad en su arquitectura interna de 4 capas (API, Application, Domain, Infrastructure). Ilustra cómo se maneja la autenticación de usuarios, la provisión de cuentas y la asignación de roles de forma aislada, con Spring Security gestionando la emisión de tokens JWT en la capa de infraestructura.
  ![WebServices](/assets/images/ChapterIV/C4/ComponentDiagram_IAM-dark.png)

- Subscription & Plan Management:
  Muestra la estructura interna de 4 capas del contexto encargado de la monetización. Detalla el flujo desde el controlador REST hasta la infraestructura que se integra con PayPal para gestionar el ciclo de vida de los planes y pagos de suscripción.
  ![WebServices](/assets/images/ChapterIV/C4/ComponentDiagram_Subscription-dark.png)

- Stakeholder & Asset Management:
  Representa las capas internas del dominio que administra la información core del negocio: la creación y vinculación de perfiles para conductores, padres de familia, estudiantes y la gestión de la flota de vehículos disponibles por organización.
  ![WebServices](/assets/images/ChapterIV/C4/ComponentDiagram_Stakeholder-dark.png)

- Route Planning & Execution:
  Detalla la arquitectura modular (Controller, Service, Domain, Repository) encargada de la logística previa al viaje. Maneja la definición de paraderos con coordenadas GPS de alta precisión, la asignación de vehículos y conductores, y la configuración de horarios y días de servicio por ruta.
  ![WebServices](/assets/images/ChapterIV/C4/ComponentDiagram_Route-dark.png)

- Notifications & Communication:
  Describe el módulo dedicado a la comunicación asíncrona en sus 4 capas. Orquesta la recepción de eventos internos emitidos por el contexto de Trip y utiliza su capa de infraestructura para despachar alertas de pánico, notificaciones de abordaje y comunicados de difusión general mediante el proveedor externo Resend.
  ![WebServices](/assets/images/ChapterIV/C4/ComponentDiagram_Notification-dark.png)

- Trip Execution & Monitoring:
  Ilustra el núcleo operativo del sistema en sus 4 capas. Muestra cómo se procesa la lógica en tiempo real durante la ejecución del viaje, gestionando el registro de abordajes por estudiante, el log de incidentes y la emisión de eventos de dominio internos que activan el contexto de Notificaciones.
  ![WebServices](/assets/images/ChapterIV/C4/ComponentDiagram_Trip-dark.png)

- Shared Kernel:
  Este diagrama expone las 4 capas transversales (Building Blocks) que fundamentan la arquitectura limpia del monolito. Detalla cómo se proveen clases base y utilidades compartidas: Middlewares en la capa API, interfaces y DTOs base en Application, Value Objects globales (TripId, StudentId) en Domain, y repositorios genéricos en Infrastructure, evitando la duplicidad de código en el resto de los Bounded Contexts.
  ![WebServices](/assets/images/ChapterIV/C4/ComponentDiagram_SharedKernel-dark.png)

**FrontEnd**

- Single Page 

![WebServices](/assets/images/ChapterIV/C4/ComponentDiagram_SPA-dark.png)
La SPA está desarrollada con Angular, Angular Material y TypeScript, organizada en módulos por bounded context. Cada módulo sigue una estructura interna de cuatro capas: Model (DTOs del dominio), Assembler (transforma respuestas del API), API Service (consume el backend vía HttpClient), y Store (estado reactivo con Angular Signals). La navegación entre módulos es gestionada por la Navigation Bar del módulo Shared, mientras que el HTTP Service centraliza todas las llamadas REST y el Map Service gestiona la integración con Leaflet.


#### 4.7.1. Class Diagrams

**BackEnd**

- Identity and Access Management:

![saferoute-iam](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-platform/refs/heads/main/safe-route-boot-developer/docs/java-saferoute-iam-ddd.puml)

Gestiona organizaciones, usuarios y roles en el entorno de la aplicación.
Organization (AggregateRoot): Maneja el ciclo de vida de la institución (métodos create(), suspend(), activate()). Se relaciona mediante Value Objects para su identificador, nombre y estado.
User (AggregateRoot): Gestiona la autenticación y la asignación de roles de los usuarios (métodos register(), authenticate(), changeRole()). Pertenece a una organización a través del OrganizationId compartido y utiliza Value Objects de seguridad como PasswordHash.
Role (Entity): Define los niveles de acceso dentro del sistema usando el Value Object

- Subscription & Plan Management:

![saferoute-subscription](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-platform/refs/heads/main/safe-route-boot-developer/docs/java-saferoute-subscription-ddd.puml)

Controla el modelo de negocio, definiendo los planes y suscripciones de cada organización.
Subscription (AggregateRoot): Controla el estado y la vigencia de una suscripción (métodos activate(), upgrade(), cancel()). Se vincula directamente a una organización y a un plan específico mediante sus identificadores.
Plan (AggregateRoot): Establece los límites operativos y económicos mediante los Value Objects RouteQuota y DriverQuota, los cuales validan que no se exceda la capacidad contratada de rutas y conductores.

- Stakeholder & Asset Management:

![saferoute-stakeholder](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-platform/refs/heads/main/safe-route-boot-developer/docs/java-saferoute-stakeholder-ddd.puml)

Modela a los actores humanos y sus agrupaciones dentro del sistema.
Parent (AggregateRoot): Representa a los apoderados e incluye una lista de entidades Child, gestionando la adición o remoción de hijos.
Driver (Entity): Define a los conductores, agregando atributos específicos de su labor como el Value Object LicenseNumber.
Child (Entity): Representa a los estudiantes, gestionando su estado de inscripción mediante el Value Object ChildEnrollmentState.
StudentGroup (Entity): Permite agrupar referencias a múltiples niños (ChildId) para facilitar su asignación.

- Fleet & Route Planning:

![saferoute-fleet](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-platform/refs/heads/main/safe-route-boot-developer/docs/java-saferoute-fleet-ddd.puml)

Encargado de la planificación logística y operativa del transporte.
Route (AggregateRoot): Define el recorrido y su programación utilizando Value Objects como DepartureTime y ServiceDays. Compone una secuencia de paradas (Stop) y se asocia a un vehículo y a una asignación específica.
Stop, Vehicle y Assignment (Entities): Stop maneja las coordenadas exactas y el orden de recojo. Vehicle controla la capacidad y disponibilidad de la unidad. Assignment vincula operativamente a un conductor con un grupo específico de niños para esa ruta.

- Trip Execution & Monitoring:

![saferoute-trip](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-platform/refs/heads/main/safe-route-boot-developer/docs/java-saferoute-trip-ddd.puml)

Trip (AggregateRoot): Controla el ciclo de vida del recorrido (métodos start(), complete()) vinculando una ruta, un conductor y una organización.
Attendance (Entity): Registra individualmente si un niño abordó o no, utilizando el Value Object BoardingState (boarded, missing, omitted).
Incident (Entity): Permite reportar cualquier problema durante el viaje, encapsulando los detalles en el Value Object IncidentDescription.

- Notifications & Communication:

![saferoute-notifications](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-platform/refs/heads/main/safe-route-boot-developer/docs/java-saferoute-notifications-ddd.puml)

Centraliza el envío de información y alertas hacia los padres de familia.
Notification (AggregateRoot): Organiza el envío de mensajes, gestionando la categoría y el estado de entrega (NotificationDeliveryState) hacia un apoderado en el contexto de un viaje específico.
Alert y Announcement (Entities): Alert se enfoca en notificaciones inmediatas o de pánico basadas en el tiempo de disparo (triggeredAt). Announcement maneja comunicados generales asociados a una ruta específica.

- Shared:

![saferoute-shared](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-platform/refs/heads/main/safe-route-boot-developer/docs/java-saferoute-shared-ddd.puml)

Actúa como el Shared Kernel transversal de toda la solución en Spring Boot.

Contiene exclusivamente Value Objects inmutables que sirven como identificadores globales (ej. OrganizationId, RouteId, ChildId) y conceptos comunes como FullName y Coordinates. Esto asegura la consistencia de los tipos de datos en la comunicación entre los distintos Bounded Contexts.

**FrontEnd**

En todos los diagramas, el componente raíz App actúa como contenedor principal: tiene composición (composes) con los componentes de cada bounded context. El manejo del estado se realiza mediante clases *Store (usando Signal<T>) , las cuales se comunican con clases *Api para las peticiones HTTP. Las clases *Assembler transforman los recursos (*Resource) de la API en modelos de dominio puro.

- Identity and Access Management:

![saferoute-iam](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-webapp/refs/heads/main/SafeRoute/docs/angular-saferoute-iam-domain.puml)
![saferoute-iam](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-webapp/refs/heads/main/SafeRoute/docs/angular-saferoute-iam-infrastructure.puml)

Gestiona la autenticación de usuarios y la configuración de la organización.

Presentation & Domain: App compone formularios de inicio de sesión (AdminLoginForm, UserLoginForm), registro (AdminRegisterForm) y gestión de organización (OrganizationForm, OrganizationProfile). Estos componentes interactúan con IamStore y consumen directamente los modelos de dominio puros (User, Organization) para reflejar y gestionar los datos de la sesión actual en la interfaz.

Application & Infrastructure: IamStore centraliza el estado con currentUserSignal y organizationSignal. Utiliza IamApi para operaciones como signIn() o createOrganization(), y UserAssembler/OrganizationAssembler para mapear las respuestas de la API (UserResource, OrganizationResource) a los modelos del dominio.

- Subscription & Plan Management:

![saferoute-subscription](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-webapp/refs/heads/main/SafeRoute/docs/angular-saferoute-subscription-domain.puml)
![saferoute-subscription](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-webapp/refs/heads/main/SafeRoute/docs/angular-saferoute-subscription-infrastructure.puml)

Maneja la visualización y selección de planes para la organización.

Presentation & Domain: App compone PlanSelector (para elegir un plan) y SubscriptionStatus. Estos componentes utilizan directamente los modelos de dominio (Subscription y Plan) como inputs para renderizar la información de negocio (como los días restantes o límites de cuota) en la UI sin depender de estructuras externas.

Application & Infrastructure: SubscriptionStore maneja subscriptionSignal y plansSignal. Se comunica con SubscriptionApi para cargar planes (getAllPlans()) o modificar la suscripción (upgradeSubscription(), cancelSubscription()), usando sus respectivos Assemblers.

- Stakeholder & Asset Management:

![saferoute-stakeholder](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-webapp/refs/heads/main/SafeRoute/docs/angular-saferoute-stakeholder-domain.puml)
![saferoute-stakeholder](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-webapp/refs/heads/main/SafeRoute/docs/angular-saferoute-stakeholder-infrastructure.puml)

Controla las vistas de listado y gestión de los actores del sistema.

Presentation & Domain: App compone componentes de lista (ParentList, DriverList, ChildList, StudentGroupList) que permiten filtrar (searchQuery), seleccionar y eliminar registros utilizando los modelos del dominio (Parent, Driver, Child, StudentGroup) como la fuente de verdad para la visualización unificada de los actores.

Application & Infrastructure: StakeholderStore maneja el estado de estas listas mediante Signals. StakeholderApi ejecuta operaciones CRUD hacia el backend, y las respuestas (ej. ParentResource) son transformadas a modelos de dominio mediante clases como ParentAssembler.

- Fleet & Route Planning:

![saferoute-fleet](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-webapp/refs/heads/main/SafeRoute/docs/angular-saferoute-fleet-domain.puml)
![saferoute-fleet](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-webapp/refs/heads/main/SafeRoute/docs/angular-saferoute-fleet-infrastructure.puml)
Interfaz para armar la logística de rutas, vehículos y asignaciones.

Presentation & Domain: App compone RouteForm (creación de rutas), StopList (gestión de paradas), VehicleList (visualización de vehículos) y AssignmentForm (asignación de conductores y niños). La interfaz gráfica se alimenta estrictamente de las entidades del dominio (Route, Stop, Vehicle, Assignment) para garantizar que la vista esté alineada con las reglas del negocio logístico.

Application & Infrastructure: FleetStore orquesta el estado de rutas, paradas, vehículos y asignaciones. FleetApi maneja las peticiones HTTP y usa Assemblers para convertir, por ejemplo, RouteResource en la entidad del dominio Route.

- Trip Execution & Monitoring:

![saferoute-trip](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-webapp/refs/heads/main/SafeRoute/docs/angular-saferoute-trip-domain.puml)
![saferoute-trip](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-webapp/refs/heads/main/SafeRoute/docs/angular-saferoute-trip-infrastructure.puml)

Pantallas operativas para el control en tiempo real de los viajes.

Presentation & Domain: App compone TripDashboard (controla inicio y fin del viaje), AttendanceChecklist (gestiona el estado de abordaje de cada niño) e IncidentForm (permite reportar incidentes). Estos componentes consumen los modelos centrales del dominio (Trip, Attendance, Incident) para reflejar de forma fidedigna el estado real de la operación.

Application & Infrastructure: TripStore centraliza el viaje actual, las asistencias y los incidentes. Delega las acciones a TripApi (ej. startTrip(), updateBoardingStatus()), apoyándose en TripAssembler, AttendanceAssembler e IncidentAssembler.

- Notifications & Communication:

![saferoute-notifications](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-webapp/refs/heads/main/SafeRoute/docs/angular-saferoute-notifications-domain.puml)
![saferoute-notifications](https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/FiveTech-NRC11896/saferoute-webapp/refs/heads/main/SafeRoute/docs/angular-saferoute-notifications-infrastructure.puml)

Centraliza la visualización y envío de notificaciones y alertas.

Presentation & Domain: App compone NotificationList (para filtrar y marcar notificaciones como leídas), AlertPanel (gestiona alertas activas y pánico) y AnnouncementForm (creación de comunicados). Las vistas dependen exclusivamente de los modelos de dominio (Notification, Alert, Announcement) para renderizar los mensajes y alertas operativas a los usuarios finales.

Application & Infrastructure: NotificationsStore maneja el estado de notificaciones, alertas y anuncios. NotificationsApi realiza las peticiones (ej. dispatchNotification(), triggerAlert()) y los Assemblers transforman los recursos recibidos en modelos limpios del dominio.
### 4.8. Database Design

**- Identity & Access Management**

Este bounded context gestiona la seguridad perimetral del sistema. La tabla `organizations` actúa como raíz estructural, siendo referenciada por prácticamente todos los demás contextos. `users` centraliza las credenciales de autenticación (`email` UNIQUE, `password_hash`) y se vincula a `organizations` y `roles` mediante FK. `roles` es una tabla de catálogo con clave `INT` que define los niveles de acceso disponibles: administrador, conductor y padre de familia.

**Tabla: organizations**
| Atributo | Tipo |
|------------|--------------|
| id | CHAR(36) (PK)|
| name | VARCHAR(100) |
| status | VARCHAR(20) |
| created_at | DATETIME |

**Métodos**
| Método | Descripción |
|---------------|--------------------------------------|
| Create() | Crea una nueva organización. |
| Activate() | Activa la organización. |
| Suspend() | Suspende la organización. |
| IsActive() | Verifica si la organización está activa. |

---

**Tabla: roles**
| Atributo | Tipo |
|----------|-------------|
| id | INT (PK) |
| name | VARCHAR(20) |

**Métodos**
| Método | Descripción |
|----------------|------------------------------------|
| GetRoleName() | Retorna el nombre del rol. |
| IsAdmin() | Verifica si el rol es administrador.|
| IsDriver() | Verifica si el rol es conductor. |
| IsParent() | Verifica si el rol es padre. |

---

**Tabla: users**
| Atributo | Tipo |
|-----------------|--------------|
| id | CHAR(36) (PK)|
| organization_id | CHAR(36) (FK)|
| role_id | INT (FK) |
| first_name | VARCHAR(100) |
| last_name | VARCHAR(100) |
| email | VARCHAR(255) |
| password_hash | VARCHAR(255) |
| created_at | DATETIME |

**Métodos**
| Método | Descripción |
|-----------------------------|------------------------------------------|
| Register() | Registra un nuevo usuario. |
| Authenticate(password) | Autentica al usuario con su contraseña. |
| ChangeRole(role) | Cambia el rol asignado al usuario. |
| GetEmail() | Retorna el email del usuario. |

---

**- Subscription & Plan Management**

Este bounded context administra el ciclo de vida comercial del servicio. La tabla `plans` es un catálogo que define los tiers disponibles y sus cuotas operativas. La tabla `subscriptions` vincula una organización a un plan y registra su estado, fecha de inicio y fecha de fin nullable, ya que una suscripción activa no tiene fecha de término definida.

**Tabla: plans**
| Atributo | Tipo |
|-------------|---------------|
| id | INT (PK) |
| plan_tier | VARCHAR(20) |
| max_routes | INT |
| max_drivers | INT |
| price | DECIMAL(10,2) |

**Métodos**
| Método | Descripción |
|---------------------------|----------------------------------------------|
| GetPlanName() | Retorna el nombre del tier del plan. |
| GetRouteLimit() | Retorna el límite de rutas del plan. |
| IsWithinRouteQuota(n) | Verifica si el valor está dentro de la cuota de rutas. |
| IsWithinDriverQuota(n) | Verifica si el valor está dentro de la cuota de conductores. |

---

**Tabla: subscriptions**
| Atributo | Tipo |
|-----------------|-------------|
| id | CHAR(36) (PK)|
| organization_id | CHAR(36) (FK)|
| plan_id | INT (FK) |
| state | VARCHAR(20) |
| start_date | DATETIME |
| end_date | DATETIME |

**Métodos**
| Método | Descripción |
|-------------------|----------------------------------------------|
| Activate() | Activa la suscripción. |
| Upgrade(planId) | Cambia el plan de la suscripción. |
| Cancel() | Cancela la suscripción. |
| GetRemainingDays()| Retorna los días restantes de la suscripción.|

---

**- Stakeholder & Asset Management**

Este bounded context maneja los perfiles de los actores críticos y los recursos físicos de la institución. Las tablas `parents` y `drivers` referencian tanto `organization_id` como `user_id` (FK hacia IAM), separando los datos de perfil de las credenciales de acceso. `children` pertenece exclusivamente a un padre mediante `parent_id` FK. `student_groups` agrupa referencias lógicas a hijos mediante la tabla de unión `student_group_children`. `vehicles` registra la flota de transporte disponible por organización.

**Tabla: parents**
| Atributo | Tipo |
|-----------------|--------------|
| id | CHAR(36) (PK)|
| organization_id | CHAR(36) (FK)|
| user_id | CHAR(36) (FK)|
| first_name | VARCHAR(100) |
| last_name | VARCHAR(100) |
| email | VARCHAR(255) |
| phone_number | VARCHAR(20) |

**Métodos**
| Método | Descripción |
|-------------------------|------------------------------------------|
| AddChild(child) | Agrega un hijo al padre. |
| RemoveChild(childId) | Elimina un hijo del padre. |
| GetChildren() | Retorna la lista de hijos del padre. |
| GetEmail() | Retorna el email del padre. |

---

**Tabla: drivers**
| Atributo | Tipo |
|-----------------|--------------|
| id | CHAR(36) (PK)|
| organization_id | CHAR(36) (FK)|
| user_id | CHAR(36) (FK)|
| first_name | VARCHAR(100) |
| last_name | VARCHAR(100) |
| email | VARCHAR(255) |
| phone_number | VARCHAR(20) |
| license_number | VARCHAR(50) |

**Métodos**
| Método | Descripción |
|------------------------------|---------------------------------------------|
| IsAvailable() | Verifica si el conductor está disponible. |
| GetLicenseNumber() | Retorna el número de licencia. |
| UpdatePhoneNumber(phone) | Actualiza el número de teléfono. |
| GetFullName() | Retorna el nombre completo del conductor. |

---

**Tabla: children**
| Atributo | Tipo |
|------------------|--------------|
| id | CHAR(36) (PK)|
| parent_id | CHAR(36) (FK)|
| first_name | VARCHAR(100) |
| last_name | VARCHAR(100) |
| age | INT |
| enrollment_state | VARCHAR(20) |

**Métodos**
| Método | Descripción |
|----------------|------------------------------------------------|
| Enroll() | Matricula al estudiante en el servicio. |
| Unenroll() | Retira la matrícula del estudiante. |
| IsEnrolled() | Verifica si el estudiante está matriculado. |
| GetFullName() | Retorna el nombre completo del estudiante. |

---

**Tabla: student_groups**
| Atributo | Tipo |
|-----------------|--------------|
| id | CHAR(36) (PK)|
| organization_id | CHAR(36) (FK)|
| name | VARCHAR(100) |
| is_finalized | BOOLEAN |

**Métodos**
| Método | Descripción |
|---------------------|-----------------------------------------------|
| AddChild(childId) | Agrega un estudiante al grupo. |
| RemoveChild(childId)| Elimina un estudiante del grupo. |
| Finalize() | Marca el grupo como finalizado. |
| GetChildCount() | Retorna la cantidad de estudiantes del grupo. |

---

**Tabla: student_group_children**
| Atributo | Tipo |
|------------------|--------------|
| student_group_id | CHAR(36) (FK)|
| child_id | CHAR(36) (FK)|

**Métodos**
| Método | Descripción |
|------------------|----------------------------------------------------|
| AssignChild() | Asocia un estudiante a un grupo. |
| RemoveChild() | Desvincula un estudiante de un grupo. |

---

**Tabla: vehicles**
| Atributo | Tipo |
|-----------------|--------------|
| id | CHAR(36) (PK)|
| organization_id | CHAR(36) (FK)|
| plate | VARCHAR(20) |
| model | VARCHAR(100) |
| brand | VARCHAR(100) |
| capacity | INT |

**Métodos**
| Método | Descripción |
|-------------------------------|------------------------------------------|
| IsAvailable() | Verifica si el vehículo está disponible. |
| GetPlate() | Retorna la placa del vehículo. |
| GetCapacity() | Retorna la capacidad del vehículo. |
| UpdateDetails(model, brand) | Actualiza los datos del vehículo. |

---

**- Route Planning & Execution**

Este bounded context coordina la planificación técnica de las rutas de transporte escolar. La tabla `routes` define cada ruta con su vehículo asignado, horario de salida y días de servicio. `stops` almacena los paraderos georreferenciados con coordenadas de alta precisión y orden de parada. `assignments` vincula una ruta con un conductor en cardinalidad 1:1, y `assignment_children` resuelve la relación muchos a muchos entre asignaciones y estudiantes.

**Tabla: routes**
| Atributo | Tipo |
|-----------------|--------------|
| id | CHAR(36) (PK)|
| organization_id | CHAR(36) (FK)|
| vehicle_id | CHAR(36) (FK)|
| name | VARCHAR(100) |
| route_state | VARCHAR(20) |
| departure_time | TIME |
| service_days | VARCHAR(100) |

**Métodos**
| Método | Descripción |
|---------------------|----------------------------------------------|
| Activate() | Activa la ruta para operación. |
| Deactivate() | Desactiva la ruta. |
| AddStop(stop) | Agrega un paradero a la ruta. |
| GetStopSequence() | Retorna la secuencia ordenada de paraderos. |

---

**Tabla: stops**
| Atributo | Tipo |
|------------|---------------|
| id | CHAR(36) (PK) |
| route_id | CHAR(36) (FK) |
| name | VARCHAR(100) |
| latitude | DECIMAL(10,8) |
| longitude | DECIMAL(11,8) |
| stop_order | INT |

**Métodos**
| Método | Descripción |
|------------------------------|----------------------------------------------|
| IsFirst() | Verifica si es el primer paradero. |
| IsLast() | Verifica si es el último paradero. |
| UpdateCoordinates(coords) | Actualiza las coordenadas del paradero. |
| GetPosition() | Retorna la posición del paradero en la ruta. |

---

**Tabla: assignments**
| Atributo | Tipo |
|-----------|--------------|
| id | CHAR(36) (PK)|
| route_id | CHAR(36) (FK)|
| driver_id | CHAR(36) (FK)|

**Métodos**
| Método | Descripción |
|-------------------------|-----------------------------------------------|
| AssignDriver(driverId) | Asigna un conductor a la ruta. |
| AssignChild(childId) | Agrega un estudiante a la asignación. |
| RemoveChild(childId) | Elimina un estudiante de la asignación. |
| GetChildCount() | Retorna la cantidad de estudiantes asignados. |

---

**Tabla: assignment_children**
| Atributo | Tipo |
|---------------|--------------|
| assignment_id | CHAR(36) (FK)|
| child_id | CHAR(36) (FK)|

**Métodos**
| Método | Descripción |
|----------------|------------------------------------------------------|
| AssignChild() | Asocia un estudiante a una asignación de ruta. |
| RemoveChild() | Desvincula un estudiante de una asignación de ruta. |

---

**- Trip Execution & Monitoring**

Este bounded context es el núcleo operativo del servicio. La tabla `trips` registra cada ejecución real de una ruta, con `start_time` y `end_time` nullable dado que el viaje puede estar en curso. `attendances` captura el estado de abordaje de cada estudiante por viaje, con `boarded_at` nullable para casos de ausencia. `incidents` referencia tanto `trip_id` como `route_id`, permitiendo trazabilidad del evento al viaje específico y a la ruta afectada.

**Tabla: trips**
| Atributo | Tipo |
|-----------------|--------------|
| id | CHAR(36) (PK)|
| organization_id | CHAR(36) (FK)|
| route_id | CHAR(36) (FK)|
| driver_id | CHAR(36) (FK)|
| trip_state | VARCHAR(20) |
| start_time | DATETIME |
| end_time | DATETIME |

**Métodos**
| Método | Descripción |
|---------------------------------|---------------------------------------------------|
| Start() | Inicia el viaje. |
| Complete() | Completa el viaje. |
| RecordBoarding(childId, state) | Registra el estado de abordaje de un estudiante. |
| IsInProgress() | Verifica si el viaje está en curso. |

---

**Tabla: attendances**
| Atributo | Tipo |
|----------------|--------------|
| id | CHAR(36) (PK)|
| trip_id | CHAR(36) (FK)|
| child_id | CHAR(36) (FK)|
| boarding_state | VARCHAR(20) |
| boarded_at | DATETIME |

**Métodos**
| Método | Descripción |
|------------------------------|-------------------------------------------------|
| UpdateBoardingState(state) | Actualiza el estado de abordaje del estudiante. |
| IsBoarded() | Verifica si el estudiante abordó. |
| GetBoardingTime() | Retorna la hora de abordaje. |

---

**Tabla: incidents**
| Atributo | Tipo |
|-------------|--------------|
| id | CHAR(36) (PK)|
| trip_id | CHAR(36) (FK)|
| route_id | CHAR(36) (FK)|
| description | TEXT |
| reported_at | DATETIME |

**Métodos**
| Método | Descripción |
|--------------------|-----------------------------------------|
| Report() | Registra el incidente. |
| GetDescription() | Retorna la descripción del incidente. |
| GetReportedAt() | Retorna la fecha de reporte. |

---

**- Notifications & Communication**

**Tabla: notifications**
| Atributo | Tipo |
|-----------------|--------------|
| id | CHAR(36) (PK)|
| organization_id | CHAR(36) (FK)|
| parent_id | CHAR(36) (FK)|
| trip_id | CHAR(36) (FK)|
| category | VARCHAR(20) |
| delivery_state | VARCHAR(20) |
| message | TEXT |
| sent_at | DATETIME |

**Métodos**
| Método | Descripción |
|------------------|----------------------------------------------------|
| Queue() | Encola la notificación para su envío. |
| Dispatch() | Despacha la notificación al destinatario. |
| MarkDelivered() | Marca la notificación como entregada. |
| GetCategory() | Retorna la categoría de la notificación. |

---

**Tabla: alerts**
| Atributo | Tipo |
|-----------------|--------------|
| id | CHAR(36) (PK)|
| notification_id | CHAR(36) (FK)|
| triggered_at | DATETIME |

**Métodos**
| Método | Descripción |
|-------------------|----------------------------------------|
| Trigger() | Activa la alerta. |
| IsPanic() | Verifica si la alerta es de pánico. |
| GetTriggeredAt() | Retorna la hora en que se activó. |

---

**Tabla: announcements**
| Atributo | Tipo |
|-----------------|--------------|
| id | CHAR(36) (PK)|
| notification_id | CHAR(36) (FK)|
| route_id | CHAR(36) (FK)|
| message | TEXT |
| published_at | DATETIME |

**Métodos**
| Método | Descripción |
|-------------------|-----------------------------------------------|
| Publish() | Publica el comunicado. |
| GetMessage() | Retorna el contenido del comunicado. |
| GetPublishedAt() | Retorna la fecha de publicación. |

#### 4.8.1. Database Diagrams

Esta sección presenta y explica los Database Diagrams para cada bounded context de SafeRoute. Los diagramas modelan la persistencia relacional del sistema, especificando tablas, columnas, tipos de dato, constraints (PK, FK, NOT NULL, UNIQUE) y las relaciones entre tablas con su cardinalidad. Todos los identificadores primarios utilizan `CHAR(36)` para soportar UUIDs, a excepción de catálogos fijos como `roles` y `plans` que usan `INT`. Las relaciones entre bounded contexts se materializan mediante columnas FK que referencian los IDs del contexto origen.
![DataBase](/assets/images/ChapterIV/DataBase/SafeRoute-DataBase.png)

**Identity and Access Management**

El bounded context de IAM persiste las entidades centrales de identidad y acceso. La tabla `organizations` actúa como raíz del sistema, siendo referenciada por prácticamente todos los demás contextos. `users` centraliza las credenciales de autenticación (`email` UNIQUE, `password_hash`) y se vincula a `organizations` y `roles` mediante FK. `roles` es una tabla de catálogo con clave `INT` que define los niveles de acceso disponibles en el sistema.

![DataBase](/assets/images/ChapterIV/DataBase/DbIAM.png)

---

**SafeRoute.Subscription**

Este contexto gestiona los planes comerciales y el estado de suscripción de cada organización. La tabla `plans` es un catálogo con `INT` PK que define los tiers disponibles y sus cuotas (`max_routes`, `max_drivers`, `price`). `subscriptions` vincula una organización a un plan mediante FK y registra el ciclo de vida de la suscripción a través de `state`, `start_date` y `end_date` (nullable, ya que una suscripción activa no tiene fecha de fin definida).

![DataBase](/assets/images/ChapterIV/DataBase/DbSubscription.png)

---

**Stakeholder & Asset Management**

Este contexto persiste los actores humanos del sistema. `parents` y `drivers` referencian tanto `organization_id` como `user_id` (FK hacia IAM), separando los datos de perfil de las credenciales de acceso. `children` pertenece exclusivamente a un padre mediante `parent_id` FK. `student_groups` agrupa referencias lógicas a hijos a través de la tabla de unión `student_group_children`, que resuelve la relación muchos a muchos entre grupos y niños con `student_group_id` + `child_id` como clave compuesta.

![DataBase](/assets/images/ChapterIV/DataBase/DbStakeHolder.png)

---

**Fleet & Route Planning**

Este contexto modela la infraestructura operativa de transporte. `vehicles` pertenece a una organización y se asigna a rutas mediante FK en `routes`. `routes` almacena `departure_time` como `TIME` y `service_days` como `VARCHAR` serializado. `stops` define los puntos geográficos de cada ruta con coordenadas decimales de alta precisión (`DECIMAL(10,8)` y `DECIMAL(11,8)`) y un `stop_order` para secuenciamiento. `assignments` relaciona una ruta con un conductor en cardinalidad 1:1, y `assignment_children` resuelve la relación muchos a muchos entre asignaciones y niños.

![DataBase](/assets/images/ChapterIV/DataBase/DbFleet.png)

---

**Trip Execution & Monitoring**

Este contexto registra la ejecución operativa de cada viaje. `trips` referencia `organization_id`, `route_id` y `driver_id` como FK, con `start_time` y `end_time` nullable dado que el viaje puede estar en curso. `attendances` registra el estado de embarque de cada niño por viaje (`trip_id` + `child_id`), con `boarded_at` nullable para casos de ausencia. `incidents` referencia tanto `trip_id` como `route_id`, permitiendo trazabilidad del incidente tanto al viaje específico como a la ruta afectada.

![DataBase](/assets/images/ChapterIV/DataBase/DbTrip.png)

---

**Notifications & Communication**

Este contexto gestiona la comunicación hacia los padres. `notifications` referencia `organization_id`, `parent_id` y `trip_id`, registrando `category`, `delivery_state` y `message` con `sent_at` obligatorio. `alerts` pertenece a una notificación mediante `notification_id` FK y registra el momento exacto del disparo. `announcements` extiende la notificación con una referencia adicional a `route_id`, permitiendo comunicados asociados a una ruta específica con su propio `message` y `published_at`.

![DataBase](/assets/images/ChapterIV/DataBase/DbNotifications.png)

---

## Capítulo V: Product Implementation, Validation & Deployment

### 5.1. Software Configuration Management

#### 5.1.1. Software Development Environment Configuration

En esta sección se describen las herramientas y tecnologías utilizadas para el desarrollo del Proyecto

##### UX/UI Design 

###### Figma: 
Herramienta de diseño colaborativo utilizada para la creación de wireframes, mockups, prototipos y diseño de interfaces. Permite trabajar en equipos en tiempo real, lo cual facilita la validación temprana de la experiencia futura del usuario.

##### Software Development

###### JetBrains Intelli J IDEA

Entorno de desarrollo integrado (IDEA) utilizado para el desarrollo del BackEnd que utiliza el idioma java.

###### GitHub

Plataforma de control de versiones utilizada para la gestión del código fuente y colaboración del equipo, implementando la metodología GitFlow para la organización del desarrollo.

###### HTML

Legnuaje de marcado para el desarrollo de las interfaces web del Frontend.

###### CSS

Lenguaje de estilos utilizados para la presentación visual de la aplicación, en el apartado del .

###### Typescript

Lenguaje utilizado para el frontend para poder hacer interfaces dinámicas e interactivas.

###### Java

Lenguaje de programación que se utilizara en el desarrollo del backend de la aplicación.

##### Software Deployment

###### GitHub Pages
Servicio utilizado para el despliegue de la landing page del proyecto.

###### Vercel
Plataforma utilizada para el despliegue del frontend desarrollado en Vue.js, permitiendo una integración continua y despliegue automatizado.

###### Railway
Plataforma utilizada para el despliegue de servicios backend y APIs, facilitando la conexión entre frontend y backend en un entorno accesible en la nube.


#### 5.1.2. Source Code Management

Para el manejo del código fuente, utilizamos Github para colaborar entre miembros de equipo en multiples repositorios. A continuación, se listan los enlaces de cada repositorio:

Organización:

Repositorio de Landing Page: https://github.com/FiveTech-NRC11896/safedrive-website.git

Repositorio del informe: https://github.com/FiveTech-NRC11896/safedrive-report.git

Repositorio del frontend: https://github.com/FiveTech-NRC11896/safedrive-webapp.git

Repositorio del backend: https://github.com/FiveTech-NRC11896/safedrive-platform.git

En el repositorio del informe, se implementa un esquema de trabajo basado en Gitflow. La rama main almacena la versión estable del informe correspondiente a cada entregable del trabajo, mientras que la rama develop concentra la integración de avances validados por cada integrante antes de su consolidación final. A partir de develop, cada integrante creará ramas feature de trabajo para las secciones asignadas. Las ramas feature seguirán una nomenclatura asociada al capítulo o bloque trabajado, por ejemplo: feature/chapter-1-introduction-and-lean-ux, o feature/chapter-5-software-configuration-management. Esta convención permite identificar con claridad qué parte del informe está siendo desarrollada y reduce el riesgo de conflictos entre los miembros del equipo.

En los repositorios del Landing Page, Frontend y Backend también se utilizará GitFlow. En cada uno de ellos, la rama main contendrá las versiones estables del producto y la rama develop servirá como rama de integración del trabajo colaborativo. A partir de develop, se crearán ramas feature/... para el desarrollo de funcionalidades específicas. A diferencia del informe, en estos repositorios las ramas no estarán organizadas por capítulos, sino por funcionalidades o componentes del sistema. Algunos ejemplos de nomenclatura son: feature/home-page, feature/dashboard o feature/route-management. Esta convención nos permite que las ramas reflejen de manera directa el alcance funcional del producto en desarrollo.

No se realizarán cambios directos sobre la rama main, ya que esta representará únicamente versiones estables y listas para consolidarse como parte de un entregable. Del mismo modo, se evitará que los integrantes trabajen de forma continua directamente sobre la rama develop, ya que el flujo previsto consiste en desarrollar primero en ramas feature, integrar luego en develop y finalmente consolidar en main cuando el avance haya sido revisado y validado. Por tanto, el flujo general de trabajo será de la siguiente forma: feature → develop → main. Este esquema se alinea con la exigencia del curso de explicar la implementación de GitFlow mediante ramas principales, ramas de features, y convenciones para releases y hotfixes.

Asimismo, si se requiere corregir errores críticos sobre una versión estable, se podrán crear ramas hotfix/..., y si se decide preparar una versión de cierre antes de una entrega, se utilizarán ramas release/... de acuerdo con el flujo definido por GitFlow.

En relación con los mensajes de cada commit, el equipo aplicará Conventional Commits para mantener un historial más legible, consistente y profesional. Esta convención facilitará la revisión de avances y permitirá identificar rápidamente el propósito de cada uno de los cambios. Algunos prefijos que se utilizarán son:

feat: incorporación de una nueva funcionalidad
fix: corrección de errores
docs: cambios en documentación
style: cambios de formato o estilo sin alterar lógica
refactor: reorganización interna sin agregar funcionalidad nueva
test: incorporación o ajuste de pruebas
chore: tareas de mantenimiento o configuración

Para el repositorio del informe se emplearán mensajes como docs(report): add project cover page o docs: add startup profile and lean ux process for chapter 1. Para los repositorios de software se utilizarán mensajes como feat: add school route registration, feat: implement student assignment to route o fix: correct login validation. Esta práctica contribuye a que la evidencia de commits sea coherente con el trabajo realizado por cada miembro.


#### 5.1.3. Source Code Style Guide & Conventions

#### Frontend (Landing Page - HTML, CSS, JavaScript)

##### Convenciones generales:

- **Idioma**: Todo el código, incluyendo nombres de variables, funciones y clases está escrito en inglés.
- **Formato de archivos**: `.html`, `.css`, `.js`
- **Estilo de código adoptado**:
  - [W3Schools HTML Style Guide](https://www.w3schools.com/html/html5_syntax.asp)
  - [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html)

##### Nomenclatura:

- **Clases CSS**: `kebab-case` (ej. `main-container`)
- **IDs HTML**: `camelCase` (ej. `mainContent`)
- **Variables JS**: `camelCase` (ej. `userName`)
- **Funciones JS**: `camelCase` (ej. `handleClick()`)

#### Frontend Web App (Angular + TypeScript)

##### Convenciones generales:

- **Idioma**: Código y los comentarios son completamente en ingles.
- **Estructura de carpetas**: Segregación por módulos y componentes.
- **Formato de archivos**: `.ts`, `.html`, `.css`

##### Estilo de código adoptado:

- [Angular Style Guide (Oficial)](https://angular.io/guide/styleguide)
- [Google TypeScript Style Guide](https://google.github.io/styleguide/tsguide.html)

##### Nomenclatura:

- **Componentes**: `PascalCase` (ej. `UserProfileComponent`)
- **Servicios**: `camelCase` + sufijo `Service` (ej. `authService`)
- **Interfaces**: `PascalCase`, prefijo `I` opcional (ej. `User`, `IUser`)
- **Archivos**: `kebab-case` (ej. `user-profile.component.ts`)
- **Variables y funciones**: `camelCase`

#### Backend (Java + Spring Boot)

##### Convenciones generales:

- **Idioma**: Código y documentación interna es en ingles.
- **Formato de archivos**: `.java`

##### Estilo de código adoptado:

- [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)
- [Spring Boot Features &amp; Best Practices](https://docs.spring.io/spring-boot/docs/current/reference/html/features.html)

##### Nomenclatura:

- **Clases**: `PascalCase` (ej. `UserService`)
- **Variables**: `camelCase` (ej. `userRepository`)
- **Constantes**: `UPPER_SNAKE_CASE` (ej. `MAX_USERS`)
- **Endpoints**: `kebab-case` para URLs (ej. `/api/user-profile`)
- **Paquetes**: Todo en minúsculas y separados por punto (ej. `com.project.backend.controller`)

#### 5.1.4. Software Deployment Configuration

En esta sección se describe la configuración necesaria para el despliegue de los principales componentes del proyecto: Landing Page, Frontend Web Application y Backend.
#### Despliegue de Landing Page

La Landing Page fue desarrollada utilizando HTML, CSS y JavaScript, y será desplegada mediante GitHub Pages, un servicio de hosting para sitios estáticos.

##### Pasos de despliegue

Crear un repositorio en GitHub destinado a la landing page.
Subir el código fuente (HTML, CSS, JS y recursos estáticos) al repositorio.
Asegurar que el archivo principal se denomine index.html y se encuentre en la raíz del proyecto.
Acceder a la sección Settings > Pages del repositorio.
Seleccionar la rama main (o master) y la carpeta raíz (/) como fuente.
GitHub generará automáticamente una URL pública para acceder a la landing page.
URL desplegada: Pendiente

##### Despliegue de Frontend Web Application
El frontend de la aplicación, desarrollado con Vue.js, será desplegado utilizando la plataforma Vercel, la cual permite integración continua y despliegue automatizado.

Pasos de despliegue
Crear o seleccionar el repositorio del frontend en GitHub.
Vincular el repositorio con la plataforma Vercel.
Configurar el entorno de despliegue (framework Vue.js).
Ejecutar el despliegue automático desde Vercel.
Obtener la URL pública generada para el acceso a la aplicación.
URL desplegada: Pendiente

##### Despliegue de Backend Services
El backend del sistema, desarrollado en C#, será desplegado utilizando Railway, una plataforma que permite exponer servicios y APIs en la nube.
Pasos de despliegue:
Crear el repositorio del backend en GitHub.
Vincular el repositorio con Railway.
Configurar las variables de entorno necesarias para la ejecución del backend.
Configurar el servicio para exponer endpoints API.
Desplegar el servicio y obtener la URL pública del backend.
URL desplegada: Pendiente

### 5.2. Landing Page, Services & Applications Implementation

#### 5.2.1. Sprint 1

##### 5.2.1.1. Sprint Planning 1

| Sprint # | Sprint 1 |
|----------|---------|
| **Sprint Planning Background** |
| Date | 2026-04-24 |
| Time | 07:00 PM |
| Location | Microsoft Teams |
| Prepared By | Renzo Revilla |
| Attendees (to planning meeting) | Todo el equipo |
| Sprint 0 Review Summary | Al tratarse del inicio del proyecto, no se cuenta con un sprint previo. Sin embargo, se definieron las bases del proyecto, incluyendo la configuración inicial del entorno y la estructura del repositorio. |
| Sprint 0 Retrospective Summary | El equipo identificó la importancia de una correcta organización y distribución de tareas desde el inicio del proyecto. Se acordó mejorar la comunicación y planificación para optimizar el desarrollo en los siguientes sprints. |
| **Sprint Goal & User Stories** | |
| Sprint 1 Goal | Nuestro enfoque es permitir que los nuevos usuarios comprendan la propuesta de valor de SafeRoute mediante una primera versión del landing page. Creemos que esto aporta claridad y genera confianza inicial en los potenciales usuarios de la plataforma. Esto se validará cuando los usuarios puedan acceder al landing page e identificar claramente sus funcionalidades principales y su propósito. |
| Sprint 1 Velocity | 15 Story Points |
| Sum of Story Points | 13 Story Points |

##### 5.2.1.2. Aspect Leaders and Collaborators

| Team Member (Last Name, First Name) | GitHub Username Leader (L) / Collaborator (C) | Landing Page Leader (L) / Collaborator (C) | UI Design Leader (L) / Collaborator (C) | Deployment Leader (L) / Collaborator (C) | Repo Management Leader (L) / Collaborator (C) |
| - | - | - | - | - | - |
| Revilla Quispe, Renzo Zamir | renzorevq24 | L | C | C | C |
| Quispe Serrano, Julio Frank | FraSe-JQ | C | C | C | L |
| Costa Morales, Christofer William | miniChorri | C | C | L | C |
| De La Cruz De Los Santos, Mathias Marcelo | Dela050406 | L | C | C | C |
| Ortega Quintana, José Zacarías | AgoxX61 | C | L | C | C |

##### 5.2.1.3. Sprint Backlog 1

| User Story ID | User Story Title | Task ID | Task Title | Description | Estimation (Hours) | Assigned To | Status |
|---------------|------------------|---------|------------|-------------|--------------------|-------------|--------|
| US19 | Visualización de Hero | T01 | Implementar Hero Section | Desarrollo de la sección principal con propuesta de valor y mensaje inicial del producto | 3 | Julio | Done |
| US22 | Consulta de Precios | T05 | Implementar Plans Section | Creación de sección de planes de suscripción con características comparativas | 3 | Julio | Done |
| US20 | Navegación de Funciones | T02 | Implementar Navbar | Creación de barra de navegación con enlaces a secciones del Landing Page | 2 | José | Done |
| US19 | Visualización de Hero | T07 | Implementar CTA y Footer | Desarrollo de llamadas a la acción y pie de página del sitio | 2 | José | Done |
| US20 | Navegación de Funciones | T03 | Implementar Features Section | Desarrollo de sección de funcionalidades principales del sistema | 3 | Mathias | Done |
| US21 | Detalle de Roles | T04 | Implementar Roles Section | Desarrollo de sección que describe los tipos de usuarios (Admin, Conductor, Padre) | 3 | Mathias | Done |
| US23 | ¿Cómo funciona? | T06 | Implementar How it Works Section | Desarrollo del flujo explicativo del funcionamiento del sistema | 2 | Christofer | Done |
| US23 | ¿Cómo funciona? | T06 | Implementar How it Works Section (Styles) | Aplicación de estilos visuales a la sección "How it Works" | 2 | Christofer | Done |
| US20 | Navegación de Funciones | T08 | Implementar Responsive Design | Adaptación del Landing Page para diferentes dispositivos | 3 | Christofer | Done |
| US20 | Navegación de Funciones | T08 | Implementar Responsive Design (i18n) | Implementación de archivos de traducción para múltiples idiomas | 2 | Christofer | Done |
| US20 | Navegación de Funciones | T08 | Implementar Responsive Design (Script) | Desarrollo de script para comportamiento responsive y cambio de idioma | 2 | Christofer | Done |

##### 5.2.1.4. Development Evidence for Sprint Review

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Commited on (Date) |
|-----------|--------|----------|----------------|---------------------|--------------------|
| saferoute-landing-page | develop | d7f8ce0 | docs: add README content | Documentation update | 2026-04-19 |
| saferoute-landing-page | develop | 9b9fa84 | chore: update meta tags | SEO improvements | 2026-04-19 |
| saferoute-landing-page | develop | a66ef43 | docs: add images to README for landing page section | Documentation images added | 2026-04-19 |
| saferoute-landing-page | develop | 1832739 | feat: add roles and features sections | Roles and features added | 2026-04-19 |
| saferoute-landing-page | develop | 293e76c | Merge branch 'feature/responsive' into develop | Integration of responsive features | 2026-04-19 |
| saferoute-landing-page | develop | 655723b | Merge branch 'feature/footer' into develop | Integration of footer section | 2026-04-19 |
| saferoute-landing-page | develop | 916d89c | Merge branch 'feature/howworks' into develop | Integration of how it works section | 2026-04-19 |
| saferoute-landing-page | develop | 61be65c | Merge branch 'feature/plans' into develop | Integration of plans feature | 2026-04-19 |
| saferoute-landing-page | develop | f5c00dc | Merge branch 'feature/hero' into develop | Integration of hero feature | 2026-04-19 |
| saferoute-landing-page | feature/responsive | 0393e68 | feat: added script.js file for translation and responsive | Script integration | 2026-04-19 |
| saferoute-landing-page | feature/responsive | 96623f1 | feat: Added all the json for the translation | Translation files added | 2026-04-19 |
| saferoute-landing-page | feature/responsive | ca60a34 | feat: Added .js file for responsive and button for changing language | Responsive behavior added | 2026-04-19 |
| saferoute-landing-page | feature/footer | 25c96ca | feat: add footer section with links and contact info | Footer section created | 2026-04-19 |
| saferoute-landing-page | feature/navbar | 7311e9d | feat: implement landing navigation section | Navbar implementation | 2026-04-19 |
| saferoute-landing-page | feature/howworks | 9d7047d | feat: Added the styles to the "How It Works" section | Styling applied | 2026-04-18 |
| saferoute-landing-page | feature/howworks | 8d7f3d6 | feat: Added How it Works section to index.html | Section structure added | 2026-04-18 |
| saferoute-landing-page | feature/plans | d294def | feat: add pricing plans section | Pricing section added | 2026-04-18 |
| saferoute-landing-page | feature/hero | e0c7125 | feat: add hero section with main headline and call to action | Hero section implementation | 2026-04-18 |
| saferoute-landing-page | develop | bc93887 | chore: initialize project structure for landing page | Initial setup of project structure | 2026-04-18 |

##### 5.2.1.5. Execution Evidence for Sprint Review

El desarrollo abarcó la implementación de las principales secciones del sitio, incluyendo la sección de roles de usuario, la sección de planes de suscripción, la sección ¿Como funciona?, así como componentes complementarios como el footer. Estas secciones permiten al usuario comprender el propósito del sistema, sus beneficios y las principales funcionalidades disponibles.

Asimismo, se implementó diseño responsivo, garantizando que la experiencia de usuario sea consistente y accesible desde distintos dispositivos.

A continuación, se presentan capturas de las principales vistas implementadas durante el Sprint:

![Landing Page - Hero](./assets/images/hero.png)
*Nota. Captura de pantalla de la sección Hero del Landing Page de SafeRoute, donde se presenta la propuesta de valor principal. Elaboración propia.*

![Landing Page - Features](./assets/images/features.png)
*Nota. Captura de pantalla de la sección de funcionalidades (Features) del Landing Page de SafeRoute, donde se describen las principales capacidades del sistema. Elaboración propia.*

![Landing Page - Roles](./assets/images/roles.png)
*Nota. Captura de pantalla de la sección de roles de usuario del Landing Page de SafeRoute, donde se explican los perfiles de Administrador, Conductor y Padre. Elaboración propia.*

![Landing Page - Plans](./assets/images/plans.png)
*Nota. Captura de pantalla de la sección de planes de suscripción del Landing Page de SafeRoute, donde se presentan las opciones disponibles para los usuarios. Elaboración propia.*

![Landing Page - Responsive](./assets/images/responsive.png)
*Nota. Captura de pantalla del diseño responsivo del Landing Page de SafeRoute en dispositivos móviles, evidenciando la adaptabilidad de la interfaz. Elaboración propia.*

##### 5.2.1.6. Services Documentation Evidence for Sprint Review

En este Sprint no se desarrollaron servicios RESTful, ya que el enfoque estuvo centrado en la implementación del Landing Page de SafeRoute.

La construcción de APIs será abordada en los siguientes Sprints, donde se integrará la lógica del sistema y la comunicación con la base de datos.

##### 5.2.1.7. Software Deployment Evidence for Sprint Review

El proceso de despliegue consistió en la configuración del repositorio en GitHub, habilitando la opción de GitHub Pages y estableciendo la rama principal como fuente de publicación. Esto permitió que cada cambio realizado en el repositorio se refleje automáticamente en el entorno de producción.

Como resultado, el Landing Page se encuentra disponible para su acceso y validación por parte de los usuarios, cumpliendo con el objetivo de presentar la propuesta de valor del producto en un entorno real.

A continuación, se presentan capturas del proceso y resultado del despliegue:

![GitHub Pages Config](./assets/images/github-pages.png)
*Nota. Captura de la configuración de GitHub Pages en el repositorio del proyecto. Elaboración propia.*

El Landing Page desplegado se encuentra disponible en el siguiente enlace:

https://fivetech-nrc11896.github.io/saferoute-landing-page/

##### 5.2.1.8. Team Collaboration Insights during Sprint

Durante el desarrollo del Sprint 1, el equipo implementó un flujo de trabajo basado en GitFlow, el cual permitió organizar de manera eficiente el desarrollo colaborativo del Landing Page del proyecto SafeRoute.

El proceso de desarrollo se estructuró de la siguiente manera:

- Cada integrante trabajó de forma independiente en una rama específica de tipo **feature**, destinada a una funcionalidad concreta del sistema (por ejemplo: `feature/hero`, `feature/navbar`, `feature/plans`, `feature/howworks`, `feature/responsive`).
- Una vez finalizado el desarrollo de cada funcionalidad, estas ramas fueron integradas en la rama **develop**, la cual actúa como rama de consolidación del proyecto.
- Posteriormente, la rama **develop** fue utilizada como base para la integración final hacia la rama **main**, donde se mantiene la versión estable del Landing Page.

Este flujo permitió:
- Trabajar en paralelo sin conflictos entre integrantes
- Mantener control sobre los cambios realizados
- Garantizar la estabilidad del producto antes de su versión final

A continuación, se presentan capturas que evidencian la actividad del equipo durante el Sprint:

![Pulse](./assets/images/pulse.png)

*Nota. Panel de analíticos del repositorio. Elaboración propia.*

![Network Graph](./assets/images/network.png)

*Nota. Gráfico de red que evidencia el flujo de trabajo basado en ramas feature integradas en develop y posteriormente fusionadas en main durante el Sprint. Elaboración propia.*


![Contributors](./assets/images/contributors.png)

*Nota. Analíticos de contribución por integrante del repositorio durante el Sprint 1. Elaboración propia.*

![Commits](./assets/images/commits.png)

*Nota. Historial de commits del repositorio evidenciando la participación de los integrantes del equipo. Elaboración propia.*

![Feature Branches](./assets/images/branches.png)

*Nota. Evidencia del uso de ramas feature dentro del flujo de trabajo GitFlow, mostrando el desarrollo independiente de funcionalidades. Elaboración propia.*

## Conclusiones

### Conclusiones y recomendaciones

El equipo logró desarrollar el Landing Page de SafeRoute cumpliendo con los objetivos del Sprint, estructurando adecuadamente la propuesta de valor en secciones clave como Hero, Features, Roles, Planes y How It Works. A partir de los Problem Statements y assumptions, se priorizó una comunicación clara y una navegación intuitiva, alineadas a las necesidades del usuario. Asimismo, se aplicó correctamente el enfoque Lean UX mediante un desarrollo incremental y colaborativo, evidenciado en el uso de Git con ramas feature integradas en develop y posteriormente en main.

### Video About-the-Team

## Bibliografía

- Autoridad de Transporte Urbano para Lima y Callao. (2024). _Cifra de movilidades escolares autorizadas disminuyó en 25% en un año_. El Comercio. Recuperado el 9 de abril de 2026, de https://elcomercio.pe/lima/cifra-de-movilidades-escolares-autorizadas-disminuyo-en-25-en-un-ano-a-que-se-debe-esta-reduccion-informe-movilidad-escolar-noticia/

- Ministerio de Educación. (2023). _Resultados del Censo Educativo 2022_. ESCALE. Recuperado el 9 de abril de 2026, de https://escale.minedu.gob.pe/documents/10156/9345030/PPT_Censo_Educativo_2023_final.pdf

- Superintendencia de Transporte Terrestre de Personas, Carga y Mercancías. (2024). _Sutran (MTC) sensibilizó a más de 47 000 escolares sobre seguridad vial_. Gob.pe. Recuperado el 9 de abril de 2026, de https://www.gob.pe/institucion/sutran/noticias/1255228-sutran-mtc-sensibilizo-a-mas-de-47-000-escolares-sobre-seguridad-vial-en-lo-que-va-del-2025

## Anexos
