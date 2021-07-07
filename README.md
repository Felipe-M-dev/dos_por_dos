# Desafío Opcional - Dos por dos

Crear el programa ```dos_por_dos.rb``` que dibuje el siguiente patrón de asteriscos y puntos intercalando hasta ```n```. Donde ```n``` es un valor ingresado por el usuario al momento de ejecutar el script.

ruby dos_por_dos.rb 5

    **..*

ruby dos_por_dos.rb 6

    **..**
     

Siempre hay que partir estudiando la solución. En este caso el patrón se repite cada 4 caracteres

caracter 1 y 2 => \*<br>
caracter 3 y 4 => .

Para resolver este tipo de patrones podemos ocupar nuevamente la operación resto (o módulo) y como el patrón se repite cada 4 caracteres entonces utilizaremos el resto de 4.

    i   i%4
    
    0   0
    1   1
    2   2
    3   3
    4   0
    5   1
    6   2
    7   3
    8   0
    9   1
    10  2
    11  3
    12  0

- Si i%4 es 0 o 1 mostraremos un \*
- En otro caso mostraremos un .
