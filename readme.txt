
El sistema de cuadrícula Bootstrap 4 tiene cinco clases:

.col- (extra small devices - screen width less than 576px)
.col-sm- (small devices - screen width equal to or greater than 576px)
.col-md- (medium devices - screen width equal to or greater than 768px)
.col-lg- (large devices - screen width equal to or greater than 992px)
.col-xl- (xlarge devices - screen width equal to or greater than 1200px)

		/*Resolucion para dispositivos moviles muy pequeños*/
		@media (max-width: 575px){

		}
		/*Resolucion para dispositivos moviles pequeños*/
		@media (min-width: 576px) and (max-width: 767px){

		}

		/*Resolucion para tables*/
		@media (min-width: 576px) and (max-width: 991px){

		}

		/*Resolucion para tables*/
		@media (min-width: 992px) {
			
		}

		Nota: Si el estilo no se encuentra dentro de los medias queries, el objeto desaparecera en esa medida.
----------------------------------------------Height y Width-----------------------------------------
¿Qué son las medidas vh y vw?
Las medidas vh y vw son medidas relativas de acuerdo al viewport. Vh hace referencia a la centésima parte de la altura del viewport y vw a la centésima parte del ancho del viewport.

height:
1vh = 1% de la altura del viewport
100vh = altura del viewport

width:
	1vw = 1% del ancho del viewport
	100vw = ancho del viewport


¿Cómo haríamos para que la imagen de fondo ocupe todo el alto de la pantalla y a continuación cuando hagamos scroll se vea el párrafo? Lo primero que se les puede ocurrir es dar height: 100% al div, pero esto no funciona porque el alto del padre depende del contenido que este conteniendo. En este caso solo contiene dos palabras y su alto sera igual al line-height de el texto, es así que eso no nos sirve.

Otra opción sería position:absolute y poner top, left, right y bottom con valor 0, pero el párrafo que sigue quedaría debajo de la imagen y no se vería. Seguro, hay muchas más opciones, pero la que mejor se adecúa es usando la medida vh, con solo agregar height: 100vh, ya tendremos nuestra imagen ocupando todo el alto.


Relativo a la ventana gráfica
También puede utilizar las utilidades para establecer el ancho y el alto en relación con la ventana gráfica.

<div class="min-vw-100">Min-width 100vw</div>
<div class="min-vh-100">Min-height 100vh</div>
<div class="vw-100">Width 100vw</div>
<div class="vh-100">Height 100vh</div>


----------------------------------------------colores CSS y nombre------------------------
https://www.rapidtables.com/web/css/css-color.html

Gray colors
Color	HTML / CSS
Color Name	Hex Code
#RRGGBB	Decimal Code
(R,G,B)
 	gainsboro	#DCDCDC	rgb(220,220,220)
 	lightgray	#D3D3D3	rgb(211,211,211)
 	silver	#C0C0C0	rgb(192,192,192)
 	darkgray	#A9A9A9	rgb(169,169,169)
 	gray	#808080	rgb(128,128,128)
 	dimgray	#696969	rgb(105,105,105)
 	lightslategray	#778899	rgb(119,136,153)
 	slategray	#708090	rgb(112,128,144)
 	darkslategray	#2F4F4F	rgb(47,79,79)
 	black	#000000	rgb(0,0,0)

 	ETC...