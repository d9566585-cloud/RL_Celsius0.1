# 🌡️ TempPredictor-ML-Skill / TempCast

<p align="center">
  <b>Corporación Universitaria Unilasallista</b><br>
  <b>Programa: Ingeniería de Software</b><br>
  <i>De la Regresión Lineal a las Skills de Inteligencia Artificial</i>
</p>

---

## 📌 Tabla de Contenidos
1. [Descripción General](#-descripción-general)
2. [Objetivos del Proyecto](#-objetivos-del-proyecto)
3. [Contexto y Problemática (Tradicional vs. Machine Learning)](#-contexto-y-problemática)
4. [Desarrollo del Modelo en Google Colab](#-desarrollo-del-modelo-en-google-colab)
5. [Arquitectura e Integración de la Skill TempCast](#-arquitectura-e-integración-de-la-skill-tempcast)
6. [Ecosistema Tecnológico y Despliegue](#-ecosistema-tecnológico-y-despliegue)
7. [Evidencias Gráficas y Recursos (Assets)](#-evidencias-gráficas-y-recursos-assets)
8. [Conclusiones](#-conclusiones)

---

## 🚀 1. Descripción General
**TempPredictor-ML-Skill** es un proyecto académico integral diseñado para explorar el ciclo completo de la Inteligencia Artificial y el desarrollo de software: desde el entrenamiento de un modelo de Machine Learning en Python hasta su integración en un flujo interactivo de IA conversacional (`TempCast`), complementado con control de versiones y despliegue web.

- **Repositorio Oficial:** `RL_Celsius0.1`
- **Plataforma de Skill:** Google Labs (Opal) / Gemini AI
- **Enlace de la Aplicación Compartida:** [Acceder a TempCast en Gemini Labs](https://gemini.google.com/gem-labs/1vJz9jAwk1iikBa4L41VfX-LF5rrji74D)

---

## 🎯 2. Objetivos del Proyecto
- **Objetivo General:** Demostrar los fundamentos del aprendizaje automático mediante un caso práctico de conversión de temperaturas y explorar su escalabilidad hacia un flujo interactivo de inteligencia artificial.
- **Objetivos Específicos:**
  - Comprender las diferencias conceptuales entre la programación tradicional y el Machine Learning.
  - Preparar y procesar un dataset de temperaturas en grados Celsius y Fahrenheit.
  - Configurar, entrenar e inferir resultados mediante un modelo predictivo en Google Colab.
  - Diseñar una experiencia interactiva estructurada por pasos (Skill).
  - Organizar y documentar el repositorio de forma profesional con soporte de Landing Page.

---

## ⚖️ 3. Contexto y Problemática
La resolución de problemas computacionales puede abordarse desde dos ópticas distintas:

1. **Programación Tradicional:** El programador define explícitamente las reglas lógicas o matemáticas. Ejemplo clásico de conversión térmica:
   $$\text{F} = \text{C} \times 1.8 + 32$$
2. **Machine Learning:** El sistema infiere patrones y ajusta sus parámetros internos a partir de ejemplos conocidos (dataset), sin requerir una fórmula rígida programada a mano. 
   *(Nota: Aunque la conversión de temperatura posee una solución matemática exacta, este proyecto utiliza dicho dominio como caso pedagógico para ilustrar el funcionamiento del aprendizaje autónomo).*

---

## 🐍 4. Desarrollo del Modelo en Google Colab
El núcleo analítico se implementó en un entorno cloud mediante un cuaderno de Python. Puedes consultarlo directamente aquí:
- **Cuaderno en Google Colab:** [Ver TempPredictor Colab Notebook](https://colab.research.google.com/drive/16oJUfmXOp6nnKx4THYan4jG5tZUOFhVQ?usp=sharing)

**Pasos clave del desarrollo:**
1. **Definición del Dataset:** Ingestión de pares de valores de temperatura ($^\circ\text{C}$ y $^\circ\text{F}$).
2. **Arquitectura:** Capa densa orientada al ajuste lineal de parámetros.
3. **Optimización y Pérdida:** Uso del optimizador `Adam` y métrica de Error Cuadrático Medio (`MSE`).
4. **Entrenamiento e Inferencia:** Ajuste iterativo por épocas de pesos y sesgos, seguido de pruebas con nuevos valores de entrada.

---

## 🤖 5. Arquitectura e Integración de la Skill TempCast
La experiencia conversacional e interactiva se estructuró en **Google Labs / Opal**, dividiendo el flujo de ejecución en 4 pasos modulares:

```text
[Historical Data File] ➔ [Prediction Days] ➔ [Analyze and Forecast Temperature] ➔ [Generate Forecast]
