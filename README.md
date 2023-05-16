# Script con Bucle Do While. 
## Ejercicio Base:

Java es en la actualidad uno de los lenguajes más demandados en el mercado por lo que los estudiantes de la Universitaria de Colombia deberán realizar una serie de ejercicio con el fin de que estos sirvan como base de su aprendizaje. Uno de ellos consiste en Pedir un número, comprobar si es primo y preguntar si quiere introducir uno o varios más, con el fin de poner en práctica lo aprendido en clases anteriores. 

### Aclaraciones:

- El ejercicio debe hacer uso del  bucle DO WHILE. 
- Como mínimo debe contener un ciclo FOR. }
- Como prioridad debes divertirte en el proceso 


### Descripción caso de uso:


![Captura](https://github.com/FABRY-MARTINEZ/proyecto1.github.io/assets/133180029/a4db7832-04e5-494f-868c-a83738bd9cd4)


| **Caso de uso** | Scrip con Bucle Do While|
|----------|----------|
| *Actores:*    |  Estudiantes 4to Semrestre  |
| *Propósito:*   | Practicar con el Bucle Do While|

   

| *Curso normal de eventos* |
|----------|
| 1. El usuario debera ingresar un Numero|
| 2. El programa debera determinar si el numero ingresado es Primo|
| 3. Se debera realizar la clasificacion del Numero asi:
for(int ind = 2; ind < num; ind++){ if(num%ind == 0){primo = false;}|


### CODIGO: 

import java.util.Scanner;

    public class Primo {
    
        public static void main(String[] args) {  
        
        Scanner entrada = new Scanner(System.in);
        System.out.print("Ingrese un número entero positivo: ");
        int num = entrada.nextInt();
        
        if (esPrimo(num)) {
            System.out.println(num + " es un número primo.");
        } else {
            System.out.println(num + " no es un número primo.");
        }
    }
        public static boolean esPrimo(int num) {
        if (num <= 1) {
            return false;
        }
        for (int i = 2; i <= Math.sqrt(num); i++) {
            if (num % i == 0) {
                return false;
            }
        }
        return true;
    }
}

### CODIGO ORIENTADO A OBJETOS:  

import java.util.Scanner;
public class Primo {

    public static void main(String[] args) {
        Primo p = new Primo();
        p.ejecutar();
    }
    
    public void ejecutar() {
        Scanner entrada = new Scanner(System.in);
        System.out.print("Ingrese un número entero positivo: ");
        int num = entrada.nextInt();
        
        if (esPrimo(num)) {
            System.out.println(num + " es un número primo.");
        } else {
            System.out.println(num + " no es un número primo.");
        }
    }
    
    public boolean esPrimo(int num) {
        if (num <= 1) {
            return false;
        }
        for (int i = 2; i <= Math.sqrt(num); i++) {
            if (num % i == 0) {
                return false;
            }
        }
        return true;
    }
}


### DIAGRAMA DE FLUJO: 
                           
![flujo](https://github.com/FABRY-MARTINEZ/proyecto1.github.io/assets/133180029/79fb770d-329b-4f39-b479-a57da5ec14b1)
     

### PSEUDOCODIGO: 

//Variable
num:entero
r:cadena

//entrada 

leer num
si num <=1 entonces  

num es primo 
si num=2 entonces

num No es primo entonces 
leer 

// salida 
fin 

### Análisis del Ejercicio:
### Aproximación Plantilla Historia de Usuario:

![jira](https://github.com/FABRY-MARTINEZ/proyecto1.github.io/assets/133180029/da317122-c43a-4dfe-975b-76a743a900b8)

