
# 🛡️ SeguridadUrbanaOptima

**Simulación y optimización de la ubicación de Centros de Atención Inmediata (CAI) para mejorar la respuesta ante delitos urbanos en Bucaramanga.**

---

## 📌 Descripción

Este proyecto tiene como objetivo principal **optimizar el tiempo de respuesta de las patrullas** ante incidentes delictivos. Para ello, se desarrolló un modelo en **AnyLogic** que simula el desplazamiento de patrullas desde los CAI hacia puntos de delito georreferenciados, considerando restricciones operativas y condiciones del entorno urbano.

---

## 🤖 Algoritmos Implementados

Se utilizaron y compararon cuatro algoritmos metaheurísticos:

- 🔹 Hill Climbing  
- 🔹 Simulated Annealing (SA)  
- 🔹 Particle Swarm Optimization (PSO)  
- 🔹 Global Harmony Search (GHS)  

Cada uno busca minimizar el tiempo total requerido para atender todos los delitos a partir de distintas configuraciones de CAI activos.

---

## 🗂️ Salida del Modelo

Al finalizar su ejecución, cada algoritmo genera un archivo `.txt` que contiene:

- El vector solución óptimo en formato binario.  
- El valor del *fitness* (tiempo total de atención en minutos).  

Este archivo es cargado posteriormente por el **módulo de movimiento**, el cual permite visualizar en el tiempo el desplazamiento de las patrullas en la ciudad de **Bucaramanga**.



## 🚀 Trabajos Futuros

Entre las mejoras y extensiones propuestas se incluyen:

- Incorporación de **datos en tiempo real**.  
- Consideración del **tráfico vehicular urbano** para ajustar la velocidad de las patrullas.  
- Simulación de **horas pico** y **tipos de delitos** para lograr un entorno más realista.  
- Evaluación de estrategias híbridas o combinadas entre algoritmos.  

---
---


## 📁 Estructura del Repositorio

A continuación, se describen las carpetas incluidas en este repositorio:

- **`datos/`**  
  Contiene los archivos Excel con los delitos clasificados por semestre y la lista de CAI que deben cargarse en cada algoritmo, con su correspondiente tiempo de atención.

- **`GHS/`**  
  Implementación del algoritmo metaheurístico **Global Harmony Search** (GHS).

- **`hill climbing/`**  
  Implementación del algoritmo **Hill Climbing**.

- **`PSO/`**  
  Implementación del algoritmo **Particle Swarm Optimization** (PSO).

- **`SA/`**  
  Implementación del algoritmo **Simulated Annealing** (SA).

- **`movimiento2/`**  
  Contiene el módulo visual que carga el archivo `.txt` generado por cada algoritmo y simula el movimiento de las patrullas en la ciudad de Bucaramanga.

Cada algoritmo, al finalizar su ejecución, genera un archivo `.txt` que contiene el cromosoma final y su valor de fitness. Este archivo es cargado por el módulo movimiento2 de simulación para representar visualmente los desplazamientos optimizados de las patrullas.



> Desarrollado como trabajo de grado en Ingeniería de Sistemas – Universidad del Cauca.
