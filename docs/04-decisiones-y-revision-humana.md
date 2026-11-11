# Decisiones y revisión humana

[← Trazabilidad](03-trazabilidad-de-requisitos.md) · [Volver al caso](../README.md) · [Siguiente: riesgos y límites →](05-riesgos-validacion-y-limites.md)

Una salida generada o asistida no avanza por el hecho de existir. Avanza cuando una persona competente para esa etapa revisa la entrada, la transformación y sus límites, y registra una decisión.

## Puertas de revisión

| Puerta | Pregunta | Resultado posible |
|---|---|---|
| G0 · alcance | ¿problema y exclusiones están claros? | aceptar / redefinir |
| G1 · brief | ¿cada requisito tiene fuente, unidad y naturaleza? | aceptar / completar |
| G2 · interpretación | ¿la propuesta conserva el significado original? | aceptar / corregir |
| G3 · parámetros | ¿valores y dependencias son coherentes para iterar? | aceptar / observar |
| G4 · geometría | ¿lo generado corresponde a los parámetros revisados? | aceptar / devolver |
| G5 · documento | ¿la salida es legible, trazable y no exagera su validez? | emitir / corregir |

## Registro de una decisión

Una revisión útil deja cuatro cosas: **qué se miró, con qué criterio, qué se decidió y qué sigue**. «Se ve bien» no es un criterio de aceptación.

```text
Artefacto:      [ID y versión]
Entrada:        [requisitos o parámetros relacionados]
Criterio:       [comprobación realizada]
Decisión:       [apto para siguiente etapa | observado]
Observaciones:  [hallazgo y acción requerida]
Responsable:    [rol de revisión]
```

La [lista de revisión humana](../examples/review-checklist.md) cubre procedencia, unidades, consistencia y comunicación responsable. Es una plantilla académica: no sustituye una revisión naval o normativa especializada.
