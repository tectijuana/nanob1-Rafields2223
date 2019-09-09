
## definicion de problemas de computo 
En  [ciencia computacional teórica](https://es.wikipedia.org/wiki/Ciencia_computacional_te%C3%B3rica "Ciencia computacional teórica"), un  **problema abstracto**  o  **problema computacional**  es una  [relación](https://es.wikipedia.org/wiki/Relaci%C3%B3n_binaria "Relación binaria")  entre un conjunto de  _instancias_  y un conjunto de  _soluciones_. Un problema abstracto permite establecer formalmente la relación deseada entre la entrada de un algoritmo y su salida. Una  **solución algorítmica**  a un problema abstracto consiste de un algoritmo que por cada instancia del problema calcula al menos una solución correspondiente –en caso de haberla– o expide un certificado de que no existe solución alguna. Un problema abstracto se convierte en un  **problema concreto**  cuando las instancias y soluciones están codificadas en forma de  [lenguajes formales](https://es.wikipedia.org/wiki/Lenguaje_formal "Lenguaje formal").

Los problemas abstractos suelen definirse en dos partes: en la primera se describe al conjunto de instancias y en la segunda se describe la solución esperada para cada instancia. Por ejemplo, el problema de ordenación de números enteros se suele definir como sigue:

**Instancia:**  Una sucesión finita de números enteros  {\displaystyle \left(a_{1},a_{2},\ldots ,a_{n}\right)}![{\displaystyle \left(a_{1},a_{2},\ldots ,a_{n}\right)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/0d990d6fff8ca170ddf11535f0c5562b882e2c3f)

**Solución:**  Una permutación  {\displaystyle \left(a_{1}^{\prime },a_{2}^{\prime },\ldots ,a_{n}^{\prime }\right)}![{\displaystyle \left(a_{1}^{\prime },a_{2}^{\prime },\ldots ,a_{n}^{\prime }\right)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/5a3446f7e725a0d342e8910eee791575bcd4f072)  de la sucesión de entrada tal que  {\displaystyle a_{1}^{\prime }\leq a_{2}^{\prime }\leq \cdots \leq a_{n}^{\prime }}![{\displaystyle a_{1}^{\prime }\leq a_{2}^{\prime }\leq \cdots \leq a_{n}^{\prime }}](https://wikimedia.org/api/rest_v1/media/math/render/svg/943e9dc2b1448df1374175347123cfd625ddf217)

Aquí tanto el conjunto de instancias y el de soluciones es el mismo, pues se trata del conjunto de todas las sucesiones finitas de números enteros. La relación que hay entre ellos asigna a cada sucesión  {\displaystyle \left(a_{1},a_{2},\ldots ,a_{n}\right)}![{\displaystyle \left(a_{1},a_{2},\ldots ,a_{n}\right)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/0d990d6fff8ca170ddf11535f0c5562b882e2c3f)  la única permutación  {\displaystyle \left(a_{1}^{\prime },a_{2}^{\prime },\ldots ,a_{n}^{\prime }\right)}![{\displaystyle \left(a_{1}^{\prime },a_{2}^{\prime },\ldots ,a_{n}^{\prime }\right)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/5a3446f7e725a0d342e8910eee791575bcd4f072)  tal que  {\displaystyle a_{1}^{\prime }\leq a_{2}^{\prime }\leq \cdots \leq a_{n}^{\prime }}![{\displaystyle a_{1}^{\prime }\leq a_{2}^{\prime }\leq \cdots \leq a_{n}^{\prime }}](https://wikimedia.org/api/rest_v1/media/math/render/svg/943e9dc2b1448df1374175347123cfd625ddf217). Por ejemplo,  {\displaystyle \left(6,9,4,5\right)}![{\displaystyle \left(6,9,4,5\right)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/43fb79763f7d47dc34f79d3bbb984568849e73ba)  tiene como solución a  {\displaystyle \left(4,5,6,9\right)}![{\displaystyle \left(4,5,6,9\right)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/5c1ff8f8fc969068bdd4a15e4363ef4a157fd9b4). Una solución algorítmica al problema de ordenamiento es el  [ordenamiento de burbuja](https://es.wikipedia.org/wiki/Ordenamiento_de_burbuja "Ordenamiento de burbuja")  porque este algoritmo produce una solución como salida cada vez que se le suministra una instancia como entrada.

## Tipos de problemas computacionales[[editar](https://es.wikipedia.org/w/index.php?title=Problema_computacional&action=edit&section=1 "Editar sección: Tipos de problemas computacionales")]

Artículo principal:  _[Problema de decisión](https://es.wikipedia.org/wiki/Problema_de_decisi%C3%B3n "Problema de decisión")_

En un  **problema de decisión**  cada instancia tiene asociada exactamente una solución "_sí_" o "_no_". Los problemas de decisión quedan completamente determinados por el conjunto  {\displaystyle Y}![Y](https://wikimedia.org/api/rest_v1/media/math/render/svg/961d67d6b454b4df2301ac571808a3538b3a6d3f)  de instancias que tienen asociada la solución "_sí_". Por ejemplo, el problema de decidir si una gráfica tiene o no un  [ciclo Hamiltoniano](https://es.wikipedia.org/wiki/Camino_hamiltoniano "Camino hamiltoniano")  queda completamente determinado su conjunto de soluciones "_sí_":

> {\displaystyle \mathrm {HAM} =\left\{G\mid G{\text{ es una gráfica hamiltoniana}}\right\}}![{\displaystyle \mathrm {HAM} =\left\{G\mid G{\text{ es una gráfica hamiltoniana}}\right\}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/8a68cc3bccf17420b43068ef6ee719aa475f9add)

Con esta representación el problema equivale a preguntar si una instancia  {\displaystyle i}![i](https://wikimedia.org/api/rest_v1/media/math/render/svg/add78d8608ad86e54951b8c8bd6c8d8416533d20)  pertenece o no al conjunto  {\displaystyle \mathrm {HAM} }![{\displaystyle \mathrm {HAM} }](https://wikimedia.org/api/rest_v1/media/math/render/svg/f912e25e8362df9746d9ce74f2dccd8c9b50aff6). En general, los problemas de decisión siempre equivalen a decidir la proposición  {\displaystyle i\in Y}![{\displaystyle i\in Y}](https://wikimedia.org/api/rest_v1/media/math/render/svg/a6d05f69e90065642a0c661cdbe4022040d5f9ee)  donde  {\displaystyle Y}![Y](https://wikimedia.org/api/rest_v1/media/math/render/svg/961d67d6b454b4df2301ac571808a3538b3a6d3f)  es el conjunto de instancias con solución "_sí_". Una solución algorítmica para un problema de decisión es un algoritmo que calcula la función característica de  {\displaystyle Y}![Y](https://wikimedia.org/api/rest_v1/media/math/render/svg/961d67d6b454b4df2301ac571808a3538b3a6d3f)  o equivalente:

> {\displaystyle \chi _{Y}(i)={\begin{cases}1&{\text{si }}i\in Y\\0&{\text{si }}i\notin Y\end{cases}}}![{\displaystyle \chi _{Y}(i)={\begin{cases}1&{\text{si }}i\in Y\\0&{\text{si }}i\notin Y\end{cases}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/31dd6fcffa43e657f94bb646a6c0d815fbd2e41c)

En los  **problemas de búsqueda**  la relación entre el conjunto de instancias y el de soluciones queda determinado por un  [predicado lógico](https://es.wikipedia.org/wiki/L%C3%B3gica_de_primer_orden "Lógica de primer orden")  {\displaystyle P(i,s)}![{\displaystyle P(i,s)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/8fad3af9139aa1dcb13b227cc96f03eae066281d)  que determina si  {\displaystyle s}![s](https://wikimedia.org/api/rest_v1/media/math/render/svg/01d131dfd7673938b947072a13a9744fe997e632)  es una solución de  {\displaystyle i}![i](https://wikimedia.org/api/rest_v1/media/math/render/svg/add78d8608ad86e54951b8c8bd6c8d8416533d20). Dada una instancia  {\displaystyle i}![i](https://wikimedia.org/api/rest_v1/media/math/render/svg/add78d8608ad86e54951b8c8bd6c8d8416533d20)  el problema consiste en encontrar, si es que existe, una solución  {\displaystyle s}![s](https://wikimedia.org/api/rest_v1/media/math/render/svg/01d131dfd7673938b947072a13a9744fe997e632)  de  {\displaystyle i}![i](https://wikimedia.org/api/rest_v1/media/math/render/svg/add78d8608ad86e54951b8c8bd6c8d8416533d20). Es decir, buscar el elemento  {\displaystyle s}![s](https://wikimedia.org/api/rest_v1/media/math/render/svg/01d131dfd7673938b947072a13a9744fe997e632)  que haga verdadera la proposición  {\displaystyle \exists s\in S.P(i,s)}![{\displaystyle \exists s\in S.P(i,s)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/f5da537204da5c39fe4e78ffad39652b9a788617). Cuando se fija el valor de  {\displaystyle i}![i](https://wikimedia.org/api/rest_v1/media/math/render/svg/add78d8608ad86e54951b8c8bd6c8d8416533d20)  y la solución es única, se dice que es un  _[problema matemático](https://es.wikipedia.org/wiki/Problema_matem%C3%A1tico "Problema matemático")_. Por ejemplo, el problema de  [factorización](https://es.wikipedia.org/wiki/Factorizaci%C3%B3n "Factorización")  de un número entero  {\displaystyle n}![n](https://wikimedia.org/api/rest_v1/media/math/render/svg/a601995d55609f2d9f5e233e36fbe9ea26011b3b)  consiste en encontrar un factor no trivial de  {\displaystyle n}![n](https://wikimedia.org/api/rest_v1/media/math/render/svg/a601995d55609f2d9f5e233e36fbe9ea26011b3b); es decir, número entero  {\displaystyle m}![m](https://wikimedia.org/api/rest_v1/media/math/render/svg/0a07d98bb302f3856cbabc47b2b9016692e3f7bc)  diferente de 1 y de  {\displaystyle n}![n](https://wikimedia.org/api/rest_v1/media/math/render/svg/a601995d55609f2d9f5e233e36fbe9ea26011b3b)  tal que  {\displaystyle m}![m](https://wikimedia.org/api/rest_v1/media/math/render/svg/0a07d98bb302f3856cbabc47b2b9016692e3f7bc)  [divida exactamente](https://es.wikipedia.org/wiki/Divisibilidad "Divisibilidad")  a  {\displaystyle n}![n](https://wikimedia.org/api/rest_v1/media/math/render/svg/a601995d55609f2d9f5e233e36fbe9ea26011b3b). En símbolos

> {\displaystyle \exists m\in \mathbf {Z} .m\neq 1\wedge m\neq n\wedge {\frac {n}{m}}\in \mathbf {Z} }![{\displaystyle \exists m\in \mathbf {Z} .m\neq 1\wedge m\neq n\wedge {\frac {n}{m}}\in \mathbf {Z} }](https://wikimedia.org/api/rest_v1/media/math/render/svg/418220decf413fce088d6e8574e84d6ba550598b)

Esta fórmula simplemente está preguntando la existencia de un factor no trivial de  {\displaystyle n}![n](https://wikimedia.org/api/rest_v1/media/math/render/svg/a601995d55609f2d9f5e233e36fbe9ea26011b3b). Una solución algorítmica a un problema de búsqueda viene dador por un algoritmo  {\displaystyle f}![f](https://wikimedia.org/api/rest_v1/media/math/render/svg/132e57acb643253e7810ee9702d9581f159a1c61)  tal que  {\displaystyle P\left(i,f(i)\right)}![{\displaystyle P\left(i,f(i)\right)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/0efa6055ac5f75ec5994aa61614bb302c2947dc8)  es verdadera siempre y cuando exista solución para  {\displaystyle i}![i](https://wikimedia.org/api/rest_v1/media/math/render/svg/add78d8608ad86e54951b8c8bd6c8d8416533d20), es decir,  {\displaystyle f}![f](https://wikimedia.org/api/rest_v1/media/math/render/svg/132e57acb643253e7810ee9702d9581f159a1c61)  siempre calcula una solución si es que esta existe. En el caso del problema de la factorización de enteros se cuenta con el algoritmo de la  [división por tentativa](https://es.wikipedia.org/wiki/Divisi%C3%B3n_por_tentativa "División por tentativa").


En un  **problema de optimización**  no solo se busca una solución, sino que se busca "_la mejor_" de todas. Cada problema de optimización puede concebirse como un problema de búsqueda y una función  {\displaystyle g}, comúnmente conocida como  _función objetivo_, que determina la calidad de las soluciones. El problema de optimización (que a su vez es de búsqueda) consiste en encontrar la solución maximice Por ejemplo, el  [problema del viajante]  no solamente exige determinar si una gráfica tiene o no un ciclo hamiltoniano, sino que además pregunta cuál es el ciclo hamiltoniano más corto. En este caso el problema de búsqueda subyacente es encontrar un ciclo hamiltoniano cualquiera y la función objetivo mide la distancia recorrida por ese ciclo.
## algoritmos cotidianos
**Algoritmo**. En  [Matemática] "Matemática"), ciencias de la  [Computación](https://www.ecured.cu/Computaci%C3%B3n "Computación")  y disciplinas relacionadas, un algoritmo (del latín, dixit algorithmus y éste a su vez del matemático persa  [Al Juarismi](https://www.ecured.cu/Al_Juarismi "Al Juarismi")) es un conjunto reescrito de instrucciones o reglas bien definidas, ordenadas y finitas que permite realizar una actividad mediante pasos sucesivos que no generen dudas a quien lo ejecute. Dados un estado inicial y una entrada, siguiendo los pasos sucesivos se llega a un estado final y se obtiene una solución. Los algoritmos son objeto de estudio de la algoritmia.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/b/bd/LampFlowchart-es.svg/220px-LampFlowchart-es.svg.png)
