# Visión y alcance

[← Volver al caso](../README.md) · [Siguiente: arquitectura →](02-arquitectura-del-flujo.md)

## El problema

En un flujo de diseño, una frase inicial puede transformarse varias veces: requisito, valor paramétrico, elemento geométrico y anotación de un plano. Si esas transformaciones no dejan rastro, corregir una decisión se vuelve lento y arriesgado.

El TFG estudia un enfoque para que ese recorrido sea **explícito, trazable y revisable**. La IA ayuda a interpretar y estructurar información, pero no sustituye la responsabilidad técnica ni aprueba el resultado.

## La hipótesis de trabajo

Una entrada estructurada y una cadena de artefactos con identidad permiten detectar ambigüedades antes de modelar, conocer qué parte del diseño depende de cada requisito, devolver una observación al punto correcto y separar una sugerencia de IA de una decisión aceptada por una persona.

## Mi contribución

Mi papel se concentra en la **conceptualización y arquitectura funcional del proceso**:

- encuadrar el problema y fijar el alcance público;
- convertir necesidades en requisitos y criterios de aceptación;
- definir el flujo entre interpretación, parámetros, geometría y documentación;
- diseñar puertas de revisión, estados y bucles de corrección;
- hacer visibles los riesgos, supuestos y límites;
- conectar lenguaje de producto, dominio naval y posibilidades técnicas.

No se atribuyen aquí resultados de construcción, pruebas, certificación ni validación profesional.

## Dentro y fuera del alcance

| Dentro del caso público | Fuera del caso público |
|---|---|
| Arquitectura funcional y flujo de decisiones | Código fuente y automatizaciones |
| Parámetros objetivo del ejercicio | Modelos 3D, CAD y planos originales |
| Esquema de trazabilidad y criterios de revisión | Datos personales, rutas locales o selección comercial definitiva |
| Riesgos y límites de validación | Afirmaciones de construcción, certificación o prestaciones reales |

El resultado buscado es un **proceso explicable**, no una demostración de autonomía total.
