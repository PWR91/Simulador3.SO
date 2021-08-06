# Simulador3.SO
## Sistemas Operativos

  Debe modificar el programa que crea el archivo .dat para crear también estructuras en memoria donde
guardará en hashmaps el numero consecutivo de cada jugador según:
- País
- Estatura
- Peso
- Edad
Luego, caundo termina de procesar los jugadores creando el archivo .dat, tendrá que guardar los
hashmaps (ver Main2). Cada hashmap en un archivo <>.idx (idx = index).

Por ejemplo, Lionel Messi generará las siguientes entradas:
País → Llave: Argentina, lista de valores: (0)
Estatura → Llave: 169 , lista de valores: (0)
Peso → Llave: 67, lista de valores: (0)
Edad → Llave: 27, lista de valores (0)

Si en el siguiente registro entrara un jugador con el mismo peso de Messi, los hashmaps quedarían así:
País → Llave: Argentina, lista de valores: (0)
Estatura → Llave: 169 , lista de valores: (0)
Peso → Llave: 67, lista de valores: (0,1)
Edad → Llave: 27, lista de valores (0)

De esta forma, cada valor particular en el hashmap será una llave y usted guardará la lista de registros
donde esta ese valor.

Ahora, deberá modificar el programa de consultas para que cuando busque una estatura, país, peso o
edad especifico EN LUGAR DE LEER REGISTRO POR REGISTRO y ver si tiene la estatura, peso, país o demás
datos solicitados, usted abre el archivo de indexes correspondiente y saca la lista de registros. 
Luego lee  1 x 1 y solo TOMA EN CUENTA LOS QUE APARECEN EN DICHA LISTA.

Hecho esto, compare cuanto tiempo le tomó leer la lista y ponerla en memoria ANTES DE IMPRIMIRLA.
COMPARE LOS TIEMPOS ENTRE USAR Y NO USAR ÍNDICES. 
