# Proyectos Destacados - Alejandro Rocamora Latorre

Este repositorio reúne los proyectos técnicos y de investigación desarrollados en el ámbito de la ingeniería acústica, el procesamiento digital de señales y el diseño de sistemas.

---

## Estudio, Diseño y Aplicación de Sistemas de Altavoces Paramétricos (2026)

* **Trabajo Final de Grado (TFG):** Universidad de Alicante
* **Calificación:** 10/10 (Matrícula de Honor)

Este proyecto aborda el estudio teórico-experimental, el diseño estructural, el procesamiento digital de señales y la implementación práctica de arreglos de transductores ultrasónicos para la generación de audio audible altamente directivo mediante la explotación de la propagación acústica no lineal en el aire.

### Diseño y Fabricación de Hardware
* **Modelado CAD:** Diseño estructural y volumétrico tridimensional optimizado utilizando el software Blender.
* **Manufactura Aditiva:** Fabricación de los chasis mediante impresión 3D bajo tecnología FDM utilizando ácido poliláctico (PLA).
* **Despliegue de Arreglos:** Implementación y ensamblaje electromecánico en fase de dos prototipos funcionales de alta densidad con transductores piezoeléctricos comerciales de 40 kHz (*TCT40-16T*):
  * Arreglo Matricial Ortogonal ($N = 64$ elementos).
  * Arreglo Simétrico Hexagonal ($N = 61$ elementos).

### Caracterización Electroacústica en Laboratorio
* **Análisis de Admitancia Eléctrica Compleja:** Evaluación experimental del comportamiento dinámico de los arreglos trazando mapas frecuenciales de conductancia ($G_E$) y susceptancia ($B_E$).
* **Instrumentación Utilizada:** Sistema gobernado mediante módulo de adquisición de datos multifunción National Instruments (NI USB-6353).
* **Conclusiones Técnicas:** La evidencia experimental desveló que la geometría hexagonal mitiga de forma óptima las desadaptaciones por capacidad parásita y los fenómenos de antirresonancia local que distorsionan el perfil multifrecuencial del modelo matricial.

### Procesamiento Digital de Señales (DSP)
* **Modelado y Predicción Acústica:** Implementación y resolución numérica en MATLAB de modelos no lineales:
  * Integral de difracción de Rayleigh (análisis de campo cercano/Fresnel y lejano/Fraunhofer).
  * Solución analítica envolvente de Berktay.
* **Algoritmos de Modulación Ultrasónica:** Desarrollo en banda base de esquemas de modulación en amplitud para forzar la demodulación natural del aire minimizando el fenómeno cuadrático de distorsión armónica:
  * `DSB-AM` (Doble Banda Lateral).
  * `SSB-AM` (Banda Lateral Única).
  * `MAM1` (Modulación de Amplitud Modificada de primer orden), validada como la opción más eficiente frente al ancho de banda finito del hardware.

### Control Espacial y Ensayos de Directividad
* **Cámara Anecoica:** Automatización y sincronización de medidas acústicas espaciales en un rango angular de $+90^\circ$ a $-90^\circ$.
* **Soporte Giratorio:** Mediciones de diagramas polares de radiación con una resolución de puntos de medida cada 2.5°.
* **Manipulación del Haz:** Validación del comportamiento colimado del haz y control dinámico del lóbulo central de radiación aplicando inversiones de fase eléctrica ($180^\circ$) sobre sub-arreglos distribuidos en anillos concéntricos.

### Ciberseguridad y Aplicaciones Críticas
* **Inyección Encubierta de Comandos de Voz (*DolphinAttack*):** Tasa de éxito del 100% en ataques inaudibles sobre asistentes domóticos comerciales (*Amazon Alexa*). El esquema paramétrico desacoplado operó modulando la voz en banda lateral inferior (`LSB-SC`) de forma inaudible por el aire, induciendo la rectificación y demodulación mecánica directamente sobre la electrónica del micrófono receptor.
* **Inhibición Acústica Silenciosa (*Jamming*):** Validación del colapso del rango dinámico y saturación de los circuitos de Control Automático de Ganancia (AGC) en terminales móviles receptores. El bloqueo se logró mediante la inyección ultrasónica masiva de ruido de banda ancha (3 kHz a 10 kHz), forzando una supresión de hasta 30 dB en la banda base audible.

---

## Investigación en Acústica Musical: Estudio de la Nota Lobo en Violonchelos (2024)

Estudio técnico-experimental del fenómeno acústico de la *nota lobo* en el violonchelo. Se realizó el modelado teórico con sistemas acoplados de 2 grados de libertad (GDL), simulaciones en MATLAB, análisis modal y mediciones reales de vibración y presión sonora. Se evaluó el efecto de distintos tipos y posiciones de dispositivos matalobos.

* **Herramientas:** MATLAB, ARTA, tarjeta de sonido TASCAM, acelerómetro Bruel & Kjaer, micrófono Behringer.
* **Coautores:** Alejandro Rocamora Latorre y Antonio Muñoz Sanchis.

---

## Proyecto de Planta Solar Fotovoltaica en Sudáfrica (2025)

Diseño y cálculo técnico de una planta solar fotovoltaica en Kroonstad, Sudáfrica. Incluye el dimensionamiento de sistemas, estimación de generación y presupuesto de obra.

* **Herramientas:** Arquímedes, AutoCAD.
* **Coautores:** Alejandro Rocamora Latorre, Daniel Esteban Robles y Antonio Muñoz Sanchis.
