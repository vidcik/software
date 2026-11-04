# ELECTRA — Plataforma de Análisis Electoral

Versión web V1.0 preparada para GitHub Pages.

## Publicar
1. Crea un repositorio en GitHub llamado `electra-analisis-electoral`.
2. Descomprime este paquete y sube **todo su contenido** a la raíz del repositorio. `index.html` debe quedar en la raíz.
3. En GitHub abre **Settings → Pages** y selecciona **GitHub Actions** como fuente de publicación.
4. Abre la pestaña **Actions** y espera a que termine `Deploy ELECTRA to GitHub Pages`.
5. La URL pública aparecerá en **Settings → Pages**.

El workflow publica automáticamente cada nuevo cambio que llegue a la rama `main`.

## Alternativa sin workflow
En Settings → Pages selecciona `Deploy from a branch`, rama `main`, carpeta `/ (root)` y guarda. Usa este método o GitHub Actions, no ambos a la vez.

## Ejecutar localmente
Windows: `py -m http.server 8000`
macOS/Linux: `python3 -m http.server 8000`
Abre `http://localhost:8000`.

## Alcance y limitaciones
- Aplicación estática; no tiene backend ni base de datos central.
- Los datos se guardan en localStorage, por navegador y dispositivo.
- No hay autenticación ni sincronización multiusuario.
- Los datos de demostración son ficticios.
- No es un sistema oficial de escrutinio ni certifica resultados.
- Antes de uso institucional deben validarse reglas legales, desempates, umbrales y fuentes.

## Estructura
- `index.html`: aplicación.
- `plantilla_electoral.csv`: ejemplo de estructura de importación.
- `.github/workflows/deploy.yml`: despliegue automático.
