# Pase de turno

Los 23 pases de octubre (del 1 al 16, tomados del grupo de WhatsApp) se cargan en la planilla al ejecutar **configurar**. El repositorio no guarda ningún dato de la planta: todo queda en la planilla.

> `Code.gs` **no se sube a este repositorio**: tiene los datos de octubre y el repositorio es público. Se pega solamente en el Apps Script de la planilla.

La página es `index.html`. La planilla de Google solo sirve para guardar los pases: se configura una vez y después no hace falta abrirla.

## Paso 1 · Planilla (una sola vez, 5 minutos)

1. Creá una planilla nueva en Google Sheets.
2. Entrá a **Extensiones > Apps Script**, borrá lo que aparece, pegá el contenido de `Code.gs` y guardá.
3. En el selector de arriba elegí **configurar** y tocá **Ejecutar**. Aceptá los permisos que pide Google. Si aparece "app no verificada", entrá en *Configuración avanzada > Ir a…*.
4. Tocá **Implementar > Nueva implementación > Aplicación web**. Elegí *Ejecutar como: Yo* y *Quién tiene acceso: Cualquier persona*, y tocá **Implementar**.
5. Copiá la URL que termina en `/exec`.

## Paso 2 · Página

1. En `index.html`, pegá la URL en `const SCRIPT_URL = "";`.
2. Subí `index.html` a un repositorio de GitHub.
3. En el repositorio, entrá a **Settings > Pages**, elegí la rama **main** y guardá.
4. Compartí el link que aparece con los supervisores.

## Listo

- Los supervisores cargan desde **Cargar turno**.
- Vos abrís el link y ves el turno cargado.
- El botón **Descargar Excel** baja el historial.
