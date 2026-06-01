# AUDITORIA_INTERNA_Q1

## Fecha
2025-03-31

## Alcance
Sistemas corporativos, AD, VPN y servidores Windows/Linux.

## Hallazgos
| Hallazgo | Criticidad | Evidencias |
|---|---|---|
| Parcheado con retraso superior a 30 dias en 19 servidores | Alta | Muestras HUSA-SRV-AD02, HUSA-SRV-PACS01 y HUSA-SRV-LAB03 |
| Cuentas administrativas nominales sin revision formal desde 2024 | Media | Listado IAM exportado el 2025-03-20 |
| Segmentacion parcial entre redes ofimaticas y clinicas | Alta | Pruebas de ruta desde VLAN-ADM a VLAN-IMG |

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
