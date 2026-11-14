# Café Origen — Inventario

Página web que muestra el inventario de una cafetería en una tabla y marca en rojo los productos con poco stock.

## Propósito

Este proyecto nació en la Práctica 4 (*El inventario corrupto*): se corrigió un archivo `inventario.xml` con errores de formato, se completó un dato faltante y la información se pasó a `inventario.json`. La página carga ese JSON con `fetch` y llena la tabla automáticamente. Los productos con **stock menor a 5** aparecen en rojo, y la columna **Estado** indica "Stock bajo" o "Disponible" para no depender solo del color.

## Autor

Omar Alejandro Salazar Castro — Matrícula 2226576

Facultad de Ingeniería Mecánica y Eléctrica, UANL · Laboratorio de programación web (Grupo 208)

## Tecnologías utilizadas

- HTML
- CSS
- JavaScript (`fetch` para cargar los datos)
- XML y JSON (formato de los datos del inventario)
- Node.js (solo para el servidor local de desarrollo)
- Git y GitHub Pages (control de versiones y publicación)

## Cómo ejecutarlo o consultarlo

**Versión publicada:** https://omaralex06.github.io/practica4-inventario-cafe-origen/

**Para correrlo localmente:**

1. Clona este repositorio:
   ```
   git clone https://github.com/OmarAlex06/practica4-inventario-cafe-origen.git
   cd practica4-inventario-cafe-origen
   ```
2. Inicia el servidor (requiere Node.js 18 o superior, no necesita `npm install`):
   ```
   node server.js
   ```
3. Abre http://localhost:3500 en el navegador.

> No abras `index.html` con doble clic: `fetch()` no puede cargar `inventario.json` desde `file://`. Usa el servidor local o la versión publicada.

## Estructura del proyecto

```
index.html         Página con la tabla
inventario.xml     Datos originales, ya corregidos
inventario.json    Datos que consume la página
css/estilos.css    Estilos (incluye el rojo del stock bajo)
js/main.js         Carga el JSON y llena la tabla
server.js          Servidor local sin dependencias
```
