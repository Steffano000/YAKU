# Yaku · Agua para tu chacra

App piloto para agricultores de **Huachac (valle del Mantaro, Junín, Perú)**. Dice cómo viene el agua cada mes para la papa, la alfalfa, el maíz y la zanahoria, y qué hacer: cada cuántos días regar y cómo cuidar el cultivo en cada fase. Funciona en castellano, en runasimi (quechua wanka) o en los dos, con audios grabados.

**Abrir la app:** el enlace de GitHub Pages de este repositorio (ver *Settings → Pages*).

## Qué hay aquí

| Archivo | Qué es |
|---|---|
| `index.html` | La app |
| `datos.js` | El pronóstico y los mensajes. Se genera cada mes; no se edita a mano |
| `audios/es/`, `audios/qu/` | Audios grabados en castellano y en quechua (nombre = id del mensaje) |
| `manifest.webmanifest`, `icono-*.png` | Para instalarla como app en el celular («Agregar a pantalla de inicio») |

## De dónde salen los datos

Pronóstico SARIMA(1,0,1)(1,1,1)[12] de la evapotranspiración (FAO-56 Penman-Monteith) y de la lluvia, con datos del reanálisis ERA5-Land (Copernicus) de 1950 a 2026 para la estación Huayao, con la lluvia calibrada con la estación. Es un pronóstico del clima del valle, no una medición de cada chacra.

## Privacidad

La app no envía datos a ningún lado. El nombre y el celular son opcionales y se guardan solo en el celular de quien los escribe.

Proyecto de tesis · Ingeniería Ambiental · Universidad Continental · 2026
