# Ordenamiento por Selecci�n 
El ordenamiento por selecci�n es un algoritmo de ordenamiento que requiere O(n^2) operaciones para ordenar una lista de n elementos.

Su funcionamiento es el siguiente:

 1. Seleccionar el primer numero
 2. Buscar el numero menor en el resto del arreglo
 3. Si el numero encontrado es menor que el primer numero se intercambian
 4. Seleccionamos el segundo numero y se repite el proceso

####Pseudocodigo
```
    para i=1 hasta n-1
      aux =A[i]
      para j=i+1 hasta n
        si A[j] < aux entonces
          aux2=j
          aux=A[j]
        fin si
      fin para
      si A[aux2]<A[i] entonces
        aux=A[i]
        A[i]= A[aux2]
        A[aux2]=aux
      fin si
    fin para
```    
######Tiempo de ejecucion
![GitHub Logo](http://www.wiris.net/demo/editor/render.png?demo-image&mml=%3Cmath%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F1998%2FMath%2FMathML%22%3E%3Cmi%3Ec%3C%2Fmi%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmi%3En%3C%2Fmi%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmi%3Ec%3C%2Fmi%3E%3Cmn%3E2%3C%2Fmn%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmi%3Ec%3C%2Fmi%3E%3Cmn%3E3%3C%2Fmn%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmunderover%3E%3Cmo%3E%26%238721%3B%3C%2Fmo%3E%3Cmrow%3E%3Cmi%3Ej%3C%2Fmi%3E%3Cmo%3E%3D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmrow%3E%3Cmrow%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmrow%3E%3C%2Fmunderover%3E%3Cmi%3Ej%3C%2Fmi%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmi%3Ec%3C%2Fmi%3E%3Cmn%3E4%3C%2Fmn%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmunderover%3E%3Cmo%3E%26%238721%3B%3C%2Fmo%3E%3Cmrow%3E%3Cmi%3Ej%3C%2Fmi%3E%3Cmo%3E%3D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmrow%3E%3Cmrow%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmrow%3E%3C%2Fmunderover%3E%3Cmi%3Ej%3C%2Fmi%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmi%3Ec%3C%2Fmi%3E%3Cmn%3E5%3C%2Fmn%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmunderover%3E%3Cmo%3E%26%238721%3B%3C%2Fmo%3E%3Cmrow%3E%3Cmi%3Ej%3C%2Fmi%3E%3Cmo%3E%3D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmrow%3E%3Cmrow%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmrow%3E%3C%2Fmunderover%3E%3Cmi%3Ej%3C%2Fmi%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmi%3Ec%3C%2Fmi%3E%3Cmn%3E6%3C%2Fmn%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmunderover%3E%3Cmo%3E%26%238721%3B%3C%2Fmo%3E%3Cmrow%3E%3Cmi%3Ej%3C%2Fmi%3E%3Cmo%3E%3D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmrow%3E%3Cmrow%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3C%2Fmrow%3E%3C%2Fmunderover%3E%3Cmi%3Ej%3C%2Fmi%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmi%3Ec%3C%2Fmi%3E%3Cmn%3E7%3C%2Fmn%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmi%3Ec%3C%2Fmi%3E%3Cmn%3E8%3C%2Fmn%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmi%3Ec%3C%2Fmi%3E%3Cmn%3E9%3C%2Fmn%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmi%3Ec%3C%2Fmi%3E%3Cmn%3E10%3C%2Fmn%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%2B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmn%3E5%3C%2Fmn%3E%3Cmo%3E%28%3C%2Fmo%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmo%3E%29%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%2B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmfrac%3E%3Cmrow%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%28%3C%2Fmo%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%2B%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmo%3E%29%3C%2Fmo%3E%3C%2Fmrow%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmfrac%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%2B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmn%3E3%3C%2Fmn%3E%3Cmfrac%3E%3Cmrow%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%28%3C%2Fmo%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmo%3E%29%3C%2Fmo%3E%3C%2Fmrow%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmfrac%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%2B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmn%3E5%3C%2Fmn%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmn%3E5%3C%2Fmn%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%2B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmfrac%3E%3Cmsup%3E%3Cmi%3En%3C%2Fmi%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmsup%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmfrac%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%2B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmfrac%3E%3Cmi%3En%3C%2Fmi%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmfrac%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E1%3C%2Fmn%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%2B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmfrac%3E%3Cmrow%3E%3Cmn%3E3%3C%2Fmn%3E%3Cmsup%3E%3Cmi%3En%3C%2Fmi%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmsup%3E%3C%2Fmrow%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmfrac%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmfrac%3E%3Cmrow%3E%3Cmn%3E3%3C%2Fmn%3E%3Cmi%3En%3C%2Fmi%3E%3C%2Fmrow%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmfrac%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmn%3E2%3C%2Fmn%3E%3Cmsup%3E%3Cmi%3En%3C%2Fmi%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmsup%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%2B%3C%2Fmo%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmn%3E5%3C%2Fmn%3E%3Cmi%3En%3C%2Fmi%3E%3Cmo%3E%26%23160%3B%3C%2Fmo%3E%3Cmo%3E%2D%3C%2Fmo%3E%3Cmn%3E6%3C%2Fmn%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3Cmi%3EO%3C%2Fmi%3E%3Cmo%3E%28%3C%2Fmo%3E%3Cmsup%3E%3Cmi%3En%3C%2Fmi%3E%3Cmn%3E2%3C%2Fmn%3E%3C%2Fmsup%3E%3Cmo%3E%29%3C%2Fmo%3E%3Cmspace%20linebreak%3D%22newline%22%2F%3E%3C%2Fmath%3E)

####Codigo en Scala
```scala
object SelectionSort{
  def main(args: Array[String]) {
  var A = Array(25, 2, 13, 89, 6)
  var aux = 0
  var aux2=  0
  for(i <- 0 to A.length - 2) {
    aux = A(i)
    for(j <- i+1 to A.length - 1) {
      if(aux > A(j)) {
        aux2 = j
        aux = A(j)
      }
    }
    if(A(aux2) < A(i)) {
      aux = A(i)
      A(i) = A(aux2)
     A(aux2) = aux
    }
  }
  for(i <- 0 to A.length-1) {
    println(A(i))
  }
 }
}
```
