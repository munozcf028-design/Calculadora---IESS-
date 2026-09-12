# Calculadora Aporte al IESS - F. Muñoz

App web instalable (PWA) para calcular aportes al IESS como **Trabajador**, **Empleador** o **Afiliado voluntario**, con historial de proyectos guardados en el propio dispositivo.

## Porcentajes configurados

| Tipo de aportación   | Porcentaje |
|-----------------------|-----------|
| Trabajador (personal) | 9.45%     |
| Empleador (patronal)  | 11.15%    |
| Afiliado voluntario   | 20.5%     |

Si el IESS actualiza estas tasas, se editan en `index.html`, dentro del objeto `RATES` (inicio del archivo `<script>`). No hace falta tocar el resto del código.

## Publicar en GitHub Pages

1. Sube todo el contenido de esta carpeta (`index.html`, `manifest.json`, `service-worker.js`, `icons/`) a un repositorio **público** de GitHub.
2. Ve a **Settings → Pages**.
3. En "Branch" selecciona **main** y la carpeta **/ (root)**, luego **Save**.
4. Espera 1–2 minutos. GitHub mostrará el link público, por ejemplo:
   `https://tuusuario.github.io/calculadora-iess/`

## Instalar en el celular

- **Android (Chrome):** abre el link → menú ⋮ → "Instalar app" (o acepta el aviso automático).
- **iPhone (Safari):** abre el link → botón compartir 📤 → "Agregar a pantalla de inicio".

Queda con ícono propio, pantalla completa y funciona sin internet para calcular y ver el historial (el guardado usa el almacenamiento local del teléfono).

## Funciones

- Cálculo de aporte personal, patronal o voluntario con su porcentaje y valor.
- Historial de proyectos: **guardar**, **modificar** y **eliminar**.
- Exportar historial a **Excel** (.xlsx).
- Exportar historial a **PDF** (usa el diálogo de impresión del navegador → "Guardar como PDF").

## Actualizar la app luego de publicada

Cualquier cambio en `index.html` (por ejemplo, un nuevo porcentaje) se edita directamente desde GitHub con el ícono de lápiz ✏️ sobre el archivo. Al guardar el cambio ("Commit changes"), el sitio publicado se actualiza automáticamente, sin necesidad de volver a subir nada.
