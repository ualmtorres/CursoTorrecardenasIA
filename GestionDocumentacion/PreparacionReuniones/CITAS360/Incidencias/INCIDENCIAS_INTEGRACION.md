# CITAS360 - Registro de Incidencias de Integracion

Fecha: 19/08/2026  
Autor: Javier Ruiz  
Version: 1.0

| Fecha | Descripcion | Impacto | Resolucion | Estado |
| --- | --- | --- | --- | --- |
| 12/05/2026 | HIS devuelve codigo no documentado para huecos bloqueados en Traumatologia. | Confirmacion no fiable. | MedTech adapta mapeo local. | En curso |
| 26/05/2026 | Cancelacion en Dermatologia queda registrada en campo historico no consumido por el conector. | Cita aparece activa en portal. | Pendiente cambio de conector. | Abierta |
| 14/06/2026 | Agenda antigua sobrescribe estado confirmado durante sincronizacion nocturna. | Doble estado entre portal y HIS. | Se propone congelar agenda antigua en piloto. | Abierta |
| 02/07/2026 | API HIS limita peticiones por minuto sin aviso previo. | Errores intermitentes en carga. | Sistemas revisa throttling. | En analisis |
| 11/08/2026 | Confirmaciones masivas generan colas no procesadas hasta el dia siguiente. | Recordatorios inconsistentes. | Requiere reintento asincrono. | Abierta |

