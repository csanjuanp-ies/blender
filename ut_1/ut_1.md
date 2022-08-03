# U.T. 1 Introducción
## Diseño en 3D, introducción y conceptos
El diseño en 3D se entiende como todo diseño que utiliza para definir su contenido el espacio vectorial de tres dimensiones. Es decir, los objetos se definirán a través de puntos con tres coordenadas (x, y z) generando polígonos o caras para la definición de dichos objetos.

Una vez creados los objetos podrán ser modificados tanto a nivel global (desplazamientos, rotaciones, escalado, etc.) como a nivel local (transoformación de sus puntos, aristas o caras).

### Elementos básicos de un objeto 3D
Todo objeto en 3D se definirá por los puntos que lo forman, que a su vez crearán arístas que uniendo al menos tres de ellas definirán una cara. El objeto mínimo que podemos definir es un **plano**, constituido por una cara y al menos tres vértices.

A continuación vemos los elementos constituyentes de cualquier objeto:
- Vértices (*vertex*).
- Aristas (*edge*).
- Caras (*face*).
![](ut_01_000.png)

Las caras se denominan en el disño 3D polígonos, siendo estas triángulos (3 vértices *triangles*), cuadrados (*quads*) o polígonos de más caras (*ngons*). El número máximo de vértices de una cara no está limitado, pero cuanto más elevado sea más compleja será la forma y por tanto la necesidad de procesamiento será mayor.

 ![](ut_01_001.png)

>Se debería mantener la complejidad de los polígonos lo más baja posible para minimizar el coste de uso de cpu. Pero aunque parezca que el mejor polígono para formar nuestro modelo sería el triángulo, no es así, se recomienda usar cuadrados o rectángulos en el mayor número posible de caras.

### Mallas
Un objeto estará constituido por múltiples caras unidas entre sí o no que le darán forma. Este conjunto de caras se denomina malla. La malla es la superficie del objeto que podemos manipular.

Es importante entender que la malla es un todo, es el objeto en sí, es lo que define nuestro objeto.

Cuando definimos la malla del objeto, podemos usar un número variable de caras en ella, pero siguiendo el principio anterior, intentaremos mantener la complejidad de la malla (número de caras) lo más bajo posible, mejorando tanto la respuesta a la hora de crear la escena fina, así como el uso de materiales (colores, texturas, etc.) en la malla.

### Centro geométrico o de transformación
 ![](ut_01_002.png)

Todo cuerpo tiene un punto geométrico ficticio que representa el centro de masas, dicho punto se denomina **centro geométrico**. En los programas de 3D el centro geométrico se utiliza como punto de referencia para realizar las transformaciones (rotaciones, escalado, etc.). Este punto se puede posicionar en cualquier lugar del espacio, pero es muy aconsejable que se encuentre en el objeto correspondiente, como el punto de referencia no tiene porqué coincidir con el centro geométrico real del objeto, lo denominaremos **centro de transformación**.

No hay que confundir el centro de transformación con el cursor 3D, que es un punto imaginario de blender en el que se llevarán las acciones del programa por defecto, por ejemplo al añadir un nueva malla se añaden en la posición del Cursor 3D.



## Instalación, requisitos y configuración

**Ejercicio**
>1.- Crear una nueva escena en blender: **Archivo->Nueva->General**
2.- Desplazar el cubo: **Pulsar G -> desplazar con el ratón**
3.- Comprobar como se ha desplazado el **centro de transformación**
4.- Ver los elementos constituyentes: **Pulsar Tabulador**
5.- Utilizar el Gizmo de rotación: Parte superior derecha con los ejes dibujados. Pulsar y desplazar.
6.- Desplazar todos los vértices: **Pulsar G -> Desplazar**
7.- Comprobar como no se ha desplazado el **centro de transformación**


## El interfaz
## Espacios de trabajo y visores
## Navegación en el entorno 3D
## Modos de vista del visor 3D
## Selección de objetos
## Introducción a la transformación de objetos
## Creación de nuevos objetos
## Grabación del fichero y copias de seguridad