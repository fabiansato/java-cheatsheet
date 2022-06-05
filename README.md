# java-cheatsheet
-------------------
## Instalación en Linux

```linux
sudo apt-get update
```

```linux
sudo apt-get upgrade
```

instalando jre:
```linux
sudo apt-get install openjdk-8-jre
```

Agregando al repositorio OpenJDK
```linux
sudo add-apt-repository ppa:openjdk-r/ppa
```
```linux
sudo apt update
```

Instalando OpenJDK
```linux
sudo apt install openjdk-11-jdk
```


Testear la versión instalada de JAVA:
```linux
java -version
```

cambiar de versión de JAVA instalada:
```linux
sudo update-alternatives --config java
```
-----------------
# Intellij Idea atajos

## main
```java
public static void main(String[] args) {
```


## sout
```java
  System.out.println();
```

-----------------
## Tipos de datos numericos:

	
Por ejemplo:

// Int:
```java
Int n = 1234567890;
```

// Long:
```java
Long nL = 123456789012345L;
```

Por ejemplo:
// Double:
```java
Double nD = 123.456123456;
```

// Float
```java
Float nF = 123.456F;
```

### como cargar variables con var (desde JAVA 10):
```java
var salary = 1000; // INT
var pension = salary * 0.03; // DOUBLE
var totalSalary = salary - pension; // DOUBLE
```

-----------------
## Tipos de datos char y boolean


```java
//chars
char letter = 'a';
char anotherLetter = '\u03AF';
//boolean
boolean boleano = true;
// nueva forma con var
var booleano = false;
```


## Operadores de asignación:

• +=: a += b es equivalente a a = a + b

• -=: a -= b es equivalente a a = a - b

• *=: a *= b es equivalente a a = a * b

• /=: a /= b es equivalente a a = a / b

• %=: a %= b es equivalente a a = a % b


## Operadores de incremento:
++: i++ es equivalente a i = i + 1

--: i-- es equivalente a i = i - 1

# Operaciones matemáticas
```java
Math.PI // 3.141592653589793
Math.E // 2.718281828459045

Math.ceil(2.1) // 3.0 (redondear hacia arriba)
Math.floar(2.1) // 2.0 (redondear hacia abajo)

Math.pow(2, 3) // 8.0 (número elevado a una potencia)
Math.sqrt(3) // 1.73... (raíz cuadrada)

Math.max(2, 3) // 3.0 (el número más grande)

// Área de un círculo (PI * r^2):
Math.PI * Math.pow(r, 2)

// Área de una esfera (4 * PI * r^2):
4 * Math.PI * Math.pow(r, 2)

// Volumen de una esfera ( (4/3) * PI * r^3):
(4/3) * Math.PI * Math.pow(r, 3)
```

## Cast en variables: Estimación y Exactitud
estimación
```java
Math.sqrt(3) // 1.7320508075688772
(int) Math.sqrt(3) // 1
```
exactitud:
```java
int a = 30;
int b = 12;

a / b // 2
(double) a / b // 2.5
```
CONVERSIONES ENTRE TIPOS

otro ejemplo:
```java
int arroba = 64;
char aa = (char)arroba;
System.out.println(aa);
```

## ParseInt 
Para el caso especial de convertir un String a cualquier otro tipo de dato, Java dispone del método parse con sintaxis:
**Tipo.parseTipo(cadena)**

```java
String edad = "18"
int edadN = Integer.parseInt(edad);
```


## No perdemos información al pasar
        De char —> int.
        De byte —> short —> int —> long
        De int —> double
        De float —> double
    PERDEMOS INFORMACIÓN
        De int —> float
        De long —> float
        De long —> double
		
		
## Conversión Automatica::.
byte -> short
short -> int
char -> int
int -> long
long -> float
float -> double

.::Cast Necesario::.
double -> float
float -> long
long -> int
int -> short
short -> byte

char <-> byte
char <-> short
int -> char

## Array

### cargar un array

 ```java
int[] ar = new int[]{ 1,2,3,4,5,6,7,8,9,10 }; //carga un array
```

### recorrer un array

```java
for(int i=0;i<ar.length;i++){ //recorre el array
        sum+=ar[i];
        }
```
		
		
