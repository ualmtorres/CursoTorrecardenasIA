# CITAS360 - Guia del Formador

Fecha: 24/08/2026  
Autor: Equipo docente  
Version: 1.0

## Uso previsto

Este documento no debe cargarse en NotebookLM. Sirve para validar si las respuestas del alumnado y de NotebookLM detectan la historia real del proyecto al cruzar actas, emails, sprints, KPIs, riesgos e incidencias.

## Historia completa real del proyecto

CITAS360 arranca en enero de 2026 como un proyecto saludable, con apoyo de direccion y alcance ambicioso pero aparentemente viable. Durante febrero y marzo se cierran analisis y arquitectura sobre un supuesto clave: que el HIS dispone de APIs estandar suficientes y que MedTech Solutions puede reutilizar conectores existentes.

En abril el portal empieza a mostrar avances, pero las decisiones de autenticacion y SMS siguen abiertas. En mayo aparecen los primeros problemas reales: los servicios HIS no responden de forma uniforme, la agenda antigua interfiere con estados y la cancelacion no es fiable. Las actas todavia presentan el proyecto como controlado, mientras los emails empiezan a revelar preocupaciones.

En junio MedTech solicita mover la entrega estable del conector HIS a julio, aunque las actas mantienen un tono prudente. La velocidad cae de 37 a 24 puntos y se acumulan defectos criticos. En julio las pruebas de carga muestran degradacion importante, Admision rechaza informalmente el flujo de cancelacion y el piloto de septiembre queda en riesgo. En agosto Direccion TIC exige plan de recuperacion.

El proyecto no esta abandonado: hay portal parcial, consulta operativa y equipos trabajando. El problema real es que los hitos centrales estan erosionados por decisiones sin cerrar, supuestos tecnicos incorrectos, retrabajo y una comunicacion oficial menos grave que la comunicacion privada.

## Cronologia de eventos

- 10/01: Documento de inicio aprueba alcance y 12 meses.
- 16/01: ACTA_01 registra arranque sin riesgos criticos.
- 14/02: Analisis funcional deja pendientes autenticacion, SMS, despliegue y agenda antigua.
- 28/02: Arquitectura asume APIs HIS estandar.
- 27/03: ACTA_06 recoge confirmacion de entrega HIS en mayo.
- 22/03: EMAIL_01 confirma entrega de conector HIS en mayo si hay ejemplos completos.
- 08/05: ACTA_08 mantiene entrega de integracion para cierre de mayo.
- 17/05: EMAIL_02 advierte que las APIs no son uniformes.
- 31/05: KPI_MAYO aun muestra salud razonable.
- 03/06: EMAIL_03 solicita mover conector estable a segunda quincena de julio.
- 30/06: KPI_JUNIO evidencia deterioro.
- 09/07: EMAIL_04 revela pruebas de carga graves.
- 24/07: EMAIL_05 indica rechazo funcional de Admision.
- 31/07: KPI_JULIO confirma deterioro acusado.
- 14/08: ACTA_12 reconoce necesidad de plan de recuperacion.
- 18/08: EMAIL_06 exige plan con fechas verificables.

## Contradicciones introducidas

- Actas de marzo y mayo indican entrega HIS en mayo; EMAIL_03 mueve entrega estable a julio.
- Arquitectura dice que la integracion HIS usa APIs estandar; incidencias y EMAIL_02 muestran codigos y campos no documentados.
- ACTA_08 dice que no hay riesgos criticos; RIESGOS_ESCALADOS registra integracion HIS y rendimiento como criticos en agosto.
- ACTA_10 habla de incidencias tecnicas en correccion y sin riesgos criticos; SPRINT_10 y EMAIL_03 muestran replanificacion relevante.
- ACTA_11 menciona "ajustes tecnicos" de rendimiento; EMAIL_04 cuantifica un problema grave con 8,7 segundos y errores.
- ACTA_11 habla de comentarios funcionales; EMAIL_05 lo califica como rechazo funcional.
- PROYECTO_INICIO plantea despliegue progresivo inicial; decisiones posteriores mantienen abierto progresivo frente a big-bang.

## Riesgos ocultos o distribuidos

- La integracion HIS es mas compleja de lo contratado: aparece en EMAIL_02, EMAIL_03, sprints e incidencias antes de ser escalada.
- El rendimiento real esta oculto en EMAIL_04 e INCIDENCIAS_RENDIMIENTO, no en las actas iniciales.
- El rechazo funcional de Admision aparece claramente solo en EMAIL_05 e INCIDENCIAS_USUARIOS.
- El proveedor SMS afecta auditoria y recordatorios, pero aparece repartido entre analisis, sprints, riesgos y estado actual.
- La agenda antigua genera dobles estados y sobrescritura nocturna, distribuido entre sprints e incidencias.

## Decisiones abiertas

- Autenticacion de pacientes.
- Estrategia de notificaciones.
- Proveedor SMS alternativo.
- Despliegue progresivo o big-bang.
- Integracion y convivencia con agenda antigua.

## Compromisos incumplidos o retrasados

- MedTech: entrega estable del conector HIS prevista para mayo, retrasada a julio y aun no estabilizada en agosto.
- Sistemas: ejemplos completos y ventanas de preproduccion llegaron tarde o con disponibilidad limitada.
- Admision: confirmacion sobre agenda antigua y validacion funcional se retrasan; finalmente hay rechazo no formalizado.
- Desarrollo: cuadro de mando y rendimiento no alcanzan calidad suficiente en julio.
- Direccion: decision sobre autenticacion y SMS se aplaza repetidamente.

## Respuestas esperadas para la demo

1. Estado real para direccion: proyecto recuperable pero en riesgo alto, con portal parcial y retrasos en HIS, rendimiento, SMS, app y aceptacion funcional.
2. Principales riesgos actuales: HIS, rendimiento, aceptacion de Admision, SMS, agenda antigua, decisiones abiertas y perdida de velocidad.
3. Compromisos abiertos: plan de recuperacion MedTech, ventanas de preproduccion, validacion funcional, piloto reducido, reestimacion de backlog, autenticacion y SMS.
4. Decisiones pendientes: autenticacion, notificaciones, proveedor SMS, despliegue, agenda antigua.
5. Preguntas al proveedor: fecha real del conector estable, esfuerzo contratado frente a cambio, plan de rendimiento, recursos asignados, mitigacion de agenda antigua, soporte a SMS y reintentos.
6. Hitos mas retrasados: integracion HIS, cancelacion, SMS, app movil, cuadro de mando y piloto completo.
7. Contradicciones: entrega HIS mayo/julio, APIs estandar/no estandar, sin riesgos criticos/riesgos escalados, ajustes tecnicos/problemas graves de carga, comentarios de mejora/rechazo funcional.
8. Responsables con mas acciones abiertas: David Vega, Javier Ruiz, Carmen Gil y Miguel Serrano; Pablo Martin acumula seguimiento y reestimacion.
9. Evolucion: saludable en enero-marzo, primeras tensiones en abril-mayo, deterioro visible en junio-julio, escalado en agosto.
10. Atencion inmediata: plan de recuperacion, alcance realista del piloto, cierre de decisiones, integracion HIS, rendimiento y validacion funcional.

