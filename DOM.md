Las siglas DOM significan Document Object Model es la estructura del documento HTML. Una página HTML está formada por múltiples etiquetas HTML, anidadas una dentro de otra, formando un árbol de etiquetas relacionadas entre sí, que se denomina árbol DOM 

## Funciones para modificar el DOM 
1- Acceder a elementos:
```javascript
//Por ID
const elementoPorId = document.getElementById('miElementoId');

// Por etiqueta
const elementosPorEtiqueta = document.getElementsByTagName('div');

// Por clase
const elementosPorClase = document.getElementsByClassName('miClase');

// Por selector CSS
const elementoPorSelector = document.querySelector('#miElementoId');

// Todos los elementos que coinciden con un selector CSS
const elementosPorSelectorAll = document.querySelectorAll('.miClase');
```

getElementById('miElementoId'): Esta función devuelve el elemento del DOM que tiene el atributo id igual a 'miElementoId'.
getElementsByTagName('div'): Devuelve una lista de todos los elementos con la etiqueta 'div'.
getElementsByClassName('miClase'): Devuelve una lista de todos los elementos que tienen la clase 'miClase'.
querySelector('#miElementoId'): Devuelve el primer elemento que coincide con el selector CSS '#miElementoId'.
querySelectorAll('.miClase'): Devuelve una lista de todos los elementos que coinciden con el selector CSS '.miClase'.

2. Acceder a elementos padres/hijos:
```javascript
javascript
function saludar() {
console.log("Hola, mundo!");
}
const elementoPadre = elementoHijo.parentNode;
const elementosHijos = elementoPadre.children;

parentNode: Accede al elemento padre del elemento actual.
children: Devuelve una lista de todos los elementos hijos del elemento actual.
```

3. Crear elementos:
```javascript
const nuevoElemento = document.createElement('div');
```
createElement('div'): Crea un nuevo elemento HTML con la etiqueta 'div' pero aún no lo agrega al DOM.
4. Añadir elementos al DOM
```javascript
const contenedor = document.getElementById('contenedor');
contenedor.appendChild(nuevoElemento);
```
appendChild(nuevoElemento): Agrega el nuevoElemento como un hijo al elemento actual en el DOM, por ejemplo, agregando un nuevo elemento 'div' a un contenedor existente.

5. Añadir/eliminar clases:
```javascript
elemento.classList.add('nuevaClase');
elemento.classList.remove('claseExistente');
```

classList.add('nuevaClase'): Agrega la clase 'nuevaClase' al elemento.
classList.remove('claseExistente'): Elimina la clase 'claseExistente' del elemento.

6. Obtener atributos:
```javascript
const valorDelAtributo = elemento.getAttribute('nombreDelAtributo');
```
getAttribute('nombreDelAtributo'): Devuelve el valor del atributo especificado (por ejemplo, 'href' en un enlace o 'src' en una imagen) del elemento.

7. Escribir texto dentro de un elemento:
```javascript
elemento.textContent = 'Nuevo texto';
```
textContent = 'Nuevo texto': Modifica el contenido de texto del elemento para que sea 'Nuevo texto'.
8. Modificar atributos:
```javascript
elemento.setAttribute('nombreDelAtributo', 'nuevoValor');
```
setAttribute('nombreDelAtributo', 'nuevoValor'): Cambia el valor del atributo especificado (por ejemplo, 'src' en una imagen) a 'nuevoValor'.


## jQuery 
¿Qué es?
jQuery es una biblioteca de JavaScript minificada de código abierto creada para simplificar las operaciones de JavaScript.
Una de las características principales de la biblioteca jQuery es el manejo de eventos. La creación de eventos, como la función de clic del mouse y el envío de formularios, sólo requiere unas pocas líneas de código. Esto ayuda a mantener el código HTML limpio y libre de varios manejadores de eventos.

Modificar los elementos HTML también es más fácil con su función de manipulación del Modelo de Objetos del Documento (DOM). La interfaz del navegador web, muy fácil de usar, te permite añadir, editar y eliminar elementos web utilizando varios métodos de eventos.

Características importantes de jQuery
1. Función hide()
La función hide() oculta los elementos HTML, haciendo que dejen de afectar a la página HTML. Sirve como método de animación si se combina con los parámetros de duración y de suavidad, así como con la función de devolución de llamada.

2. Función show()
La función show() muestra los elementos HTML. Sólo funciona en elementos ocultos por la función hide(). Además, se convierte en una función de método de animación si se le da un parámetro, al igual que hide().
3. Función toggle()
La función toggle() modifica la visibilidad de los elementos HTML en función de su propiedad de visualización CSS mediante un evento de clic
4. Función fadeIn()
La función fadeIn() modifica la opacidad de los elementos HTML para que aparezcan gradualmente en la página HTML. 
5. Función fadeOut()
Esta función de jQuery funciona de forma opuesta a la función fadeIn(). Al igual que hide() y show(), fadeIn() y fadeOut() se convierten en métodos de animación si se les da un parámetro.
6. Función fadeToggle()
La función fadeToggle() funciona de forma similar a la función toggle(). Permite al usuario mostrar u ocultar elementos específicos de forma gradual.
7. Función slideUp()
La función slideUp() oculta elementos con una animación deslizante. Acompáñala con los parámetros de duración y de suavidad para ajustar la duración de la animación.

8. Función slideDown()
La función slideDown() muestra elementos con una animación deslizante. También acepta los parámetros de duración y de suavidad.
10. Función slideToggle()
La función slideToggle() te permite alternar entre las funciones slideUp() y slideDown() para mostrar u ocultar elementos.
12. Función animate()
Esta función anima elementos utilizando una o varias propiedades CSS. Al igual que las funciones anteriores, te permite ajustar la duración de la animación y el modo de transición, así como activar la siguiente función una vez completada.