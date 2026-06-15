# Importar desde Excel, IFC y `.db`

Además de los formatos nativos, IngePresupuestos importa desde hojas de cálculo, modelos BIM y su propia base de datos.

## Excel (`.xlsx`)

Si tu presupuesto está en Excel —exportado de cualquier software o armado a mano— puedes importarlo.

1. **Importar → Excel**.
2. Selecciona el archivo de **presupuesto** y, si lo tienes, el de **ACU**.
3. Confirma.

!!! tip "Para que la importación salga bien"
    El Excel debe tener una tabla con columnas reconocibles: **Ítem, Descripción, Unidad, Metrado, Precio**. IngePresupuestos detecta el encabezado automáticamente. Si tu archivo viene de PowerCost, S10 o Delphin, usa mejor la guía específica de cada uno.

## BIM — modelos IFC (`.ifc`)

Puedes importar cantidades desde un modelo **IFC** (de Revit, ArchiCAD, Tekla, etc.) para generar partidas a partir de los elementos del modelo.

1. **Importar → IFC**.
2. Selecciona el archivo `.ifc`.
3. Revisa los elementos y cantidades detectados y confirma.

## Base de datos de IngePresupuestos (`.db`)

Para **mover un proyecto entre computadoras** o compartirlo con un colega que también use IngePresupuestos:

=== "Exportar"

    1. Abre el proyecto.
    2. **Exportar → Base de datos (`.db`)**.
    3. Guarda el archivo y compártelo.

=== "Importar"

    1. **Importar → IngePresupuestos (`.db`)**.
    2. Selecciona el archivo `.db`.
    3. Elige el proyecto a importar y confirma.

La exportación `.db` conserva **todo**: partidas, ACU, insumos, metrados, cronograma, fórmula polinómica y pie de presupuesto.

!!! tip "Atajo: abrir un `.db` directamente"
    Con un proyecto abierto, también puedes ir a **Archivo → Abrir → Desde archivo (`.db`)**: eliges el archivo, IngePresupuestos lo agrega al programa y lo abre en una pestaña. Si el `.db` contiene varios proyectos, te deja elegir cuál.
