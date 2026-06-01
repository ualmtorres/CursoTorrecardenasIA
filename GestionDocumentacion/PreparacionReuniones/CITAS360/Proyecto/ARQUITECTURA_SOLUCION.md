# CITAS360 - Arquitectura de Solucion

Fecha: 28/02/2026  
Autor: Javier Ruiz, Responsable Sistemas  
Version: 1.0  
Participantes: Javier Ruiz, Laura Moreno, David Vega, Miguel Serrano

## Componentes

La solucion se compone de portal web, aplicacion movil, API de citas, modulo de notificaciones, conectores con HIS y agenda de especialistas, y repositorio analitico para cuadro de mando.

## Integraciones

El portal y la app consumiran la API de citas publicada por MedTech Solutions. La API intercambiara informacion con el HIS corporativo mediante los servicios REST documentados por Sistemas. Las agendas de especialistas se sincronizaran mediante un conector nocturno y una consulta bajo demanda para cambios recientes.

## Seguridad

La autenticacion de pacientes queda pendiente de decision. La arquitectura soporta token temporal por SMS y autenticacion reforzada con segundo factor. La decision debe cerrarse antes del inicio del piloto para evitar reconfiguracion de flujos.

## Entornos

- Desarrollo: gestionado por MedTech Solutions.
- Integracion: alojado en infraestructura HUSA.
- Preproduccion: compartido con otros proyectos corporativos.
- Produccion: pendiente de dimensionamiento final.

## Supuestos tecnicos

Se asume que las APIs del HIS permiten consulta, confirmacion y cancelacion con codigos estandar de respuesta. No se contemplan desarrollos especificos en el HIS salvo configuracion de permisos tecnicos. El proveedor confirma que el conector de agenda reutiliza componentes ya implantados en otros hospitales.

## Riesgos tecnicos

El entorno de preproduccion tiene ventanas limitadas por mantenimiento corporativo. La disponibilidad de los servicios HIS dependera de la agenda de Sistemas. La estrategia SMS no puede cerrarse hasta elegir proveedor definitivo.

