---
title: "Lección 12 - Publica el sitio con GitHub Pages"
description: "Usa la aplicación de GitHub Copilot para configurar un flujo de trabajo de Pages, revisar su solicitud de incorporación de cambios y comprobar que Space Quiz está disponible en línea."
authors:
  - jamesmontemagno
lastUpdated: 2026-10-12
---

Publica Space Quiz con GitHub Pages para que todo el mundo pueda acceder a él. Copilot puede preparar el flujo de trabajo y guiarte durante la publicación, pero tú sigues siendo responsable de revisar los cambios y confirmar que el sitio está disponible.

En esta lección:

- Pide a Copilot que configure la publicación con GitHub Pages.
- Revisa el flujo de trabajo y la solicitud de incorporación de cambios antes de combinarla.
- Sigue el proceso de publicación y comprueba el sitio publicado.

## Escenario

Space Quiz ya está en un repositorio de GitHub, pero la gente aún necesita una forma sencilla de probarlo. Publicar el sitio de un solo archivo con GitHub Pages lo pone a disposición desde una URL pública sin añadir un servidor ni una dependencia del entorno de ejecución.

## Pide a Copilot que publique el sitio

En la sesión de la aplicación Copilot para `space-quiz`, envía este mensaje:

```plaintext
Habilita GitHub Pages para este repositorio. Crea un flujo de trabajo de GitHub Actions que compile el sitio web si es necesario y lo publique en GitHub Pages. Añade un README que describa la aplicación y cómo ejecutarla en local si aún no existe. Crea una solicitud de incorporación de cambios con estos cambios y combínala cuando pasen las comprobaciones obligatorias. Supervisa la publicación hasta que se complete correctamente y, después, indica la URL final del sitio web. Si no tienes permiso para habilitar Pages o combinar la solicitud, dime exactamente qué tengo que aprobar o hacer; no indiques que se ha completado correctamente hasta que el sitio esté disponible.
```

![Diagrama de tres etapas: una solicitud de incorporación de cambios de Space Quiz combinada; una ejecución correcta de Deploy website en GitHub Actions con los pasos Build website, Upload artifact y Deploy to Pages; y Space Quiz publicado en yourname.github.io/space-quiz/.](../../../_images/first-steps-app-pages-deploy.svg)

> [!WARNING]
> Este mensaje pide al agente que cree y combine una solicitud de incorporación de cambios y cambie la configuración de Pages del repositorio. Revisa las diferencias, los permisos de publicación y las solicitudes de aprobación de GitHub antes de continuar.

## Revisa el flujo de trabajo y comprueba la publicación

1. Confirma que el README solo se añade si el repositorio aún no tiene uno.
2. Revisa los cambios de la solicitud de incorporación de cambios, incluidos los pasos de compilación y publicación del flujo de trabajo.
3. Combina los cambios solo cuando pasen las comprobaciones obligatorias de la solicitud.
4. Sigue la ejecución de publicación de GitHub Actions hasta que se complete correctamente.
5. Abre la URL indicada y confirma que Space Quiz se carga.

Si el agente no puede habilitar Pages o combinar la solicitud de incorporación de cambios, sigue las instrucciones concretas que te proporcione. No des la tarea por terminada hasta que la publicación se complete correctamente y el sitio esté disponible.

## Resumen y próximos pasos

Space Quiz ya está disponible como sitio web y has comprobado la publicación en lugar de depender del informe del agente. Continúa con la [Lección 13: Repaso y próximos pasos][next-lesson].

[next-lesson]: ../13-review/
