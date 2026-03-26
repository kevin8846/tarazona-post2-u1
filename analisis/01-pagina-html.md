# Análisis 1: Petición GET — example.com
## Información general
- URL: https://example.com
- Método: GET
- Código de estado: [304 Not Modified]
## Headers de Request
| Header | Valor |
|--------|-------|
| Host | [example.com] |
| User-Agent | [Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/146.0.0.0 Safari/537.36] |
| Accept | [text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,/;q=0.8] |
## Headers de Response
| Header | Valor | Significado |
|--------|-------|-------------|
| Content-Type | [text/html; charset=UTF-8] | [Especifica que el cuerpo de la respuesta es un documento HTML con codificación de caracteres universal.] |
| Cache-Control | [max-age=604800] | [Indica que el navegador puede considerar el recurso como "fresco" y almacenarlo en caché hasta por 7 días.] |
## Tiempos de carga
| Fase | Tiempo (ms) |
|------|------------|
| DNS Lookup | [0 ms] |
| TTFB | [45 ms] |
## Conclusión
[La petición arrojó un código 304, lo que demuestra que el navegador ya poseía una copia del recurso y el servidor confirmó que no hubo cambios mediante el uso de ETags. Se observa una integración con Cloudflare que sirve el contenido como un "HIT" de caché, optimizando la velocidad de entrega. Los tiempos de carga son mínimos debido a que no se requirió una transferencia completa de datos, mejorando la eficiencia del ancho de banda.]