#    Optimizador de Cortes para Mueble de TV

Un algoritmo inteligente para optimizar el aprovechamiento de tableros de madera en la construcción de muebles de TV, maximizando la eficiencia del material y respetando la orientación correcta de las vetas.

##    Descripción

Este proyecto optimiza el corte de piezas de madera para un mueble de TV utilizando el método de "tiras", que agrupa las piezas por altura y las distribuye eficientemente en tableros estándar de 260 x 183 cm.

###    Características Principales

- **Optimización inteligente**: Algoritmo de tiras que maximiza el aprovechamiento del material
- **Respeto de vetas**: Garantiza que las fibras de madera corran en la dirección correcta (260 cm)
- **Análisis de viabilidad**: Calcula si es posible realizar todos los cortes en 2 tableros
- **Generación automática**: Crea archivos de texto profesionales para operativa
- **Control de calidad**: Incluye checklists y verificaciones

##    Funcionalidades

### 1. Análisis de Viabilidad
- Calcula el área total necesaria vs. disponible
- Determina la viabilidad del proyecto con 2 tableros
- Proporciona porcentajes de utilización y márgenes

### 2. Optimización por Tiras
- Agrupa piezas por altura similar
- Distribuye eficientemente a lo largo del ancho (260 cm)
- Minimiza desperdicios y maximiza aprovechamiento

### 3. Generación de Documentos
- Archivo de texto profesional para operativa
- Checklist de verificación completo
- Campos para firmas de operario y supervisor
- Formato listo para imprimir

##    Especificaciones del Proyecto

### Tableros
- **Dimensiones**: 260 x 183 cm
- **Orientación de vetas**: A lo largo de 260 cm
- **Cantidad objetivo**: 2 tableros máximo

### Piezas del Mueble
El código incluye todas las piezas necesarias para un mueble de TV completo:
- Tapas superiores e inferiores
- Laterales y divisorias
- Fondos y tapas basculantes
- Repisas de diferentes tamaños

##    Uso

### Instalación
```bash
# Clonar el repositorio
git clone https://github.com/tu-usuario/optimizador-cortes-mueble-tv.git

# Navegar al directorio
cd optimizador-cortes-mueble-tv
```

### Ejecución
```bash
# Ejecutar el optimizador
python optimizador_cortes.py
```

### Salida
El programa genera:
1. **Análisis en consola**: Muestra la viabilidad y estadísticas
2. **Archivo de texto**: `PLAN_CORTES_MUEBLE_TV.txt` con el plan completo de cortes

##    Ejemplo de Salida

```
=== ANÁLISIS DE VIABILIDAD PARA 2 TABLEROS ===

   Resumen:
   Total piezas: 32
   Área total necesaria: 89,456.0 cm²
   Área disponible (2 tableros): 95,160.0 cm²
   Utilización teórica: 94.0%
     VIABLE: 6.0% de margen disponible

   TABLERO 1:
   Altura utilizada: 180.0 cm de 183 cm
   Piezas (18): Repisa sup. 220x20, Tapa sup. central, etc.

   TABLERO 2:
   Altura utilizada: 176.4 cm de 183 cm
   Piezas (14): Repisas dobles 50x20, Laterales, etc.
```

##    Configuración

### Modificar Dimensiones del Tablero
```python
BOARD_WIDTH = 260  # cm (dirección de las vetas)
BOARD_HEIGHT = 183  # cm
```

### Agregar/Modificar Piezas
```python
pieces_final = [
    ("Nombre_Pieza", ancho, alto, cantidad),
    # Agregar más piezas aquí
]
```

##  Consideraciones Importantes

### Orientación de Vetas
- Las vetas siempre corren paralelas a la dimensión de 260 cm
- Esto garantiza máxima resistencia estructural
- Mejor apariencia estética en el mueble terminado

### Tolerancias
- Considerar el grosor de la sierra en las medidas finales
- Verificar medidas antes de cada corte
- Marcar cada pieza antes de cortar

##    Estructura del Proyecto

```
optimizador-cortes-mueble-tv/
├── README.md
├── optimizador_cortes.py
├── PLAN_CORTES_MUEBLE_TV.txt (generado)
└── LICENSE
```

##    Algoritmo

### Método de Tiras
1. **Agrupación**: Organiza piezas por altura similar
2. **Distribución**: Coloca piezas secuencialmente a lo largo del ancho
3. **Optimización**: Minimiza desperdicios y maximiza aprovechamiento
4. **Verificación**: Confirma que todas las piezas caben en 2 tableros

### Ventajas del Método
- Respeta naturalmente la orientación de las vetas
- Facilita el proceso de corte real
- Minimiza los errores de posicionamiento
- Optimiza el aprovechamiento del material

##    Métricas de Rendimiento

- **Eficiencia típica**: 90-95% de aprovechamiento
- **Piezas promedio**: 30-35 piezas por proyecto
- **Tiempo de cálculo**: < 1 segundo
- **Precisión**: ±0.1 cm en cálculos

##  Contribución

##  Licencia

##    Autor

Desarrollado para optimizar procesos de carpintería y maximizar el aprovechamiento de materiales en proyectos de mobiliario.

##    Próximas Mejoras

- [ ] Interfaz gráfica para visualizar los cortes
- [ ] Soporte para múltiples tipos de tableros
- [ ] Exportación a formatos CAD
- [ ] Cálculo automático de costos
- [ ] Optimización para diferentes tipos de madera


#    Wood Cutting Optimizer for TV Furniture

Smart wood cutting optimizer that maximizes material usage and generates professional cut plans. Automatically arranges furniture pieces across wood panels using strip-based optimization algorithms, ensuring proper grain orientation and minimal waste. Generates detailed cutting instructions with built-in quality controls, making complex woodworking projects more efficient and cost-effective.

## 📋 Description

This project optimizes wood cutting for TV furniture using the "strip method", which groups pieces by height and distributes them efficiently across standard 260 x 183 cm panels.

###    Key Features

- **Intelligent optimization**: Strip-based algorithm that maximizes material usage
- **Grain orientation respect**: Ensures wood fibers run in the correct direction (260 cm)
- **Feasibility analysis**: Calculates if all cuts can be made within 2 panels
- **Automatic generation**: Creates professional text files for workshop operations
- **Quality control**: Includes checklists and verification procedures

##    Features

### 1. Feasibility Analysis
- Calculates total area needed vs. available
- Determines project viability with 2 panels
- Provides utilization percentages and margins

### 2. Strip-Based Optimization
- Groups pieces by similar height
- Distributes efficiently along the width (260 cm)
- Minimizes waste and maximizes usage

### 3. Document Generation
- Professional text file for workshop operations
- Complete verification checklist
- Fields for operator and supervisor signatures
- Print-ready format

##    Project Specifications

### Wood Panels
- **Dimensions**: 260 x 183 cm
- **Grain orientation**: Along 260 cm length
- **Target quantity**: Maximum 2 panels

### Furniture Pieces
The code includes all pieces needed for a complete TV furniture unit:
- Top and bottom panels
- Sides and dividers
- Backs and hinged doors
- Shelves of various sizes

##   Usage

### Installation
```bash
# Clone the repository
git clone https://github.com/your-username/wood-cutting-optimizer.git

# Navigate to directory
cd wood-cutting-optimizer
```

### Execution
```bash
# Run the optimizer
python cutting_optimizer.py
```

### Output
The program generates:
1. **Console analysis**: Shows feasibility and statistics
2. **Text file**: `TV_FURNITURE_CUTTING_PLAN.txt` with complete cutting plan

##    Example Output

```
=== FEASIBILITY ANALYSIS FOR 2 PANELS ===

   Summary:
   Total pieces: 32
   Total area needed: 89,456.0 cm²
   Available area (2 panels): 95,160.0 cm²
   Theoretical utilization: 94.0%
      VIABLE: 6.0% margin available

   PANEL 1:
   Height used: 180.0 cm of 183 cm
   Pieces (18): Top shelf 220x20, Central top panel, etc.

   PANEL 2:
   Height used: 176.4 cm of 183 cm
   Pieces (14): Double shelves 50x20, Sides, etc.
```

##   Configuration

### Modify Panel Dimensions
```python
BOARD_WIDTH = 260  # cm (grain direction)
BOARD_HEIGHT = 183  # cm
```

### Add/Modify Pieces
```python
pieces_final = [
    ("Piece_Name", width, height, quantity),
    # Add more pieces here
]
```

##    Important Considerations

### Grain Orientation
- Grain always runs parallel to the 260 cm dimension
- This ensures maximum structural strength
- Better aesthetic appearance in finished furniture

### Tolerances
- Consider saw blade thickness in final measurements
- Verify measurements before each cut
- Mark each piece before cutting

##    Project Structure

```
wood-cutting-optimizer/
├── README.md
├── cutting_optimizer.py
├── TV_FURNITURE_CUTTING_PLAN.txt (generated)
└── LICENSE
```

##    Algorithm

### Strip Method
1. **Grouping**: Organizes pieces by similar height
2. **Distribution**: Places pieces sequentially along the width
3. **Optimization**: Minimizes waste and maximizes usage
4. **Verification**: Confirms all pieces fit within 2 panels

### Method Advantages
- Naturally respects grain orientation
- Facilitates actual cutting process
- Minimizes positioning errors
- Optimizes material usage

##    Performance Metrics

- **Typical efficiency**: 90-95% material usage
- **Average pieces**: 30-35 pieces per project
- **Calculation time**: < 1 second
- **Precision**: ±0.1 cm in calculations

##    Contributing

##    License

This project is licensed under the MIT License. See the `LICENSE` file for details.

##    Author

Developed to optimize carpentry processes and maximize material usage in furniture projects.

##    Future Improvements

- [ ] Graphical interface for cut visualization
- [ ] Support for multiple panel types
- [ ] CAD format export
- [ ] Automatic cost calculation
- [ ] Optimization for different wood types

---

