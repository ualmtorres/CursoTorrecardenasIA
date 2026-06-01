# AUDITORIA_EXTERNA_ANUAL

## Fecha
2025-12-15

## Alcance
Revision independiente de madurez de ciberseguridad hospitalaria.

## Hallazgos
| Hallazgo | Criticidad | Evidencias |
|---|---|---|
| Riesgo agregado superior al reflejado en actas mensuales | Alta | Divergencia entre KPIs tecnicos y actas de comision |
| Dependencia operativa relevante de SecureHealth Consulting | Media | Falta de transferencia completa en gestion SIEM y escaneo |
| Infraestructura legacy condiciona parcheado, segmentacion y MFA | Critica | Dependencias cruzadas AD, PACS, laboratorio y biomédicos |

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
