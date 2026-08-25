# Generala en C++

*[English version below](#generala-in-c)*

Implementación en C++ del clásico juego de dados **Generala**, jugable por consola, con modo de 1 y 2 jugadores.

Proyecto desarrollado en el marco de la Universidad Tecnológica Nacional (UTN - FRGP).

## Funcionalidades

- Modo **1 jugador** y modo **2 jugadores**, con comparación de puntajes y desempate a dados en caso de empate.
- Sistema completo de tiradas: hasta 3 lanzamientos por ronda, con posibilidad de elegir qué dados volver a tirar.
- Modo manual opcional, para definir a mano el valor de los dados relanzados (útil para testear combinaciones).
- Cálculo automático de todas las combinaciones de puntaje: Generala (servida y no servida), Póker, Full, Escalera y juegos menores.
- Registro del mejor puntaje histórico de la partida.
- Interfaz de consola con colores y posicionamiento de texto usando [rlutil](https://github.com/tapio/rlutil).

## Tecnologías

- **C++** (estándar del compilador GCC/MinGW)
- [rlutil.h](https://github.com/tapio/rlutil) para el manejo de la consola (colores, cursor, limpiar pantalla)
- Proyecto de **Code::Blocks** (`Generala.cbp`)

## Estructura del proyecto

```
├── main.cpp              # Punto de entrada y menú principal
├── funciones.cpp         # Lógica del juego: turnos, tiradas, combinaciones y puntaje
├── include/
│   └── funciones.h       # Declaraciones de las funciones del juego
├── rlutil.h               # Librería de terceros para interfaz de consola
└── Generala.cbp           # Proyecto de Code::Blocks
```

## Cómo compilar y ejecutar

1. Abrir `Generala.cbp` con [Code::Blocks](http://www.codeblocks.org/) (con un compilador GCC/MinGW configurado).
2. Compilar el proyecto (`Build`).
3. Ejecutar el binario generado en `bin/Debug/`.

También se puede compilar manualmente con GCC:

```bash
g++ main.cpp funciones.cpp -Iinclude -o generala
./generala
```

## Desarrollo

Proyecto desarrollado en equipo por:

- Francisco Cristiani
- Francisco Sackmann
- Franco Pacheco
- Rodrigo Godoy

---

## Generala in C++

C++ implementation of the classic **Generala** dice game, playable from the console, with 1-player and 2-player modes.

Developed as part of the Universidad Tecnológica Nacional (UTN - FRGP).

### Features

- **1-player** and **2-player** modes, with score comparison and a dice tie-breaker.
- Full roll system: up to 3 rolls per round, with the option to choose which dice to re-roll.
- Optional manual mode, to manually set the value of re-rolled dice (useful for testing combinations).
- Automatic scoring for every combination: Generala (served and unserved), Four of a Kind, Full House, Straight, and lower-value combos.
- Tracks the best score across the session.
- Console interface with colors and text positioning using [rlutil](https://github.com/tapio/rlutil).

### Technologies

- **C++** (GCC/MinGW compiler standard)
- [rlutil.h](https://github.com/tapio/rlutil) for console handling (colors, cursor, clear screen)
- **Code::Blocks** project (`Generala.cbp`)

### Project structure

```
├── main.cpp              # Entry point and main menu
├── funciones.cpp         # Game logic: turns, rolls, combinations and scoring
├── include/
│   └── funciones.h       # Game function declarations
├── rlutil.h               # Third-party library for the console interface
└── Generala.cbp           # Code::Blocks project
```

### How to build and run

1. Open `Generala.cbp` with [Code::Blocks](http://www.codeblocks.org/) (with a GCC/MinGW compiler configured).
2. Build the project.
3. Run the binary generated in `bin/Debug/`.

You can also compile it manually with GCC:

```bash
g++ main.cpp funciones.cpp -Iinclude -o generala
./generala
```

### Team

Developed as a team by:

- Francisco Cristiani
- Francisco Sackmann
- Franco Pacheco
- Rodrigo Godoy
