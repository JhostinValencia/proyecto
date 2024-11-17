# Calculadora básica en Python

def suma(a, b):
  return a + b

def resta(a, b):
  return a - b

def multiplicacion(a, b):
  return a * b

def division(a, b):
  if b == 0:
    return "Error: División por cero"
  return a / b

print("Calculadora básica")
print("1. Suma")
print("2. Resta")
print("3. Multiplicación")
print("4. División")

opcion = input("Ingrese una opción: ")

if opcion == "1":
  a = float(input("Ingrese el primer número: "))
  b = float(input("Ingrese el segundo número: "))
  print("Resultado:", suma(a, b))
elif opcion == "2":
  a = float(input("Ingrese el primer número: "))
  b = float(input("Ingrese el segundo número: "))
  print("Resultado:", resta(a, b))
elif opcion == "3":
  a = float(input("Ingrese el primer número: "))
  b = float(input("Ingrese el segundo número: "))
  print("Resultado:", multiplicacion(a, b))
elif opcion == "4":
  a = float(input("Ingrese el primer número: "))
  b = float(input("Ingrese el segundo número: "))
  print("Resultado:", division(a, b))
else:
  print("Opción inválida")
// Conversor de unidades en Java

import java.util.Scanner;

public class ConversorDeUnidades {
  public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);
    System.out.println("Conversor de unidades");
    System.out.println("1. Celsius a Fahrenheit");
    System.out.println("2. Fahrenheit a Celsius");
    System.out.println("3. Kilómetros a millas");
    System.out.println("4. Millas a kilómetros");
    int opcion = scanner.nextInt();
    if (opcion == 1) {
      double celsius = scanner.nextDouble();
      double fahrenheit = celsius * 9 / 5 + 32;
      System.out.println("Resultado: " + fahrenheit + "°F");
    } else if (opcion == 2) {
      double fahrenheit = scanner.nextDouble();
      double celsius = (fahrenheit - 32) * 5 / 9;
      System.out.println("Resultado: " + celsius + "°C");
    } else if (opcion == 3) {
      double kilometros = scanner.nextDouble();
      double millas = kilometros * 0.621371;
      System.out.println("Resultado: " + millas + " millas");
    } else if (opcion == 4) {
      double millas = scanner.nextDouble();
      double kilometros = millas * 1.60934;
      System.out.println("Resultado: " + kilometros + " kilómetros");
    } else {
      System.out.println("Opción inválida");
    }
  }
}
