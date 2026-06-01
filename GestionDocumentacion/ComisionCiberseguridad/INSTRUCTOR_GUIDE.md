# HUSA Ciberseguridad - Guia del Formador

Fecha: 01/06/2026  
Autor: Equipo docente  
Version: 1.1

## Uso previsto

Este documento no debe cargarse en NotebookLM. Sirve para validar si las respuestas del alumnado y de NotebookLM detectan la situacion real de ciberseguridad al cruzar actas, auditorias, informes de vulnerabilidades, inventarios, incidencias, emails, planes de accion y KPIs.

El corpus que si debe importarse esta en las subcarpetas `Actas`, `Auditorias`, `Vulnerabilidades`, `Inventario`, `Incidencias`, `Emails`, `Planes` y `KPIs`.

## Historia completa real del escenario

El Hospital Universitario Santa Aurelia empieza enero de 2025 con una situacion aparentemente controlada. La Direccion TIC convoca una Comision Extraordinaria de Ciberseguridad para ordenar riesgos y revisar prioridades, pero las primeras actas todavia presentan el estado como razonablemente estable. Hay vulnerabilidades y acciones abiertas, aunque nada parece critico por si solo.

Durante el primer trimestre aparecen los primeros sintomas: retrasos de parcheado, cuentas privilegiadas sin revision completa, segmentacion parcial y dependencias entre Active Directory, PACS, laboratorio y VPN. Las actas mantienen un tono optimista, mientras la auditoria interna Q1 ya deja evidencias de servidores con retrasos superiores a 30 dias y rutas de red entre segmentos que no deberian comunicarse tan facilmente.

En abril y mayo la situacion empieza a deteriorarse. El informe de vulnerabilidades de abril sube el numero de criticidades y muestra problemas repetidos en PACS, AD secundario y laboratorio. Los KPIs de mayo todavia son defendibles, pero ya marcan deterioro: parcheado al 90%, 7 vulnerabilidades criticas abiertas, SLA al 83% y solo 38% de cuentas privilegiadas revisadas. En paralelo, SecureHealth Consulting advierte por email de un patron repetido de intentos fallidos, cuentas tecnicas amplias y servidores sin parchear.

En junio se rompe una expectativa importante: MFA no finaliza segun lo previsto. Laura Moreno informa de incompatibilidades con Radiologia y proveedores biomedicos, y tambien de fatiga del equipo de Sistemas. A partir de aqui el problema deja de ser una lista de tareas pendientes y se convierte en una acumulacion de riesgo: MFA parcial, VPN antigua, Active Directory heredado, exceso de privilegios y equipos biomedicos sin soporte.

En julio y agosto las senales operativas aumentan. Aparecen accesos privilegiados fuera de horario, incremento de bloqueos de cuentas tecnicas, actividad VPN anomala y microsegmentacion incompleta. Pablo Martin advierte que hay trafico de UCI y PACS que nadie quiere firmar como necesario, pero tampoco autorizan cortar. Los KPIs de agosto confirman la tendencia: baja el parcheado, suben las vulnerabilidades criticas y empeora el SLA.

En septiembre y octubre se hace visible que los problemas son recurrentes, no puntuales. La auditoria Q3 mantiene hallazgos de segmentacion, cuentas compartidas y activos sin propietario. El informe de octubre eleva la situacion a 24 vulnerabilidades criticas abiertas y 61 altas. Algunas actas siguen hablando de situacion "estable con salvedades" o "fase de refuerzo", pero el inventario y los informes tecnicos muestran sistemas legacy, 17 activos biomedicos sin responsable confirmado y 42 servidores fuera de soporte identificados en el seguimiento de parches.

En noviembre y diciembre la auditoria externa anual formula la clave del escenario: el riesgo agregado es superior al reflejado en las actas mensuales. La auditoria RGPD suma preocupacion por exceso de privilegios y trazabilidad incompleta fuera de horario. El email de SecureHealth del 04/12 pide escalado por coincidencia temporal entre VPN, bloqueos de cuentas y actividad administrativa nocturna. No hay evidencia suficiente para declarar un incidente, pero si una tendencia emergente que justifica investigacion tecnica urgente.

La historia real no es que el hospital haya sufrido un incidente confirmado. La historia real es que la organizacion esta normalizando demasiadas excepciones y esta infravalorando un riesgo acumulado. El deterioro nace de decisiones abiertas, deuda tecnica, dependencia del proveedor, fatiga operativa y senales de actividad anomala que solo resultan preocupantes cuando se correlacionan.

## Cronologia de eventos

- 20/01: VULNERABILIDADES_ENERO registra 3 criticidades, 14 altas y 63 medias; la situacion aun parece controlada.
- 28/01: ACTA_COMISION_01 abre el seguimiento extraordinario con una vision gestionable.
- 11/02: INCIDENTES_Q1 registra bloqueo de 9 cuentas por contrasenas fallidas.
- 18/03: INCIDENTES_Q1 recoge VPN desde ubicacion no habitual para proveedor, validada como falso positivo.
- 20/03: AUDITORIA_INTERNA_Q1 evidencia revision incompleta de cuentas privilegiadas.
- 21/03: EMAIL_01 advierte que se estan dando por cerradas vulnerabilidades que dependen de excepciones.
- 31/03: AUDITORIA_INTERNA_Q1 identifica parcheado retrasado, cuentas administrativas sin revision formal y segmentacion parcial.
- 17/04: INCIDENTES_Q2 registra malware contenido en estacion administrativa.
- 22/04: VULNERABILIDADES_ABRIL sube a 7 criticidades y 26 altas.
- 16/05: EMAIL_02 de SecureHealth advierte de intentos fallidos, cuentas tecnicas amplias y servidores sin parchear.
- 31/05: KPI_MAYO muestra 90% de parcheado, 7 criticidades abiertas y 38% de cuentas privilegiadas revisadas.
- 09/06: INCIDENTES_Q2 recoge errores de configuracion en reglas de firewall clinico.
- 28/06: EMAIL_03 confirma que MFA no llega a junio por incompatibilidades y fatiga de Sistemas.
- 30/06: AUDITORIA_INTERNA_Q2 repite retrasos de parcheado y eleva preocupacion por AD heredado.
- 23/07: VULNERABILIDADES_JULIO sube a 13 criticidades y 41 altas.
- 31/07: INCIDENTES_Q3 registra acceso privilegiado fuera de horario a HUSA-SRV-PACS01.
- 19/08: INCIDENTES_Q3 registra incremento de bloqueos de cuentas tecnicas.
- 22/08: EMAIL_04 advierte que la microsegmentacion no puede completarse sin propietarios ni mapa de dependencias.
- 31/08: KPI_AGOSTO muestra deterioro: 84% de parcheado, 13 criticidades abiertas y SLA al 71%.
- 14/09: INCIDENTES_Q3 registra actividad VPN anomala desde dos paises en 24 horas.
- 30/09: AUDITORIA_INTERNA_Q3 repite segmentacion incompleta, cuentas compartidas y activos sin propietario.
- 10/10: INCIDENTES_Q4 registra intentos repetidos contra portal de proveedores.
- 24/10: VULNERABILIDADES_OCTUBRE sube a 24 criticidades, 61 altas y 174 medias.
- 31/10: EMAIL_05 anticipa que las actas muestran progreso, pero los datos tecnicos reflejan deterioro.
- 06/11: INCIDENTES_Q4 registra uso de cuenta HUSA-admin-guardia en madrugada sin aprobacion previa.
- 18/11: AUDITORIA_RGPD detecta exceso de privilegios y trazabilidad incompleta fuera de horario.
- 30/11: KPI_NOVIEMBRE muestra 78% de parcheado, 21 criticidades abiertas y 19 hallazgos pendientes.
- 03/12: INCIDENTES_Q4 correlaciona VPN y autenticacion AD.
- 04/12: EMAIL_06 pide reunion tecnica urgente por coincidencia entre VPN, bloqueos de cuentas y actividad administrativa nocturna.
- 12/12: AUDITORIA_INTERNA_Q4 mantiene 24 vulnerabilidades criticas abiertas y prueba de restauracion completa no ejecutada.
- 15/12: AUDITORIA_EXTERNA_ANUAL concluye que el riesgo agregado es superior al reflejado en actas.
- 19/12: ACTA_COMISION_12 cierra el ano sin incidente mayor declarado, pero con decisiones clave todavia abiertas.

## Contradicciones introducidas

- Las actas describen varios meses como controlados o gestionables; KPIs, auditorias y vulnerabilidades muestran deterioro progresivo.
- Algunas actas declaran pocas o ninguna vulnerabilidad critica pendiente; VULNERABILIDADES_ABRIL, JULIO y OCTUBRE muestran criticidades abiertas y crecientes.
- Las actas tratan excepciones como riesgo aceptado; EMAIL_01 advierte que esas excepciones estan ocultando vulnerabilidades reales.
- ACTA_COMISION_06 mantiene seguimiento de MFA como proyecto en marcha; EMAIL_03 confirma que no se puede cerrar en junio.
- Las actas informan avance de inventario y propietarios; EQUIPOS_BIOMEDICOS mantiene 17 activos sin responsable tecnico o funcional confirmado.
- La situacion oficial habla de progreso en segmentacion; EMAIL_04 indica que en produccion faltan propietarios y mapas de dependencias.
- Las actas reducen el peso de eventos aislados; INCIDENTES_Q3, INCIDENTES_Q4 y EMAIL_06 permiten ver un patron cuando se correlacionan.
- La comision mantiene abierto PAM y SOC externo como decisiones presupuestarias; auditorias y RGPD muestran que ya son controles necesarios para trazabilidad y privilegios.
- El seguimiento de parches identifica 42 servidores fuera de soporte; las actas comunican porcentajes de parcheado relativamente altos.
- La auditoria externa anual concluye que el riesgo agregado es mayor que el reflejado oficialmente.

## Riesgos ocultos o distribuidos

- El retraso de parcheado aparece repartido entre vulnerabilidades, auditorias, KPIs, planes y emails; no se concentra en un unico documento.
- Active Directory heredado aparece como dependencia tecnica, no como crisis explicita, pero condiciona MFA, PACS, laboratorio, privilegios y autenticacion.
- El riesgo biomédico se reparte entre inventario, auditorias, planes y segmentacion; los equipos sin soporte no aparecen como incidente critico aislado.
- La segmentacion incompleta aparece en auditorias, emails y planes de red; las actas la presentan como avance parcial.
- El exceso de privilegios aparece en cuentas, RGPD, incidentes fuera de horario y necesidad de PAM.
- La dependencia de SecureHealth Consulting se ve en SIEM, escaneo, recomendaciones y escalados; no se formula como debilidad hasta la auditoria externa.
- La fatiga de Sistemas aparece sobre todo en EMAIL_03, pero explica retrasos de parches, MFA y validaciones tecnicas.
- El posible incidente futuro se infiere al cruzar bloqueos, VPN anomala, actividad nocturna, cuentas privilegiadas y criticidades sin cerrar.

## Decisiones abiertas

- MFA obligatorio para perfiles tecnicos, proveedores y accesos VPN.
- Renovacion de Active Directory y elevacion del nivel funcional.
- Implantacion de PAM para cuentas privilegiadas y sesiones administrativas.
- Contratacion o formalizacion de SOC externo.
- Microsegmentacion completa de redes clinicas y biomedicas.
- Sustitucion de VPN o actualizacion mayor de la plataforma.
- Modelo de gobierno para dispositivos biomedicos legacy.

## Compromisos incumplidos o retrasados

- Seguridad: revision de cuentas privilegiadas queda parcial durante todo el ano; PAM sigue pendiente.
- Sistemas: parcheado y cierre de vulnerabilidades criticas se retrasa de forma acumulativa; 24 criticidades siguen abiertas en diciembre.
- Infraestructura: renovacion de Active Directory no se aprueba y los controladores heredados siguen condicionando cambios.
- Redes: microsegmentacion avanza en pruebas, pero no se completa en produccion por falta de dependencias y propietarios.
- Continuidad: prueba de restauracion completa y ejercicio de crisis ciber se aplazan.
- SecureHealth Consulting: entrega lecturas tecnicas y alertas, pero el hospital depende excesivamente de su operacion para SIEM y escaneo.
- Direccion TIC: decisiones de MFA, PAM, SOC, AD, VPN y biomédicos legacy se aplazan repetidamente.

## Respuestas esperadas para la demo

1. Estado real para Direccion: situacion sin incidente grave declarado, pero con riesgo alto y creciente por acumulacion de vulnerabilidades, deuda tecnica, privilegios excesivos, MFA incompleto, AD heredado, biomédicos legacy y segmentacion incompleta.
2. Principales riesgos actuales: parcheado retrasado, Active Directory obsoleto, VPN con MFA parcial, equipos biomedicos sin soporte, exceso de privilegios, cuentas tecnicas amplias, microsegmentacion incompleta y continuidad no probada.
3. Acciones pendientes: cierre de criticidades, revision completa de privilegios, renovacion AD, microsegmentacion, MFA obligatorio, decision PAM, SOC externo, sustitucion VPN, inventario biomédico con propietarios y prueba de restauracion completa.
4. Hallazgos repetidos: parcheado con retraso, segmentacion parcial, cuentas privilegiadas sin revision completa, activos sin propietario, AD heredado y dependencias legacy.
5. Decisiones pendientes: MFA, AD, PAM, SOC externo, microsegmentacion, VPN y gestion de biomédicos legacy.
6. Responsables con mas acciones abiertas: Laura Moreno por parcheado, sistemas y aplicaciones; Carlos Navarro por seguridad, privilegios y MFA; Javier Ruiz por AD e infraestructura heredada; Pablo Martin por VPN y segmentacion; Marta Sanchez por continuidad; Ana Beltran por decisiones estrategicas.
7. Evolucion: estable en enero-febrero, primeras senales en marzo-abril, deterioro visible en mayo-junio, acumulacion operativa en julio-septiembre y riesgo alto en octubre-diciembre.
8. Contradicciones: tono optimista de actas frente a KPIs y auditorias; criticidades declaradas como aceptadas frente a vulnerabilidades abiertas; propietarios supuestamente asignados frente a 17 activos biomédicos sin responsable; MFA previsto en junio frente a retrasos; progreso de segmentacion frente a dependencias sin mapear.
9. Preguntas a SecureHealth: que alertas correlacionadas ven, que evidencias sostienen el escalado, que cobertura real tiene el SIEM, que activos quedan fuera, que priorizacion recomiendan, que tareas dependen del hospital y que limitaciones impiden confirmar o descartar actividad hostil.
10. Tres iniciativas prioritarias: cerrar criticidades y parcheado legacy con excepciones formales, implantar MFA/PAM para accesos privilegiados y VPN, y acelerar microsegmentacion junto con gobierno de biomédicos legacy. Como soporte, decidir renovacion AD y mejorar continuidad.
11. Activos de mayor riesgo: HUSA-SRV-AD01, HUSA-SRV-AD02, HUSA-SRV-PACS01, HUSA-SRV-LAB03, HUSA-VPN-GW01, HUSA-SRV-BKP01, estaciones UCI-MON-07 a UCI-MON-14, RX-EST-03 y cuentas `HUSA-admin-guardia`, `svc_pacs_sync`, `svc_farma_his` y `vpn-proveedor-biomed`.
12. Senales que anticipan incidente futuro: bloqueos de cuentas, VPN desde ubicaciones inusuales, actividad administrativa nocturna, intentos contra portal de proveedores, criticidades abiertas mas de 90 dias, cuentas compartidas, MFA incompleto y trazabilidad RGPD insuficiente.

## Prompts recomendados para NotebookLM

- Resume en una pagina el estado real de ciberseguridad para Direccion, separando hechos, inferencias e hipotesis.
- Reconstruye una cronologia de enero a diciembre con los hitos que muestran deterioro.
- Detecta contradicciones entre actas, auditorias, KPIs, vulnerabilidades, inventario y emails.
- Que acciones comprometidas siguen pendientes y quien es responsable?
- Que decisiones estrategicas continuan abiertas y que impacto tiene cada una?
- Observas una tendencia emergente que no este tratada explicitamente como incidente?
- Que preguntas deberia plantear Ana Beltran a SecureHealth Consulting?
- Prioriza tres iniciativas para los proximos 90 dias y justificalas con evidencias del corpus.

## Criterios de evaluacion

Una respuesta buena debe citar documentos concretos, evitar afirmar que hay un ataque confirmado, distinguir evidencias de hipotesis y explicar por que la situacion empeora aunque las actas mantengan un tono prudente.

Una respuesta incompleta suele limitarse a resumir actas, listar vulnerabilidades sin correlacionarlas o aceptar como cierre real acciones que en los planes y emails aparecen retrasadas.
