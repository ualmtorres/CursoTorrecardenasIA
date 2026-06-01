# Pliego de Prescripciones Técnicas

## Expediente

Expediente ficticio HUSA-PI-2026-017 para la contratación de una Plataforma Integral de Gestión de Citas y Portal del Paciente del Hospital Universitario Santa Aurelia (HUSA).

Presupuesto base estimado: 2.800.000 euros, impuestos excluidos. Duración prevista: 24 meses, incluyendo implantación, migración, formación, soporte inicial y transición a explotación ordinaria.

## Objeto

El objeto del contrato es el suministro, implantación, integración, puesta en marcha y soporte de una plataforma corporativa para la gestión multicanal de citas, portal web del paciente, aplicación móvil, recordatorios SMS, notificaciones push y cuadro de mando de actividad asistencial no clínica.

La solución deberá integrarse con los sistemas corporativos del HUSA sin sustituir al HIS como sistema maestro de historia clínica ni modificar la responsabilidad de los sistemas departamentales.

## Alcance funcional

La plataforma deberá cubrir, como mínimo:

* Agenda centralizada por centro, servicio, profesional, recurso, acto asistencial y modalidad.
* Gestión de cita presencial, telefónica, teleconsulta y pruebas diagnósticas.
* Reprogramación, cancelación, lista de espera, huecos preferentes y bloqueo por reglas.
* Portal web responsivo para pacientes, personas autorizadas y representantes.
* Aplicación móvil iOS y Android con autenticación reforzada.
* Gestión de consentimientos informativos no clínicos asociados a procesos de cita.
* Notificaciones SMS, correo electrónico y push configurables por tipo de evento.
* Integración con laboratorio para preparación de pruebas, instrucciones y avisos.
* Integración con imagen médica para citas de radiología, resonancia, TAC, ecografía y pruebas especiales.
* Cuadro de mando con actividad, no asistencia, demoras, reprogramaciones, canales y cumplimiento de SLA.
* Administración delegada por unidades, perfiles y circuitos.

El sistema deberá permitir al paciente consultar citas futuras, descargar justificantes de asistencia, confirmar asistencia, modificar datos de contacto bajo validación y recibir instrucciones previas. No se exige acceso completo a la historia clínica electrónica.

## Requisitos técnicos

La solución deberá ser web, escalable y compatible con despliegue en nube privada o nube pública europea. Se valorará arquitectura modular, APIs documentadas, observabilidad, automatización de despliegues y separación clara entre capa de presentación, servicios de negocio, integración y datos.

Requisitos mínimos:

* Disponibilidad global mínima del 99,90% en horario 24x7.
* RPO máximo de 30 minutos y RTO máximo de 4 horas para servicios críticos.
* Trazabilidad completa de acciones de usuario y procesos automáticos.
* APIs REST o equivalentes documentadas con versionado.
* Compatibilidad con integración HL7 v2, FHIR R4 o mensajería equivalente.
* Exportación de datos operativos en formatos abiertos.
* Monitorización de rendimiento, colas, integraciones y errores funcionales.
* Separación de entornos de desarrollo, preproducción y producción.
* Pruebas de carga para 70.000 usuarios registrados, 8.000 accesos diarios y picos de 1.200 sesiones concurrentes.

La plataforma deberá soportar crecimiento del 30% anual durante tres años sin rediseño mayor.

## Integraciones obligatorias

El adjudicatario deberá integrar la plataforma con:

* HIS corporativo ficticio HUSA-Core v8.
* Maestro de pacientes HUSA-MPI.
* Sistema de laboratorio LabAurelia.
* Sistema RIS/PACS ImagoSuite.
* Directorio corporativo y federación de identidad.
* Pasarela SMS corporativa.
* Plataforma de notificaciones push.
* Sistema de analítica corporativa DataHUSA.

Las integraciones deberán incluir análisis, diseño, construcción, pruebas unitarias, pruebas integradas, documentación y transferencia de conocimiento. Las excepciones o dependencias de terceros deberán declararse expresamente.

## Seguridad y protección de datos

La solución tratará datos personales de salud en sentido amplio, aunque no almacenará informes clínicos completos salvo metadatos necesarios para la cita.

Requisitos:

* Autenticación multifactor para profesionales y administradores.
* Identidad federada para pacientes con medios admitidos por el hospital.
* Control de acceso por rol, centro, servicio y operación.
* Cifrado en tránsito TLS 1.2 o superior y cifrado en reposo.
* Registro de auditoría inalterable con retención mínima de 5 años.
* Gestión de consentimientos y autorizaciones de representantes.
* Evaluación de impacto de protección de datos antes de producción.
* Pruebas de seguridad antes del paso a producción.
* Gestión de vulnerabilidades con plan de remediación.
* Ubicación de datos y soporte dentro del Espacio Económico Europeo.

El licitador deberá describir medidas de continuidad, segregación de funciones, gestión de secretos, copias, restauración y tratamiento de incidencias.

## Soporte y mantenimiento

Durante la implantación se exige soporte de proyecto en horario laboral ampliado. Tras la puesta en producción, se exige soporte de primer año incluido, con:

* Atención 24x7 para incidencias críticas.
* Horario 8:00-20:00 en días laborables para incidencias no críticas.
* Tiempo de respuesta crítica: 30 minutos.
* Tiempo de resolución objetivo crítica: 4 horas o plan de contingencia aprobado.
* Reunión mensual de seguimiento.
* Bolsa mínima de 240 horas de evolución menor durante el primer año.

Se deberá detallar el modelo de soporte, niveles, herramientas, perfiles asignados y transición a operación.

## Formación y gestión del cambio

Se requiere:

* Formación a administradores funcionales.
* Formación a personal TIC.
* Formación a unidades de admisión y citación.
* Materiales reutilizables en formato editable.
* Sesiones de formador de formadores.
* Plan de comunicación interna.
* Plan de acompañamiento durante arranque.

La oferta deberá incluir número de sesiones, perfiles destinatarios, duración, materiales y modalidad.

## Migración

El adjudicatario deberá realizar la migración de datos necesarios para operar el sistema desde el arranque. Como mínimo:

* Citas futuras.
* Catálogo de servicios, agendas, prestaciones y recursos.
* Datos de contacto validados disponibles.
* Histórico mínimo de reprogramaciones de 12 meses para análisis operativo.
* Configuración de reglas de agenda y modelos de parametrización.

El licitador deberá proponer estrategia de extracción, transformación, validación, pruebas, marcha atrás y conciliación.

## Hitos mínimos

* Mes 1: arranque y plan detallado.
* Mes 3: diseño funcional y técnico aprobado.
* Mes 6: prototipo navegable y diseño de integraciones.
* Mes 9: primer piloto con agendas seleccionadas.
* Mes 12: integración con HIS y MPI en preproducción.
* Mes 15: laboratorio e imagen en preproducción.
* Mes 18: piloto ampliado y formación.
* Mes 21: producción progresiva.
* Mes 24: estabilización, transferencia y cierre.

Se aceptarán propuestas alternativas justificadas siempre que no reduzcan garantías de calidad, seguridad o continuidad.
