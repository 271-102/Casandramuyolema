# Casandramuyolema
Arreglos Multidimensionales
 def ordenar_fila(matriz, fila):
        """Ordena una fila específica de la matriz en orden ascendente."""
        for i in range(len(matriz[fila])):
            for j in range(0, len(matriz[fila]) - i - 1):
                if matriz[fila][j] > matriz[fila][j + 1]:
                    # Intercambiar los elementos si están en el orden incorrecto
                    matriz[fila][j], matriz[fila][j + 1] = matriz[fila][j + 1], matriz[fila][j]


    # Crear una matriz 3x3
    matriz = [
        [9, 7, 5],
        [8, 2, 6],
        [3, 1, 4]
    ]

    # Mostrar la matriz original
    print("Matriz original:")
    for fila in matriz:
        print(fila)

    # Ordenar la fila 1 (índice 0)
    ordenar_fila(matriz, 0)

    # Mostrar la matriz después de la ordenación
    print("\nMatriz después de ordenar la fila 1:")
    for fila in matriz:
        print(fila)
