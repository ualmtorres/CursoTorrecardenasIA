# CUENTAS_PRIVILEGIADAS

## Cuentas y perfiles
| Cuenta o grupo | Uso | Responsable | Revision |
|---|---|---|---|
| Domain Admins | Administracion AD | Carlos Navarro | Parcial |
| HUSA-admin-guardia | Soporte fuera de horario | Laura Moreno | Uso compartido detectado |
| svc_pacs_sync | Integracion PACS | Laura Moreno | Privilegios excesivos |
| svc_farma_his | Conector farmacia-HIS | Laura Moreno | Pendiente reduccion |
| vpn-proveedor-biomed | Acceso proveedor biomédico | Pablo Martin | Sin MFA obligatorio |
| secops_securehealth | Operacion SIEM | David Vega | Dependencia externa alta |

## Riesgos
- Revision anual incompleta y sin evidencias uniformes.
- Accesos administrativos fuera de horario aparecen en incidentes de Q3 y Q4.
- PAM no implantado; la trazabilidad depende de logs dispersos.
