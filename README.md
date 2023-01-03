<div align='center'>
  <img height="60" src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/1920px-HTML5_logo_and_wordmark.svg.png">
  <h1>Preguntas/Respuestas de HTML para entrevista</h1>
  <i>Con respuestas detalladas en Español 🇪🇸</i>
</div>

---

## Índice

- [Índice](#índice)
  - [¿Qué es HTML?](#qué-es-html)
  - [¿Cuál es la estructura básica de un documento HTML?](#cuál-es-la-estructura-básica-de-un-documento-html)
  - [¿Qué es el DOM?](#que-es-el-dom)
  - [¿Cuál es la diferencia entre elementos y etiquetas en HTML?](#cuál-es-la-diferencia-entre-elementos-y-etiquetas-en-html)
  - [¿Qué son los atributos y cómo usarlos?](#qué-son-los-atributos-y-como-usarlos)
  - [¿Qué es el HTML semántico?](#qué-es-el-html-semántico)
  - [Accesibilidad en HTML](#accesibilidad-en-html)
  - [¿Cuáles son las APIs que proporciona HTML 5?](#cuáles-son-las-apis-que-proporciona-html5)
  - [¿Qué son los Web Components?](#qué-son-los-web-components)

---

### ¿Qué es HTML?
 
HTML (HyperText Markup Language), es un lenguaje de marcado utilizado para estructurar mediante etiquetas una página web y sus contenidos (texto, imágenes, videos, juegos, entre otros.)

**Aclaración:** HTML no es un lenguaje de programación.

**[⬆ Volver a índice](#índice)**

---

### ¿Cuál es la estructura básica de un documento HTML?
Un documento HTML está compuesto de tres partes:
 - Una línea que contiene la información de la versión de HTML
 - Una sección de cabecera declarativa (delimitada por el elemento `<head>`). El elemento `head` contiene el title y la meta data del documento web
 - Una sección que contiene el cuerpo del documento (delimitada por el elemento `<body>`. Acá podemos encontrar la información que se desea mostrar en la página web

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="utf-8">
    <title>Mi página de prueba</title>
  </head>
  <body>
    <p>Este es un texto de prueba</p>
  </body>
</html>
```
 
**[⬆ Volver a índice](#índice)**

---

### ¿Qué es el DOM?

El Document Object Model  (DOM) es una interfaz de programación para documentos web. Representa la página para que los programas puedan cambiar la estructura, el estilo y el contenido del documento. El DOM representa el documento como nodos y objetos; de esa manera, los lenguajes de programación pueden interactuar con la página web.

**[⬆ Volver a índice](#índice)**

---

### ¿Cuál es la diferencia entre elementos y etiquetas en HTML?

| Elementos                                                                                                                                                                                   | Etiquetas                                                                                                                                                                           |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| El elemento es un componente individual de la página web o documento HTML. Representa la semántica o el significado. Por ejemplo, el elemento de `title` representa el título del documento. | Es la raíz del documento HTML que se utiliza para especificar que el documento es HTML. Por ejemplo, la etiqueta `head` se usa para contener todo el elemento head en el archivo HTML. |

**[⬆ Volver a índice](#índice)**

---

### ¿Qué son los atributos y cómo usarlos?

Cada etiqueta tiene atributos adicionales que cambian la forma en que se comporta o se muestra. Por ejemplo, una etiqueta `<input>` tiene un atributo de `type`, que puede usar para especificar si es un campo de texto, una casilla de verificación, un botón de radio o una de muchas opciones más.

Los atributos se especifican directamente después del nombre de la etiqueta, dentro de los dos corchetes angulares `< />`. Solo deben aparecer en las etiquetas de apertura o en las etiquetas de cierre automático. Pero, nunca pueden estar en etiquetas de cierre.

```html
<!-- Text field -->
<input type="text" />
<!-- Checkbox -->
<input type="checkbox" />
<!-- Radio button -->
<input type="radio" value="on" />
```

**[⬆ Volver a índice](#índice)**

---

### ¿Qué es el HTML semántico?
Muchas personas no tienen una idea clara de lo que es la Web Semántica. La mejor definición informal se puede encontrar en el artículo de Scientific American de mayo de 2001 "La Web Semántica" (Berners-Lee et al.), que dice _"La Web Semántica es una extensión de la web actual en la que se le da a la información un significado bien definido, permitiendo que las computadoras y las personas trabajen mejor en cooperación"_.

**[⬆ Volver a índice](#índice)**

---

### Accesibilidad en HTML

Escriba HTML teniendo en cuenta la accesibilidad. Proporcione al usuario una buena manera de navegar e interactuar con su sitio. Haga que su código HTML sea lo más semántico posible, de modo que el código sea fácil de entender para los visitantes y los lectores de pantalla.

Algunas recomendaciones:

- HTML Semántico: HTML semántico significa usar elementos HTML correctos para su propósito correcto tanto como sea posible.
- Cabeceras: Agregar las cabeceras (`h1`, `h2`... ,`h6`) de manera correcta y en orden descendente 
- Texto alternativo: Agregar el atributio `alt` en las imágenes
- Declarar el idioma: `<html lang="es">`
- ARIA: También conocido como WAI-ARIA, significa _Accessible Rich Internet Applications_. ARIA define una variedad de extensiones de marcado, generalmente atributos HTML5, que se pueden agregar a los elementos para brindar a los lectores de pantalla más información sobre el elemento y ayudar a los usuarios con discapacidades visuales a comprender mejor lo que sucede en la página web

**[⬆ Volver a índice](#índice)**

---

### ¿Cuáles son las APIs que proporciona HTML 5?

Está sería una lista de las APIs más populares y/o más usadas en HTML:

| Api                      | ¿Qué hace?                                                                                               |
|--------------------------|----------------------------------------------------------------------------------------------------------|
| Canvas 2D Context        | Permite dibujar y manipular gráficos en el navegador.                                                    |
| Drag and Drop            | Permite arrastrar y soltar elementos dentro y entre las ventanas del navegador.                          |
| File API                 | Proporciona programas con acceso seguro al sistema de archivos del dispositivo.                          |
| Forms                    | Da acceso a los programas a los nuevos tipos de datos definidos en HTML5.                                |
| Geolocation              | Proporciona a las aplicaciones web acceso a datos de ubicación geográfica de el dispositivo del usuario. |
| History API              | Permite que los programas manipulen el historial del navegador.                                          |
| Internationalization API | Proporciona acceso a formato sensible a la configuración regional y comparación de cadenas.              |
| Web Audio API            | API para procesar y sintetizar audio.                                                                    |
| Web storage              | Permite el almacenamiento de pares clave-valor en el navegador.                                          |
| Web sockets              | Abre una sesión de comunicación interactiva entre el navegador y el servidor.                            |
| Web Workers              | Permite que JavaScript ejecute scripts en segundo plano.                                                 |

**[⬆ Volver a índice](#índice)**

---

### ¿Qué son los Web Components?

Los Web Components son un conjunto de diferentes tecnologías que permiten crear elementos personalizados reutilizables, con su funcionalidad encapsulada lejos del resto de su código, y utilizarlos en sus aplicaciones web sin temor a colisiones de código.

Consta de las siguientes tecnologías:

- **Custom elements**: Un conjunto de API de JavaScript que le permiten definir elementos personalizados y su comportamiento, que luego se pueden usar como se desee en su interfaz de usuario.
- **Shadow DOM**: Un conjunto de API de JavaScript para adjuntar un árbol Shadow DOM a un elemento que se representa por separado del DOM del documento principal, y permite controlar la funcionalidad asociada. De esta manera, es posible mantener privadas las características de un elemento, de modo que se puedan escribir y diseñar sin temor a colisionar con otras partes del documento.
- **HTML templates**: Los elementos `<template>` y `<slot>` le permiten escribir plantillas de marcado que no se muestran en la página representada. Estos se pueden reutilizar varias veces como base de la estructura de un elemento personalizado.

**[⬆ Volver a índice](#índice)**

---