La idea detrás de cualquier sistema Exceso es la de desplazar las cadenas en bloque, con respecto a un sistema BSS(n). Como ejemplo, veamos la siguiente figura:

!["comparación"](https://raw.githubusercontent.com/Orga-UNQ/mumuki-guia-text-sistema-exceso/master/images/compracionbss3-exceso.png "comparación")

En el segundo sistema, las cadenas tienen el mismo orden que el primero pero estan desplazadas 4 lugares hacia la izquierda. Esto permite representar números negativos, siendo el rango de este sistema: ```[-4 a 3]```

### Para representar un valor 

Pensemos en un mecanismo para representar valores, siempre con la idea de reusar la representación en BSS. Sabemos que Rbss "sabe" representar números solamente positivos, así que primero deben "adaptarse" el valor a un correpondiente positivo. Por ejemplo, consideremos el sistema del gráfico anterior y pensemos como representar el valor **-1**. Este valor se corresponde con el 3, ya que la cadena que los representa (en dos sistemas distintos) es la misma: **011**. 

Pasemos en limpio 2 pasos:

1. Desplazar el -1 al 3, sumándole el delta (que es 4)
2. Calcular ***Rbss(3)=011***


Veamos otro caso: representar el -2


1. Desplazar el valor: **-2+4=2**
2. Calcular ***Rbss(2)=010***

¿Cómo comprobar lo anterior? Si! Interpretando!

### Para interpretar una cadena

Combinemos, para esto, dos herramientas conocidas: 

* La interpretación en BSS (Ibss)
* La dualidad entre la representación y la interpretación: si para representar se suma, entonces para interpretar... se resta!

Entonces definamos dos pasos para interpretar una cadena, por ejemplo **011**

1. interpretar: I(011) = 3
2. desplazar: 3-4=**-1**


### Poniendo en práctica

¿Cual es la cadena que representa el valor -2 en el sistema Exceso(4, 8)?