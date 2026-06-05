# Estados del proyecto

Cada proyecto tiene un **estado** que refleja en qué punto de su ciclo de vida está. El estado **protege el trabajo ya consolidado**: a medida que el proyecto avanza, se van bloqueando partes para evitar cambios accidentales.

<!-- CAPTURA: el chip de estado desplegable en la barra superior del proyecto -->

## Los cuatro estados

| Estado | Significado |
|--------|-------------|
| :material-pencil: **En elaboración** | Estás armando el presupuesto. **Todo es editable.** |
| :material-magnify: **En revisión** | El presupuesto está listo y en revisión. Se bloquea el presupuesto y el pie. |
| :material-check-circle: **Aprobado** | El expediente fue aprobado. Se bloquea además las especificaciones. |
| :material-flag-checkered: **Ejecutado** | La obra se está ejecutando o terminó. Se bloquea **todo**, incluido el cronograma. |

## Qué se puede editar en cada estado

A medida que avanzas, se bloquean más cosas:

| Puedes editar… | En elaboración | En revisión | Aprobado | Ejecutado |
|----------------|:---:|:---:|:---:|:---:|
| **Presupuesto** (partidas, ACU, metrados, subpresupuestos) | ✅ | 🔒 | 🔒 | 🔒 |
| **Pie de presupuesto** (rubros, GG, IGV) | ✅ | 🔒 | 🔒 | 🔒 |
| **Especificaciones técnicas** | ✅ | ✅ | 🔒 | 🔒 |
| **Cronograma** (Gantt, valorizado) | ✅ | ✅ | ✅ | 🔒 |

!!! info "¿Por qué este bloqueo progresivo?"
    La idea es que, una vez revisado y aprobado el presupuesto, no se modifiquen los precios por error — pero todavía puedas ajustar especificaciones o el cronograma mientras la obra no arranca. Cuando la obra ya está en ejecución, todo queda fijo.

## Cambiar el estado

1. Dentro del proyecto, en la **barra superior**, haz clic en la **etiqueta de estado**.
2. Elige el nuevo estado en el menú.

El cambio es **reversible**: si necesitas corregir algo, vuelve el proyecto a **En elaboración** y se desbloquea todo de nuevo.

!!! tip "Si intentas editar algo bloqueado"
    El programa te avisa con un mensaje que te dice **qué sí puedes hacer** en el estado actual y cómo desbloquear (volviendo a *En elaboración*). No pierdes nada: solo evita cambios involuntarios.
