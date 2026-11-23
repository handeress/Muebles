# Muebles

App para consultar los muebles en el taller sin descargar documentos: plano de armado, 3D, lista de corte, herrajes y un modo taller para identificar piezas sin marcar dictando sus medidas.

- App: https://handeress.github.io/Muebles/ (código público, sin datos).
- Datos: repo privado `handeress/Bitacora-datos`, carpeta `muebles/` (formato en su README). Los escribe Claude con la habilidad despiece-muebles; la app solo lee.
- Llave: la misma de la Bitácora; la toma sola si la Bitácora ya se abrió en el mismo navegador, o se pega en Ajustes (⚙).
- Sin señal: muestra lo último que descargó. El dictado de Android casi siempre necesita internet; sin señal se escriben las medidas.
- Prueba sin datos: `?demo`.

## Pestañas

- **Plano:** hojas del plano de armado en imagen; tocar una la abre en grande con zoom.
- **3D:** el visor del mueble (pantalla completa).
- **Corte:** piezas por material con código, cantidad, medida, medida final si se rebaja en taller, y cantos (R rígido, F flexible).
- **Herrajes:** lista para chulear (se guarda en el aparato).
- **Historial:** lo que está por revisar y los cambios, modificaciones y eventos del mueble, del más nuevo al más viejo.
- **Taller:** escribe o dicta largo y ancho (mm por defecto; se puede cambiar a cm). Responde el código en pantalla y en voz, avisa si la pieza es de otro mueble, lleva la cuenta de las identificadas y muestra las que faltan.

## Versiones

Subir `CACHE` en `sw.js` y `VERSION` en `index.html` en cada cambio.

- 1.0 (22/11/2026): primera versión con cocineta y closet de Suesca.
- 1.1 (22/11/2026): mm por defecto, avisos de revisión por mueble y por pieza, pestaña Historial (cambios, modificaciones y eventos), muebles de Fontanar (BBQ y mesas de noche).

- 1.3 (23-nov-2026): botón Instalar en el celular; atrás va de subpágina a la página inicial del elemento, luego al inicio y luego cierra la app.

- 1.4 (23-nov-2026): recuerda el elemento y la pestaña al recargar (12 h); el 3D guarda su vista (cámara, filtros, corte, separación, abierto) y se recarga solo si el celular lo borra al cambiar de app.
