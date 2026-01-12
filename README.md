# 🚕 Project Zuber - Análisis de Movilidad en Chicago

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green.svg)
![SQL](https://img.shields.io/badge/SQL-Database-orange.svg)
![Scipy](https://img.shields.io/badge/Scipy-Statistics-red.svg)

---

## 📋 Contexto del Proyecto

**Zuber** es una startup de movilidad compartida que busca ingresar al competitivo mercado de Chicago. Para tomar decisiones estratégicas basadas en datos, se realizó un análisis exhaustivo de los patrones de comportamiento de usuarios, preferencias de servicio y el impacto de factores externos (como el clima) en la demanda de taxis.

Este proyecto combina **extracción de datos con SQL**, **limpieza y transformación (ETL)**, y **análisis estadístico** para generar insights accionables que respalden la estrategia de penetración de mercado y optimización operativa.

---

## 🎯 Objetivo General

Analizar los patrones de viajes en taxi en Chicago para:
- Identificar los barrios con mayor demanda
- Evaluar el desempeño de las empresas de taxis
- Determinar el impacto del clima en la duración de los viajes
- Proporcionar recomendaciones estratégicas para Zuber

---

## 📊 Datos Utilizados

El análisis se basó en tres conjuntos de datos extraídos mediante consultas SQL:

| Dataset | Descripción | Variables Clave |
|---------|-------------|-----------------|
| **company_and_trips** | Viajes por empresa de taxis (15-16 nov 2017) | `company_name`, `trips_amount` |
| **dropoff_location_avg** | Promedio de viajes por barrio (nov 2017) | `dropoff_location_name`, `average_trips` |
| **start_weather** | Viajes Loop → O'Hare Airport | `start_ts`, `weather_conditions`, `duration_seconds` |

---

## 🔍 Metodología

```mermaid
graph LR
    A[Extracción SQL] --> B[Limpieza ETL]
    B --> C[Análisis Exploratorio]
    C --> D[Pruebas Estadísticas]
    D --> E[Insights y Recomendaciones]
