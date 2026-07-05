# KID-FIT — Plataforma Web Educativa e Interactiva

Bienvenido al repositorio oficial de **KID-FIT**, una plataforma web de diseño adaptable (Responsive Web Design) orientada a niños, padres de familia y docentes en Guatemala. Este software surge como una solución digital viable, democrática y de bajo costo frente a las barreras estructurales de infraestructura y al alarmante 86.9% de sedentarismo en los adolescentes del país. 

El objetivo es descentralizar el acceso a guías interactivas, rutinas clasificadas según las etapas motrices del Currículo Nacional Base (CNB) y alternativas lúdicas e inclusivas para niños con discapacidad.

---

## 🛠️ 1. Stack Tecnológico

La arquitectura del proyecto está pensada para ser multiplataforma, escalable y fuertemente tipada. Se utilizarán las siguientes tecnologías:

*   **Frontend Core:** `React Native` / `Flutter` para garantizar un despliegue multi-dispositivo ágil y consistente.
*   **Sistema de Diseño:** `Tamagui` para la implementación de estilos dinámicos, fuentes y componentes optimizados para la visualización infantil.
*   **Lenguaje de Programación:** `TypeScript` para asegurar la estabilidad técnica del sitio, algoritmos de cálculo y flujos lógicos estructurados.
*   **Procesamiento Inteligente:** `MediaPipe` Módulo propuesto para el seguimiento de ejercicios en pantalla a través de la cámara.
*   **Ecosistema Backend & Auth:** `Supabase` para la gestión de accesos seguros y almacenamiento de recursos en la nube.
*   **Base de Datos:** `PostgreSQL` como motor relacional para la persistencia de ejercicios, usuarios y métricas de descanso.

---

## 🎨 2. Lineamientos de Diseño (UI/UX)

### Paleta de Colores Oficial
Para mantener la coherencia institucional y el enfoque infantil, se deben utilizar estrictamente los siguientes códigos hexadecimales:

| Color | Código Hex | Uso en la Interfaz | Significado  |
| :--- | :--- | :--- | :--- |
| **Azul** | `#1976D2` | Encabezados y menú principal  | Confianza y seguridad  |
| **Verde** | `#4CAF50` | Botones de acciones principales  | Salud y bienestar  |
| **Naranja** | `#FF9800` | Botones secundarios y alertas de acción  | Energía y motivación  |
| **Azul Medianoche** | `#191970` | Textos institucionales o variantes de contraste  | Seriedad y confianza institucional  |
| **Blanco** | `#FFFFFF` | Fondo principal de la aplicación  | Limpieza y claridad  |
| **Gris Claro** | `#F5F5F5` | Separadores y fondos de secciones  | Organización y contraste  |

### Tipografía (Google Fonts)
*   **Títulos principales y Subtítulos:** `Poppins Bold` 
*   **Texto de contenido y párrafos:** `Roboto Regular`  *(Alternativas válidas: Open Sans, Montserrat, Nunito)* .

---

## 📐 3. Lógica de Negocio y Clasificación (Base de Datos)

Las rutinas y validaciones del sistema deben segmentarse en el código según las especificaciones del CNB y la OMS recopiladas en la investigación :

### A. Etapas Motrices e Infantiles
*   **5 a 6 años (Preprimaria):** Correr, saltar con uno o ambos pies, giros, juegos de persecución, rondas rítmicas .
*   **7 a 12 años (Primaria):** Carreras de velocidad, relevos, dominio de balón (fútbol, baloncesto, voleibol), saltos de cuerda .

### B. Temporizadores y Tiempos de Descanso Obligatorios
*   **Rango 5 a 12 años:** 30 a 45 minutos por sesión (idealmente 2 veces por semana).
*   **Pausas de recuperación:** Entre circuitos o ejercicios intensos se deben programar pausas obligatorias de `1 a 2 minutos` para hidratación .
*   **Módulo de Sueño:** El sistema informará y validará que los niños cumplan entre `9 y 11 horas` de sueño nocturno ininterrumpido .

---

## 🗺️ 4. Estructura de Módulos de la Aplicación

El router de la aplicación frontend debe mapear las siguientes vistas base:

1.  **Inicio:** Presentación del proyecto KID-FIT y concientización sobre la salud infantil .
2.  **Ejercicios por Edades:** Módulo interactivo con rutinas recomendadas de 6 a 12 años .
3.  **Ejercicios Inclusivos:** Actividades y dinámicas adaptadas para niños con discapacidad .
4.  **Recomendaciones:** Guías de tiempos de ejercicio, descanso, hidratación y alimentación saludable .
5.  **Noticias y Recursos:** Sección informativa con datos actualizados de DIGEF, MINEDUC y la OMS .
6.  **Contacto:** Formulario para la resolución de dudas o soporte técnico .

---

## 🚀 5. Roadmap de Implementación (Próximos Pasos)

### Fase 1: Arquitectura Base e Infraestructura
*     Configurar el entorno de desarrollo con TypeScript y levantar la estructura del proyecto con Tamagui .
*     Inicializar las tablas relacionales en PostgreSQL dentro de Supabase (`usuarios`, `ejercicios`, `bitacora_rutinas`) .

### Fase 2: Core Features (Programación Lógica)
*     Desarrollar la **Calculadora de Índice de Masa Corporal (IMC)** basada en los estándares de salud recopilados .
*     Implementar el **Cronómetro de Rutinas** automatizado con alertas visuales para los tiempos de descanso e hidratación .

### Fase 3: Interacción y Gamificación (Mejoras Futuras)
*     Diseñar el sistema de retos semanales e insignias/logros para incentivar el juego activo en los niños .
*     Integrar la API de mapas para la geolocalización de instalaciones deportivas seguras en los municipios de Guatemala .
*     Acoplar el procesamiento con MediaPipe para la detección del movimiento en tiempo real .

---

## 👥 Equipo de Investigación y Desarrollo (Célula)
Este proyecto se sustenta en la investigación técnica presentada por :
*   Brandon Estiben Ixén | Carlos Elias Tzoy Velasco | Cleidy Priscilia Pérez Casia 
*   Daniel Aguilar Rodríguez | Frisly Alejandro Melchor | Irma Yaneht Arias García 
*   Joseph Fernando Ramírez Montenegro | Lester Alexander García Felipe | Marco Antonio Canux Raquec 
*   María José Montepeque Zet | Sergio Ricardo Ajú Miranda | Allison Rocío Vargas Mejía 

**Catedrática:** Nathalie   
**Institución:** CAMPUSLANDS — Guatemala, 30 de julio de 2026 