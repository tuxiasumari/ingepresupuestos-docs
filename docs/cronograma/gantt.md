# Diagrama de Gantt

El **Gantt** de IngePresupuestos funciona al estilo de MS Project: tareas con barras en el tiempo, dependencias entre ellas, holguras, hitos y **ruta crítica**.

![Diagrama de Gantt con ruta crítica](../img/gantt.jpeg)

## La tabla y el gráfico

A la izquierda tienes la tabla de tareas (número, descripción, duración, inicio, fin, predecesoras) y a la derecha las barras en el calendario. La columna **#** numera todas las filas por posición, incluyendo:

- **#1** el proyecto,
- **#2** el hito de Inicio (puedes referenciarlo como predecesora),
- las cabeceras de cada subpresupuesto,
- las partidas,
- y el hito de **Fin**.

## Dependencias

Defines qué tarea depende de cuál con la notación en español:

| Notación | Significado |
|----------|-------------|
| **FC** | Fin → Comienzo (la más común). |
| **CC** | Comienzo → Comienzo. |
| **FF** | Fin → Fin. |
| **CF** | Comienzo → Fin. |

Puedes agregar **desfase** (lag) y porcentaje. Las predecesoras se escriben por el número de fila (ej. `5FC`, `5FC+3d`).

!!! tip "Deshacer y rehacer dependencias"
    ¿Creaste o moviste una dependencia por error? Pulsa **Ctrl + Z** para deshacer y **Ctrl + Y** (o **Ctrl + Shift + Z**) para rehacer. Funciona al crear una dependencia arrastrando una barra, al cambiar su tipo, lag o porcentaje, al borrar flechas (incluso varias a la vez) y al escribir predecesoras en la tabla.

## Plazo del proyecto

Arriba a la derecha verás **Plazo: N días · M programados**:

- **Plazo** son los **días contractuales** que definiste en los datos del proyecto.
- **Programados** son los días que realmente ocupa tu programación (según las duraciones y dependencias).

Ambos pueden no coincidir: tu programación puede terminar antes o después del plazo contractual. Para cambiarlo, usa el enlace **✏ Editar plazo** que está junto al dato: abre los datos del proyecto y, al guardar, el Gantt se actualiza al instante —incluida la línea de **fin de plazo**.

## Ruta crítica y holguras

IngePresupuestos calcula la **ruta crítica** (las tareas que no pueden retrasarse sin atrasar la obra) y las **holguras** de las demás. Las tareas críticas se resaltan.

## Hitos

Puedes marcar tareas como **hitos** (puntos de control sin duración) para señalar entregas o etapas clave.

!!! tip "Para imprimir"
    El Gantt se imprime con un formato propio que ajusta el tamaño de papel automáticamente (de A4 hasta A0) según la cantidad de tareas. Ver [Exportar a MS Project](ms-project.md) para llevarlo a otros programas.
