# Proyecto de Circuitos Cuánticos

Este repositorio contiene dos códigos auxiliares que han sido utilizados en el desarrollo de mi proyecto de fin de grado. A continuación se presenta un README que describe cada uno de ellos por separado.

---
### Instalación de dependencias
pip install qiskit qiskit-aer matplotlib pylatexenc


## Parte 1: PFGCircuits

### Descripción
Este código implementa y muestra la Transformada Cuántica de Fourier (QFT) utilizando las funciones de Qiskit. Además, muestra las gráficas que comparan la complejidad computacional del algoritmo de Simon y del algoritmo de Shor con sus contrapartes clásicas.

### Características principales
- Implementación de la QFT para 3 qubits.
- Visualización del circuito cuántico.
- Simulación y análisis del resultado.
- Uso de Qiskit para construir y simular el circuito.
- Visaulización de la gráficas de complejidad computacional

### Uso
- Ejecutar el notebook `PFGCircuits.ipynb`.
- El código construye el circuito QFT, lo simula y muestra los resultados.
- Se puede modificar el estado inicial para experimentar con diferentes entradas.

---

## Parte 2: ShorSimonQPE

### Descripción
Este código aborda la implementación del algoritmo de Estimación de Fase Cuántica (QPE), junto con los algoritmos de Shor y Simon, que son fundamentales para la computación cuántica y la criptografía cuántica.

### Características principales
- Implementación del algoritmo QPE para estimar fases de operadores unitarios.
- Ejecución en backend real de IBM Quantum.
- Construcción y transpile del circuito cuántico para optimización en hardware real.
- Uso avanzado de puertas cuánticas y control de ancillas.
- Visualización del circuito y resultados obtenidos.

### Uso
- Ejecutar el notebook `ShorSimonQPEGit.ipynb`.
- Configurar acceso a IBM Quantum para ejecutar en hardware real o usar simuladores, para ello tan solo debes introducir tu token(https://quantum.ibm.com/).
- Analizar los resultados.

### Notas
- Permite experimentar con diferentes configuraciones y profundidades del circuito.




