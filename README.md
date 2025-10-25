# AluraBank

Documento de referencia para el proyecto front-end "AluraBank": una pequeña aplicación web estática que demuestra un formulario de apertura de cuenta con validaciones front-end.

## Descripción

Este repositorio contiene los archivos de una página web estática (HTML/CSS/JS) creada como ejercicio/práctica. El proyecto incluye formularios para abrir una cuenta y varios scripts de validación y utilidades.

Está pensado para aprender y practicar:
- Maquetación HTML y estilos CSS modularizados.
- Validación de formularios con JavaScript.
- Uso básico de módulos JS y organización de assets (imágenes, estilos, páginas).

## Formulario de creación de cuenta para el banco virtual AluraBank

![Formulario de creación de cuenta - AluraBank](img/alurabank1.gif)

**Pasos para registrarse.**

![Reconocimiento facial](img/alurabank2.png)



## Características principales

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)


- Formularios multi-página para apertura de cuenta (3 pasos).
- Validaciones de campos: edad, CUIT (archivo `validar-cuit.js`, `validar-edad.js`).
- Manejo de errores personalizado (`customErrors.js`).
- Código separado en la carpeta `js/` para facilitar lectura y mantenimiento.

## Estructura del proyecto

Raíz del proyecto (archivos y carpetas relevantes):

- `index.html` — Página principal.
- `README.md` — Este archivo.
- `img/` — Imágenes usadas en la interfaz.
- `js/` — Scripts JavaScript:
	- `camera.js`
	- `customErrors.js`
	- `main.js`
	- `validar-cuit.js`
	- `validar-edad.js`
- `pages/` — Páginas del flujo de apertura de cuenta:
	- `abrir-cuenta-form.html`
	- `abrir-cuenta-form-2.html`
	- `abrir-cuenta-form-3.html`
- `styles/` — Estilos globales y específicos por página/componentes.

## Cómo abrir y probar el proyecto (modo simple)

Al tratarse de una página estática, la forma más simple es abrir `index.html` en el navegador (doble clic). Algunas APIs modernas o importaciones pueden requerir servir los archivos desde un servidor local.

Opciones para servir localmente (recomendado):

Usando Python 3 (servidor HTTP simple) — ejecuta desde la raíz del proyecto:

```bash
python3 -m http.server 8000
```

Luego abre en tu navegador:

```
http://localhost:8000
```

Alternativa con Node (si prefieres `http-server`):

```bash
npm install -g http-server
http-server -p 8000
```

## Desarrollo

- Edita los archivos HTML en la raíz o en `pages/`.
- Modifica estilos en `styles/` y `styles/formulario/` según corresponda.
- Los scripts están en `js/`; agrégalos o modifícalos respetando el orden de carga en los HTML.

Consejos rápidos:
- Usar la consola del navegador (DevTools) para depurar validaciones JS.
- Para cambios en CSS, recarga con cache-bypass (Cmd+Shift+R en macOS).

## Tests

No hay tests automatizados incluidos en este repositorio. Si deseas añadir pruebas, se puede proponer una estructura con Jest (para funciones puras) o pruebas end-to-end con Playwright/Cypress para flujos de formulario.

## Contribución

Si quieres contribuir:
1. Haz fork del proyecto.
2. Crea una rama con una descripción clara del cambio.
3. Abre un pull request describiendo el motivo y los pasos para reproducir.

## Autor

Desarrollado por Lucero Uzuriaga
✨ Portafolio creado con pasión y dedicación.

## Licencia

Este proyecto está bajo la licencia MIT.
Consulta el archivo LICENSE para más detalles.
