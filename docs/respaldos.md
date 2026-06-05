# Respaldos y tus datos

Tus proyectos viven en tu PC, en un archivo de base de datos estándar. IngePresupuestos los respalda solo y tú tienes control total sobre ellos.

## Dónde están tus datos

Toda tu información se guarda en un archivo **`presupuestos.db`** (una base de datos **SQLite** estándar), ubicado en la carpeta de datos de la aplicación:

| Sistema | Ubicación |
|---------|-----------|
| **Windows** | `%APPDATA%\ingepresupuestos\` |
| **Linux** | `~/.local/share/ingepresupuestos/` |

!!! tip "Formato abierto"
    Al ser SQLite estándar, puedes abrir ese archivo con herramientas como **DB Browser for SQLite**, DBeaver o Python. **No es un formato propietario**: tus datos siempre son tuyos.

## Copias de seguridad automáticas

IngePresupuestos crea copias de seguridad solo:

- **Diarias** (conserva las últimas 7).
- **Al cerrar** la aplicación (conserva las últimas 10).
- **Manuales**, cuando tú las pidas (conserva las últimas 10).

Las copias son **atómicas** (no se corrompen aunque cierres a medias).

## Mover o compartir un proyecto

Para llevar un proyecto a otra PC o compartirlo con un colega, **exporta a `.db`** (Exportar → Base de datos) y la otra persona lo **importa**. Ver [Importar desde `.db`](importar/excel-otros.md#base-de-datos-de-ingepresupuestos-db).

!!! warning "Haz tu propia copia también"
    Las copias automáticas viven en tu mismo equipo. Para estar tranquilo ante un fallo de disco, guarda de vez en cuando una copia del `.db` en una nube o disco externo.
