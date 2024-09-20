# practica-3-numeros
#mi programa de operaciones 
print ("Angel Andrey Muñoz Centeno: ")
#Esta es la operacion como variable
def suma(x, y):
    return x + y
#Esta es la operacion como variable
def resta(x, y):
    return x - y
#Esta es la operacion como variable
def multiplicacion(x, y):
    return x * y
#Esta es la operacion como variable
def division(x, y):
    if y == 0:
        return "Error: División por cero"
    return x / y
#Lo que se muestra a continuacion son las opciones que se le muestran al usuario
def main():
    print("Seleccione la operación:")
    print("1. Sumar")
    print("2. Restar")
    print("3. Multiplicar")
    print("4. Dividir")

    while True:
        opcion = input("Ingrese su opción (1/2/3/4): ")#Aqui el usuario ingresa Una de las variables

        if opcion in ['1', '2', '3', '4']:
            num1 = float(input("Ingrese el primer número: "))
            num2 = float(input("Ingrese el segundo número: "))

            if opcion == '1':
                print(f"{num1} + {num2} = {suma(num1, num2)}")
            elif opcion == '2':
                print(f"{num1} - {num2} = {resta(num1, num2)}")
            elif opcion == '3':
                print(f"{num1} * {num2} = {multiplicacion(num1, num2)}")
            elif opcion == '4':
                print(f"{num1} / {num2} = {division(num1, num2)}")
        else:
            print("Opción no válida. Intente de nuevo.")

        siguiente = input("¿Desea realizar otra operación? (s/n): ")
        if siguiente.lower() != 's':
            break
if __name__ == "__main__":
    main()
    ![image](https://github.com/user-attachments/assets/54260597-55ed-4380-a472-d004307d0c6c)
