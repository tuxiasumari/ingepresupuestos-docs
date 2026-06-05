# Instalación

IngePresupuestos funciona en **Windows** y **Linux** con la misma aplicación y los mismos archivos de proyecto. No necesita internet para trabajar ni instalar Office o MS Project.

Descarga siempre la última versión desde **[ingepresupuestos.com](https://ingepresupuestos.com/#descargar)**.

## Windows

1. Descarga el instalador **`.exe`** (o la versión portable `.zip` si prefieres no instalar).
2. Haz doble clic en el instalador y sigue el asistente.
3. Si aparece la pantalla azul **«Windows protegió tu PC»**, haz clic en **Más información → Ejecutar de todas formas**.

    !!! note "¿Por qué sale ese aviso?"
        Es la advertencia normal de SmartScreen para programas que aún no tienen una firma de pago. IngePresupuestos es seguro; el aviso desaparecerá cuando incorporemos la firma comercial.

4. Al terminar, busca **IngePresupuestos** en el menú Inicio y ábrelo.

La versión **portable** (`.zip`) no se instala: descomprímela y ejecuta `IngePresupuestos.exe` desde la carpeta.

## Linux

=== "AppImage (recomendado)"

    1. Descarga el archivo **`.AppImage`**.
    2. Dale permisos de ejecución:

        ```bash
        chmod +x IngePresupuestos-*.AppImage
        ```

    3. Haz doble clic (o ejecútalo desde la terminal). No requiere instalación.

=== "Portable (.tar.gz)"

    1. Descarga el **`.tar.gz`** y descomprímelo:

        ```bash
        tar -xzf ingepresupuestos-linux.tar.gz
        ```

    2. Entra a la carpeta y ejecuta el binario `IngePresupuestos`.

## Actualizaciones

Cuando haya una versión nueva, el programa te avisa automáticamente al abrirlo, con un resumen de las novedades y un botón para descargarla. También puedes revisarlo manualmente en **Configuración → Acerca de → Buscar actualizaciones**.

## Tus datos

Tu información vive en tu PC, en un archivo **SQLite estándar** (`presupuestos.db`). El programa hace **copias de seguridad automáticas** cada día. Puedes abrir ese archivo con cualquier herramienta SQLite si lo necesitas — no es un formato propietario.

---

**Siguiente paso:** [Tu primer proyecto :octicons-arrow-right-24:](primer-proyecto.md){ .md-button .md-button--primary }
