---
title: Hello World con p5.js
subtitle: 'Demo básica de p5.js'
summary: Demo básica de p5.js integrada en Hugo/Academic
authors:
- chema
tags:
- Academic
- Hugo
- Tecnología
- Programación
- Javascript
- P5.js
- Tutorial
- Ejemplo
categories:
- Tecnología
- Programación
- Javascript
- P5.js
- Tutorial
date: "2020-04-16T00:00:00Z"
lastmod: "2020-04-16T00:00:00Z"
featured: false
draft: false
toc: true
type: docs

menu:
  p5.js:
    parent: Hello World
    weight: 2

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight:

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Placement options: 1 = Full column width, 2 = Out-set, 3 = Screen-width
# Focal point options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
image:
  placement: 1
  caption: 'Logo P5.js'
  focal_point: ""
  preview_only: false
---
Este es el primer ejemplo de código usando *[p5.js](https://p5js.org/)* integrado en un post con Hugo. Debajo del sketch está el código que lo genera.


{{< p5 file="helloWorld.js">}}

Al ver el código, veréis que tiene un par de funciones más que el clásico HelloWorld:
* <code>getPos(...)</code>:el canvas (lienzo) se coloca dentro de un elemento <code> div id="sketch"</code>. Esta función me devuelve en coordenadas absolutas la posición de ese <code>div</code>. Me va a ayudar para la siguiente función.
* <code>centerCanvasDivHorizontally()</code>: esta función me centra el canvas horizontalmente dependiendo del tamaño del mismo. Lo he desarrollado para que al ejecutarse la anchura sea 3/4 de la anchura de la ventana. Al final de la función modifico directamente el CSS del <code>div</code> que lo contiene para asegurar que los bordes se vean adecuadamente.

Sobre posicionamiento del canvas, en esta web dan varios trucos: [Positioning your canvas](https://github.com/processing/p5.js/wiki/Positioning-your-canvas).

{{< showCodeFile staticPath= "/static/js/p5_sketches/" file="helloWorld.js" language="js">}}
