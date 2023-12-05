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

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/6ff0fb88-a761-41ea-951f-204d7cfe966c)


## Clase Anónima
Son clases que **se crean para ser usadas solo 1 vez**

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/6e2105d4-a2cc-4250-a231-583d5f47e38a)

Las clases anónimas es una clase **sin nombre** y que hereda de la clase abstracta que "queremos instanciar"

**Interfaz con 1 único método = Interfaz funcional = Lambda**

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/337bdb1f-b329-495a-8370-1b592389c017)

Pero si tiene 1 argumento el método del interfase:

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/32cb5abd-d458-4b88-8968-e3cb54ae9647)

Lo implementamos así (en la parte de abajo es cómo se implementaría con lambda):

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/93a4e26d-c55b-4230-9cf0-2a3ab5ddf04e)

Ahora con 2 argumentos en el método del interfase:

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/3f2eaf16-3a9b-488c-8854-ce3104ccbb25)

Lo implementamos así (en la parte de abajo es cómo se implementaría con lambda):

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/bcd8a77f-2b6e-4acd-b345-c8e58e7d563c)

Si la clase anónima tiene 2 o más lineas de código, encerramos entre llaves:

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/846bf20a-12fe-4952-91ee-66430210cf36)

**Solu Stuardo problema con clase Estudiante (ERROR)**
![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/97f23dbf-af3b-459a-a6c5-ef902d9a66cb)

## Lambda
**Anónimo** porque no tiene nombre como un método normal
**Función** lista de parámetros, cuerpo, tipo de retorno, excepciones (como un método normal)


## Practica

Creamos interfazFinal;

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/bf9f3c1b-da6b-493b-b6fc-2e87ab4476c8)

Asignamos método del estudiante:

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/31a033df-2111-47ab-a904-03592a0bee00)

Implementamos el lambda: (Un ejemplo est arriba)

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/14e01ff4-dd7a-4f04-a010-ea0d7d53ed39)

Si pongo con llaves el rerturn del lambda no es implícito, **COLOCAMOS return** y un ";" al final

![image](https://github.com/SergioABS0813/CLASE-IWEB-14/assets/134556600/164b5fb1-23e9-4cae-91bb-d6ee9b28b7bf)




