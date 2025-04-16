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
   - Poner en superposición a todos los qubits
   - Para cada módulo \( m_i \) en la descomposición de \( G \):
     - Aplicar rotaciones controladas entre qubits.  

5. **Medición y Postprocesado Clásico**  
   - Medir el registro principal en la base estándar.  
   - Convertir resultados a vectores en base mixta usando:  
   - Calcular generadores de \( H \) mediante eliminación gaussiana sobre vectores obtenidos.
---

## Uso del Algoritmo

### Configuración Inicial
 1. **Definir el Grupo \( G \)**  
      - Introducir el grupo en la variable group
      - Detereminar la estructura del grupo en la variuable moduli

2. **Implementar la Función \( f \)**  
   Aplicar la funciín f a la hora de realizar el f_mapping. En el código actual f=> f(x)=x

3. **Parámetros de Ejecución**  
   - `shots`: Número de mediciones cuánticas (default: 1024).  
   - `optimization_level`: Nivel de optimización del circuito (0-3).  
   - `tolerance`: Umbral para filtrar mediciones irrelevantes (default: 0.01).
     
## Notas
El código completo está explicado con mucho más detalle en la memoria del Proyecto, especificamente pág. 35-42
[Link del proyecto]

# Visualización de la QFT

El código QFTImage proporciona una visualización para comparar la QFT normal con la QFT que se ha desarrollado en este proyecto.

Todas las demostraciones y detalles referentes a esta optimización están recogidas en la memoria del proyecto
