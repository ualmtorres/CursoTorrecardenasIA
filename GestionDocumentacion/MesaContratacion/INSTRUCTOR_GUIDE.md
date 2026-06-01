# Guía del formador

Este documento no debe cargarse en NotebookLM durante la práctica.

## Historia real del escenario

El Hospital Universitario Santa Aurelia licita una plataforma de citas y portal del paciente. Las tres ofertas son plausibles y ninguna debe resultar ganadora de forma inmediata.

HealthTech Solutions es la propuesta técnicamente más sólida: arquitectura madura, seguridad detallada, integraciones bien presupuestadas y migración completa. Sus puntos débiles son coste alto, coste recurrente elevado y dependencia de perfiles especializados.

MediNova Digital ofrece buen equilibrio inicial: precio razonable, buena experiencia de paciente, producto SaaS y despliegue ágil. Sus riesgos son escalabilidad, menor experiencia en hospitales universitarios grandes y tendencia a dejar complejidades para iteraciones posteriores.

Hospital Systems Group conoce bien los hospitales y presenta experiencia funcional excelente. Su precio es muy inferior al resto, con calendario agresivo, pocas horas, soporte reducido, migración poco presupuestada y bajo número de perfiles senior. No se dice explícitamente que sea una oferta anormalmente baja; la demo debe conducir a que se infiera al cruzar documentos.

## Contradicciones sembradas

* HSG afirma que la migración completa está incluida, pero en aclaraciones limita el histórico a carga selectiva salvo extracción normalizada.
* HSG declara todas las integraciones incluidas, pero asigna 620 horas totales y depende de conectores reutilizables.
* HSG compromete 99,92%, pero aclara que ciertas funciones operarán en diferido si sistemas externos no están disponibles.
* MediNova afirma app completa, pero representantes complejos pasan a una iteración posterior.
* MediNova mantiene disponibilidad, pero su dimensionamiento base no cubre plenamente los picos del PPT.
* HealthTech incluye integración HIS, pero no cambios en sistemas origen.

## Riesgos ocultos

* Posible insuficiencia de esfuerzo en HSG: 12.600 horas frente a 29.800 y 19.400.
* Coste bajo de migración HSG: 85.000 euros frente a 260.000 y 180.000.
* Soporte HSG más limitado: 8:00-17:00 ordinario y 180 horas evolutivas.
* Escalabilidad MediNova condicionada a ajuste de capacidad.
* Dependencia HealthTech de especialistas certificados y coste recurrente alto.

## Preguntas recomendadas para la demo

* Resume cada oferta en una página.
* Compara fortalezas y debilidades de los tres licitadores.
* ¿Qué contradicciones aparecen entre ofertas y aclaraciones?
* ¿Qué propuesta tiene más riesgo de ejecución y por qué?
* ¿Hay indicios de que alguna oferta deba justificarse mejor?
* ¿Qué preguntas formularías a la mesa antes de adjudicar?
* ¿Qué oferta parece más sólida técnicamente?
* ¿Cuál tiene mejor equilibrio entre coste y riesgo?
* Tengo una reunión en 15 minutos. ¿Qué necesito saber?

## Respuestas esperadas

NotebookLM debería identificar a HealthTech como fuerte técnicamente pero cara; MediNova como equilibrada pero con dudas de escala y complejidad; HSG como experta y barata pero con señales acumuladas de riesgo de ejecución.

La respuesta ideal no debe afirmar de forma automática que HSG incumple, sino recomendar solicitar justificación adicional sobre coste, horas, integraciones, migración, soporte, calendario y perfiles senior.

