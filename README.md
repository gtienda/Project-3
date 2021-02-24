# Keeping Up With the Javascript: ES6

## www.pirple.com

## Project #3: Classes

## Author: Guadalupe Tienda López

## Country: México

## Language: Spanish / Español

</br>

**my github:** [<https://github.com/gtienda/Project-3.git>]

## Detalles

Una empresa de construcción lo contrató para ayudar a construir el "cerebro" de un conjunto de ascensores en un edificio nuevo. Su tarea es escribir el código que controlará los ascensores y decirle a cada ascensor a qué piso viajar a continuación.

### Crear el edificio

El edificio es la estructura principal del sistema de ascensores (A y B). El constructor nos proporciona el piso mínimo (pisoMin) y el piso máximo (pisoMax).
El piso -1 corresponde al SÓTANO, el 0 al LOBBY, el 10 al PENTHOUSE.

```javascript
const building = new Building(-1, 10);
```

### Crear los elevadores A y B

El constructor nos proporciona el nombre, el piso mínimo (pisoMin) y el piso máximo (piso Max) a los que se moverá cada elevador.

```javascript
const elevatorA = new Elevator('A', -1,  9);
const elevatorB = new Elevator('B',  0, 10);
```

### Agregar los elevadores a la estructura del edificio

Forma correcta de agregar los elevadores a la estructura del edicio.

```javascript
building.addElevator(elevatorA);
building.addElevator(elevatorB);
```

### Hacer funcionar los elevadores

Para hacer funcionar los ascensores, necesitamos usar el método de construcción llamado `callElevator`, indicando a cuál piso se está llamando y hacia que piso quiere ir. El edificio selecciona el ascensor más cercano para realizar el viaje.

```javascript
building.callElevator(7, 10);
```

### Conocer dónde están los elevadores

Este método nos ayuda a conocer en qué piso están los elevadores y conocer su Status.

```javascript
building.getElevatorsStatus();
```
