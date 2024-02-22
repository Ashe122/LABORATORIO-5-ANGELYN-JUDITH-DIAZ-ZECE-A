
//Angelyn Judith Diaz zeceña 5090-23-1407

#include <iostream> //Es una biblioteca que sirve para las funciones basicas de entrada y salida de datos. 

using namespace std;

// Aqui se realiza la operacion de Suma de números pares e impares
int sumaParesImparesHastaN(int numero, bool sumarPares) {
    int suma = 0;
    for (int i = 1; i <= numero; i++) {
        // Comprueba si el número es par o impar según el numero que dió el usuario
        if ((i % 2 == 0 && sumarPares) || (i % 2 != 0 && !sumarPares)) {
            suma += i;  // Suma el número al resultado
        }
    }
    return suma;
}

// Aqui se realiza la operacion del Factorial con bucle while
int calcularFactorial(int numero) {
    int resultado = 1;
    cout << "El factorial de " << numero << " ("
         << numero << "!) se calcula como: ";
    // Calcula el factorial utilizando un bucle while
    while (numero > 1) {
        cout << numero << " × ";  // Muestra el paso del cálculo
        resultado *= numero;  // Multiplica el resultado por el número actual
        numero--;
    }
    cout << "1, que es igual a " << resultado << "." << endl;
    return resultado;
}

// Aqui se realiza el contador de dígitos
int contarDigitos(int numero) {
    int contador = 0;
    // Utiliza un bucle do-while para contar la cantidad de dígitos
    do {
        contador++;
        numero /= 10;
    } while (numero != 0);
    return contador;
}

// Aqui se realiza el Ordenamiento de números  de forma (ascendente)
void ordenarNumeros(int &a, int &b, int &c) {
    //  Aqui se ordenan tres números de menor a mayor sin utilizar los arrays
    if (a > b) {
        swap(a, b);
    }
    if (a > c) {
        swap(a, c);
    }
    if (b > c) {
        swap(b, c);
    }
}

// Aqui se realiza la Suma de dígitos de un número
int sumaDigitos(int numero) {
    int suma = 0;
    // Aqui se utiliza un bucle while para sumar los dígitos del número
    while (numero != 0) {
        suma += numero % 10;
        numero /= 10;
    }
    return suma;
}

int main() {// Declaración de variable para almacenar el número ingresado por el usuario
    int numero;

//  Aqui Solicita al usuario ingresar un número
    cout << "Ingrese un número: ";
    cin >> numero;

    //  Ejemplos de uso de las funciones definidas anteriormente
    cout << " Suma de pares hasta " << numero << ": " << sumaParesImparesHastaN(numero, true) << endl;
    cout << " Suma de impares hasta " << numero << ": " << sumaParesImparesHastaN(numero, false) << endl;

    calcularFactorial(numero); //  Aqui se Llama a la función para calcular y mostrar el factorial del número ingresado

    cout << " Contador de dígitos de " << numero << ": " << contarDigitos(numero) << endl;

    int num1, num2, num3; //Aqui se declaran tres variables enteras para almacenar los números ingresados por el usuario
    cout << "Ingrese tres números separados por espacios: ";
    cin >> num1 >> num2 >> num3;
    ordenarNumeros(num1, num2, num3); // en esta parte del codigo, se Llama a la función para ordenar los tres números de menor a mayor
    cout << "Numeros ordenados: " << num1 << ", " << num2 << ", " << num3 << endl;

    int numeroSumaDigitos; //Aqui tambien se declara una variable para almacenar el número ingresado por el usuario para la suma de dígitos
    cout << "Ingrese un número para sumar sus dígitos: ";
    cin >> numeroSumaDigitos;
    cout << "Suma de dígitos de " << numeroSumaDigitos << ": " << sumaDigitos(numeroSumaDigitos) << endl;

// Indica que el programa se ejecutó correctamente
    return 0; 
}