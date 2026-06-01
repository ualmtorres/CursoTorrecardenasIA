# CITAS360 - Analisis Funcional

Fecha: 14/02/2026  
Autor: Carmen Gil, Responsable de Admision; Laura Moreno, Responsable Desarrollo  
Version: 1.1  
Participantes: Carmen Gil, Laura Moreno, Miguel Serrano, Pablo Martin, equipo funcional de Admision

## Vision funcional

CITAS360 permitira al paciente consultar sus citas pendientes, confirmar asistencia, solicitar cancelacion y recibir recordatorios. El personal de Admision dispondra de trazabilidad de acciones realizadas por el paciente y podra revisar incidencias de sincronizacion.

## Procesos incluidos

1. Consulta de citas programadas.
2. Confirmacion de asistencia.
3. Solicitud de anulacion por parte del paciente.
4. Envio de recordatorio SMS.
5. Consulta de historico de cambios.
6. Panel de actividad para responsables de Admision.

## Reglas funcionales

- Una cita solo podra cancelarse desde el portal si faltan mas de 72 horas.
- Las citas de pruebas diagnosticas quedan fuera del piloto inicial.
- Las citas confirmadas por SMS deberan reflejarse en el HIS el mismo dia.
- Las agendas bloqueadas por especialistas no deberan exponerse al paciente.
- El canal movil replicara las mismas reglas del portal web.

## Decisiones pendientes

- Autenticacion de pacientes: clave temporal SMS, certificado digital o doble factor con datos administrativos.
- Estrategia de notificaciones: SMS unico, SMS mas correo electronico o mensajeria push para la app.
- Proveedor SMS alternativo si el actual no soporta acuse fiable.
- Despliegue progresivo por servicios o big-bang de consultas externas.
- Tratamiento de agenda antigua durante el piloto.

## Validacion funcional

Admision valida el flujo general de consulta y confirmacion. Queda pendiente validar el flujo de anulacion, porque algunos servicios siguen gestionando huecos libres mediante reglas locales no documentadas. El equipo funcional solicita que el motivo de cancelacion se capture de forma obligatoria.

## Observaciones

La version 1.1 corrige la matriz de permisos y elimina la posibilidad de reprogramacion directa por parte del paciente. MedTech Solutions considera que el cambio no afecta al plazo de mayo para entrega de integracion, siempre que las reglas de HIS se mantengan estables.

