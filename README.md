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
