# Algoritmo Cuántico para el Problema del Subgrupo Oculto Abeliano (HSP)

Implementación del algoritmo HSP para grupos abelianos finitos. Incluye una QFT optimizada y una función de extracción de generadores del subgrupo oculto.

---

## Pipeline del Algoritmo

1. **Preparación de Registros Cuánticos**  
   - Registro principal: \( n \)-qubits para representar elementos de \( G \).  
   - Ancillas: \( k \)-qubits para almacenar \( f(g) \).  
   - Registro clásico: \( n \)-bits para mediciones finales.

2. **Inicialización del Estado Cuántico**  
   - Aplicar la QFT a todos los qubits del registro principal:  


3. **Aplicación del Oracle \( U_f \)**  
   - Implementar la función (f) mediante compuertas controladas:  
    
   - Colapsar a superposición de cosets:  


4. **Transformada de Fourier Cuántica Modular (QFT\(_G\))**  
   - Para cada módulo \( m_i \) en la descomposición de \( G \):  
     - Aplicar rotaciones controladas entre qubits.  
     - Finalizar con puertas Hadamard en el qubit objetivo.  


5. **Medición y Postprocesado Clásico**  
   - Medir el registro principal en la base estándar.  
   - Convertir resultados a vectores en base mixta usando:  
     \[
     \text{int\_to\_mixed\_base}(valor, [m_1, \dots, m_k])
     \]
   - Calcular generadores de \( H \) mediante eliminación gaussiana sobre vectores obtenidos.

---

## Uso del Algoritmo

### Configuración Inicial
1. **Definir el Grupo \( G \)**  
   Especificar los módulos \( [m_1, \dots, m_k] \) que definen \( G = \mathbb{Z}_{m_1} \times \cdots \times \mathbb{Z}_{m_k} \).

2. **Implementar la Función \( f \)**  
   Crear un circuito cuántico que compute \( f(g) \), asegurando que sea constante en los cosets de \( H \).

3. **Parámetros de Ejecución**  
   - `shots`: Número de mediciones cuánticas (default: 1024).  
   - `optimization_level`: Nivel de optimización del circuito (0-3).  
   - `tolerance`: Umbral para filtrar mediciones irrelevantes (default: 0.01).

### Flujo de Trabajo
