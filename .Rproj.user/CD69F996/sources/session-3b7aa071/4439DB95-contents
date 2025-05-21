# Exercicis de funcions

#Funció per comprovar si un nombre és primer:

esPrimer<-function(nombre){
  
  if (nombre <= 1) {
    print("El nombre NO ÉS primer")
    return(FALSE)
  }
  
  for(i in 2:sqrt(nombre)){
    if(nombre %% i == 0){
      print("El nombre NO ÉS primer")
      return(FALSE)
    } else {
      print("El nombre ÉS primer")
      return(TRUE)
    }
  }
}

esPrimer(13)

#Funció recursiva del càlcul de factorial:

factorialRecursiu<- function(nombre) {
  if(nombre <= 1) {
    return(1)
  } else {
    return(nombre * factorialRecursiu(nombre-1))
  }
}

resultatFactorial <- factorialRecursiu(5)
print(paste("El factorial és", resultatFactorial))


# Funció per veure si dos nombres són amics:

sumaDivisors<-function(nombre){
  divisors<-c()
  for(i in 1:(nombre-1)){
    if(nombre %% i == 0){
      divisors<-c(divisors, i)
    }
  }
  return(sum(divisors))
}

nombresAmics<-function(n1, n2){
  divisors_n1<-sumaDivisors(n1)
  divisors_n2<-sumaDivisors(n2)
  if(divisors_n1 == n2 && divisors_n2 == n1){
    print(paste(n1, " i ", n2, " són amics"))
  }
  else{
    print(paste(n1, " i ", n2, " NO són amics"))
  }
}
nombresAmics(220, 284)


#Funció per veure si un nombre és perfecte:

nombrePerfecte <- function(nombre){
  if(sumaDivisors(nombre)==nombre){
    print(paste("El nombre ", nombre, " és perfecte"))
  } else {
    print(paste("El nombre ", nombre, " NO és perfecte"))
  }
}

nombrePerfecte(6)
