= Plataformas de desarrollo asistido por IA
:description: Plan de tutorial sobre herramientas tipo Firebase Studio, Replit, Bolt.new, Lovable, v0 y GitHub Spark.
:toc: right
:toc-title: Contenidos
:toclevels: 3
:sectnums:

Proporción recomendada del tutorial:

* 25% explicación conceptual.
* 35% plataformas individuales.
* 10% comparativa y criterios de decisión.
* 30% ejercicios, checklist y conclusiones.

== 1. Introducción

En los últimos años han aparecido herramientas que permiten describir una aplicación en lenguaje natural, generar una primera versión funcional, modificarla conversando con un asistente de IA y, en muchos casos, publicarla desde el propio entorno.

Firebase Studio, Replit, Bolt.new, Lovable, v0 o GitHub Spark pertenecen a esta familia. No son exactamente editores de código tradicionales, tampoco son plataformas no-code puras y tampoco son simples chatbots que devuelven fragmentos de código. Ocupan una zona intermedia: convierten intención, requisitos y conversación en software ejecutable.

En este tutorial las llamaremos **plataformas de desarrollo asistido por IA**.

NOTE: El objetivo de esta primera parte no es elegir todavía una herramienta concreta, sino entender la categoría: qué son, qué prometen, por qué han surgido, qué problemas ayudan a resolver y qué riesgos introducen.

=== 1.1 Objetivos de aprendizaje

Al terminar este apartado deberías poder:

* explicar qué es una plataforma de desarrollo asistido por IA,
* distinguirla de un editor con IA, una herramienta no-code y un entorno cloud tradicional,
* identificar para qué tipos de trabajo resulta útil,
* reconocer sus límites antes de usarla en un proyecto real,
* decidir cuándo puede emplearse como apoyo de prototipado y cuándo exige gobierno técnico estricto,
* formular criterios iniciales para evaluar herramientas como Firebase Studio, Replit, Bolt.new, Lovable, v0 o GitHub Spark.

=== 1.2 Cómo llamaremos a estas herramientas

El nombre elegido para este tutorial es **plataformas de desarrollo asistido por IA**.

La expresión es deliberadamente amplia. Permite incluir herramientas con enfoques distintos:

* Firebase Studio, más ligado al ecosistema Firebase y Google Cloud.
* Replit, más cercano a un entorno completo de desarrollo en navegador.
* Bolt.new y Lovable, muy orientadas a pasar rápido de una idea a una aplicación web.
* v0, especialmente fuerte en interfaces, React, Next.js y componentes visuales.
* GitHub Spark, conectado con GitHub, Copilot y el flujo de trabajo de repositorios.

En otros contextos también encontrarás nombres como:

* plataformas _prompt-to-app_,
* entornos de desarrollo generativo,
* plataformas de prototipado con IA,
* herramientas de _vibe coding_,
* AI app builders,
* AI-native development platforms.

En este documento usaremos **plataformas de desarrollo asistido por IA** como término principal. Reservaremos _prompt-to-app_ para un flujo más concreto: describir una aplicación con lenguaje natural y obtener una primera versión ejecutable.

[NOTE]
====
No existe todavía una terminología universalmente aceptada. La categoría está evolucionando y cada proveedor intenta nombrarla desde su propio producto. Por eso es más útil entender las capacidades que memorizar una etiqueta.
====

=== 1.3 La nueva capa entre la idea y el software

Estas plataformas intentan reducir la distancia entre una intención y una aplicación funcional.

En un desarrollo tradicional, una idea suele recorrer varias etapas:

1. descripción de necesidad,
2. análisis funcional,
3. diseño de interfaz,
4. diseño técnico,
5. creación del repositorio,
6. configuración del entorno,
7. desarrollo,
8. pruebas,
9. despliegue,
10. revisión con usuarios.

Las plataformas de desarrollo asistido por IA no eliminan todas esas etapas, pero comprimen muchas de ellas en un mismo espacio de trabajo. Una persona puede escribir:

[source,text]
----
Necesito una aplicación para registrar solicitudes internas,
ver su estado, filtrar por servicio y generar un pequeño panel de seguimiento.
----

Y la plataforma puede responder creando:

* una estructura inicial de proyecto,
* pantallas,
* componentes de interfaz,
* rutas,
* modelos de datos,
* lógica básica,
* estilos,
* una vista previa navegable,
* e incluso una opción de despliegue.

La clave no es que la primera respuesta sea perfecta. Casi nunca lo será. La clave es que aparece un objeto discutible: algo que se puede ver, probar, corregir, enseñar y criticar.

Ese cambio es importante. Muchas conversaciones de producto se atascan porque las personas imaginan cosas distintas cuando leen el mismo requisito. Una demo imperfecta puede alinear mejor al equipo que diez páginas de descripción abstracta.

=== 1.4 Qué piezas suelen combinar

Aunque cada producto lo hace a su manera, estas plataformas suelen reunir varias capacidades.

[cols="2,4,4",options="header"]
|===
| Pieza | Qué aporta | Por qué importa

| Workspace en navegador
| Un entorno donde editar, ejecutar y revisar la aplicación sin preparar una máquina local compleja.
| Reduce fricción de entrada y facilita formación, demos y colaboración.

| Asistente o agente de IA
| Interpreta instrucciones, modifica código, propone cambios y explica partes del proyecto.
| Permite iterar por conversación, no sólo escribiendo código manualmente.

| Generación de código
| Crea componentes, rutas, servicios, modelos, estilos o pruebas iniciales.
| Acelera el arranque y evita empezar desde una pantalla en blanco.

| Vista previa instantánea
| Muestra la aplicación mientras se construye.
| Convierte requisitos en algo verificable por usuarios y equipo técnico.

| Integraciones de backend
| Conecta autenticación, base de datos, almacenamiento, funciones o APIs.
| Permite que el prototipo deje de ser sólo una maqueta visual.

| Despliegue o publicación
| Permite compartir una URL o desplegar una versión inicial.
| Facilita validación temprana con usuarios, docentes, clientes o equipos internos.

| Control de código
| Exporta, sincroniza o versiona el proyecto en Git o repositorios equivalentes.
| Es fundamental si el prototipo debe evolucionar hacia software mantenible.

| Gestión visual
| Algunas plataformas permiten editar interfaz, datos o flujos desde controles visuales.
| Acerca el proceso a perfiles de producto, diseño o negocio.
|===

La combinación exacta cambia según la plataforma. Por eso no conviene evaluarlas sólo por “qué modelo de IA usan”, sino por el flujo completo que ofrecen.

=== 1.5 En qué se diferencian de herramientas cercanas

Estas plataformas se solapan con otras categorías, pero no son exactamente lo mismo.

[cols="2,4,4",options="header"]
|===
| Categoría | Qué suele hacer | Diferencia principal

| Editor con IA
| Ayuda a escribir, completar o refactorizar código dentro de un entorno de desarrollo.
| Normalmente presupone que ya existe un proyecto técnico y una persona desarrolladora al mando.

| No-code
| Permite crear aplicaciones mediante interfaces visuales, reglas y conectores.
| Suele ocultar más el código y priorizar configuración visual sobre generación programática.

| Low-code
| Combina configuración visual con extensiones mediante código.
| Está más orientado a plataformas empresariales y procesos internos estructurados.

| Prototipado visual
| Diseña pantallas, flujos y experiencias de usuario.
| A menudo no genera una aplicación funcional con backend y lógica real.

| Entorno cloud de desarrollo
| Proporciona una máquina o workspace remoto para programar.
| No necesariamente incluye generación de aplicación por lenguaje natural.

| Plataforma de desarrollo asistido por IA
| Combina intención en lenguaje natural, generación de código, ejecución, iteración y, a veces, despliegue.
| Intenta unir ideación, prototipo y desarrollo inicial en un flujo continuo.
|===

La frontera no siempre es limpia. Por ejemplo, Replit puede actuar como entorno cloud de desarrollo y como plataforma asistida por IA. v0 puede funcionar como generador de interfaces y como punto de entrada a una aplicación Next.js. Firebase Studio puede ser prototipador, workspace y puerta de entrada al ecosistema Firebase.

=== 1.6 Por qué aparecen ahora

Estas plataformas no surgen por una sola causa. Aparecen por la convergencia de varias presiones.

La primera es la presión por construir más rápido. Equipos de producto, unidades de negocio, departamentos de innovación y áreas TIC necesitan validar ideas sin esperar ciclos largos de desarrollo. Un prototipo funcional puede servir para decidir si merece la pena invertir más.

La segunda es la escasez de capacidad técnica. Casi todas las organizaciones tienen más necesidades de software que equipos disponibles para atenderlas. Estas plataformas prometen ampliar quién puede participar en las primeras fases de creación.

La tercera es la madurez de los modelos generativos. Los modelos actuales pueden producir código razonable, explicar errores, transformar requisitos en componentes, generar documentación y proponer pruebas iniciales. No sustituyen el criterio profesional, pero sí cambian la economía del primer borrador.

La cuarta es la normalización del cloud. Muchas aplicaciones ya se construyen con servicios gestionados: autenticación, almacenamiento, funciones, bases de datos, hosting, colas, APIs. Si esas piezas ya están disponibles como servicios, una plataforma puede conectarlas más rápido.

La quinta es cultural. El llamado _vibe coding_ ha popularizado una forma de trabajo más conversacional: describir, probar, corregir, volver a pedir, ajustar. Esa forma de trabajar puede ser útil para explorar, siempre que no se confunda con ingeniería completa.

=== 1.7 Qué trabajo descargan

Estas plataformas son especialmente útiles en el arranque de un proyecto, cuando todavía hay muchas decisiones abiertas y conviene aprender rápido.

Pueden ayudar a:

* pasar de idea a prototipo en minutos u horas,
* crear MVPs funcionales,
* generar interfaces iniciales,
* probar variantes de navegación o flujo,
* construir herramientas internas de bajo riesgo,
* preparar demos para comités o sesiones de trabajo,
* ayudar a perfiles no técnicos a expresar requisitos,
* generar una primera estructura de proyecto,
* producir ejemplos de datos,
* crear documentación inicial,
* explorar integraciones sencillas,
* acelerar pruebas de concepto.

En formación tienen un valor especial. Permiten que el alumnado vea cómo una decisión funcional se traduce en pantallas, datos, validaciones, rutas, errores y despliegue. También ayudan a discutir la diferencia entre una demo convincente y una solución técnicamente defendible.

=== 1.8 Un ejemplo sencillo

Imagina que un hospital quiere explorar una herramienta interna para registrar incidencias no clínicas de mantenimiento.

Una petición inicial podría ser:

[source,text]
----
Crea una aplicación web para registrar incidencias de mantenimiento.
Debe permitir crear una incidencia, asignarle prioridad, seleccionar ubicación,
ver un listado filtrable y cambiar el estado entre abierta, en curso y cerrada.
----

Una plataforma de desarrollo asistido por IA podría generar una primera aplicación con:

* formulario de alta,
* listado de incidencias,
* filtro por estado,
* selector de prioridad,
* estilos básicos,
* datos de ejemplo,
* y una vista previa.

Eso permite hacer preguntas mejores:

* ¿Faltan campos?
* ¿Quién puede cambiar el estado?
* ¿Hace falta adjuntar fotos?
* ¿Debe integrarse con directorio corporativo?
* ¿Qué datos son sensibles?
* ¿Cuánto tiempo debe conservarse la información?
* ¿Quién mantiene la herramienta?

La plataforma acelera la conversación, pero no elimina las decisiones. De hecho, al hacer visible el prototipo, hace que aparezcan antes.

=== 1.9 La parte de la promesa que conviene no creerse

El riesgo principal de estas herramientas no es que hagan demos malas. El riesgo principal es que hagan demos suficientemente buenas como para que alguien las confunda con sistemas listos para producción.

Estas plataformas no resuelven por sí solas:

* arquitectura seria,
* seguridad y cumplimiento normativo,
* gobernanza del dato,
* control de accesos,
* privacidad,
* mantenimiento a largo plazo,
* pruebas profundas,
* escalabilidad real,
* observabilidad,
* integración compleja con sistemas legacy,
* responsabilidad legal sobre el código generado,
* control de costes cloud,
* gestión del ciclo de vida de producto.

[WARNING]
====
Una demo que funciona no equivale a una aplicación preparada para producción. Antes de desplegar en un entorno real hacen falta revisión de código, pruebas, seguridad, control de datos, observabilidad, plan de mantenimiento y responsables claros.
====

=== 1.10 Dónde deben entrar con cautela

No deberían usarse sin gobierno técnico y revisión experta en:

* sistemas clínicos, financieros o críticos,
* aplicaciones con datos personales sensibles,
* entornos regulados,
* proyectos con requisitos fuertes de ciberseguridad,
* sistemas core de negocio,
* integraciones complejas con ERP, HIS, HCE, IAM corporativo o sistemas legacy,
* productos donde no se pueda aceptar dependencia fuerte del proveedor,
* contextos donde no esté claro quién revisa, prueba, despliega y mantiene el resultado.

En esos casos, la recomendación no tiene por qué ser prohibirlas. Puede ser usarlas con límites:

* sólo con datos ficticios o anonimizados,
* sólo para prototipos,
* sólo en entornos aislados,
* con revisión técnica obligatoria,
* con versionado en Git,
* con análisis de seguridad,
* con presupuesto y alertas de coste,
* con documentación de supuestos,
* con una persona responsable del ciclo de vida del prototipo.

=== 1.11 Criterio práctico para este tutorial

En este tutorial trataremos estas plataformas como aceleradores de aprendizaje, prototipado y desarrollo inicial.

La idea central será:

[quote]
____
Úsalas para llegar antes a una primera versión discutible, no para saltarte las decisiones técnicas que hacen que una aplicación sea segura, mantenible y gobernable.
____

Por tanto, al revisar cada plataforma nos haremos siempre las mismas preguntas:

* ¿Qué permite construir rápidamente?
* ¿Qué parte del ciclo de vida cubre?
* ¿Qué control ofrece sobre el código?
* ¿Cómo se despliega?
* ¿Cómo se pagan sus límites reales?
* ¿Qué riesgos introduce?
* ¿Cuándo es una buena elección?
* ¿Cuándo conviene evitarla?

=== 1.12 Ideas clave del apartado

* Las plataformas de desarrollo asistido por IA combinan lenguaje natural, generación de código, vista previa, edición y, a menudo, despliegue.
* No son exactamente no-code, low-code, editores con IA ni simples generadores de código.
* Su valor principal está en acelerar exploración, prototipado, aprendizaje y primeras versiones.
* Su mayor riesgo es convertir una demo atractiva en una falsa sensación de sistema terminado.
* En entornos críticos o regulados deben usarse con gobierno, revisión, trazabilidad y límites claros.
* La pregunta importante no es si la herramienta “programa bien”, sino si encaja con el caso, el equipo, los datos, el riesgo y el ciclo de vida esperado.

== 2. Panorama actual de alternativas

=== 2.1 Criterios de selección

Incluir solo herramientas que cumplan al menos varios de estos criterios:

* generación de app desde lenguaje natural,
* edición iterativa con IA,
* vista previa ejecutable,
* despliegue o hosting integrado,
* integración con GitHub o cloud,
* uso real en prototipado o MVP,
* relevancia actual en mercado.

=== 2.2 Mapa rápido

[cols="2,3,3,3",options="header"]
|===
| Herramienta | Mejor para | Perfil principal | Advertencia

| Firebase Studio
| Prototipos y apps conectadas al ecosistema Firebase/Google Cloud
| Equipos que ya usan Firebase, Flutter, web o Google Cloud
| Dependencia fuerte del ecosistema Google

| Replit
| Desarrollo completo en navegador con agentes y despliegue
| Makers, estudiantes, equipos pequeños, prototipos funcionales
| Coste variable y necesidad de controlar uso

| Bolt.new
| Crear apps web rápidamente desde prompts
| Prototipado web rápido
| Consumo por tokens y necesidad de revisar código

| Lovable
| Apps web visualmente cuidadas y MVPs rápidos
| No-code/low-code, founders, producto
| Riesgo de quedarse corto en backend complejo

| v0 by Vercel
| UI, componentes React/Next.js y frontends modernos
| Equipos frontend, diseño-producto
| No es siempre la mejor opción para backend completo

| GitHub Spark
| Apps inteligentes integradas en GitHub
| Equipos GitHub/Copilot
| Producto aún en preview y sujeto a cambios

| Base44
| Apps completas no-code con backend gestionado
| Usuarios no técnicos y MVPs internos
| Menor control profundo que un stack propio
|===

== 3. Firebase Studio

=== 3.1 Descripción

Qué es, qué promete, qué piezas integra.

Firebase Studio es especialmente relevante porque combina workspace en navegador, IA con Gemini, prototipado de apps y conexión con Firebase/Google Cloud. Según la documentación oficial, el acceso está disponible sin coste, con límites de workspaces, y algunas integraciones como Firebase App Hosting pueden requerir Cloud Billing. Firebase indica 3 workspaces sin Google Developer Program, 10 con plan Standard y 30 con Premium. También advierte que enlazar facturación puede pasar el proyecto a Blaze y generar cargos por servicios de pago. Fuente: Firebase Studio pricing. ([firebase.google.com](https://firebase.google.com/docs/studio/pricing))

=== 3.2 Casos de uso

* Prototipos web.
* Apps Firebase-first.
* Demos internas.
* Apps con autenticación, hosting o datos en Firebase.
* Formación en desarrollo cloud.
* Experimentos con Gemini y generación de interfaces.

=== 3.3 Flujo típico

1. Crear workspace.
2. Elegir plantilla.
3. Describir app.
4. Iterar con el agente.
5. Conectar servicios Firebase.
6. Probar.
7. Desplegar o exportar.

=== 3.4 Planes y costes

Explicar:

* coste de acceso,
* límites de workspaces,
* relación con Google Developer Program,
* riesgo de Cloud Billing,
* diferencia entre prototipo gratuito y app con servicios de pago.

=== 3.5 Fortalezas

=== 3.6 Limitaciones

=== 3.7 Cuándo elegirla

=== 3.8 Cuándo evitarla

== 4. Replit

...

== 5. Bolt.new

...

== 6. Lovable

...

== 7. v0 by Vercel

...

== 8. GitHub Spark

...

== 9. Base44

...


== 10. Comparativa práctica

=== 10.1 Comparativa por tipo de usuario

[cols="2,3,3",options="header"]
|===
| Perfil | Herramientas recomendadas | Motivo

| Docente / formación
| Firebase Studio, Replit, Bolt.new
| Fácil empezar, buen valor demostrativo

| Founder no técnico
| Lovable, Base44, Bolt.new
| Rapidez para MVP y validación

| Equipo frontend
| v0, Lovable, Bolt.new
| Mejor generación visual y React/Next.js

| Equipo ya en Google Cloud
| Firebase Studio
| Integración natural con Firebase y GCP

| Equipo ya en GitHub Enterprise
| GitHub Spark, Replit
| Integración con GitHub/Copilot y flujos existentes

| Prototipo interno rápido
| Replit, Bolt.new, Lovable, Firebase Studio
| Permiten pasar de idea a demo funcional
|===

=== 10.2 Comparativa por criterio

[cols="2,1,1,1,1,1,1",options="header"]
|===
| Criterio | Firebase Studio | Replit | Bolt | Lovable | v0 | Spark

| Facilidad inicial
| Alta | Alta | Alta | Alta | Alta | Alta

| Control de código
| Medio/Alto | Alto | Medio/Alto | Medio | Alto frontend | Alto si se usa GitHub

| Backend integrado
| Firebase | Sí | Variable | Sí/gestionado | Limitado/externo | Integrado

| Mejor para frontend
| Medio | Medio | Alto | Alto | Muy alto | Medio

| Mejor para full-stack
| Alto en Firebase | Alto | Alto | Medio/Alto | Medio | Alto

| Coste predecible
| Medio | Medio/Bajo | Medio | Medio | Medio | Medio

| Entorno empresarial
| Google Cloud | Enterprise | Teams | Enterprise | Vercel Enterprise | GitHub Enterprise

| Riesgo de lock-in
| Alto | Medio | Medio | Alto | Medio | Medio/Alto
|===

=== 10.3 Comparativa de riesgos

* Costes variables por créditos, tokens o uso cloud.
* Dependencia de proveedor.
* Código generado difícil de mantener.
* Seguridad no garantizada.
* Falta de pruebas.
* Problemas de escalabilidad.
* Riesgo de datos sensibles en prompts.
* Incertidumbre en productos en preview.

== 11. Cómo evaluar una plataforma antes de usarla

=== 11.1 Checklist técnico

* ¿Puedo exportar el código?
* ¿Puedo versionarlo en Git?
* ¿Dónde se ejecuta?
* ¿Dónde se almacenan los datos?
* ¿Qué ocurre si cancelo el plan?
* ¿Hay logs?
* ¿Hay control de secretos?
* ¿Permite pruebas?
* ¿Permite despliegue propio?
* ¿Cumple requisitos de seguridad?

=== 11.2 Checklist económico

* ¿El precio es por usuario, crédito, token, workspace o uso cloud?
* ¿Hay costes de hosting separados?
* ¿Hay límites de mensajes?
* ¿Hay límites de despliegue?
* ¿Qué pasa al superar límites?
* ¿Se pueden poner presupuestos o alertas?
* ¿Existe plan enterprise?

=== 11.3 Checklist de gobierno

* ¿Quién puede crear apps?
* ¿Quién revisa el código?
* ¿Quién aprueba despliegues?
* ¿Qué datos se pueden introducir en prompts?
* ¿Qué apps pueden pasar a producción?
* ¿Qué documentación mínima se exige?

== 12. Taller práctico

=== 12.1 Ejercicio 1 - Clasificar herramientas

Dado un conjunto de necesidades, elegir plataforma y justificar.

=== 12.2 Ejercicio 2 - Crear un prototipo

Construir una app sencilla:
* formulario,
* listado,
* autenticación simulada,
* persistencia básica,
* despliegue o preview.

=== 12.3 Ejercicio 3 - Auditoría del prototipo

Revisar:
* seguridad,
* datos,
* dependencias,
* coste,
* mantenibilidad,
* portabilidad.

=== 12.4 Ejercicio 4 - Decisión de uso

Preparar una recomendación:
* usar,
* usar sólo para prototipo,
* usar con restricciones,
* no usar.

== 13. Conclusiones

Ideas clave:

* Estas plataformas no sustituyen al desarrollo profesional; cambian dónde empieza.
* Son excelentes para prototipos, MVPs, formación y exploración.
* El mayor riesgo no es que generen código malo, sino que se use sin revisión.
* El coste real no siempre es el plan mensual: también importan tokens, créditos, hosting, bases de datos, despliegue y tiempo de corrección.
* En entornos hospitalarios o regulados deben usarse con gobierno, trazabilidad y revisión técnica.
* La pregunta correcta no es “qué herramienta es mejor”, sino “qué herramienta encaja con este caso, este equipo, estos datos y este nivel de riesgo”.
