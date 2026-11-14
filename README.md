# Modpack Pure FPS / Optimización — Minecraft 1.16.5 Forge

Pack centrado exclusivamente en **optimización y rendimiento**, con **{len(files)} archivos `.jar` Forge**. No incluye mapas, inventario, decoración, contenido, voz ni utilidades generales que no aporten rendimiento.

<p align="center"><a href="https://github.com/josepalbacamacho-design/minecraft-1.16.5-fps-modpack-forge/releases/latest/download/Modpack-FPS-1.16.5-Forge-PURE.zip"><img src="https://img.shields.io/badge/Descargar%20pack-PURE%20FPS-brightgreen?style=for-the-badge" alt="Descargar pack Pure FPS Forge 1.16.5"></a></p>

**[Descargar el pack Pure FPS completo](https://github.com/josepalbacamacho-design/minecraft-1.16.5-fps-modpack-forge/releases/latest/download/Modpack-FPS-1.16.5-Forge-PURE.zip)** · [Ver la release](https://github.com/josepalbacamacho-design/minecraft-1.16.5-fps-modpack-forge/releases/latest)

## Optimizadores incluidos

- **Renderizado y FPS:** Rubidium, Rubidium Extra, Oculus y Entity Culling. También incluye **ChunkGuard**, el mod propio del pack para adaptar la distancia de chunks según el tiempo de tick, y **Menu Panels**, un añadido de cliente para reemplazar el menú principal con tres paneles de imágenes. También incluye **MemoryGuard**, que monitoriza la memoria y ofrece limpieza manual o automática opcional.
- **Memoria y carga:** FerriteCore, ModernFix, Memory Leak Fix, Saturn, Lightspeed, Ksyxis, Kerria y Opotato.
- **Entidades, lógica y generación:** AI Improvements, FastChest Revived, Structure Layout Optimizer, Radon y Dimensional Threading Reforked.
- **Red y tiempos de espera:** Packet Fixer, Fast IP Ping y FastQuit.
- **Arranque y eventos de Forge:** AsyncLogger, Remove Reloading Screen y FastEvent.
- **Entrada y tirones de cámara:** Ixeris, que mejora el sondeo de eventos y la entrada de alta frecuencia, especialmente con ratones de polling rate alto.
- **Ahorro en segundo plano:** Dynamic FPS y FPS Reducer.

## Candidatos revisados pero no incluidos por defecto

**Purescale** puede usar escalado y generación de frames, pero depende mucho de la GPU, la resolución y el método de escalado. **Distant Horizons** cambia radicalmente el sistema de distancia de renderizado y puede requerir ajustes específicos con shaders. Por eso se dejan fuera del ZIP universal para evitar que el pack falle o rinda peor en equipos que no los necesitan.

## No mezclar

Este pack usa **Rubidium** como renderizador. No añadas Embeddium, OptiFine, Sodium, otra versión de Rubidium ni mods Fabric. Oculus es la opción de shaders compatible con esta rama; prueba primero sin shaders para medir el rendimiento base. No combines este pack con otro mod de iluminación o renderizado principal.

## Requisitos

- Minecraft Java **1.16.5**.
- Minecraft Forge **36.2.39**.
- Java **8 de 64 bits**.
- RAM recomendada: **3–4 GB**, dejando memoria libre para el sistema.
- Para Dimensional Threading, usa más hilos de CPU que dimensiones activas y desactívalo si un mod de dimensiones presenta incompatibilidad.

## Instalación y prueba

Instala Forge 36.2.39, inicia una vez la instancia y copia los `.jar` de `mods/` en su carpeta `mods`. Mide primero sin shaders, con la misma distancia de renderizado y el mismo mundo. Después activa un shader ligero solo si el equipo tiene margen. Si usas Windows y un ratón de alta frecuencia, prueba Ixeris y compara FPS mínimos y estabilidad de cámara.

Si aparece un crash, guarda `logs/latest.log` y el crash report. No añadas mods al azar: revisa primero `Caused by`, `Missing`, `Duplicate`, `Mixin` o `Incompatible`.

## Archivos

- `mods/`: los 31 archivos Forge, incluidos `chunkguard-1.0.0.jar`, `menupanels-1.0.0.jar` y `memoryguard-1.0.0.jar`.
- `LISTA-DE-MODS.md`: inventario validado desde `META-INF/mods.toml`.
- `sources.json`: metadatos y fuentes de los archivos.
- `Modpack-FPS-1.16.5-Forge-PURE.zip`: ZIP de la variante de optimización pura.


### Compatibilidad con Java 8

Ixeris fue retirado del pack: las builds 1.16.5 revisadas incluyen clases compiladas para Java 17 y causan `UnsupportedClassVersionError` en Java 8.


### FastQuit

FastQuit fue retirado porque provocaba un crash al entrar a servidores multijugador: `Config class com.kingcontaria.fastquit.config.ModConfig has not been registered`.


### Better Biome Blend y LazyDFU

Better Biome Blend fue retirado por incompatibilidad con Rubidium detectada por Opotato. LazyDFU no se añadió porque las builds para 1.16.5 encontradas son Fabric y no Forge.


### MemoryGuard 2.0

Actualizado a `memoryguard-2.0.0.jar`: limpieza automática conservadora, protección durante ráfagas de chunks, limpieza al descargar mundos y recomendación de `-Xmx`. La memoria máxima se configura en el launcher, no durante la partida.


### RegorBoost Client

Añadido `regorboost-client-1.0.0.jar`, un mod solo de cliente para FPS, distancia de renderizado, memoria, partículas, entidades y ping. No modifica el servidor ni requiere instalación en Regorland. Se activa o desactiva con `F8`.


### RegorBoost Client 1.0.1

Actualizado a `regorboost-client-1.0.1.jar`. El límite máximo del cliente queda fijado en **150 FPS**. Ningún mod propio del pack aplica otro límite de FPS.


### Menu Panels 1.0.1

Actualizado `menupanels-1.0.1.jar`: reemplaza la textura de Doofus Jerry por la imagen recibida, verifica rutas `assets/menupanels/textures/gui/` y conserva la proporción de las tres imágenes con separadores negros.


### LazyDFU Forge 0.1.3

Añadido `lazydfu-0.1.3.jar`, build Forge compatible con Minecraft 1.16.5 y Java 8. ModernFix lo recomienda para diferir la inicialización de DataFixerUpper y evitar su advertencia de arranque.


### CoreFusion 1.0.0

Añadido `corefusion-1.0.0.jar`: complemento para memoria, chunks, entidades y partículas. Funciona en mundos individuales y servidores dedicados. Detecta ChunkGuard para no ejecutar un segundo controlador de distancia. Las funciones que pueden cambiar el gameplay están desactivadas por defecto.
