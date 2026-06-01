# Oferta técnica - HealthTech Solutions

## Resumen ejecutivo

HealthTech Solutions propone implantar HeliCare Access Suite, plataforma modular para gestión de citas, portal del paciente, aplicación móvil e integración sanitaria. La propuesta se basa en una arquitectura de microservicios desplegable en nube europea, con motor de reglas de agenda, capa de interoperabilidad y cuadro de mando operativo.

La compañía plantea un proyecto de 24 meses con fuerte dedicación de especialistas en integración, seguridad y arquitectura. El enfoque prioriza robustez técnica, pruebas intensivas y reducción de riesgo en integraciones críticas.

## Cobertura funcional

HeliCare Access Suite cubre agenda centralizada, citación multicanal, reprogramación, cancelación, listas de espera, huecos preferentes, confirmación de asistencia y gestión de no presentados. El portal web permite consultar citas, descargar justificantes, actualizar contacto, recibir instrucciones y gestionar autorizaciones.

La app móvil replica las funciones principales del portal e incorpora notificaciones push, agenda personal, confirmación rápida y credenciales biométricas del dispositivo como segundo factor local, subordinadas a la identidad federada del hospital.

El motor de reglas permite configurar ventanas de citación, prioridades, incompatibilidades de pruebas, preparación previa, cupos por agenda, bloqueos por campañas, circuitos de alta resolución y reglas por especialidad. HealthTech indica que algunas reglas complejas requerirán parametrización avanzada por consultores certificados.

## Arquitectura

La arquitectura propuesta separa:

* Portal y app móvil.
* API Gateway.
* Servicios de agenda, notificación, paciente, reglas y analítica.
* Bus de interoperabilidad.
* Repositorio operacional.
* Data marts para cuadro de mando.

El despliegue se realizará en contenedores, con observabilidad basada en métricas, trazas y logs centralizados. HealthTech compromete disponibilidad del 99,95% para los servicios críticos 24x7, siempre que la infraestructura final cumpla los requisitos mínimos indicados en su anexo técnico.

## Integraciones

HealthTech propone un equipo específico de interoperabilidad para HUSA-Core v8, HUSA-MPI, LabAurelia, ImagoSuite, identidad, SMS, push y DataHUSA. La integración con HIS se plantea mediante HL7 v2 para eventos de citación y FHIR R4 para consulta de recursos cuando esté disponible.

Para laboratorio se contempla sincronización de citas, instrucciones de preparación y estado de prueba. Para imagen se propone integración con RIS mediante mensajes de orden y estado, y enlaces contextuales hacia visor cuando proceda.

La oferta indica que la integración con HIS está incluida. En un anexo se precisa que la disponibilidad de entornos de prueba estables y documentación de interfaces es una dependencia crítica del hospital.

## Seguridad y privacidad

La solución incorpora MFA para profesionales, control de acceso por rol, auditoría, cifrado en tránsito y reposo, gestión de secretos, pruebas SAST/DAST y revisión de arquitectura de seguridad. HealthTech propone realizar evaluación de impacto, análisis de riesgos y pruebas de intrusión antes de producción.

Los datos se alojarán en región europea. El soporte de nivel 3 podrá requerir intervención de especialistas del centro de excelencia de la compañía, siempre bajo acceso controlado, trazado y autorizado por HUSA.

## Migración

HealthTech propone migrar citas futuras, catálogos, agendas, reglas, datos de contacto y 12 meses de histórico de reprogramaciones. La estrategia incluye tres ciclos de carga, validación con usuarios clave, reconciliación automática y plan de marcha atrás.

La empresa advierte que la calidad de datos de contacto condicionará la activación de recordatorios y notificaciones. Propone una fase de depuración con reglas de normalización y muestreo.

## Plan de implantación

El plan mantiene los 24 meses:

* Meses 1-3: análisis detallado y gobierno.
* Meses 4-6: diseño funcional, técnico y prototipo.
* Meses 7-10: construcción base e integración HIS/MPI.
* Meses 11-15: laboratorio, imagen, identidad y notificaciones.
* Meses 16-18: migración piloto, pruebas de carga y seguridad.
* Meses 19-21: piloto ampliado y formación.
* Meses 22-24: despliegue progresivo, estabilización y transferencia.

El cronograma incluye puntos de decisión para no avanzar a producción si las pruebas de integración o seguridad no alcanzan criterios de aceptación.

## Equipo propuesto

Equipo medio estimado de 12,4 ETC durante el proyecto, con director de proyecto senior, arquitecto sanitario, arquitecto cloud, responsable de interoperabilidad, 4 especialistas de integración, 2 desarrolladores de adaptación, especialista de seguridad, responsable UX, consultores funcionales, analista BI, formadores y equipo de soporte.

HealthTech señala que los perfiles de arquitectura, interoperabilidad avanzada y seguridad son recursos especializados con disponibilidad planificada. Cualquier ampliación de alcance requerirá reservar ventanas adicionales.

## Soporte y formación

Se incluye soporte 24x7 para incidencias críticas durante el primer año, soporte 8:00-20:00 para incidencias no críticas, 360 horas evolutivas y formación presencial y remota. La propuesta contempla 42 sesiones formativas y materiales editables.

## Riesgos identificados por el licitador

* Complejidad de agenda por variabilidad entre servicios.
* Calidad de datos de contacto.
* Dependencia de documentación y disponibilidad de terceros.
* Gestión del cambio en unidades con circuitos locales.
* Necesidad de perfiles especializados para integraciones sanitarias.

HealthTech propone mitigarlos mediante gobierno técnico semanal, comité mensual, prototipos tempranos y pruebas progresivas.

