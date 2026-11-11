# Arquitectura del flujo

[← Visión y alcance](01-vision-y-alcance.md) · [Volver al caso](../README.md) · [Siguiente: trazabilidad →](03-trazabilidad-de-requisitos.md)

![Placa de arquitectura y trazabilidad](../assets/traceability-plate.svg)

```mermaid
flowchart TB
    subgraph I[1 · Entrada controlada]
      A[Objetivo académico] --> B[Brief estructurado] --> C[Registro de supuestos]
    end
    subgraph S[2 · Asistencia semántica]
      D[LLM: interpretar y proponer estructura] --> E[Detección de campos incompletos]
    end
    subgraph P[3 · Modelo paramétrico]
      F[Parámetros con unidad y estado] --> G[Generación mediante Fusion 360 API]
    end
    subgraph O[4 · Documentación]
      H[Vistas y exportación] --> J[Intercambio con AutoCAD]
    end
    B --> D --> E --> F --> G --> H --> J --> K{Revisión humana}
    K -->|Apto| L[Decisión registrada]
    K -->|Corregir requisito| B
    K -->|Corregir parámetro| F
```

## Contratos entre etapas

| Transición | Salida esperada | Puerta de control |
|---|---|---|
| Necesidad → brief | requisitos y supuestos visibles | ¿hay ambigüedades críticas? |
| Brief → interpretación | propuesta estructurada, nunca aprobación automática | ¿conserva la intención? |
| Interpretación → parámetros | valores tipados con estado | ¿valor, unidad y condición son coherentes? |
| Parámetros → geometría | elementos paramétricos identificables | ¿corresponden a la entrada? |
| Geometría → documento | vistas o planos de revisión | ¿la salida es legible y trazable? |
| Documento → siguiente etapa | decisión registrada | ¿una persona autoriza avanzar? |

## Papel del LLM

Puede apoyar la extracción de requisitos, detectar campos ausentes y normalizar una estructura. No puede aprobar seguridad, estabilidad, estructura, navegabilidad, cumplimiento reglamentario ni aptitud para fabricación. Tampoco convierte una estimación en una medición.

```mermaid
stateDiagram-v2
    [*] --> Borrador
    Borrador --> EnRevision: entrada completa
    EnRevision --> Observado: falta o conflicto
    Observado --> Borrador: corrección
    EnRevision --> AptoParaIterar: revisión humana
    AptoParaIterar --> Sustituido: nueva versión
```

«Apto para iterar» solo significa que el artefacto puede pasar a la siguiente etapa académica definida.
