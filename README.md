# Generala en C++

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
