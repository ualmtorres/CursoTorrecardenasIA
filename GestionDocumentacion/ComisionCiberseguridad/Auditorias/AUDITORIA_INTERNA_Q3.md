# AUDITORIA_INTERNA_Q3

## Fecha
2025-09-30

## Alcance
Privilegios, biomédicos, trazabilidad y red.

## Hallazgos
| Hallazgo | Criticidad | Evidencias |
|---|---|---|
| Hallazgo recurrente: segmentacion incompleta en equipamiento biomédico | Alta | Ecografos y estaciones de monitorizacion comparten rutas con servicios internos |
| Cuentas privilegiadas compartidas en tareas de guardia | Alta | Evidencia en tickets nocturnos de julio y agosto |
| Activos sin propietario claro en electromedicina | Media | 17 activos sin responsable funcional asignado |

## Recomendaciones
- Aprobar calendario cerrado de remediacion con excepciones justificadas por riesgo asistencial.
- Separar decisiones presupuestarias de medidas urgentes de contencion.
- Implantar revision mensual de privilegios, evidencias y responsables.
- Priorizar MFA, PAM, renovacion AD, microsegmentacion y gobierno de biomédicos legacy.

## Plan de accion
| Accion | Responsable | Fecha | Estado |
|---|---|---:|---|
| Cierre de vulnerabilidades criticas no excepcionadas | Laura Moreno | 2026-01-31 | Abierta |
| Decision sobre renovacion Active Directory | Ana Beltran | 2026-02-15 | Pendiente |
| Propuesta PAM y SOC externo | Carlos Navarro y David Vega | 2026-01-20 | En preparacion |
| Inventario biomédico con propietario tecnico y funcional | Javier Ruiz | 2026-02-28 | Abierta |

## Nota de consistencia
Varios hallazgos ya aparecian en revisiones anteriores. La criticidad se eleva cuando el mismo punto combina retraso tecnico, ausencia de propietario y exposicion mediante VPN o cuentas privilegiadas.
