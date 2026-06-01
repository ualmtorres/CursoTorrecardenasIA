# AUDITORIA_INTERNA_Q4

## Fecha
2025-12-12

## Alcance
Cierre anual de remediacion, accesos, vulnerabilidades y continuidad.

## Hallazgos
| Hallazgo | Criticidad | Evidencias |
|---|---|---|
| Persisten 24 vulnerabilidades criticas abiertas | Critica | Escaneo de octubre y validacion de noviembre |
| Prueba de restauracion completa no ejecutada | Alta | Plan de continuidad aplazado dos veces |
| Renovacion de Active Directory sin decision aprobada | Alta | Actas de mayo a noviembre mantienen el punto abierto |

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
