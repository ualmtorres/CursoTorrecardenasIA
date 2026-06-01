# APLICACIONES

## Inventario de aplicaciones
| Aplicacion | Uso | Responsable | Estado |
|---|---|---|---|
| HUSA-HIS | Historia clinica | Laura Moreno | Soportada, con conectores antiguos |
| HUSA-PACS | Imagen medica | Laura Moreno | Parcialmente legacy |
| HUSA-LIS | Laboratorio | Laura Moreno | Pendiente validacion de parches |
| HUSA-FARMA | Farmacia | Laura Moreno | Dependencia con librerias no soportadas |
| Portal Proveedores | Gestion externa | Carlos Navarro | MFA no obligatorio para todos los perfiles |
| Consola SIEM SecureHealth | Monitorizacion | David Vega | Operacion externalizada |

## Riesgos
- Existen aplicaciones criticas que siguen autenticando contra grupos antiguos de Active Directory.
- Algunas cuentas tecnicas no tienen propietario funcional claro.
- La documentacion de dependencias se actualiza a demanda, no como proceso formal.
