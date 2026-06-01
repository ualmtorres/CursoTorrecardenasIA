# AUDITORIA_RGPD

## Fecha
2025-11-18

## Alcance
Controles de acceso, trazabilidad y minimizacion en sistemas con datos personales.

## Hallazgos
| Hallazgo | Criticidad | Evidencias |
|---|---|---|
| Exceso de privilegios en perfiles tecnicos con acceso a sistemas clinicos | Alta | Matriz de permisos HIS y PACS |
| Registro de accesos privilegiados incompleto fuera de horario | Alta | Eventos VPN y administracion local sin justificacion documentada |
| Inventario de tratamientos dependiente de aplicaciones no actualizadas | Media | Farmacia y laboratorio conservan conectores antiguos |

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
