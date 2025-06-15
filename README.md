# ciberseguridad
def adivina_numero():
    
    #El objetivo es que el jugador adivine un número secreto entre 1 y 20.
    
    print("¡Bienvenido al juego: Adivina el número del 1 al 20!")
      # Definimos las variables.
    num_secreto = 10
       # Inicializa el contador de intentos del jugador a cero.
    intentos = 0 
      #Es una bandera booleana que controla el bucle; es False mientras no se adivine.
    adivinado = False
       # Bucle principal del juego (Estructura Repetitiva) ---
       # El bucle 'while' se ejecuta mientras la variable 'adivinado' sea False.
       # Esto significa que el juego continúa hasta que el jugador adivina el número.
    while not adivinado:
       
          # Solicita al jugador que ingrese un número y lo convierte a un entero.
        intento = int(input("Ingresa un número entre 1 y 20: "))
          # Incrementa el contador de intentos después de cada entrada válida.
    intentos += 1
    # Estructuras Lógicas (Condicionales)
            # Valida si el número ingresado está dentro del rango permitido (1 a 20).
    if intento < 1 or intento > 20:
            print("Número fuera de rango.Por favor, ingresa un número entre 1 y 20.")
    elif intento == num_secreto:

            adivinado = True
    print(f"¡Felicidades! ¡Has adivinado el número {num_secreto} en {intentos} intentos!")            elif intento < num_secreto:
    print("El número secreto es mayor. ¡Intenta de nuevo!")
