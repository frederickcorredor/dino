# dino.github.io
Este es un script de JavaScript que crea un juego simple utilizando el elemento canvas en una página HTML.

Aquí hay una explicación general de cómo funciona el código:

Variables globales: Al comienzo del script, se declaran varias variables globales que se utilizarán en el juego, como el lienzo (canvas), su contexto (ctx), un objeto para representar al dinosaurio, un arreglo de árboles, coordenadas para el piso, imágenes y variables para controlar el juego, como la puntuación, la velocidad y más.

Inicio: La función Inicio() se llama cuando se carga la página. En esta función, se inicializan las variables, se configura el evento del teclado, y se inicia un bucle de animación llamado FrameLoop() utilizando window.setInterval.

FrameLoop: Esta función se encarga de actualizar y renderizar el juego en cada fotograma. Aquí se llama a varias funciones para dibujar el fondo, manejar el salto del personaje, dibujar el personaje, crear árboles, llevar un registro de la puntuación, aumentar la velocidad del juego y revisar las colisiones.

AgregarEventoTeclado: Esta función configura los eventos del teclado, lo que permite que el jugador controle el salto del personaje utilizando las teclas de flecha arriba (38), la barra espaciadora (32) y reiniciar el juego con la tecla Enter (13).

InicializarJSON: Aquí se inicializan objetos JSON que representan al dinosaurio y las nubes en el fondo del juego. Estos objetos contienen información sobre sus coordenadas y dimensiones.

CrearArbol: Esta función genera nuevos árboles en el juego en intervalos regulares. Los árboles son almacenados en el arreglo arbol.

DibujarFondo: Dibuja el fondo del juego, incluyendo el cielo, las nubes, la puntuación, el suelo y una línea divisoria en el suelo.

MoverNubes: Mueve las imágenes de nubes en el fondo del juego para dar la ilusión de movimiento.

DibujarPersonaje: Dibuja el dinosaurio en el lienzo. Cambia de imagen del dinosaurio en cada fotograma para crear una sensación de animación.

SaltoPersonaje: Controla el salto del dinosaurio. El dinosaurio sube y luego baja hasta tocar el suelo nuevamente.

DibujarrArboles: Dibuja los árboles en el juego, y si un árbol sale de la pantalla, se elimina del arreglo.

Puntuación: Calcula la puntuación del jugador en función de la cantidad de árboles saltados.

SubirVelocidadJuego: Aumenta la velocidad del juego a medida que el jugador acumula más puntos.

RevisarColisiones: Verifica si el dinosaurio colisiona con algún árbol. Si ocurre una colisión, el juego se detiene y se muestra un mensaje para reiniciar.

RestablecerJuego: Restablece todas las variables para reiniciar el juego cuando el jugador presiona la tecla Enter.

Este código crea un juego simple de saltos con un dinosaurio que debe esquivar los árboles. La puntuación aumenta a medida que se saltan más árboles, y la velocidad del juego aumenta a medida que el jugador acumula más puntos.
