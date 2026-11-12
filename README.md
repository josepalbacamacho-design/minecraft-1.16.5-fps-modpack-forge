# Modpack FPS / Rendimiento — Minecraft 1.16.5 Forge

Pack grande de rendimiento para Minecraft Java **1.16.5 + Forge**, con **95 archivos `.jar`** y dependencias obligatorias verificadas.

<p align="center"><a href="https://github.com/josepalbacamacho-design/minecraft-1.16.5-fps-modpack-forge/releases/latest/download/Modpack-FPS-1.16.5-Forge.zip"><img src="https://img.shields.io/badge/Descargar%20pack-Forge%201.16.5-brightgreen?style=for-the-badge" alt="Descargar pack Forge 1.16.5"></a></p>

**[Descargar el pack completo en ZIP](https://github.com/josepalbacamacho-design/minecraft-1.16.5-fps-modpack-forge/releases/latest/download/Modpack-FPS-1.16.5-Forge.zip)** · [Ver la release](https://github.com/josepalbacamacho-design/minecraft-1.16.5-fps-modpack-forge/releases/latest)

## Núcleo de rendimiento

La base Forge usa **Rubidium** para renderizado, **Oculus** para shaders, **FerriteCore** y **ModernFix** para memoria y carga, **Entity Culling**, **Saturn**, **AI Improvements**, **Dynamic FPS**, **FastQuit** y optimizadores de chunks, iluminación y red.

En esta versión Oculus declara incompatibilidad con Embeddium, por eso el pack usa Rubidium. No instales Embeddium, OptiFine ni otra copia de Rubidium junto con este pack. Se dejó **Jade** como visor de información; WTHIT fue excluido porque ambos usan el mismo ID Forge `waila`.

## Requisitos

- Minecraft Java **1.16.5**.
- **Minecraft Forge 36.2.39** o una versión Forge 36.x compatible.
- Java **8 de 64 bits**.
- RAM inicial: **3–4 GB**; no asignes casi toda la memoria del equipo.
- La primera prueba debe hacerse sin shaders activados.

## Instalación

1. Instala Minecraft 1.16.5 y Forge 36.2.39.
2. Inicia una vez el perfil Forge.
3. Copia todos los `.jar` de `mods/` a la carpeta `mods` de esa instancia.
4. Inicia el juego. Activa shaders solo después de confirmar que el pack base arranca.
5. No mezcles mods Fabric, NeoForge, Embeddium, OptiFine ni versiones de Minecraft distintas.

Si aparece un crash, guarda `logs/latest.log` y el crash report. Revisa primero la primera excepción `Caused by`, `Missing`, `Duplicate` o `Incompatible`; no añadas más mods hasta corregirla.

## Cliente y servidor

El pack está orientado principalmente al cliente. Los mods de renderizado, interfaz, mapas y FPS no deben copiarse automáticamente a un servidor dedicado. Prueba el servidor con una selección separada de mods comunes.

## Archivos

- `mods/`: los 95 archivos Forge.
- `LISTA-DE-MODS.md`: inventario generado desde `mods.toml`.
- `sources.json`: versiones e IDs detectados en los JAR.
- `descargar-mods.sh` y `descargar-mods.bat`: scripts de descarga desde la rama `main`.
- `Modpack-FPS-1.16.5-Forge.zip`: ZIP completo del pack.
