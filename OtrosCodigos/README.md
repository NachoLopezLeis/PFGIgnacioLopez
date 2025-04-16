# Proyecto de Circuitos Cuánticos

Este repositorio contiene dos códigos principales relacionados con circuitos y algoritmos cuánticos. A continuación se presenta un README unificado que describe cada uno de ellos por separado.

---

## Parte 1: Demostración de la Transformada Cuántica de Fourier (QFT) con 3 Qubits

### Descripción
Este código implementa y demuestra la Transformada Cuántica de Fourier (QFT) utilizando un circuito de 3 qubits. La QFT es un algoritmo fundamental en computación cuántica que transforma estados cuánticos en el dominio de Fourier y es la base de muchos algoritmos cuánticos, como el algoritmo de Shor.

### Características principales
- Implementación de la QFT para 3 qubits.
- Visualización del circuito cuántico.
- Simulación y análisis del resultado.
- Uso de Qiskit para construir y simular el circuito.
- Instalación de dependencias necesarias (Qiskit, matplotlib, pylatexenc).

### Requisitos
- Python 3.x
- Qiskit
- matplotlib
- pylatexenc

### Instalación de dependencias
pip install qiskit qiskit-aer matplotlib pylatexenc


### Uso
- Ejecutar el notebook `PFGCircuits.ipynb`.
- El código construye el circuito QFT, lo simula y muestra los resultados.
- Se puede modificar el estado inicial para experimentar con diferentes entradas.

### Referencia
Este código es útil para entender cómo funciona la QFT y su implementación práctica en simuladores cuánticos.

---

## Parte 2: Implementación de Quantum Phase Estimation (QPE) y Algoritmos de Shor y Simon

### Descripción
Este código aborda la implementación del algoritmo de Estimación de Fase Cuántica (QPE), junto con algoritmos relacionados como los de Shor y Simon, que son fundamentales para la computación cuántica y la criptografía cuántica.

### Características principales
- Implementación del algoritmo QPE para estimar fases de operadores unitarios.
- Ejecución en backend real de IBM Quantum (ibm_kyiv).
- Construcción y transpile del circuito cuántico para optimización en hardware real.
- Uso avanzado de puertas cuánticas y control de ancillas.
- Visualización del circuito y resultados obtenidos.

### Requisitos
- Python 3.x
- Qiskit

### Uso
- Ejecutar el notebook `ShorSimonQPEGit.ipynb`.
- Configurar acceso a IBM Quantum para ejecutar en hardware real o usar simuladores.
- Analizar los resultados para comprender la estimación de fase y su aplicación en algoritmos cuánticos.

### Notas
- El código muestra la complejidad y profundidad del algoritmo QPE.
- Permite experimentar con diferentes configuraciones y profundidades del circuito.

---

# Contribuciones

Las contribuciones son bienvenidas. Por favor, abra un issue o un pull request para sugerir mejoras o reportar problemas.

# Licencia

Este proyecto está bajo la licencia MIT.

---

# Contacto

Para dudas o comentarios, por favor contacte al mantenedor del repositorio.


