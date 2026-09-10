# Taller 1 - Fundamentos Web
**Nombre:** Brayan josé Rodríguez Landázuri

Este repositorio contiene el primer taller de HTML de la asignatura Fundamentos de Programación Web.

## Estructura del Proyecto
- `index.html`: Estructura principal, contenido textual, tablas, formularios y elementos multimedia organizados de forma semántica.
- `multimedia/`: Carpeta que contiene los recursos locales requeridos (imágenes, audio y video).
- `README.md`: Documentación del taller y evidencias de la resolución del reto de verificación.

## Verificación de código

### Caso A
* **Problema identificado:** La etiqueta `<img>` está utilizando incorrectamente el atributo `href` para enlazar la ruta del archivo. El atributo `href` es exclusivo de etiquetas como `<a>` o `<link>`.
* **Corrección realizada:** Se reemplazó `href` por el atributo correcto `src`, quedando de la siguiente forma: `<img src="multimedia/perfil.jpg" alt="Fotografía del estudiante">`.
* **Fuente consultada:** MDN Web Docs - Elemento HTML <img>.

### Caso B
* **Problema identificado:** La etiqueta de enlace `<a>` está utilizando de forma errónea el atributo `src` para apuntar a la dirección web.
* **Corrección realizada:** Se corrigió cambiando el atributo `src` por el atributo estándar `href`, quedando así: `<a href="https://mozilla.org">Consultar MDN</a>`.
* **Fuente consultada:** MDN Web Docs - Elemento HTML <a>.

### Caso C
* **Problema identificado:** Dentro de la etiqueta `<video>`, el elemento secundario `<source>` utiliza incorrectamente el atributo `href` para definir la ubicación del archivo multimedia.
* **Corrección realizada:** Se modificó para emplear el atributo nativo `src`, estructurándose de esta manera: `<source src="multimedia/video.mp4" type="video/mp4">`.
* **Fuente consultada:** MDN Web Docs - Elemento HTML <source>.

### Caso D
* **Problema identificado:** El valor `"correo"` asignado al atributo `type` no es un tipo de entrada válido ni reconocido por los estándares actuales de HTML5.
* **Corrección realizada:** Se cambió por el valor estándar y compatible para campos de correo electrónico: `<input type="email" name="correo">`.
* **Fuente consultada:** Especificación de tipos de input - WHATWG HTML Living Standard.

### Caso E
* **La afirmación es:** Completamente FALSA.
* **Justificación:** En HTML5, la etiqueta correcta y estandarizada para insertar imágenes es `<img>`. Además, `<img>` es clasificado como un "elemento vacío" (void element), lo que significa que no contiene contenido de texto interno y **está prohibido cerrarlo con una etiqueta de cierre independiente** (`</img>`). Escribir `<image></image>` viola la sintaxis estándar de HTML5.
* **Fuente consultada:** MDN Web Docs - Elementos vacíos en HTML.

---

## Respuestas a las Preguntas de la Guía

### 1. ¿Qué información aparece dentro de la ventana del navegador al crear la estructura inicial y dónde se observa el contenido de `<title>`?
Al cargar la estructura base vacía, la ventana principal del navegador se muestra completamente en blanco. El texto definido dentro de `<title>` se visualiza exclusivamente en la pestaña superior del navegador o en la barra de título de la ventana.

### 2. ¿Para qué sirve `target="_blank"` en los enlaces?
Sirve para ordenarle al navegador que abra el hipervínculo en una pestaña o ventana nueva, permitiendo que el usuario consulte el sitio web externo sin perder o abandonar la página universitaria actual.

### 3. ¿Qué diferencia se identifica entre `<video>` e `<iframe>`?
La etiqueta `<video>` se usa para cargar y reproducir de forma nativa archivos de video propios almacenados localmente o en un servidor directo. En cambio, `<iframe>` se utiliza para incrustar un marco que renderiza un documento o reproductor web completamente externo (como un video de YouTube) consumiendo los recursos y funciones del proveedor original.

### 4. ¿Cuál es la diferencia conceptual entre `<progress>` y `<meter>`?
- `<progress>` se utiliza exclusivamente para indicar el estado de avance o completitud de una tarea que progresa en el tiempo (por ejemplo, el porcentaje de carga de un archivo).
- `<meter>` se emplea para representar mediciones escalares o valores fraccionarios fijos dentro de un rango numérico perfectamente conocido (por ejemplo, el nivel de uso de almacenamiento o una calificación numérica).
