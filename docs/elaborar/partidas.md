# Partidas y subpresupuestos

La pestaña **Partidas** es el corazón del presupuesto: aquí armas su estructura jerárquica.

![Árbol de partidas del presupuesto](../img/partidas.jpeg)

## La jerarquía

El presupuesto se organiza como un árbol de varios niveles:

- **Títulos** (y subtítulos): agrupan partidas. No tienen metrado ni precio; su monto es la suma de lo que contienen. Se muestran en colores por nivel (rojo, arándano, morado…).
- **Partidas**: las hojas del árbol. Tienen unidad, metrado y un precio unitario que sale de su análisis de costos.

## Numeración automática

No tienes que escribir los códigos. IngePresupuestos numera las filas automáticamente según su posición y nivel:

```
01            TRABAJOS PRELIMINARES        (título)
01.01           Cartel de obra             (partida)
01.02           Movilización               (partida)
02            MOVIMIENTO DE TIERRAS        (título)
02.01           Excavación                 (partida)
```

Si **reordenas** partidas (arrastrándolas) o cambias su nivel, la numeración se recalcula sola.

## Acciones comunes

| Quiero… | Cómo |
|---------|------|
| Agregar un título | Botón **Título** en la barra de herramientas. |
| Agregar una partida | Botón **Partida**. |
| Subir / bajar de nivel | Selecciona la fila y usa **Alt+←** / **Alt+→** (o los botones de mover). |
| Reordenar | Arrastra la fila a su nueva posición. |
| Copiar partidas entre proyectos | **Ctrl+C** en un proyecto y **Ctrl+V** en otro (conserva ACU, metrados, acero y especificaciones). |

## Subpresupuestos

Cuando una obra tiene varios frentes o especialidades, puedes dividirla en **subpresupuestos** (por ejemplo: Estructuras, Arquitectura, Instalaciones). Cada subpresupuesto agrupa su propio conjunto de partidas, y el Resumen los totaliza por separado y en conjunto.

---

**Siguiente:** [Análisis de Costos Unitarios :octicons-arrow-right-24:](acu.md){ .md-button .md-button--primary }
