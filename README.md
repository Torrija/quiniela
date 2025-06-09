⚽ Proyecto Quiniela: Asesoramiento y Seguimiento de Apuestas de Fútbol 📊
Este proyecto es una plataforma web dinámica diseñada para una peña (grupo de apuestas) de Quiniela, ofreciendo herramientas robustas tanto para el seguimiento en tiempo real de las jornadas como para el asesoramiento estratégico en la elaboración de pronósticos.
Construido íntegramente en el frontend y alojado en GitHub Pages, este sistema demuestra cómo se pueden superar las limitaciones de un hosting estático para ofrecer funcionalidades avanzadas y un "aprendizaje" basado en datos históricos.

✨ Características Principales
Seguimiento en Tiempo Real: Visualización detallada del estado de las apuestas de la peña durante una jornada en curso, con actualizaciones en vivo de los resultados y su impacto en los pronósticos.
Gestión de Apuestas: Permite la carga y comparación de las apuestas realizadas por los miembros de la peña con los resultados oficiales.
Sección de Comentarios: Un espacio integrado para la comunicación y el debate entre los miembros de la peña.

📈 Sistema de Asesoramiento de Apuestas (Consejero de Quiniela):
Basado en Datos Históricos: Un innovador módulo que "aprende" del análisis de 66 jornadas pasadas de Quiniela.
Múltiples Fuentes de Probabilidad: Utiliza datos de Técnicos (Jugados), Quinielista, LAE y Probables para analizar patrones.
Recomendaciones Inteligentes: Ofrece sugerencias de Fijos, Dobles o Triples para cada partido de una nueva jornada.
Fiabilidad Histórica: Cada recomendación viene acompañada de un porcentaje de fiabilidad, indicando la precisión de esa regla en los datos históricos.
Proceso de "Aprendizaje" Offline: Dada la naturaleza estática del hosting, el análisis de datos y la derivación de reglas se realizan offline, siendo luego implementadas como heurísticas en el código JavaScript.

🛠️ Tecnologías Utilizadas
HTML5: Estructura de las páginas web.
CSS3: Estilos y diseño responsivo para una experiencia de usuario óptima.
JavaScript (Vanilla JS): Lógica principal del proyecto, incluyendo el procesamiento de datos, la interactividad del usuario y la implementación del sistema de asesoramiento.
JSON: Formato para almacenar y gestionar los datos de las apuestas de la peña, los datos de la jornada actual y el extenso historial de jornadas pasadas.
GitHub Pages: Alojamiento estático del sitio web.

🚀 Cómo Funciona el Asesoramiento
El "Consejero de Quiniela" funciona aplicando un conjunto de reglas derivadas de un análisis exhaustivo de las 66 jornadas históricas proporcionadas. Estas reglas, codificadas en JavaScript, evalúan las probabilidades (1, X, 2) de las diferentes fuentes para un partido de la jornada actual y sugieren la combinación (fijo, doble, triple) que históricamente ha mostrado mayor éxito bajo condiciones similares.

📚 Estructura del Repositorio
quiniela/
├── index.html                   // Página principal del informe
├── quiniela-jornada.html        // Página de seguimiento de jornada en vivo
├── quiniela-jornada-script.js   // Lógica JS para seguimiento de jornada
├── quiniela-jornada-style.css   // Estilos CSS para seguimiento de jornada
├── data.json                    // Datos de apuestas de la peña
├── quiniela_jornada_XX.json     // Datos de la jornada actual en vivo
├── consejero-quiniela.html      // Página del sistema de asesoramiento
├── consejero-quiniela-script.js // Lógica JS del consejero
├── consejero-quiniela-style.css // Estilos CSS del consejero
└── historical_quiniela_data.json// Base de datos histórica (66 jornadas)