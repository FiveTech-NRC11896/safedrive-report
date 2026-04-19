![Logo UPC](assets/images/LogoUpc.png)

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
**Nombre del producto:** SafeDrive

**Relación de integrantes:**

- U20XXXXXXXX - [Apellidos, Nombres]
- U201717085 - Revilla Quispe, Renzo Zamir
- U20241D922 - Quispe Serrano, Julio Frank
- U20XXXXXXXX - [Apellidos, Nombres]
- U202316852 - Ortega Quintana, José Zacarias

**Abril, 2026**

---

## Registro de Versiones del Informe

| Avance | Fecha      | Autor | Descripción de Modificación |
| :----- | :--------- | :---- | :-------------------------- |
| AV1    | --/04/2026 | "-"   | "-"                         |

---

## Project Report Collaboration Insights

El equipo ha utilizado un flujo de trabajo en github: [safedrive-report](https://github.com/FiveTech-NRC11896/safedrive-report)

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

|                Foto                | Apellidos y Nombres         |    Código     | Carrera                | Resumen                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| :--------------------------------: | :-------------------------- | :-----------: | :--------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|              ![foto]               | [Apellido 1], [Nombre 1]    | [U20XXXXXXXX] | Ingeniería de Software | [Descripción de conocimientos técnicos y habilidades que aporta al equipo]                                                                                                                                                                                                                                                                                                                                                                             |
|              ![Renzo Revilla](./assets/images/renzo.png)              | Revilla Quispe, Renzo Zamir   | U201717085 | Ingeniería de Software | Soy Renzo Revilla, estudiante de Ingenieria de Software en la Universidad Peruana de Ciencias Aplicadas, con experiencia en desarrollo web y movil. Me destaco por mis habilidades en comunicacion efectiva y trabajo en equipo, lo que facilita la coordinación y el cumplimiento de objetivos dentro del grupo. Disfruto de la natacion y del aprendizaje continuo. Mi aporte al equipo se centra en el desarrollo tecnico y en la gestion del proyecto, contribuyendo a mantener un trabajo organizado y eficiente.  |
| ![foto](assets/images/FrankFT.png) | Quispe Serrano, Julio Frank | [U20241D922]  | Ingeniería de Software | Mi nombre es Julio Frank Quispe Serrano, tengo 20 años,actualmente estoy cursando el 5to ciclo de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Soy un apasionado por la programación, el gym y explorador de música en distintos géneros. Mi aporte en este grupo será el de brindar soluciones prácticas y eficientes ante situaciones de adversidad que estanquen la fluidez de la elaboración del trabajo. |
|              ![foto]               | [Apellido 4], [Nombre 4]    | [U20XXXXXXXX] | Ingeniería de Software | [Descripción de conocimientos técnicos y habilidades que aporta al equipo]                                                                                                                                                                                                                                                                                                                                                                             |
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
*Nota.* Adaptado de Resultados del Censo Educativo 2022 (p. 12), por Ministerio de Educación, 2023.


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
Los padres de familia con hijos en nivel inicial, kínder y primaria que utilizan un servicio de transporte escolar ya contratado, y los transportistas escolares  como por ejemplo los conductores independientes o responsables de pequeñas empresas que operan ese servicio. Dentro de la plataforma, cualquiera de estos segmentos puede asumir además el rol de Administrador.
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
| Sección | Contenido |
| :----- | :--------- |
| 1. Business Problem | El transporte escolar privado en el Perú opera de forma tradicional y sin soporte tecnológico. Los padres no tienen visibilidad sobre el trayecto de sus hijos y los transportistas gestionan su operación con llamadas, WhatsApp y hojas privadas, lo que genera errores, ineficiencia y una experiencia de servicio poco confiable.|
| 2. Business Outcomes| Lograr que el 75% de administradores completen el registro de su operación en los primeros 15 días. Retener al 80% de suscriptores activos durante los primeros 3 meses. Alcanzar una tasa de upgrade del plan Básico al Intermedio del 20% en los primeros 3 meses de uso.|
| 3. Users | Los segmentos que interactúan con SafeRoute son los padres de familia con hijos en nivel inicial, kínder y primaria que utilizan un servicio de transporte escolar ya contratado, y los transportistas escolares conductores independientes o responsables de pequeñas empresas que operan ese servicio. Cualquiera de estos puede asumir además el rol de Administrador dentro de la plataforma.|
| 4. User Outcomes & Benefits | Los padres buscan reducir su incertidumbre sobre el trayecto de sus hijos, pudiendo monitorear el estado del viaje sin necesidad de interrumpir al conductor. Los transportistas buscan gestionar rutas, alumnos e incidencias de forma digital, reduciendo errores operativos y proyectando mayor profesionalismo frente a las familias. Quienes asumen el rol de administrador buscan centralizar toda la operación del servicio en un solo panel, eliminando la coordinación manual y el uso de herramientas desconectadas.|
| 5. Solution Ideas | Ofrecemos un panel de administración de usuarios, conductores, hijos y rutas. Tambien, Check-list de abordaje digital por conductor. Vista de paradas y estado del trayecto para padres. Registro de incidencias por ruta. Historial de trayectos por comunidad de ruta. Seguimiento GPS en tiempo real (plan Completo). Apertura a integración IoT futura.|
| 6. Hypotheses | - Si ofrecemos a los padres una vista de estado del trayecto, al menos el 70% la consultará diariamente en las primeras 4 semanas.<br> - Si ofrecemos al conductor una interfaz operativa simple, el 80% de los trayectos tendrán el check-list completado en las primeras 4 semanas.<br> - Si ofrecemos al administrador un panel único de gestión, el 75% completará su registro en los primeros 15 días.<br> - Si demostramos el valor del plan Intermedio, el 20% de administradores del plan Básico harán upgrade en los primeros 3 meses.|
| 7. What's the most important thing we need to learn first? | ¿El administrador del servicio percibe suficiente valor en SafeRoute como para abandonar los métodos informales actuales y pagar una suscripción mensual?|
| 8. What's the least amount of work we need to do to learn the next most important thing? | Realizar entrevistas con 3 a 5 administradores de servicios de transporte escolar (padres representantes o transportistas independientes) para validar su disposición al cambio y las funcionalidades que consideran imprescindibles antes de desarrollar el MVP.|

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

### 3.2. Impact Mapping

### 3.3. Product Backlog

---

## Capítulo IV: Product Design

### 4.1. Style Guidelines

#### 4.1.1. General Style Guidelines

#### 4.1.2. Web Style Guidelines

### 4.2. Information Architecture

#### 4.2.1. Organization Systems

#### 4.2.2. Labeling Systems

#### 4.2.3. SEO Tags and Meta Tags

#### 4.2.4. Searching Systems

#### 4.2.5. Navigation Systems

### 4.3. Landing Page UI Design

#### 4.3.1. Landing Page Wireframe

#### 4.3.2. Landing Page Mock-up

### 4.4. Web Applications UX/UI Design

#### 4.4.1. Web Applications Wireframes

#### 4.4.2. Web Applications Wireflow Diagrams

#### 4.4.2. Web Applications Mock-ups

#### 4.4.3. Web Applications User Flow Diagrams

### 4.5. Web Applications Prototyping

### 4.6. Domain-Driven Software Architecture

#### 4.6.1. Design-Level Event Storming

#### 4.6.2. Software Architecture Context Diagram

#### 4.6.3. Software Architecture Container Diagrams

#### 4.6.4. Software Architecture Components Diagrams

### 4.7. Software Object-Oriented Design

#### 4.7.1. Class Diagrams

### 4.8. Database Design

#### 4.8.1. Database Diagrams

---

## Capítulo V: Product Implementation, Validation & Deployment

### 5.1. Software Configuration Management

#### 5.1.1. Software Development Environment Configuration

#### 5.1.2. Source Code Management

#### 5.1.3. Source Code Style Guide & Conventions

#### 5.1.4. Software Deployment Configuration

### 5.2. Landing Page, Services & Applications Implementation

#### 5.2.X. Sprint n

##### 5.2.X.1. Sprint Planning n

##### 5.2.X.2. Aspect Leaders and Collaborators

##### 5.2.X.3. Sprint Backlog n

##### 5.2.X.4. Development Evidence for Sprint Review

##### 5.2.X.5. Execution Evidence for Sprint Review

##### 5.2.X.6. Services Documentation Evidence for Sprint Review

##### 5.2.X.7. Software Deployment Evidence for Sprint Review

##### 5.2.X.8. Team Collaboration Insights during Sprint

---

## Conclusiones

### Conclusiones y recomendaciones

### Video About-the-Team

## Bibliografía
- Autoridad de Transporte Urbano para Lima y Callao. (2024). *Cifra de movilidades escolares autorizadas disminuyó en 25% en un año*. El Comercio. Recuperado el 9 de abril de 2026, de https://elcomercio.pe/lima/cifra-de-movilidades-escolares-autorizadas-disminuyo-en-25-en-un-ano-a-que-se-debe-esta-reduccion-informe-movilidad-escolar-noticia/

- Ministerio de Educación. (2023). *Resultados del Censo Educativo 2022*. ESCALE. Recuperado el 9 de abril de 2026, de https://escale.minedu.gob.pe/documents/10156/9345030/PPT_Censo_Educativo_2023_final.pdf

- Superintendencia de Transporte Terrestre de Personas, Carga y Mercancías. (2024). *Sutran (MTC) sensibilizó a más de 47 000 escolares sobre seguridad vial*. Gob.pe. Recuperado el 9 de abril de 2026, de https://www.gob.pe/institucion/sutran/noticias/1255228-sutran-mtc-sensibilizo-a-mas-de-47-000-escolares-sobre-seguridad-vial-en-lo-que-va-del-2025

## Anexos
