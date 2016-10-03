La idea detrás de cualquier sistema Exceso es la de desplazar las cadenas en bloque, con respecto a un sistema BSS(n). Como ejemplo, veamos la siguiente figura:

!["comparación"](https://raw.githubusercontent.com/Orga-UNQ/mumuki-guia-text-sistema-exceso/master/images/compracionbss3-exceso.png "comparación")

En el segundo sistema, las cadenas tienen el mismo orden que el primero pero estan desplazadas 4 lugares hacia la izquierda. Esto permite representar números negativos, siendo el rango de este sistema: ```[-4 a 3]```

### Para representar un valor 

Pensemos en un mecanismo para representar valores.