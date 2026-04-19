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

#### 2.1.1. Análisis competitivo

#### 2.1.2. Estrategias y tácticas frente a competidores

### 2.2. Entrevistas

#### 2.2.1. Diseño de entrevistas

#### 2.2.2. Registro de entrevistas

#### 2.2.3. Análisis de entrevistas

### 2.3. Needfinding

#### 2.3.1. User Personas

#### 2.3.2. User Task Matrix

#### 2.3.3. User Journey Mapping

#### 2.3.4. Empathy Mapping

### 2.4. Big Picture Event Storming

### 2.5. Ubiquitous Language

---

## Capítulo III: Requirements Specification

### 3.1. User Stories

### 3.2. Impact Mapping

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
