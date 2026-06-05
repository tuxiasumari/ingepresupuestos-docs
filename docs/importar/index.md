# Importar desde otros programas

Una de las mayores ventajas de IngePresupuestos es que **lee directamente los archivos de tu software actual** — no tienes que volver a digitar el presupuesto ni pasar todo por Excel a mano.

## Formatos soportados

| Software | Formato | Notas |
|----------|---------|-------|
| **S10** | `.S2K` / `.bkf` / `.bak` | A través de IngeConverter (incluido gratis). |
| **Delphin Express** | `.sqlite` | Importa proyecto, biblioteca e índices INEI. |
| **PowerCost** | `.prs` (Access) | También sus exportaciones a Excel. |
| **PowerCost / S10 / Delphin** | `.xlsx` | Presupuesto + ACU exportados a Excel. |
| **BIM** | `.ifc` | De Revit, ArchiCAD o Tekla. |
| **IngePresupuestos** | `.db` | Para mover proyectos entre PCs. |

## Cómo importar

1. En el panel principal, haz clic en **Importar**.
2. Elige el **software de origen** y el **formato**.
3. Selecciona el archivo (o los archivos: algunos formatos usan uno para el presupuesto y otro para el ACU).
4. Revisa el resumen y confirma. El proyecto aparece en tu lista, listo para editar.

!!! tip "El pie de presupuesto"
    Al importar, los rubros del pie (gastos generales, utilidad, supervisión, etc.) se cargan **desactivados**. Actívalos según los necesite tu proyecto desde la pestaña **Pie de presupuesto**.

## Guías por programa

<div class="grid cards" markdown>

-   :material-file-excel: **PowerCost**

    ---

    Importa el presupuesto y el ACU desde los Excel de PowerCost.

    [:octicons-arrow-right-24: Ver guía](powercost.md)

-   :material-database-arrow-down: **S10**

    ---

    Convierte tus backups `.S2K` con IngeConverter.

    [:octicons-arrow-right-24: Ver guía](s10.md)

</div>
