# Entrenabilidad

App de planificación y seguimiento de entrenamiento (clientes, sesiones, asistencia, tests por capacidad física, macrociclo y hábitos).

## Obtener el APK

1. Ve a la pestaña **Actions** del repositorio.
2. Abre la última ejecución de **Compilar APK** (o toca **Run workflow** para lanzarla).
3. Al terminar, baja el archivo **entrenabilidad-apk** desde la sección *Artifacts*, descomprímelo y pasa `app-debug.apk` al celular.

Los datos se guardan en el propio teléfono. Haz respaldos desde **Ajustes > Copiar respaldo**.

La app vive en `www/index.html`. Cada vez que se cambia y se sube a `main`, el APK se compila de nuevo.

## Actualizar sin perder datos
El APK se firma siempre con la misma llave (`signing/debug.keystore`), así que una versión nueva se instala encima de la anterior y conserva los datos del teléfono. Si algún día cambias la llave, habrá que desinstalar la app una vez (y restaurar desde un respaldo).
