# java-cheatsheet
 

------------------------------
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
Tipos de datos para números enteros (sin decimales):

• byte: Ocupa 1 byte de memoria y su rango es de -128 hasta 127.	
• short: Ocupa 2 bytes de memoria y su rango es de -32,768 hasta 32,727.	
• int: Ocupa 4 bytes de memoria y su rango es de -2,147,483,648 hasta 2,147,483,647. 	
	Es muy cómodo de usar, ya que no es tan pequeño para que no quepan nuestros números ni tan grande como para desperdiciar mucha memoria. Puede almacenar hasta 10 dígitos.	
• long: Ocupa 8 bytes de memoria y su rango es de -9,223,372,036,854,775,808 hasta 9,223,372,036,854,775,807. Para diferenciarlo de un tipo de dato long debemos terminar el número con la letra L.
	
Por ejemplo:

// Int:
```java
Int n = 1234567890;
```

// Long:
```java
Long nL = 123456789012345L;
```

Tipos de datos para números flotantes (con decimales):

• float: Ocupan 4 bytes de memoria y su rango es de 1.40129846432481707e-45 hasta 3.40282346638528860e+38. Así como long, debemos colocar una letra F al final.
	
• double: Ocupan 8 bytes de memoria y su rango es de 4.94065645841246544e-324d hasta 1.79769313486231570e+308d.
	
Por ejemplo:
// Double:
```java
Double nD = 123.456123456;
```

// Float
```java
Float nF = 123.456F;
```


-----------------
## Tipos de datos char y boolean


char: Ocupa 2 bytes y solo puede almacenar 1 dígito, debemos usar comillas simples en vez de comillas dobles.
boolean: Son un tipo de dato lógico, solo aceptan los valores true y false. También ocupa 2 bytes y almacena únicamente 1 dígito.

Seguro te diste cuenta que siempre debemos escribir el tipo de dato de nuestras variables antes de definir su nombre y valor. Pero esto cambia a partir de Java 10: solo debemos escribir la palabra reservada var y Java definirá el tipo de dato de nuestras variables automáticamente:

```java
//chars
char letter = 'a';
char anotherLetter = '\u03AF';
//boolean
var booleano = false;
```
