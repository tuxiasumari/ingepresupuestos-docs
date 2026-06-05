# Exportar a MS Project

El Gantt de IngePresupuestos se exporta a un **XML estándar (MSPDI)**, el formato de Microsoft Project. Lo importante: es un **formato abierto** que abre no solo en Project, sino también en programas **gratuitos**.

## Programas que lo abren

- **Microsoft Project**
- **ProjectLibre** (gratuito)
- **OpenProj** (gratuito)
- **GanttProject** (gratuito)
- **Primavera P6** también lo lee.

Así no necesitas una licencia de Project para seguir trabajando tu cronograma.

## Cómo exportar

1. En la vista del Gantt, pulsa **Exportar → MS Project (XML)**.
2. Guarda el archivo `.xml`.
3. Ábrelo desde Project, ProjectLibre, OpenProj o GanttProject.

!!! success "Se exporta fiel"
    El XML conserva las duraciones, las dependencias, los hitos y el calendario. Las tareas mantienen sus relaciones para que el cronograma se vea igual en el otro programa.

!!! note "No es un `.mpp`"
    El formato es **XML MSPDI**, no el `.mpp` binario de Microsoft. La gran ventaja es que los programas libres sí pueden abrir el XML, mientras que el `.mpp` suele requerir Project.
