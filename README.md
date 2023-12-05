# CLASE-IWEB-14
Filters, Lambda, Interfases

## Creamos Package Filters
Aqui iran los filtros que usemos

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/37156756-74fa-497d-a614-0fc6dd2d59a5)

## Creación de Filtros

Creamos la clase Filter2:

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/7bc3b474-2349-443d-8e29-7f3ee09a887d)

Implementamos el método doFilter (**debido a que estamos heredando de la clase Filter**) y tenemos un método abstracto llamado "doFilter":

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/9e79ac10-7ae2-4865-a101-b479448d6f3f)

OJO: FilterChain sirve para poder concatenar con otros filtros (**Sirve para avisar qué filtro es anterior o posterior en el que estamos**)

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/56b650d6-d16e-47d6-a538-8d44ab701c02)

Casteamos en Http Servlet: (porque doFilter no tiene Http)

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/98492cfc-a5d6-4d08-a1fa-2ff939050c24)

Creamos la lógica del filtro usando **filterChain siempre lleva al siguiente (sea filtro o no)**

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/0302610a-b7d1-454f-b99c-76261082733f)

**Escoger Servlets**: (filtro 1 es el filtro 2 solo que ya estaba trabajado por el Profe)

En esta parte colocamos los nombres de los servlets a los que se va a aplicar el filtro

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/309a2b49-f0bd-4042-a369-1439d7c17a4c)

**OJO: Si 2 filtros apuntan hacia un mismo servlet entonces la prioridad la tiene el mapeo por URL y luego por nombre**

## JAVA INTERFACES
Una interfase es un conjunto de métodos y clases abstractas

Creamos una clase Interface:

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/b9c98c62-b20b-4472-9ed8-a7d2bc333145)

Implementamos la interfase en la clase Estudiante:

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/74ce0ee6-3591-4b4d-97b3-0ab27e1847a0)

**Si la clase hereda o "implementa interfase" entonces esa clase se "vuelve" esa interfase**

Por eso, **mejor tomamos la opción de agregar una "clase intermedia"** que "implementa la interfase" y como esta se "convertirá" en la interfase, entonces ya podemos usar el método que recibia como parámetro la interfase.

## Clase Anónima









