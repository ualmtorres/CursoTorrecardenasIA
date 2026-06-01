# CITAS360 - Sprint 11

Fecha: 22/06/2026 - 19/07/2026  
Autor: Pablo Martin, Scrum Master  
Version: 1.0  
Participantes: Laura Moreno, David Vega, Javier Ruiz, Carmen Gil, Miguel Serrano

## Objetivos

- Ejecutar pruebas de carga.
- Preparar piloto minimo viable.
- Resolver defectos criticos de confirmacion y cancelacion.
- Avanzar app movil con alcance reducido.

## Historias

| Historia | Descripcion | Responsable | Estado |
| --- | --- | --- | --- |
| H-46 | Como paciente quiero consultar citas desde app movil. | MedTech | Parcial |
| H-47 | Como sistema quiero soportar 500 usuarios concurrentes. | MedTech / Desarrollo HUSA | No terminada |
| H-48 | Como Admision quiero estado final claro tras cancelacion. | Desarrollo HUSA | No terminada |
| H-49 | Como direccion quiero panel diario de actividad. | Desarrollo HUSA | Parcial |
| H-50 | Como sistema quiero sincronizar agenda antigua sin pisar estados. | MedTech | No terminada |

## Tareas

- Analizar llamadas redundantes desde portal.
- Proponer cola asincrona para confirmaciones.
- Rediseñar mensajes de cancelacion.
- Preparar escenario de piloto reducido.
- Reestimar integracion con agenda antigua.

## Bloqueos

Las pruebas de carga muestran degradacion grave por encima de 300 usuarios concurrentes. La agenda antigua no tiene decision de convivencia. Admision no valida el flujo de cancelacion.

## Incidencias

- Errores 503 durante confirmaciones simultaneas.
- Tiempo medio de respuesta de 8,7 segundos en carga.
- App movil bloqueada por autenticacion y notificaciones.
- SMS puede enviarse despues de cancelacion si la cola no se actualiza.

## Velocidad

Velocidad prevista: 36 puntos.  
Velocidad real: 18 puntos.

## Comentario

La velocidad real cae a la mitad de la prevista. El equipo recomienda congelar alcance nuevo y concentrarse en integracion, rendimiento y validacion funcional.

