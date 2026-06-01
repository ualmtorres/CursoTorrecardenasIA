# Oferta técnica - Hospital Systems Group

## Resumen ejecutivo

Hospital Systems Group propone implantar HSG CitaSalud, plataforma consolidada en entornos hospitalarios con amplia experiencia en gestión de admisión, citación y procesos administrativos. La propuesta destaca conocimiento del ámbito hospitalario, rapidez de implantación y reutilización de conectores existentes.

HSG plantea un calendario de 18 meses, con producción progresiva desde el mes 12. La empresa sostiene que su experiencia previa permite reducir esfuerzo de análisis y acelerar las integraciones.

## Cobertura funcional

CitaSalud cubre agendas, citación multicanal, reprogramación, cancelación, listas de espera, gestión de ausencias, reglas por servicio, portal web y app móvil. Incluye administración por perfiles y gestión de mensajes.

La oferta incorpora cuadro de mando con actividad diaria, citas por canal, ausencias, tiempos de espera, cancelaciones y uso de notificaciones. HSG propone adaptar informes existentes a DataHUSA.

El portal permite consultar citas, justificar asistencia, cancelar y recibir instrucciones. La app móvil incluye notificaciones push y consulta de agenda. HSG indica que algunas operaciones administrativas avanzadas estarán disponibles inicialmente para servicios incluidos en el piloto y se extenderán por oleadas.

## Arquitectura

La arquitectura se basa en un núcleo transaccional, portal web, app móvil, módulo de integración y módulo BI. HSG propone despliegue en infraestructura designada por HUSA o nube europea gestionada.

La disponibilidad comprometida es 99,92%. La solución dispone de monitorización técnica, logs centralizados y alarmas. El dimensionamiento se basa en 60.000 usuarios registrados y 900 sesiones concurrentes, ampliable mediante nodos adicionales.

HSG subraya que la plataforma ya opera en entornos hospitalarios con agendas complejas, lo que reduce incertidumbre funcional.

## Integraciones

HSG declara incluidos los conectores con HIS, MPI, laboratorio, imagen, SMS, push y analítica. Para HUSA-Core v8 propone reutilizar un conector HL7 similar al empleado en otros proyectos, sujeto a ajuste de mapeos. Para LabAurelia e ImagoSuite prevé intercambio de eventos básicos y estados de cita.

La oferta estima 620 horas totales para integraciones, distribuidas entre HIS/MPI, laboratorio, imagen, identidad, SMS, push y DataHUSA. Se indica que esta cifra podrá optimizarse si HUSA facilita especificaciones definitivas y acceso temprano a entornos.

## Seguridad y privacidad

CitaSalud incluye control de acceso por rol, MFA para administradores, cifrado, trazabilidad y auditoría. HSG se compromete a colaborar en la evaluación de impacto y a ejecutar pruebas de seguridad. La empresa propone usar componentes ya validados en otros hospitales.

La oferta menciona soporte remoto seguro mediante bastión o VPN corporativa. El detalle de gestión de secretos y rotación de credenciales se aportará en fase de diseño técnico.

## Migración

HSG incluye migración de citas futuras, agendas, recursos y catálogos. Para histórico de reprogramaciones propone una migración selectiva centrada en los datos requeridos por informes de actividad. El presupuesto reserva 140 horas para migración y conciliación.

HSG afirma que la migración completa está incluida, aunque su plan asume que el hospital entregará extracciones normalizadas desde sistemas origen.

## Plan de implantación

* Mes 1: arranque y confirmación de alcance.
* Meses 2-3: análisis funcional y técnico.
* Meses 4-6: parametrización, portal y app base.
* Meses 7-9: integraciones HIS/MPI, SMS y push.
* Meses 10-11: laboratorio, imagen y analítica.
* Mes 12: piloto en consultas externas y radiología.
* Meses 13-15: extensión a servicios principales.
* Meses 16-18: estabilización, formación final y cierre.

HSG propone trabajar con decisiones semanales y aceptación por silencio positivo cuando no haya observaciones en cinco días laborables.

## Equipo propuesto

Equipo medio estimado de 6,2 ETC, con director de proyecto, jefe funcional sanitario, arquitecto técnico compartido, dos analistas de integración, consultor de parametrización, desarrollador, formador y soporte. Los perfiles senior se concentran en arranque, diseño y revisiones de hitos.

HSG indica que su conocimiento sectorial permite una menor dedicación media sin comprometer resultados.

## Soporte y formación

Se incluye soporte crítico 24x7, soporte ordinario 8:00-17:00, 180 horas evolutivas y 24 sesiones de formación. El acompañamiento presencial al arranque se concentra en las dos primeras semanas de producción.

## Riesgos identificados

* Acceso tardío a entornos.
* Validación lenta de catálogos.
* Disponibilidad de interlocutores funcionales.
* Dependencia de especificaciones definitivas de sistemas departamentales.

HSG considera los riesgos controlables por su experiencia hospitalaria y metodología acelerada.

