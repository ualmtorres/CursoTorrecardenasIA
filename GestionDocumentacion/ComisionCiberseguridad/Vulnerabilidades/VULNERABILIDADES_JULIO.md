# VULNERABILIDADES_JULIO

## Fecha
2025-07-23

## Resumen
- Vulnerabilidades criticas abiertas: 13
- Vulnerabilidades altas abiertas: 41
- Vulnerabilidades medias abiertas: 126
- Evolucion: El volumen crece por aplazamientos, equipos biomédicos sin soporte y dependencias de aplicaciones antiguas.

## Sistemas afectados
| Sistema | Tipo | Estado de remediacion |
|---|---|---|
| HUSA-SRV-AD01 / HUSA-SRV-AD02 | Active Directory | Parcheado condicionado por compatibilidad y ventana no aprobada |
| HUSA-SRV-PACS01 | Imagen medica | Excepcion temporal por dependencia de visor legacy |
| HUSA-SRV-LAB03 | Laboratorio | Pendiente de validacion con proveedor LIS |
| HUSA-VPN-GW01 | Acceso remoto | Requiere sustitucion o actualizacion mayor |
| Estaciones biomédicas UCI-MON-07 a UCI-MON-14 | Biomédico | Sin soporte del fabricante para sistema operativo |

## Criticas
- Ejecucion remota en componentes expuestos a redes internas clinicas.
- Elevacion de privilegios en servidores Windows con administracion compartida.
- Debilidades de autenticacion en VPN para perfiles tecnicos sin MFA.

## Altas y medias
- Cifrados debiles, servicios SMB heredados, librerias sin soporte y firmware antiguo.
- Riesgo acumulado por coexistencia de excepciones tecnicas durante varios meses.

## Observaciones
El informe tecnico no coincide plenamente con las cifras comunicadas en algunas actas, donde se informan menos vulnerabilidades criticas pendientes por considerar ciertas excepciones como riesgo aceptado.
