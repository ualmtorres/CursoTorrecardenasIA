# Proyecto CITAS360 - Documento de Inicio

Fecha: 10/01/2026  
Autor: Miguel Serrano, Jefe de Proyecto  
Version: 1.0  
Participantes: Ana Beltran, Miguel Serrano, Javier Ruiz, Laura Moreno, Carmen Gil, David Vega

## Resumen ejecutivo

CITAS360 es el programa de modernizacion de la gestion de citas medicas del Hospital Universitario Santa Aurelia. El proyecto se inicia con una duracion prevista de 12 meses, desde enero hasta diciembre de 2026, y tiene como objetivo disponer de un canal digital integrado para pacientes y profesionales.

El alcance aprobado incluye portal web para pacientes, aplicacion movil, confirmacion automatica de citas, recordatorios SMS, integracion con el HIS corporativo, integracion con agenda de especialistas y cuadro de mando de actividad.

## Objetivos

- Reducir llamadas al area de Admision en un 25% durante los seis meses posteriores a la puesta en produccion.
- Permitir consulta, confirmacion y cancelacion de citas desde web y movil.
- Automatizar recordatorios SMS con al menos 48 horas de antelacion.
- Sincronizar las citas confirmadas con el HIS corporativo y las agendas de especialistas.
- Ofrecer indicadores diarios de actividad, anulaciones, no presentados y ocupacion de agendas.

## Alcance inicial

El proyecto se ejecutara en cuatro bloques: analisis y diseno, desarrollo de canales digitales, integraciones corporativas y despliegue piloto. La puesta en produccion se plantea inicialmente como despliegue progresivo, empezando por consultas externas de Traumatologia y Dermatologia.

Quedan pendientes de decision, durante el primer trimestre, los siguientes puntos: mecanismo de autenticacion de pacientes, estrategia definitiva de notificaciones, seleccion de proveedor SMS, continuidad de la agenda antigua durante el piloto y modelo de despliegue final.

## Gobierno

La direccion TIC, representada por Ana Beltran, actuara como sponsor. Miguel Serrano dirigira el proyecto. MedTech Solutions sera el proveedor principal, con David Vega como responsable. Javier Ruiz coordinara sistemas, Laura Moreno el desarrollo interno y Carmen Gil la validacion funcional desde Admision.

## Planificacion de alto nivel

- Enero-febrero: analisis funcional y arquitectura.
- Marzo-abril: desarrollo inicial del portal y servicios de citas.
- Mayo-junio: integraciones HIS, agenda de especialistas y SMS.
- Julio-agosto: piloto funcional y pruebas de rendimiento.
- Septiembre-octubre: estabilizacion y despliegue ampliado.
- Noviembre-diciembre: cierre, transferencia y cuadro de mando consolidado.

## Supuestos

El HIS corporativo expondra APIs estandar suficientes para consulta y actualizacion de citas. Las agendas de especialistas podran sincronizarse mediante los conectores actuales. El proveedor SMS se seleccionara antes de abril. El area de Admision dispondra de usuarios clave para pruebas quincenales.

## Riesgos iniciales

En el arranque no se identifican riesgos criticos. Se registran como riesgos medios la dependencia del HIS, la disponibilidad de usuarios clave y la decision pendiente sobre autenticacion de pacientes.

