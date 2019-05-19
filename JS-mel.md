# Javascript

## 1 : JSON *"Javascript Object Notation"*
El formato JSON tiene varios caracteres importantes, los cuales son

Coma ***","***
	: Las comas separan los elementos dentro de un JSON, sean arreglos, objetos o valores simples

Corchetes cuadrados ***"[ ]"***
	: Representan ***arreglo***, y contienen cualquier clase de valores, incluyendo arreglos u objetos

**Ejemplo de arreglo**
``` json
	[ 25, 32, "sandia", null, "come tierra" ]
```
	
llaves ***"{ }"*** y Dos puntos ***":"***
	: las llaves denotan *objeto*, los objetos están constituidos por elementos clave-valor, separados por dos puntos. El valor de un objeto puede ser un objeto o arreglo, pero no su clave

**Ejemplo de Objeto**
``` json
	{
		"clave": "valor",
		"un_arreglo": [
			1,
			2,
			"sandia"
		],
		"un_objeto_vacio": { }
	}
```

Los objetos y arreglos se pueden anidar entre ellos, logrando tener muchísimos datos ordenados sin problemas

## REST Verbs

Las peticiones HTTP se obtienen a través de varios métodos, cada uno con un fin específico, los cuales son

*Nota: Se pueden dar otros usos a los métodos, pero el uso descrito abajo es el recomendado, para hacer la API intuitiva*

|**Verbo HTTP**|**Características**|
|:---|:---:|
|GET|Obtener datos del servidor. |


## Fetch API


## REST responses