# AUDITORIA_INTERNA_Q2

## Fecha
2025-06-30

## Alcance
Continuidad, aplicaciones clinicas, red y excepciones de parcheado.

## Hallazgos
| Hallazgo | Criticidad | Evidencias |
|---|---|---|
| Se repite retraso de parcheado, ahora en 31 servidores | Alta | Backlog SEGUIMIENTO_PARCHES actualizado el 2025-06-21 |
| Controladores de dominio con version y nivel funcional heredados | Alta | AD01 y AD02 mantienen dependencias con aplicaciones antiguas |
| MFA no desplegado en perfiles tecnicos de VPN | Media | Excepciones aprobadas por incompatibilidad con cliente antiguo |

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
