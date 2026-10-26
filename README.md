🧬 Genómica ecológica de Prochlorococcus
Diversidad genómica y diferenciación ecológica de cianobacterias marinas

<p align="center">
<img src="https://img.shields.io/badge/Área-Ecología%20marina-167D8D?style=for-the-badge" alt="Ecología marina"/>
<img src="https://img.shields.io/badge/Enfoque-Genómica%20comparativa-4267B2?style=for-the-badge" alt="Genómica comparativa"/>
<img src="https://img.shields.io/badge/Datos-NCBI%20%7C%20ENA-398564?style=for-the-badge" alt="Datos públicos"/>
<img src="https://img.shields.io/badge/Pipeline-Bactopia-7D5BA6?style=for-the-badge" alt="Bactopia"/>
</p>

📖 Descripción del proyecto

Este proyecto propone caracterizar la diversidad genómica de cianobacterias marinas del género Prochlorococcus mediante el análisis comparativo de lecturas públicas de secuenciación.

Se utilizarán datos disponibles en repositorios científicos de acceso público para desarrollar un flujo de análisis reproducible que integre control de calidad, ensamblaje genómico, anotación, análisis de pangenoma, filogenia y evaluación estadística.

Desde una perspectiva ecológica, se busca explorar la variación genómica entre aislamientos y evaluar si determinados patrones se relacionan con su procedencia ambiental y geográfica.

Importante: la asociación entre diversidad genómica y condiciones ambientales constituye una hipótesis que deberá evaluarse con los datos y metadatos disponibles.

🌊 Contexto ecológico

Prochlorococcus es un grupo de cianobacterias fotosintéticas ampliamente distribuido en ambientes marinos, especialmente en aguas oceánicas cálidas y oligotróficas.

Su diversidad genética y funcional ofrece una oportunidad para estudiar la variación entre linajes microbianos y formular preguntas sobre adaptación ambiental, distribución y funcionamiento de los ecosistemas marinos.

La genómica comparativa permitirá identificar genes compartidos y variables entre los genomas analizados. Sin embargo, la presencia de un gen no demuestra por sí sola que se exprese ni que proporcione una ventaja adaptativa en el ambiente.

❓ Pregunta de investigación

¿En qué medida varía la composición del pangenoma de aislamientos de Prochlorococcus y qué relación presentan sus patrones de diversidad genómica con la procedencia geográfica y las variables ambientales disponibles?

💡 Hipótesis

Los aislamientos de Prochlorococcus presentan variación en sus genes centrales y accesorios. Parte de esa variación podría asociarse con diferencias ambientales o geográficas, aunque también puede explicarse por el parentesco evolutivo y por diferencias técnicas entre los estudios de origen.

🎯 Objetivos
Objetivo general

Caracterizar la diversidad genómica de Prochlorococcus mediante un flujo reproducible de análisis de lecturas públicas y evaluar su relación con la procedencia ambiental de los aislamientos.

Objetivos específicos
Identificar y seleccionar lecturas públicas de secuenciación con metadatos verificables.
Evaluar la calidad de las lecturas y de los ensamblajes genómicos.
Obtener anotaciones comparables de los genomas seleccionados.
Caracterizar los genes centrales y accesorios mediante análisis de pangenoma.
Explorar las relaciones filogenéticas entre los aislamientos.
Evaluar patrones de asociación entre diversidad genómica y variables ambientales disponibles.
Documentar los procedimientos, scripts, parámetros y resultados para facilitar la reproducibilidad.
🗃️ Fuentes de datos
Repositorio	Información	Enlace
NCBI BioProject	Proyectos de secuenciación	NCBI
NCBI SRA	Lecturas crudas de secuenciación	SRA
NCBI Assembly	Genomas ensamblados	Assembly
ENA	Lecturas, muestras y metadatos	ENA Browser
Proyectos candidatos
BioProject	Descripción preliminar	Estado
PRJNA664924	Aislamientos de Prochlorococcus HLII del Pacífico occidental y bacterias asociadas	Pendiente de auditoría de lecturas y metadatos
PRJNA418029	Genomas de aislamientos de Prochlorococcus marinus de regiones del Pacífico occidental y mar de China Meridional	Candidato complementario

La selección definitiva dependerá de la disponibilidad de FASTQ, la calidad de las lecturas, la comparabilidad de los aislamientos y la información ambiental documentada.

🧪 Metodología general
text
Selección de proyectos públicos
            │
            ▼
Auditoría de muestras y metadatos
            │
            ▼
Descarga de lecturas crudas
            │
            ▼
Control de calidad
            │
            ▼
Ensamblaje y anotación genómica
            │
            ▼
Pangenoma y filogenia
            │
            ▼
Análisis estadístico
            │
            ▼
Interpretación ecológica
            │
            ▼
Documentación y reproducibilidad

Herramientas principales
Herramienta	Función
Bactopia	Flujo de análisis genómico bacteriano
FastQC / MultiQC	Inspección y resumen de calidad de lecturas
Python	Validación de metadatos y procesamiento de tablas
R	Análisis estadístico y visualización
Git / GitHub	Control de versiones y documentación

Las herramientas concretas y sus versiones se registrarán conforme se implemente el flujo.

📊 Resultados que se generarán

Los siguientes son productos previstos, no resultados ya obtenidos.

Producto	Descripción
Control de calidad	Resumen de métricas por muestra
Ensamblajes	Genomas reconstruidos a partir de lecturas
Anotación	Tabla de genes y funciones anotadas
Pangenoma	Matriz de genes centrales y accesorios
Filogenia	Árbol de relaciones entre aislamientos
Estadística	Comparaciones y evaluación de asociaciones
Figuras	Gráficas reproducibles para el informe
Informe final	Interpretación ecológica y limitaciones
📁 Organización del repositorio
text
config/       Parámetros del análisis
data/         Documentación y metadatos
workflow/     Scripts de ejecución del pipeline
scripts/      Procesamiento y análisis estadístico
environment/  Registro de versiones de software
results/      Resultados generados por el análisis
docs/         Métodos y reproducibilidad
report/       Propuesta, resultados y discusión


Los archivos FASTQ y los archivos intermedios voluminosos no se incluirán directamente en el repositorio. Se documentarán sus fuentes y las instrucciones necesarias para recuperarlos.

🔁 Reproducibilidad

Para facilitar la reproducción del estudio se conservarán:

Accesiones públicas y metadatos de las muestras.
Versiones de los programas utilizados.
Scripts y parámetros de ejecución.
Criterios de inclusión y exclusión.
Tablas y figuras finales.
Documentación de los pasos de procesamiento.
Limitaciones y decisiones metodológicas.

Las conclusiones se elaborarán únicamente a partir de los resultados obtenidos y de los análisis efectivamente ejecutados.

⚠️ Limitaciones
Los metadatos ambientales pueden ser incompletos.
Los distintos proyectos pueden utilizar tecnologías y protocolos de secuenciación diferentes.
La estructura filogenética puede confundirse con patrones de distribución geográfica.
La anotación genómica representa potencial funcional, no actividad biológica demostrada.
La disponibilidad de datos públicos no garantiza que todas las muestras sean comparables.
📚 Referencias y recursos
Bactopia — documentación y código
NCBI BioProject
NCBI SRA
European Nucleotide Archive

Las publicaciones específicas y las referencias metodológicas utilizadas se incorporarán a medida que se cierre el diseño del análisis.

<p align="center">
**Proyecto académico de Ecología Genómica Marina**
</p>

<p align="center">
Investigación reproducible con datos públicos y herramientas de código abierto.
</p>
