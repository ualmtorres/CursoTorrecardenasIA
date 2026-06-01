# SERVIDORES

## Inventario resumido
| Activo | Funcion | SO | Propietario | Riesgo |
|---|---|---|---|---|
| HUSA-SRV-AD01 | Controlador dominio primario | Windows Server 2012 R2 | Javier Ruiz | Alto: version heredada y dependencias antiguas |
| HUSA-SRV-AD02 | Controlador dominio secundario | Windows Server 2012 R2 | Javier Ruiz | Alto: parches diferidos |
| HUSA-SRV-PACS01 | Imagen medica | Windows Server 2012 R2 | Laura Moreno | Alto: visor legacy bloquea actualizacion |
| HUSA-SRV-LAB03 | Laboratorio | Windows Server 2016 | Laura Moreno | Medio: proveedor LIS valida lento |
| HUSA-SRV-FAR02 | Farmacia | Linux 7.x | Laura Moreno | Medio: librerias obsoletas |
| HUSA-SRV-BKP01 | Copias | Appliance propietario | Marta Sanchez | Alto: prueba de restauracion incompleta |
| HUSA-VPN-GW01 | VPN | Firmware legacy | Pablo Martin | Alto: MFA parcial y reglas antiguas |

## Dependencias ocultas
- PACS y laboratorio usan grupos de AD heredados que impiden elevar nivel funcional sin pruebas.
- Farmacia mantiene conector con HIS mediante cuenta tecnica con privilegios superiores a los necesarios.
- Backup depende de rutas de red que todavia atraviesan segmentos compartidos.
