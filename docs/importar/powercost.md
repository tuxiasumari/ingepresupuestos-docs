# Importar desde PowerCost

IngePresupuestos importa presupuestos de **PowerCost** de dos maneras: desde su base nativa `.prs` o desde los archivos **Excel** que exporta (presupuesto y ACU).

## Desde Excel (presupuesto + ACU)

PowerCost te permite exportar dos archivos: el **presupuesto** y el **análisis de costos unitarios (ACU)**. IngePresupuestos los lee juntos.

1. En PowerCost, exporta a Excel el **presupuesto** y el **ACU** de la obra.
2. En IngePresupuestos: **Importar → PowerCost → Excel**.
3. Selecciona el archivo de **presupuesto** y el de **ACU**.
4. Confirma. El proyecto se crea con sus partidas, su jerarquía, los ACU y los insumos.

!!! success "Qué se importa correctamente"
    - La **jerarquía** completa (componentes, títulos, subpartidas y partidas).
    - El **análisis de costos unitarios** de cada partida, sin insumos duplicados.
    - Los **insumos** consolidados, reutilizando el mismo recurso del catálogo (un solo «peón», un solo cemento, etc.).
    - El **monto total**, idéntico al de PowerCost.

## Sobre los códigos de partida

En PowerCost cada partida puede numerarse de varias formas (numérico, letra, número romano o un **código propio** de la entidad), e incluso saltar correlativos. Por eso sus códigos a veces se ven como `101.A`, `503.A3` o `500. A`.

Esos códigos son un **estilo de numeración**, no una jerarquía. Al importar, IngePresupuestos **renumera limpio** (01, 01.01, 01.01.01…) según la estructura real de títulos, para que el árbol del presupuesto quede bien anidado. El total y los análisis no cambian.

## Verificar después de importar

Te recomendamos revisar:

1. Que el **monto total** coincida con PowerCost (debería ser idéntico salvo centavos por redondeo).
2. Que cada partida muestre su **ACU** con la mano de obra, materiales, equipo y, si corresponde, las **herramientas manuales (%MO)**.
3. Que la **jerarquía** (títulos y subpartidas) se vea correcta en el árbol.

!!! note "¿El monto cambia al pulsar «Recalcular»?"
    Si tras importar todo cuadra pero al **recalcular** el total varía, suele deberse a que en el ACU original faltaba algún insumo de porcentaje (como las herramientas manuales). Asegúrate de exportar el ACU **completo** desde PowerCost. Con la versión actual de IngePresupuestos esto ya se importa correctamente.

## Desde la base `.prs`

Si tienes el archivo `.prs` de PowerCost (una base de datos Access):

1. **Importar → PowerCost → `.prs`**.
2. Selecciona el archivo. Si tiene contraseña interna, IngePresupuestos la maneja automáticamente.
3. Confirma.

---

¿Vienes de **S10**? [Ver la guía de S10 :octicons-arrow-right-24:](s10.md)
