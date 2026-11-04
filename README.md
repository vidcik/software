# ELECTRA V2.0 — Inteligencia electoral

Prototipo web estático, en español, con identidad visual oscura tipo centro de operaciones.

## Módulos
- Resumen ejecutivo con indicadores y distribución de votos.
- Geografía electoral con Leaflet y OpenStreetMap; los puntos se alimentan de coordenadas lat/lon.
- Resultados agregados por organización política.
- Indicadores: NEP electoral y simulación D'Hondt.
- Gestión de registros manuales, importación/exportación CSV y persistencia en `localStorage`.

## Ejecutar localmente
Abre `index.html` en un navegador moderno. Para evitar restricciones del navegador, también puedes ejecutar `python -m http.server 8000` en esta carpeta y visitar `http://localhost:8000`.

## Publicar en GitHub Pages
El workflow de `.github/workflows/deploy.yml` publica el contenido de la rama `vdcan` mediante GitHub Actions.

## Consideraciones
- Los datos iniciales son ficticios y solo sirven para probar la interfaz.
- El mapa necesita conexión a internet para cargar los mosaicos de OpenStreetMap y Leaflet desde CDN.
- Los registros se guardan localmente en el navegador; no existe backend ni sincronización entre usuarios.
- La asignación D'Hondt es una simulación simplificada. No sustituye el escrutinio ni las reglas oficiales de una elección.
