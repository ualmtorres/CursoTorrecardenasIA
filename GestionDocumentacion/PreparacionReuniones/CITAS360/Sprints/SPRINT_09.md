# CITAS360 - Sprint 09

Fecha: 18/05/2026 - 31/05/2026  
Autor: Pablo Martin, Scrum Master  
Version: 1.0  
Participantes: Laura Moreno, David Vega, Javier Ruiz, Carmen Gil

## Objetivos

- Estabilizar consulta de citas contra HIS.
- Avanzar confirmacion y cancelacion con servicios piloto.
- Incorporar cambios solicitados por usuarios de Admision.
- Preparar primera version de cuadro de mando.

## Historias

| Historia | Descripcion | Responsable | Estado |
| --- | --- | --- | --- |
| H-38 | Como paciente quiero ver solo citas futuras. | MedTech | Terminada |
| H-39 | Como Admision quiero distinguir estados sincronizados y pendientes. | Desarrollo HUSA | Terminada |
| H-40 | Como paciente quiero cancelar una cita si faltan mas de 72 horas. | MedTech | No terminada |
| H-41 | Como directivo quiero ver citas confirmadas por servicio. | Desarrollo HUSA | Parcial |

## Tareas

- Ajustar Dermatologia por campo historico de anulaciones.
- Crear filtros de citas futuras.
- Diseñar etiquetas de estado para usuarios.
- Preparar extraccion diaria para cuadro de mando.

## Bloqueos

La cancelacion depende de un comportamiento del HIS distinto entre servicios. La agenda antigua sobrescribe algunos estados durante la sincronizacion nocturna.

## Incidencias

- Citas anuladas siguen apareciendo activas.
- El cuadro de mando no recibe anulaciones fiables.
- Usuarios piloto no comprenden el estado "pendiente de sincronizar".

## Velocidad

Velocidad prevista: 40 puntos.  
Velocidad real: 31 puntos.

## Comentario

La velocidad baja por retrabajo de integracion. Se recomienda no comprometer nuevas historias de app movil hasta cerrar confirmacion y cancelacion.

