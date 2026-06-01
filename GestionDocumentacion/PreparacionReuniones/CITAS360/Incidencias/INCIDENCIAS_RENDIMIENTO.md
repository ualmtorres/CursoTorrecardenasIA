# CITAS360 - Registro de Incidencias de Rendimiento

Fecha: 19/08/2026  
Autor: Laura Moreno  
Version: 1.0

| Fecha | Descripcion | Impacto | Resolucion | Estado |
| --- | --- | --- | --- | --- |
| 07/06/2026 | Portal tarda mas de 4 segundos al consultar citas con historico amplio. | Experiencia degradada. | Cache parcial de citas futuras. | Resuelta |
| 08/07/2026 | Prueba con 300 usuarios concurrentes eleva respuesta media a 8,7 segundos. | Riesgo para piloto. | Analisis de llamadas redundantes. | Abierta |
| 15/07/2026 | Confirmacion simultanea genera bloqueo temporal en API de citas. | Errores 503 intermitentes. | MedTech propone cola. | En curso |
| 04/08/2026 | Cuadro de mando tarda mas de 40 segundos en cargar datos diarios. | No usable por direccion. | Rehacer consultas agregadas. | Abierta |

