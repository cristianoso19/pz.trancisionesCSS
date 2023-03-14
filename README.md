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

## Transform
Podemos hacer que los elementos cambien su tamaño o sus caracteristicas iniciales:
* roten
* escale
* etc

[🔗 Transform|Can I Use](https://caniuse.com/?search=transform)

[🔗 Gradient Backgrounds](https://cssgradient.io/gradient-backgrounds/)

[🔗 Gradient animaitor](https://www.gradient-animator.com/)

[🔥🔥🔥 Web Animations](https://tympanus.net/codrops/)

## Transform rotate, scale, skew y matrix
Además de translate, existen otras funciones que permiten transformar el elemento HTML para iniciar una animación.
<img src="https://media0.giphy.com/media/KRRSOKFINjskbRNENr/giphy.gif?cid=790b7611ee396f136b7b48c308d54e717611117f428e9871&rid=giphy.gif&ct=g">


### Rotate para transformaciones

Rotate es una función de la propiedad transform que te permite rotar un elemento HTML a través de los ejes del navegador. El valor que recibe es un ángulo, por ejemplo, “45deg” (45 grados) o “2rad” (2 radianes). Los ángulos positivos están en sentido horario, y los negativos en sentido antihorario.

```css
selector {
    transform: rotate(45deg);
}
```

<img src="https://cdn.document360.io/da52b302-22aa-4a71-9908-ba18e68ffee7/Images/Documentation/animationland05.PNG">

Dependiendo del eje en el que rotes el elemento, existe una función.

|Tipo	|Valor con los argumentos que recibe |
|-------|------------------------------------|
|Eje X y Y|	rotate(angle)|
|Eje X	|rotateX(angle)
|Eje Y	|rotateY(angle)
|Eje Z	|rotateZ(angle)
|Múltiple	|rotate3d(x,y,z,angle)

[Ejemplo](https://codi.link/PGRpdiBjbGFzcz0iY29udGFpbmVyIj4NCiAgPGRpdiBjbGFzcz0ic2hhZG93Ij4NCiAgPGRpdiBjbGFzcz0icm90YXRlIGVqZVhZIj5yb3RhdGU8L2Rpdj4NCjwvZGl2Pg0KDQo8ZGl2IGNsYXNzPSJzaGFkb3ciPg0KICA8ZGl2IGNsYXNzPSJyb3RhdGUgZWplWCI+cm90YXRlWDwvZGl2Pg0KPC9kaXY+DQoNCjxkaXYgY2xhc3M9InNoYWRvdyI+DQogIDxkaXYgY2xhc3M9InJvdGF0ZSBlamVZIj5yb3RhdGVZPC9kaXY+DQo8L2Rpdj4NCjwvZGl2Pg0KDQo=%7CLmNvbnRhaW5lciB7DQogIGRpc3BsYXk6IGZsZXg7DQogIGZsZXgtZGlyZWN0aW9uOiBjb2x1bW47DQogIGdhcDogM3JlbTsNCiAgd2lkdGg6IDEwMCU7DQogIGhlaWdodDogYXV0bzsNCiAgYWxpZ24taXRlbXM6IGNlbnRlcjsNCn0NCg0KLmNvbnRhaW5lciBkaXZ7DQogIHdpZHRoOiAyMDBweDsNCiAgaGVpZ2h0OiAyMDBweDsNCn0NCg0KLnNoYWRvd3sNCiAgYm9yZGVyOiAxcHggc29saWQgdHJhbnNwYXJlbnQ7DQogIGJhY2tncm91bmQtY29sb3I6IGdyZXk7DQp9DQoNCi5yb3RhdGV7DQogIGRpc3BsYXk6IGdyaWQ7DQogIGJvcmRlcjogMXB4IHNvbGlkIGJsYWNrOw0KICBwbGFjZS1jb250ZW50OiBjZW50ZXI7DQogIGZvbnQtc2l6ZTogMS41cmVtOw0KICBiYWNrZ3JvdW5kLWNvbG9yOiBza3libHVlOw0KICBjdXJzb3I6IHBvaW50ZXI7DQoNCn0NCg0KLyogwqFQcnVlYmEgY29uIGxvIHF1ZSBxdWllcmFzISEgKi8NCi5lamVYWTpob3ZlciB7DQogIHRyYW5zZm9ybTogcm90YXRlKDQ1ZGVnKTsNCn0NCg0KLmVqZVg6aG92ZXIgew0KICB0cmFuc2Zvcm06IHJvdGF0ZVgoNDVkZWcpOw0KfQ0KDQouZWplWTpob3ZlciB7DQogIHRyYW5zZm9ybTogcm90YXRlWSg0NWRlZyk7DQp9%7C)

### Scale para transformaciones

Scale es una función de la propiedad transform que te permite escalar un elemento HTML a través de sus ejes. El valor que recibe es un número multiplicador al elemento original.

Si el elemento es igual a 1 entonces sigue como el original; mayor a 1 aumenta de tamaño; y, menor a 1 disminuye de tamaño.

```css
selector {
    transform: scale(0.8);
}
```
<img src="https://cdn.document360.io/da52b302-22aa-4a71-9908-ba18e68ffee7/Images/Documentation/animationland06.PNG">

Dependiendo del eje en el que escales el elemento, existe una función.

|Tipo|	Valor con los argumentos que recibe|
|----|--------------------------------------|
|Eje X y Y|	scale(x)|
|Eje X|	scaleX(x)|
|Eje Y|	scaleY(y)|
|Eje Z|	scaleZ(z)|
|Múltiple|	scale3d(x,y,z)|

[Ejemplo](https://codi.link/PGRpdiBjbGFzcz0iY29udGFpbmVyIj4NCiAgPGRpdiBjbGFzcz0ic2hhZG93Ij4NCiAgPGRpdiBjbGFzcz0ic2NhbGUgZWplWFkiPnNjYWxlPC9kaXY+DQo8L2Rpdj4NCg0KPGRpdiBjbGFzcz0ic2hhZG93Ij4NCiAgPGRpdiBjbGFzcz0ic2NhbGUgZWplWCI+c2NhbGVYPC9kaXY+DQo8L2Rpdj4NCg0KPGRpdiBjbGFzcz0ic2hhZG93Ij4NCiAgPGRpdiBjbGFzcz0ic2NhbGUgZWplWSI+c2NhbGVZPC9kaXY+DQo8L2Rpdj4NCjwvZGl2Pg0KDQo=%7CLmNvbnRhaW5lciB7DQogIGRpc3BsYXk6IGZsZXg7DQogIGZsZXgtZGlyZWN0aW9uOiBjb2x1bW47DQogIGdhcDogM3JlbTsNCiAgd2lkdGg6IDEwMCU7DQogIGhlaWdodDogYXV0bzsNCiAgYWxpZ24taXRlbXM6IGNlbnRlcjsNCiAgbWFyZ2luOiAycmVtOw0KfQ0KDQouY29udGFpbmVyIGRpdnsNCiAgd2lkdGg6IDIwMHB4Ow0KICBoZWlnaHQ6IDIwMHB4Ow0KfQ0KDQouc2hhZG93ew0KICBib3JkZXI6IDFweCBzb2xpZCB0cmFuc3BhcmVudDsNCiAgYmFja2dyb3VuZC1jb2xvcjogZ3JleTsNCn0NCg0KLnNjYWxlew0KICBkaXNwbGF5OiBncmlkOw0KICBib3JkZXI6IDFweCBzb2xpZCBibGFjazsNCiAgcGxhY2UtY29udGVudDogY2VudGVyOw0KICBmb250LXNpemU6IDEuNXJlbTsNCiAgYmFja2dyb3VuZC1jb2xvcjogc2t5Ymx1ZTsNCiAgY3Vyc29yOiBwb2ludGVyOw0KDQp9DQoNCi8qIMKhUHJ1ZWJhIGNvbiBsbyBxdWUgcXVpZXJhcyEhICovDQouZWplWFk6aG92ZXIgew0KICB0cmFuc2Zvcm06IHNjYWxlKDEuMik7DQp9DQoNCi5lamVYOmhvdmVyIHsNCiAgdHJhbnNmb3JtOiBzY2FsZVgoMS41KTsNCn0NCg0KLmVqZVk6aG92ZXIgew0KICB0cmFuc2Zvcm06IHNjYWxlWSgwLjgpOw0KfQ==%7C)

### Skew para transformaciones
Skew es una función de la propiedad transform que te permite torcer un elemento HTML a través de sus ejes en dos dimensiones. El valor que recibe es un ángulo para cada eje en el que el elemento se distorsionará.
```css
selector {
    transform: skew(45deg, 45deg);
}
```
<img src="https://cdn.document360.io/da52b302-22aa-4a71-9908-ba18e68ffee7/Images/Documentation/animationland07.PNG">

|Tipo|	Valor con los argumentos que recibe|
|----|-------------------------------------|
|Eje X y Y|	skew(angleX, angleY)|
|Eje X|	skewX(angle)|
|Eje Y|	skewY(angle)|

### Matrix para transformaciones
Matrix es una función de la propiedad transform que te permite realizar varios efectos en uno solo.
[Documentacion](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/matrix)

### Orden en el código para transformaciones
Solamente puede existir una sola propiedad transform en el código de CSS, por lo que si escribimos otra regla CSS con otra transformación, esta se sobreescribirá y solo ejecutará la última. Por ende, utiliza varias funciones en la misma propiedad transform para realizar varias transformaciones.

```css
/*Mal (solo rotará el elemento)*/

selector {
    transform: translate(100px,  100px);
    transform: rotate(45deg);
 }
/*Bien (realizará ambas transformaciones)*/

selector {
    transform: translate(100px, 100px) rotate(45deg);
}
```

## Transform Origin 
El origen es el punto en el cual la transformación se ejecutará. La propiedad transform-origin permite cambiar el origen de las transformaciones, que por defecto está en el centro del elemento.
<img src="https://cdn.document360.io/da52b302-22aa-4a71-9908-ba18e68ffee7/Images/Documentation/animationland08.PNG">

[🔗 Link Ejemplos](https://codi.link/PGRpdiBjbGFzcz0iY29udGFpbmVyIj4NCiAgPGRpdiBjbGFzcz0ic2hhZG93Ij4NCiAgPGRpdiBjbGFzcz0idHJhbnNmb3JtIHJvdGF0ZSI+cm90YXRlPC9kaXY+DQo8L2Rpdj4NCg0KPGRpdiBjbGFzcz0ic2hhZG93Ij4NCiAgPGRpdiBjbGFzcz0idHJhbnNmb3JtIHNjYWxlIj5zY2FsZTwvZGl2Pg0KPC9kaXY+DQoNCjxkaXYgY2xhc3M9InNoYWRvdyI+DQogIDxkaXYgY2xhc3M9InRyYW5zZm9ybSBza2V3Ij5za2V3PC9kaXY+DQo8L2Rpdj4NCjwvZGl2Pg0KDQo=%7CLmNvbnRhaW5lciB7DQogIGRpc3BsYXk6IGZsZXg7DQogIGZsZXgtZGlyZWN0aW9uOiBjb2x1bW47DQogIGdhcDogM3JlbTsNCiAgd2lkdGg6IDEwMCU7DQogIGhlaWdodDogYXV0bzsNCiAgYWxpZ24taXRlbXM6IGNlbnRlcjsNCiAgbWFyZ2luOiAycmVtIDAgOHJlbSAwOw0KfQ0KDQouY29udGFpbmVyIGRpdnsNCiAgd2lkdGg6IDIwMHB4Ow0KICBoZWlnaHQ6IDIwMHB4Ow0KfQ0KDQouc2hhZG93ew0KICBib3JkZXI6IDFweCBzb2xpZCB0cmFuc3BhcmVudDsNCiAgYmFja2dyb3VuZC1jb2xvcjogZ3JleTsNCn0NCg0KLnRyYW5zZm9ybXsNCiAgcG9zaXRpb246IHJlbGF0aXZlOw0KICBkaXNwbGF5OiBncmlkOw0KICBib3JkZXI6IDFweCBzb2xpZCBibGFjazsNCiAgcGxhY2UtY29udGVudDogY2VudGVyOw0KICBmb250LXNpemU6IDEuNXJlbTsNCiAgYmFja2dyb3VuZC1jb2xvcjogc2t5Ymx1ZTsNCiAgY3Vyc29yOiBwb2ludGVyOw0KLyogwqFQcnVlYmEgY29uIGxvIHF1ZSBxdWllcmFzISEgKi8NCiAgdHJhbnNmb3JtLW9yaWdpbjogbGVmdCB0b3A7DQoNCn0NCg0KLnRyYW5zZm9ybTo6YWZ0ZXJ7DQogIGNvbnRlbnQ6ICIiOw0KICB3aWR0aDogMTBweDsNCiAgaGVpZ2h0OiAxMHB4Ow0KICBiYWNrZ3JvdW5kLWNvbG9yOiByZWQ7DQogIGJvcmRlci1yYWRpdXM6IDUwJTsNCiAgcG9zaXRpb246IGFic29sdXRlOw0KICB0b3A6IC01cHg7DQogIGxlZnQ6IC01cHg7DQp9DQoNCi50cmFuc2Zvcm06OmJlZm9yZXsNCiAgY29udGVudDogIm9yaWdpbiI7DQogIGZvbnQtc2l6ZTogc21hbGw7DQogIHBvc2l0aW9uOiBhYnNvbHV0ZTsNCiAgdG9wOiAtMjBweDsNCiAgbGVmdDogLTE1cHg7DQp9DQoNCi8qIFRyYW5zZm9ybWFjaW9uZXMgKi8NCi5yb3RhdGU6aG92ZXIgew0KICB0cmFuc2Zvcm06IHJvdGF0ZSg0NWRlZyk7DQp9DQoNCi5zY2FsZTpob3ZlciB7DQogIHRyYW5zZm9ybTogc2NhbGUoMS4yKTsNCn0NCg0KLnNrZXc6aG92ZXIgew0KICB0cmFuc2Zvcm06IHNrZXcoMjVkZWcsIDI1ZGVnKQ0KfQ==%7C)