# Oferta técnica - MediNova Digital

## Resumen ejecutivo

MediNova Digital propone la implantación de MediNova PatientFlow, solución SaaS sanitaria orientada a experiencia de paciente, rapidez de despliegue y reducción de coste total. La propuesta enfatiza portal web, aplicación móvil, comunicación multicanal y configuración funcional por personal del hospital.

MediNova plantea un proyecto de 22 meses, con primeros resultados visibles en el mes 6 y despliegue gradual por servicios. La oferta económica se apoya en un modelo de licenciamiento por uso y soporte remoto.

## Cobertura funcional

PatientFlow cubre citación multicanal, consulta de citas, cancelación, confirmación, recordatorios, listas de espera simples, reprogramación por reglas básicas, portal web y app móvil. Incluye un asistente de preparación de cita que muestra instrucciones definidas por el hospital.

El producto dispone de panel de administración para parametrizar agendas, textos de notificación, formularios y reglas. MediNova destaca que las unidades funcionales pueden mantener parte de la configuración sin intervención técnica.

Para procesos complejos, como pruebas encadenadas, circuitos quirúrgicos o agendas con restricciones múltiples, la propuesta ofrece configuración mediante modelos reutilizables de agenda. La empresa indica que las reglas avanzadas se abordarán en talleres de diseño y que las excepciones se resolverán mediante parametrización o evolutivo menor.

## Portal y app

El portal web es responsivo y accesible, con identificación mediante federación hospitalaria o credenciales verificadas. La app móvil permite notificaciones push, consulta de agenda, cancelación, avisos y mensajes informativos. MediNova incluye publicación en tiendas y mantenimiento de versiones durante el contrato.

La oferta indica que la app soportará todas las operaciones principales desde el arranque. En el detalle funcional se reserva la gestión de representantes y autorizaciones complejas para una segunda iteración dentro del primer año de producción.

## Arquitectura

PatientFlow se entrega como SaaS multi-tenant con segregación lógica por cliente, base de datos cifrada y servicios desplegados en región europea. La arquitectura utiliza APIs REST, colas de eventos, monitorización integrada y consola de administración.

MediNova compromete disponibilidad del 99,90%. La escalabilidad se basa en autoescalado horizontal, aunque la oferta de dimensionamiento toma como referencia 5.000 accesos diarios y picos de 600 sesiones concurrentes. La empresa propone ajustar capacidad cuando HUSA proporcione métricas reales de campaña.

## Integraciones

La integración con HUSA-Core v8 y HUSA-MPI se realizará mediante adaptadores configurables. Para LabAurelia e ImagoSuite se propone una primera integración de consulta y sincronización de eventos básicos, ampliable a estados avanzados.

La propuesta incluye SMS, push e integración con DataHUSA mediante exportaciones programadas. La integración FHIR se ofrece cuando los sistemas origen publiquen recursos compatibles; en caso contrario se utilizarán mensajes HL7 v2 o servicios intermedios.

MediNova no prevé desarrollos a medida extensos, salvo adaptadores específicos limitados. Considera que la mayor parte del alcance puede resolverse con parametrización del producto.

## Seguridad y privacidad

La oferta incluye MFA para administradores, auditoría, cifrado, control de acceso, registros de actividad, segregación por entorno y soporte a evaluación de impacto. Para pacientes, se admite identidad federada y mecanismos de verificación de contacto.

MediNova propone pruebas de seguridad antes de producción y revisión anual. Los accesos de soporte se realizarán mediante consola con aprobación del hospital.

## Migración

MediNova incluye migración de citas futuras, agendas, catálogo básico y datos de contacto. Para el histórico de reprogramaciones propone cargar datos agregados en el cuadro de mando cuando la extracción detallada sea compleja. La empresa sostiene que el valor operativo principal reside en citas futuras y reglas activas.

La estrategia contempla una carga inicial, una carga de ensayo y una carga final. La depuración de datos queda compartida con el hospital.

## Plan de implantación

* Meses 1-2: arranque, análisis y acceso a entornos.
* Meses 3-5: configuración base, portal y notificaciones.
* Meses 6-8: piloto de consultas externas.
* Meses 9-12: HIS, MPI y analítica inicial.
* Meses 13-16: laboratorio, imagen y app móvil completa.
* Meses 17-19: migración, formación y expansión.
* Meses 20-22: estabilización y cierre.

MediNova propone iniciar con servicios voluntarios para acelerar adopción y evitar retrasos por procesos complejos.

## Equipo propuesto

Equipo medio estimado de 8,1 ETC, con director de proyecto, consultor funcional senior, arquitecto SaaS, dos especialistas de integración, responsable de seguridad compartido, UX, analista de datos, formadores y soporte remoto.

La empresa presenta referencias en hospitales comarcales, redes ambulatorias y portales ciudadanos de salud. Declara experiencia limitada en hospitales universitarios de alta complejidad, compensada por un producto estándar y metodología iterativa.

## Soporte y formación

Se incluye soporte crítico 24x7, soporte ordinario 8:00-18:00 ampliable, 240 horas evolutivas y 28 sesiones formativas. La oferta incluye centro de ayuda para usuarios internos y documentación editable.

## Riesgos identificados

* Complejidad de reglas locales de agenda.
* Necesidad de ajustar dimensionamiento tras conocer picos reales.
* Dependencia de APIs o mensajes disponibles en sistemas origen.
* Priorización de integraciones avanzadas según valor operativo.

MediNova propone gestión ágil, pilotos tempranos y adaptación progresiva.
