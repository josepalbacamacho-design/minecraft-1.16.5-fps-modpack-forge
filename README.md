# Modpack Pure FPS / Optimización — Minecraft 1.16.5 Forge

Pack enfocado exclusivamente en **optimización y rendimiento**, con **23 archivos `.jar` Forge**. No incluye mapas, mods de inventario, decoración, contenido, voz ni utilidades generales que no aporten rendimiento.

<p align="center"><a href="https://github.com/josepalbacamacho-design/minecraft-1.16.5-fps-modpack-forge/releases/latest/download/Modpack-FPS-1.16.5-Forge-PURE.zip"><img src="https://img.shields.io/badge/Descargar%20pack-PURE%20FPS-brightgreen?style=for-the-badge" alt="Descargar pack Pure FPS Forge 1.16.5"></a></p>

**[Descargar el pack Pure FPS completo](https://github.com/josepalbacamacho-design/minecraft-1.16.5-fps-modpack-forge/releases/latest/download/Modpack-FPS-1.16.5-Forge-PURE.zip)** · [Ver la release](https://github.com/josepalbacamacho-design/minecraft-1.16.5-fps-modpack-forge/releases/latest)

## Qué optimiza

- **Renderizado y FPS:** Rubidium, Rubidium Extra, Oculus y Entity Culling.
- **Memoria y carga:** FerriteCore, ModernFix, Memory Leak Fix, Saturn, Lightspeed y Ksyxis.
- **Entidades, lógica y generación:** AI Improvements, FastChest Revived, Structure Layout Optimizer y Radon.
- **Red y tiempos de espera:** Packet Fixer, Fast IP Ping y FastQuit.
- **Arranque y pantalla de carga:** AsyncLogger y Remove Reloading Screen.
- **Ahorro cuando el juego está en segundo plano:** Dynamic FPS y FPS Reducer.
- **Diagnóstico y estabilidad técnica:** las optimizaciones incluidas están pensadas para funcionar juntas en Forge 1.16.5; no se mezclan dos renderizadores principales.

## Importante: no mezclar

Este pack usa **Rubidium** como renderizador. No añadas Embeddium, OptiFine, Sodium, otra versión de Rubidium ni mods Fabric. Oculus se mantiene como opción de shaders compatible con esta rama; prueba primero sin shaders para medir el rendimiento base.

## Requisitos

- Minecraft Java **1.16.5**.
- Minecraft Forge **36.2.39**.
- Java **8 de 64 bits**.
- RAM recomendada: **3–4 GB**, dejando memoria libre para el sistema.

## Instalación

Instala Forge 36.2.39, inicia una vez la instancia y copia los `.jar` de `mods/` en su carpeta `mods`. Mide primero sin shaders, con la misma distancia de renderizado y el mismo mundo. Después activa un shader ligero solo si el equipo tiene margen.

Si aparece un crash, guarda `logs/latest.log` y el crash report. No añadas mods al azar: revisa primero `Caused by`, `Missing`, `Duplicate`, `Mixin` o `Incompatible`.

## Archivos

- `mods/`: los 23 archivos Forge.
- `LISTA-DE-MODS.md`: inventario validado desde `META-INF/mods.toml`.
- `sources.json`: metadatos y IDs detectados.
- `Modpack-FPS-1.16.5-Forge-PURE.zip`: ZIP de la variante de optimización pura.
