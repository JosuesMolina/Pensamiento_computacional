# obtener calificaciones del periodo 
Algoritmo getPromedioCalificaciones
	Definir numCalificaciones Como Entero
	numCalificaciones <- 1
	Definir promedio Como Real
	Escribir "Escribe el numero de calificaciones del periodo"
	leer numCalificaciones 
	Dimension calificacion[numCalificaciones]

	para i <- 1 hasta numCalificaciones con paso 1 haces 
		Escribir  "Escribe tu calificacion #", i
		leer calificacion[i]
		Si calificacion[i] > 10 y calificacion[i] < 5 Entonces
			Escribir "Debes escribir una calificacion mayor a 4 y menor a 11 "
			Escribir  "Escribe tu calificacion #", i
			leer calificacion[i]
		Fin Si
	FinPara
	
	para i <- 1 Hasta  numCalificaciones Con Paso 1 haces
		promedio = promedio + calificacion[i]
	FinPara
	promedio <- (promedio)/numCalificaciones
	Mostrar  "Tu promedio del periodo es de:", promedio
	
FinAlgoritmo
