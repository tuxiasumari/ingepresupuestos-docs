# Cronograma de obra

A partir del presupuesto, IngePresupuestos arma la **programación de la obra**: un diagrama de Gantt con ruta crítica, el cronograma valorizado, la adquisición de insumos por período y la curva S.

<div class="grid cards" markdown>

-   :material-chart-gantt: **[Diagrama de Gantt](gantt.md)**

    Programación visual con dependencias, holguras y ruta crítica.

-   :material-cash-multiple: **[Cronograma valorizado](valorizado.md)**

    Cuánto se ejecuta (en S/) cada mes.

-   :material-truck-delivery: **[Adquisición de insumos](adquisiciones.md)**

    Qué insumos comprar y cuándo.

-   :material-chart-bell-curve: **[Curva S](curva-s.md)**

    El avance acumulado en el tiempo.

-   :material-microsoft: **[Exportar a MS Project](ms-project.md)**

    Lleva el Gantt a Project, ProjectLibre u OpenProj.

</div>

## Duración de las tareas

La duración de cada partida se estima a partir de su metrado y su rendimiento:

$$
\text{Duración (días)} = \left\lceil \frac{\text{metrado}}{\text{rendimiento}} \right\rceil
$$

Puedes ajustar manualmente las duraciones y las dependencias entre tareas.
