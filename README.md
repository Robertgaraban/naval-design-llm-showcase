# RF-4 (TFG) · diseño naval asistido por IA

**Tipo:** proyecto académico

**Estado:** en curso — Trabajo Final de Grado, 2026

## Qué demuestra este repositorio

Este repositorio documenta un planteamiento para traducir especificaciones de diseño naval a geometría y planos revisables con apoyo de modelos de lenguaje, la API de Python de Fusion 360 y un flujo de intercambio con AutoCAD.

La evidencia pública es un brief de arquitectura: explica el problema, el flujo propuesto, los parámetros de diseño y los puntos de revisión humana. No publica los scripts, los modelos 3D ni los planos.

## Qué no demuestra

- Los valores de eslora, velocidad, autonomía, propulsión y sensores son **parámetros de diseño objetivo, no mediciones**.
- El vehículo no se presenta como construido ni probado.
- El flujo no está validado para uso profesional, certificación, fabricación ni aprobación por una sociedad de clasificación.
- No es una herramienta oficial de la Universitat Politècnica de Catalunya ni de la Facultat de Nàutica de Barcelona.
- Las marcas y herramientas citadas describen el entorno estudiado; no implican patrocinio ni colaboración institucional.

## Problema académico

El trabajo estudia cómo mantener la relación entre una especificación, los parámetros del diseño, la geometría y la documentación técnica. El objetivo es que cada decisión pueda revisarse y corregirse antes de producir un entregable académico.

## Flujo estudiado

1. Especificación estructurada de requisitos y parámetros.
2. Interpretación asistida por un modelo de lenguaje.
3. Generación paramétrica mediante la API de Python de Fusion 360.
4. Preparación de vistas y planos 2D/DXF mediante un flujo de intercambio con AutoCAD.
5. Revisión humana de parámetros, geometría y documentación.

## Parámetros de diseño (objetivo, no medidos)

| Parámetro | Valor de trabajo |
|---|---:|
| Eslora total | 4,80 m |
| Manga total | 2,00 m |
| Calado | 0,35 m |
| Desplazamiento estimado | 180 kg |
| Velocidad objetivo máxima | 5 nudos |
| Velocidad objetivo de crucero | 3 nudos |
| Autonomía objetivo | 1,9 h a velocidad de crucero |

Las categorías de percepción consideradas en el diseño son posicionamiento GNSS, cámara, unidad inercial, detección de obstáculos y recepción AIS. No se presentan modelos comerciales como selección final.

## Contenido

- `README.md`: brief público del planteamiento académico y sus límites.

## Contexto

Trabajo Final de Grado en desarrollo en la Facultat de Nàutica de Barcelona, Universitat Politècnica de Catalunya.

**Autor:** Robert Garabán.
