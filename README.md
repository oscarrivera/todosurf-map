# TODOSURF map

Mapa de spots de surf (TODOSURF). Leaflet, capas agrupadas, Bootstrap 4
y un selector Select2. El PHP de `index.php` solo redirige o sirve la
página estática; la lógica está en `main.js`.

## Cómo verlo

Servir el directorio con cualquier HTTP estático (no abrir solo con
`file://` si las peticiones a `data.js` o a CDNs fallan):

```bash
python3 -m http.server 8080
```

Abrir `http://127.0.0.1:8080/`.

## Archivos

- `index.html` — cascarón y dependencias (CDN)
- `main.js` — mapa, popups, capas
- `styles.css`
- `lib/leaflet-groupedlayercontrol/`
- `mapa.png` — recurso gráfico

Proyecto de 2018–2019. Las URLs de CDN llevan `integrity`; si un paquete
cambia de hash, hay que actualizarlo. No hay backend propio en este repo.
