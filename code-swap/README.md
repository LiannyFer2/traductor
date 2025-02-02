**Resumen**

Esta es una herramienta diseñada para traducir código entre los lenguajes de programación Python y Java, dirigida especialmente a estudiantes de primeros semestres de ciencias de la computación. Su propósito principal es facilitar el aprendizaje y uso de estos lenguajes, centrándose en algoritmos básicos que incluyan ciclos basicos (Ejemplo: for, if, while). La aplicación permite a los usuarios ingresar código en uno de los lenguajes y obtener una traducción precisa al otro, simplificando así la comprensión y conversión de sintaxis y estructuras, sin abordar grados de complejidad avanzados.

**Justificación**

La necesidad surge de las dificultades comunes que enfrentan los estudiantes de primeros semestres de ciencias de la computación al trabajar con múltiples lenguajes de programación. Traducir código manualmente entre Python y Java no solo es tedioso, sino que también aumenta el riesgo de errores, lo que puede ralentizar el proceso de aprendizaje. Al automatizar la traducción de código,este programa ofrece una solución eficiente y confiable, permitiendo a los estudiantes concentrarse en entender la lógica y estructura subyacente en lugar de preocuparse por los detalles sintácticos.

Además, la escalabilidad del proyecto justifica su desarrollo continuo. La inclusión futura de más lenguajes de programación ampliará su alcance y utilidad, convirtiéndola en una herramienta integral para la comunidad de estudiantes de ciencias de la computación. Funcionalidades adicionales como la detección de errores y las sugerencias de optimización incrementarán su valor educativo, ayudando a los usuarios a mejorar no solo en la traducción, sino también en la calidad del código que escriben. En resumen, esto no solo responde a una necesidad actual, sino que también se posiciona como una herramienta versátil y de largo plazo para el aprendizaje y la programación eficiente en los primeros semestres de ciencias de la computación.

**Pasos para ejecutarlo**

1. Ingresar al repositorio de GitHub y descargar el archivo .zip, hacer clic en "Code" y luego en "Download ZIP".
2. Extraer el archivo descargado.
3. Abrir Visual Studio Code.
4. Hacer clic en "File" y luego en "Open Folder".
5. Seleccionar la carpeta extraída.
6. Abrir el archivo "app.py".
(Es importante tener instalado Flask; para instalar Flask, abrir la terminal y ejecutar el comando “pip install flask”, y tener un intérprete de Python configurado).
7. Hacer clic en el botón de ejecutar (ubicado en la parte superior derecha de la ventana).
8. Se generará un enlace http; copiar el enlace, abrir un navegador y pegar el enlace.
Siguiendo estos pasos, el programa se ejecutará correctamente.

**Funciones del Programa**

Traducción de Código: La función principal es traducir código entre Python y Java, enfocándose en algoritmos básicos que incluyan ciclos basicos. Esto facilita la comprensión y el aprendizaje de ambas sintaxis para estudiantes de primeros semestres de ciencias de la computación.

Interfaz de Usuario Intuitiva: el programa cuenta con una interfaz de usuario fácil de usar que permite a los estudiantes ingresar su código y obtener resultados rápidamente. La interfaz está diseñada para ser accesible incluso para aquellos con poca experiencia en programación, proporcionando una experiencia de usuario fluida y eficiente.


**Maneras de Escalar el Programa**

Incorporación de Más Lenguajes de Programación: Para escalar, se puede ampliar su capacidad para traducir entre más lenguajes de programación además de Python y Java. Añadir soporte para lenguajes como C++, JavaScript y Ruby aumentará su utilidad y atractivo, atrayendo a una base de usuarios más amplia y diversificada de estudiantes de ciencias de la computación en sus primeros semestres.

**Ejemplo de codigos que soporta**

Soporta ciclos anidados: 
Ejemplo: 
#Bucle for con range
print("Bucle for con range:")
for i in range(1, 6):
    print(i)

#Bucle while
print("\nBucle while:")
count = 0
while count < 5:
    print(count)
    count += 1

#Declaración if con condiciones anidadas
print("\nDeclaración if con condiciones anidadas:")
x = 10
if x > 5:
    print("x es mayor que 5")
    if x > 8:
        print("x también es mayor que 8")
else:
    print("x es menor o igual que 5")


Soporta ciclos anidados:
Ejemplo:

#Ciclos anidados
print("\nCiclos anidados:")
for i in range(1, 4):
    for j in range(1, 4):
        print(f"i: {i}, j: {j}")

Soporta el uso de estructuras lógicas como and, or y not.
Ejemplo: 

#Ejemplo de estructuras lógicas
x = 5
y = 10
z = 15

#Usando operador and
if x < y and y < z:
    print("x es menor que y y y es menor que z")

#Usando operador or
if x < y or x < z:
    print("x es menor que y o x es menor que z")

#Usando operador not
if not(x > y):
    print("x no es mayor que y")

Soporta ciclos con otros ciclos dentro.
Ejemplo, if dentro de un while:

#Ejemplo de bucle while con declaración if dentro
contador = 0

while contador < 5:
    if contador % 2 == 0:
        print(f"{contador} es par")
    else:
        print(f"{contador} es impar")
    
    contador += 1

EJEMPLO CODIGO PARA QUE PRUEBE:

def suma(a, b):
    return a + b

def resta(a, b):
    return a - b

def multiplicacion(a, b):
    return a * b

def division(a, b):
    if b != 0:
        return a / b
    else:
        return "Error: No se puede dividir por cero"

def calculadora():
    while True:
        print("\nBienvenido a la calculadora básica")
        print("Operaciones disponibles:")
        print("1. Suma")
        print("2. Resta")
        print("3. Multiplicación")
        print("4. División")
        print("5. Salir")
        
        opcion = input("Ingrese el número de la operación que desea realizar: ")
        
        if opcion == '5':
            print("Gracias por usar la calculadora. ¡Adiós!")
            break
        
        num1 = float(input("Ingrese el primer número: "))
        num2 = float(input("Ingrese el segundo número: "))
        
        if opcion == '1':
            resultado = suma(num1, num2)
            print(f"El resultado de la suma es: {resultado}")
        elif opcion == '2':
            resultado = resta(num1, num2)
            print(f"El resultado de la resta es: {resultado}")
        elif opcion == '3':
            resultado = multiplicacion(num1, num2)
            print(f"El resultado de la multiplicación es: {resultado}")
        elif opcion == '4':
            resultado = division(num1, num2)
            print(f"El resultado de la división es: {resultado}")
        else:
            print("Opción no válida. Intente nuevamente.")
        
        #Ciclo for para mostrar los resultados previos
        resultados = [suma(num1, num2), resta(num1, num2), multiplicacion(num1, num2), division(num1, num2)]
        print("\nResultados previos:")
        for i in range(len(resultados)):
            if i == 0:
                print(f"Suma: {resultados[i]}")
            elif i == 1:
                print(f"Resta: {resultados[i]}")
            elif i == 2:
                print(f"Multiplicación: {resultados[i]}")
            elif i == 3:
                print(f"División: {resultados[i]}")
        
        #Preguntar al usuario si desea realizar otra operación
        continuar = input("¿Desea realizar otra operación? (sí/no): ").strip().lower()
        if continuar != 'sí':
            print("Gracias por usar la calculadora. ¡Adiós!")
            break

#Ejecutar la calculadora
calculadora()



