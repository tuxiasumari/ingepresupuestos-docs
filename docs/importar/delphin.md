# Importar desde Delphin Express

IngePresupuestos lee directamente la base nativa **`.sqlite`** de Delphin Express, trayendo el proyecto, la biblioteca de costos y los índices INEI.

## Pasos

1. En IngePresupuestos: **Importar → Delphin Express**.
2. Selecciona el archivo **`.sqlite`** de Delphin.
3. Si la base contiene varios presupuestos, elige el que quieres importar.
4. Confirma. El proyecto se crea con sus partidas, ACU e insumos.

!!! info "Sobre el formato `.dprj`"
    Delphin también guarda archivos `.dprj`, pero ese formato no se puede leer (usa una serialización interna de .NET). Usa siempre el **`.sqlite`**, o exporta a **Excel** desde Delphin e impórtalo como Excel.

## Qué se importa

- Las **partidas** con su jerarquía, unidad y metrado.
- El **análisis de costos unitarios** de cada partida.
- Los **insumos**, reutilizando el mismo recurso del catálogo cuando coinciden (aunque cambie el código).
- Los **índices unificados (INEI)** asociados a los insumos, útiles para la fórmula polinómica.

!!! tip "El pie de presupuesto"
    Igual que con los demás importadores, los rubros del pie (gastos generales, utilidad, etc.) entran **desactivados**. Actívalos según tu proyecto.
