# pz.trancisionesCSS
Curso de platzi transiciones con css 

## 5 razones para animaciones en la web

1. 🧠 Las animaciones tienen beneficios para el cerebro: reduce el esfuerzo que hace el usuario y enfocarlo en las partes importates.
2. 🗣️ Las animaciones se comunican: los humanos tratamos de armar un hilo conductor asociandolo a la vida real.
3. 📲 Las animaciones conectan contextos: deben comunicar lo mismo independientemente de la plataforma para que el usuario tenga la sensaciòn de estar en el mismo lugar.
4. 🕺 Coreografía de UI: Coincidir las animaciones al menos que comuniquen lo mismo. Coherencia en las animaciones.
5. 🔊 Las animaciones llaman la atenciòn: nos ayudan a comunicar y expresar lo que debe sentirse.

## Propiedades para crear animaciones con CSS y propiedades animables
* 🎁 Transform `transform()`: Hace una transformacion del elemento HTML, cambiamos una posicion inicial a otra en el transcurso del tiempo.
🔗 [Transform Cheat Sheet](https://static.platzi.com/media/public/uploads/transformaciones_en_2d_y_3d_d712736c-5368-4c9b-8827-331dc347d536.pdf).
* ➡️ Transition `transition()`: Ir de un lado A a B, en el eje x sin cambio en medio del punto a y b.
🔗 [Transition Cheat Sheet](https://static.platzi.com/media/public/uploads/transiciones_2093f06d-4937-4ba1-999d-73e1b9a56cca.pdf).
* 🤖 Animation: Lo mismo que transition pero si puede haber un cambio en medio del punto a y b.
🔗 [Animation Cheat Sheet](https://static.platzi.com/media/public/uploads/animaciones_5bda2325-fb2e-4060-9751-5863d226fcf1.pdf).

<img src="https://media.giphy.com/media/gCSOFQybTbM3pome6c/giphy.gif">

> 💡 Animable: que sus valores cambien gradualmente durante un periodo de tiempo.

## Pseudo-clases y pseudo-elementos en las animaciones

> 🚀 [HTML Color Codes](https://htmlcolorcodes.com/)

Un trigger es un accionador de animaciones, es decir, el evento inicial que desencadena una animación. Algunos ejemplos son:

* Pasar el mouse sobre un elemento.
* Dar clic a un elemento.
* Al deslizar la pantalla.
* Al recargar la página web.
* Las pseudo-clases y pseudo-elementos ayudan a activar las animaciones.

**Pseudo-clases**
Una pseudo-clase define el estilo de un estado especial de un elemento.

* Índice de pseudo-clases estándar{target="_blank"}.

**Sintaxis**
selector:pseudo-clase { propiedad: valor; }
**:link**
La pseudo-clase :link representa el estado de un elemento que no ha sido visitado.

Ejemplo usando :link{target="_blank"}
**:visited**
La pseudo-clase :visited representa el estado de un elemento que ya ha sido visitado.

Ejemplo usando :visited{target="_blank"}
**:hover**
La pseudo-clase :hover representa el estado en el cual el cursor está encima del elemento.

Ejemplo usando :hover{target="_blank"}
**:not()**
La pseudo-clase :not() representa el estado en el cual no coinciden los selectores que se indiquen.

Ejemplo usando :not(){target="_blank"}
**:nth-child()**
La pseudo-clase :nth-child() representa el estado en el cual coinciden los hijos del elemento según el valor indicado.

Valores de palabras clave:

* odd: Los elementos hijos en posiciones impares.
* even: Los elementos hijos en posiciones pares.

*Fórmula matemática:* An+B donde A y B son números enteros.

* Ejemplo usando :nth-child(){target="_blank"}

**Pseudos-elementos**
Un pseudo-elemento define el estilo de una parte específica de un elemento.

* Lista de pseudo-elementos{target="_blank"}.

**Sintaxis**
```selector::pseudo-elemento { propiedad: valor; }```
**::before**
La pseudo-elemento ::before sirve para agregar un contenido antes del elemento. El contenido es agregado mediante la propiedad CSS content.

* Ejemplo usando ::before{target="_blank"}

**::after**
La pseudo-elemento ::after sirve para agregar un contenido después del elemento. El contenido es agregado mediante la propiedad CSS content.

* Ejemplo usando ::after{target="_blank"}

## Timing Function

Son importantes por que nos hablan de la acelaración de los elementos.

> 🔗 [Easings.net](https://easings.net/)
> 🔗 [CUbic-bezier](https://cubic-bezier.com/#.17,.67,.83,.67)

## Planos y ejes

Existen 3 ejes x y z,