# 🤖 Agente de IA para Búsqueda de Empleo (Implementación)

## 📌 Sobre este proyecto
Este repositorio documenta mi experiencia **implementando y configurando** un agente autónomo de IA de código abierto para automatizar mi búsqueda de empleo como Desarrollador Full Stack / Android Junior. 

*Nota de transparencia: La lógica central del agente está construida sobre la librería open-source `job-hunt-agent`. Mi trabajo consistió en desplegarlo, configurar el entorno, integrar las APIs y adaptar el flujo a mis necesidades.*

## 🎯 ¿Qué logra este flujo de trabajo?
1. **Lectura de CV:** Extrae y estructura mi información profesional desde un PDF usando un LLM.
2. **Búsqueda autónoma:** Rastrea ofertas en vivo en LinkedIn e Indeed (mediante JobSpy).
3. **Evaluación:** Asigna un "Fit Score" (puntuación) a cada oferta según mis habilidades y preferencias.
4. **Generación de documentos:** Redacta versiones personalizadas de mi CV y cartas de presentación para las ofertas con mayor puntaje.

## 🛠️ Tecnologías y Herramientas que configuré e integré
* **Python:** Gestión de entornos virtuales (`venv`) y ejecución de scripts.
* **OpenRouter (API):** Integración de modelos de lenguaje (LLMs) para el razonamiento del agente.
* **LangChain / DeepAgents:** Orquestación del agente y sus herramientas.
* **JobSpy:** Extracción de datos (scraping) de portales de empleo en tiempo real.
* **Streamlit:** Despliegue de la interfaz gráfica (UI) para interactuar con el agente.

## 🚀 Proceso de Implementación
1. Instalación del paquete y creación del entorno virtual aislado.
2. Configuración de variables de entorno (`.env`) para el manejo seguro de API Keys.
3. Generación del perfil estructurado (`profile.json` y `profile.md`) a partir de mi currículum.
4. Ejecución de la interfaz web para interactuar con el agente mediante prompts.
5. Automatización de la creación de documentos (CVs y cartas) en formato Markdown.

## 📈 Principales Aprendizajes
* **Integración de IA:** Comprensión del ciclo de vida de un agente (prompt, herramientas, memoria).
* **Seguridad:** Manejo de credenciales y APIs mediante variables de entorno.
* **Automatización:** Uso de IA para optimizar procesos repetitivos y de alto esfuerzo cognitivo (como adaptar un CV).

## ⚠️ Nota de Seguridad
Este repositorio **no contiene** claves de API (API Keys). El archivo `.env` está excluido mediante `.gitignore` para proteger las credenciales.
