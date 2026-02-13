Algoritmo SegundoMayorYSegundoMenor

    Definir arreglo Como Entero
    Definir i, mayor, segMayor, menor, segMenor Como Entero

    Leer arreglo

    mayor <- -infinito
    segMayor <- -infinito
    menor <- infinito
    segMenor <- infinito

    Para i <- 0 Hasta longitud(arreglo)-1 Hacer

        num <- arreglo[i]

        // Actualizar mayor y segundo mayor
        Si num > mayor Entonces
            segMayor <- mayor
            mayor <- num
        SinoSi num > segMayor Y num <> mayor Entonces
            segMayor <- num
        FinSi

        // Actualizar menor y segundo menor
        Si num < menor Entonces
            segMenor <- menor
            menor <- num
        SinoSi num < segMenor Y num <> menor Entonces
            segMenor <- num
        FinSi

    FinPara

    Escribir "Segundo mayor: ", segMayor
    Escribir "Segundo menor: ", segMenor

FinAlgoritmo
