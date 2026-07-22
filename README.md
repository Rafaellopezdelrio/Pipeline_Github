# Pipeline_Github

Práctica de **integración continua con GitHub Actions**: configuración de un workflow
que se ejecuta automáticamente sobre el repositorio.

## Qué contiene

```
.github/workflows/   → definición del workflow (triggers, jobs y steps)
package.json         → proyecto Node.js y sus scripts
```

## Qué he practicado

- Estructura de un workflow de GitHub Actions: eventos que lo disparan, *jobs* y *steps*
- Ejecución automática de tareas en cada cambio del repositorio
- Uso de acciones del marketplace (checkout del código, setup de Node)
- Comprobación de resultados desde la pestaña **Actions**

## Por qué importa en QA

La automatización solo aporta valor si se ejecuta sola. Un pipeline permite lanzar la
suite de tests en cada push o pull request y detectar regresiones antes de que lleguen
a producción, sin depender de que alguien se acuerde de ejecutarlos a mano.

## Cómo verlo

1. Abrir la pestaña **Actions** del repositorio
2. Seleccionar una ejecución para ver los *steps* y sus logs
3. El workflow se lanza automáticamente según los eventos definidos en el YAML
